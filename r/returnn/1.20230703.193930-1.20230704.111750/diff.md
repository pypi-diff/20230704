# Comparing `tmp/returnn-1.20230703.193930.tar.gz` & `tmp/returnn-1.20230704.111750.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230703.193930.tar", last modified: Mon Jul  3 17:47:15 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230704.111750.tar", last modified: Tue Jul  4 09:33:33 2023, max compression
```

## Comparing `returnn-1.20230703.193930.tar` & `returnn-1.20230704.111750.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21015 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100183 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   152240 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   302020 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35646 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72979 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   568467 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 09:33:11.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-04 09:33:13.000000 returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21015 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100183 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152240 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302020 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35646 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72979 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:33:33.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 09:33:10.000000 returnn-1.20230704.111750/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230703.193930/.gitignore` & `returnn-1.20230704.111750/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/.gitmodules` & `returnn-1.20230704.111750/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/CHANGELOG.md` & `returnn-1.20230704.111750/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/CODEOWNERS` & `returnn-1.20230704.111750/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/CONTRIBUTING.md` & `returnn-1.20230704.111750/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/LICENSE` & `returnn-1.20230704.111750/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/MANIFEST.in` & `returnn-1.20230704.111750/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/PKG-INFO` & `returnn-1.20230704.111750/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230703.193930
+Version: 1.20230704.111750
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230703.193930/README.rst` & `returnn-1.20230704.111750/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/__init__.py` & `returnn-1.20230704.111750/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/12AX.cluster_map` & `returnn-1.20230704.111750/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-fwd.config` & `returnn-1.20230704.111750/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-horovod-mpi.py` & `returnn-1.20230704.111750/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230704.111750/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-hyper-param-tuning.config` & `returnn-1.20230704.111750/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-iter-dataset.py` & `returnn-1.20230704.111750/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-list-devices.py` & `returnn-1.20230704.111750/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-lua-torch-layer.config` & `returnn-1.20230704.111750/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230704.111750/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-returnn-as-framework.py` & `returnn-1.20230704.111750/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-rf.config` & `returnn-1.20230704.111750/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-rhn-enwik8.config` & `returnn-1.20230704.111750/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-sprint-interface.py` & `returnn-1.20230704.111750/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-att-copy.config` & `returnn-1.20230704.111750/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-attention.config` & `returnn-1.20230704.111750/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-enc-dec.config` & `returnn-1.20230704.111750/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230704.111750/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230704.111750/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230704.111750/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230704.111750/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230704.111750/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-rec-self-att.config` & `returnn-1.20230704.111750/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230704.111750/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230704.111750/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230704.111750/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-torch.config` & `returnn-1.20230704.111750/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230704.111750/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/demo.sh` & `returnn-1.20230704.111750/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230704.111750/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/README.txt` & `returnn-1.20230704.111750/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/config_demo` & `returnn-1.20230704.111750/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230704.111750/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/config_real` & `returnn-1.20230704.111750/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230704.111750/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/decode.py` & `returnn-1.20230704.111750/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230704.111750/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230704.111750/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230704.111750/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230704.111750/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230704.111750/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230704.111750/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230704.111750/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230704.111750/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/__init__.py` & `returnn-1.20230704.111750/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/__main__.py` & `returnn-1.20230704.111750/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/__old_mod_loader__.py` & `returnn-1.20230704.111750/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/__setup__.py` & `returnn-1.20230704.111750/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/config.py` & `returnn-1.20230704.111750/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/audio.py` & `returnn-1.20230704.111750/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/basic.py` & `returnn-1.20230704.111750/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/bundle_file.py` & `returnn-1.20230704.111750/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/cached.py` & `returnn-1.20230704.111750/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/cached2.py` & `returnn-1.20230704.111750/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/generating.py` & `returnn-1.20230704.111750/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/hdf.py` & `returnn-1.20230704.111750/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/lm.py` & `returnn-1.20230704.111750/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/map.py` & `returnn-1.20230704.111750/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/meta.py` & `returnn-1.20230704.111750/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/multi_proc.py` & `returnn-1.20230704.111750/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/normalization_data.py` & `returnn-1.20230704.111750/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/numpy_dump.py` & `returnn-1.20230704.111750/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/raw_wav.py` & `returnn-1.20230704.111750/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/sprint.py` & `returnn-1.20230704.111750/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/stereo.py` & `returnn-1.20230704.111750/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230704.111750/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/datasets/util/vocabulary.py` & `returnn-1.20230704.111750/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/engine/base.py` & `returnn-1.20230704.111750/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/engine/batch.py` & `returnn-1.20230704.111750/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230704.111750/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/edit.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/select.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/transform.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/extern/graph_editor/util.py` & `returnn-1.20230704.111750/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/forward_iface.py` & `returnn-1.20230704.111750/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/__init__.py` & `returnn-1.20230704.111750/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/_backend.py` & `returnn-1.20230704.111750/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/_numpy_backend.py` & `returnn-1.20230704.111750/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/_utils.py` & `returnn-1.20230704.111750/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/array_.py` & `returnn-1.20230704.111750/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/attention.py` & `returnn-1.20230704.111750/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/cond.py` & `returnn-1.20230704.111750/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/const.py` & `returnn-1.20230704.111750/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/container.py` & `returnn-1.20230704.111750/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/conv.py` & `returnn-1.20230704.111750/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/device.py` & `returnn-1.20230704.111750/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/dims.py` & `returnn-1.20230704.111750/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/dropout.py` & `returnn-1.20230704.111750/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/dtype.py` & `returnn-1.20230704.111750/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/encoder/base.py` & `returnn-1.20230704.111750/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/encoder/conformer.py` & `returnn-1.20230704.111750/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/init.py` & `returnn-1.20230704.111750/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/linear.py` & `returnn-1.20230704.111750/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/loop.py` & `returnn-1.20230704.111750/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/loss.py` & `returnn-1.20230704.111750/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/math_.py` & `returnn-1.20230704.111750/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/matmul.py` & `returnn-1.20230704.111750/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/module.py` & `returnn-1.20230704.111750/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/normalization.py` & `returnn-1.20230704.111750/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/parameter.py` & `returnn-1.20230704.111750/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/rand.py` & `returnn-1.20230704.111750/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/rec.py` & `returnn-1.20230704.111750/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/reduce.py` & `returnn-1.20230704.111750/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/run_ctx.py` & `returnn-1.20230704.111750/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/signal.py` & `returnn-1.20230704.111750/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/state.py` & `returnn-1.20230704.111750/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/tensor_array.py` & `returnn-1.20230704.111750/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/frontend/types.py` & `returnn-1.20230704.111750/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/import_/common.py` & `returnn-1.20230704.111750/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/import_/git.py` & `returnn-1.20230704.111750/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/import_/import_.py` & `returnn-1.20230704.111750/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/learning_rate_control.py` & `returnn-1.20230704.111750/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/log.py` & `returnn-1.20230704.111750/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/native_op.cpp` & `returnn-1.20230704.111750/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/native_op.py` & `returnn-1.20230704.111750/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/pretrain.py` & `returnn-1.20230704.111750/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/sprint/cache.py` & `returnn-1.20230704.111750/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/sprint/control.py` & `returnn-1.20230704.111750/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/sprint/error_signals.py` & `returnn-1.20230704.111750/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/sprint/extern_interface.py` & `returnn-1.20230704.111750/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/sprint/interface.py` & `returnn-1.20230704.111750/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/_dim_extra.py` & `returnn-1.20230704.111750/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/_tensor_extra.py` & `returnn-1.20230704.111750/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230704.111750/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230704.111750/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230704.111750/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/dim.py` & `returnn-1.20230704.111750/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/marked_dim.py` & `returnn-1.20230704.111750/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/tensor.py` & `returnn-1.20230704.111750/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/tensor_dict.py` & `returnn-1.20230704.111750/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tensor/utils.py` & `returnn-1.20230704.111750/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/compat.py` & `returnn-1.20230704.111750/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/data_pipeline.py` & `returnn-1.20230704.111750/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/distributed.py` & `returnn-1.20230704.111750/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/engine.py` & `returnn-1.20230704.111750/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230704.111750/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230704.111750/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/horovod.py` & `returnn-1.20230704.111750/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230704.111750/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/layers/base.py` & `returnn-1.20230704.111750/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/layers/basic.py` & `returnn-1.20230704.111750/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/layers/rec.py` & `returnn-1.20230704.111750/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/layers/segmental_model.py` & `returnn-1.20230704.111750/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/layers/signal_processing.py` & `returnn-1.20230704.111750/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/layers/variable.py` & `returnn-1.20230704.111750/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/native_op.py` & `returnn-1.20230704.111750/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/network.py` & `returnn-1.20230704.111750/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/sprint.py` & `returnn-1.20230704.111750/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/updater.py` & `returnn-1.20230704.111750/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/util/basic.py` & `returnn-1.20230704.111750/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/util/data.py` & `returnn-1.20230704.111750/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20230704.111750/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/util/ken_lm.py` & `returnn-1.20230704.111750/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/tf/util/open_fst.py` & `returnn-1.20230704.111750/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/data/pipeline.py` & `returnn-1.20230704.111750/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230704.111750/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/data/tensor_utils.py` & `returnn-1.20230704.111750/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/distributed.py` & `returnn-1.20230704.111750/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/engine.py` & `returnn-1.20230704.111750/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/frontend/_backend.py` & `returnn-1.20230704.111750/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/frontend/_rand.py` & `returnn-1.20230704.111750/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/frontend/bridge.py` & `returnn-1.20230704.111750/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/torch/updater.py` & `returnn-1.20230704.111750/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/basic.py` & `returnn-1.20230704.111750/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/better_exchook.py` & `returnn-1.20230704.111750/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/bpe.py` & `returnn-1.20230704.111750/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/debug.py` & `returnn-1.20230704.111750/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/debug_helpers.py` & `returnn-1.20230704.111750/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/fsa.py` & `returnn-1.20230704.111750/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230704.111750/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/pprint.py` & `returnn-1.20230704.111750/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/py-to-pickle.cpp` & `returnn-1.20230704.111750/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/sig_proc.py` & `returnn-1.20230704.111750/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn/util/task_system.py` & `returnn-1.20230704.111750/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/returnn.egg-info/PKG-INFO` & `returnn-1.20230704.111750/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230703.193930
+Version: 1.20230704.111750
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230703.193930/returnn.egg-info/SOURCES.txt` & `returnn-1.20230704.111750/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/setup.py` & `returnn-1.20230704.111750/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/DummySprintExec.py` & `returnn-1.20230704.111750/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230704.111750/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230704.111750/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230704.111750/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/_set_num_threads1.py` & `returnn-1.20230704.111750/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/_setup_test_env.py` & `returnn-1.20230704.111750/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/bpe-unicode-demo.codes` & `returnn-1.20230704.111750/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/bpe-unicode-demo.vocab` & `returnn-1.20230704.111750/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/lexicon_opt.isyms` & `returnn-1.20230704.111750/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/lexicon_opt.jpg` & `returnn-1.20230704.111750/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/lint_common.py` & `returnn-1.20230704.111750/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/pycharm-inspect.py` & `returnn-1.20230704.111750/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/pylint.py` & `returnn-1.20230704.111750/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/returnn-as-framework.py` & `returnn-1.20230704.111750/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/rf_utils.py` & `returnn-1.20230704.111750/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/spelling.dic` & `returnn-1.20230704.111750/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_Config.py` & `returnn-1.20230704.111750/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_Dataset.py` & `returnn-1.20230704.111750/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_Fsa.py` & `returnn-1.20230704.111750/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_GeneratingDataset.py` & `returnn-1.20230704.111750/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_HDFDataset.py` & `returnn-1.20230704.111750/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_LearningRateControl.py` & `returnn-1.20230704.111750/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_Log.py` & `returnn-1.20230704.111750/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_MultiProcDataset.py` & `returnn-1.20230704.111750/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_PTDataset.py` & `returnn-1.20230704.111750/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_Pretrain.py` & `returnn-1.20230704.111750/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_ResNet.py` & `returnn-1.20230704.111750/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_SprintDataset.py` & `returnn-1.20230704.111750/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_SprintInterface.py` & `returnn-1.20230704.111750/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TFEngine.py` & `returnn-1.20230704.111750/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TFNativeOp.py` & `returnn-1.20230704.111750/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TFNetworkLayer.py` & `returnn-1.20230704.111750/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230704.111750/tests/test_TFNetworkRecLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12972,14 +12972,297 @@
             ),
         ]
         assert len(collected_pos_encs) == len(ref_pos_encs) == n_time
         for i in range(n_time):
             assert_allclose(ref_pos_encs[i], collected_pos_encs[i], rtol=1e-06, err_msg=f"step {i}")
 
 
+def test_rel_pos_self_attention_left_ctx_explicit_vs_layer():
+    # We have some left context, which we want to add to the keys and values,
+    # but not to the queries.
+    # We can either implement self-attention by hand,
+    # or use the layer, but for the layer, it operates on the whole sequence,
+    # so it would calculate unnecessary queries for the left context,
+    # and we would then slice the output.
+    # So via the layer, it would be less efficient.
+    # Anyway, this test here is to compare both outputs for equality.
+    # Additionally, it uses relative positional encoding.
+    # Originally, the concatenated input was [B*C, 2*W, D].
+
+    import math
+    from returnn.tensor import batch_dim
+    from test_TFNetworkLayer import make_feed_dict
+
+    n_total_dim = 64
+    n_head = 2
+    enc_att_num_heads_dim = Dim(n_head, name="heads")
+    enc_dim_per_head_dim = Dim(n_total_dim // n_head, name="dim_per_head")
+    chunk_size_dim = Dim(23, name="chunk_size")
+    concat_window_dim = 2 * chunk_size_dim
+    in_feat_dim = Dim(13, name="in_feat")
+
+    extern_data_dict = {
+        "left_ctx": {
+            "dim_tags": [batch_dim, chunk_size_dim, in_feat_dim],
+            "time_dim_axis": 1,
+            "available_for_inference": True,
+        },
+        "data": {"dim_tags": [batch_dim, chunk_size_dim, in_feat_dim], "time_dim_axis": 1},
+    }
+
+    net_dict_common = {
+        "conformer_block_01_self_att_ln": {"class": "copy", "from": "data"},
+        "conformer_block_01_self_att_ln_concat": {
+            "class": "concat",
+            "from": [("data:left_ctx", chunk_size_dim), ("data", chunk_size_dim)],
+            "out_dim": concat_window_dim,
+        },
+        "output": {"class": "copy", "from": "conformer_block_01_self_att_dropout"},
+    }
+
+    net_dict_w_layer = {
+        "conformer_block_01_self_att_ln_rel_pos_enc": {
+            "class": "relative_positional_encoding",
+            "clipping": 16,
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', "
+            "scale=1.0)",
+            "from": "conformer_block_01_self_att_ln_concat",  # [B*C, 2*W, D]
+            "n_out": n_total_dim // n_head,
+        },
+        "conformer_block_01_self_att": {
+            "attention_dropout": 0.1,
+            "class": "self_attention",
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', scale=0.5)",
+            "from": "conformer_block_01_self_att_ln_concat",
+            "key_shift": "conformer_block_01_self_att_ln_rel_pos_enc",
+            "n_out": n_total_dim,
+            "num_heads": n_head,
+            "total_key_dim": n_total_dim,
+        },
+        "conformer_block_01_self_att_splits": {
+            "axis": "T",
+            "class": "split",
+            "from": "conformer_block_01_self_att",
+            "num_splits": 2,
+        },
+        "conformer_block_01_self_att_split_2": {
+            "class": "copy",
+            "from": "conformer_block_01_self_att_splits/1",
+        },
+        "conformer_block_01_self_att_linear": {
+            "L2": 0.0001,
+            "activation": None,
+            "class": "linear",
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', scale=1.0)",
+            "from": "conformer_block_01_self_att_split_2",
+            "n_out": n_total_dim,
+            "with_bias": False,
+        },
+        "conformer_block_01_self_att_dropout": {
+            "class": "dropout",
+            "dropout": 0.1,
+            "from": "conformer_block_01_self_att_linear",
+        },
+    }
+
+    net_dict_explicit = {
+        "conformer_block_01_self_att_ln_K": {
+            "L2": 0.0,
+            "class": "linear",
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', scale=0.5)",
+            "from": "conformer_block_01_self_att_ln_concat",  # [B*C, 2*W, D]
+            "n_out": n_total_dim,
+            "with_bias": False,
+        },
+        "conformer_block_01_self_att_ln_K_H": {
+            "axis": "f",
+            "class": "split_dims",
+            "dims": (enc_att_num_heads_dim, enc_dim_per_head_dim),
+            "from": "conformer_block_01_self_att_ln_K",
+        },
+        "conformer_block_01_self_att_ln_Q": {
+            "L2": 0.0,
+            "class": "linear",
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', scale=0.5)",
+            "from": "conformer_block_01_self_att_ln",  # [B*C, W, D]
+            "n_out": n_total_dim,
+            "with_bias": False,
+        },
+        "conformer_block_01_self_att_ln_Q_H": {
+            "axis": "f",
+            "class": "split_dims",
+            "dims": (enc_att_num_heads_dim, enc_dim_per_head_dim),
+            "from": "conformer_block_01_self_att_ln_Q",
+        },
+        "conformer_block_01_self_att_ln_V": {
+            "L2": 0.0,
+            "class": "linear",
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', scale=0.5)",
+            "from": "conformer_block_01_self_att_ln_concat",
+            "n_out": n_total_dim,
+            "with_bias": False,
+        },
+        "conformer_block_01_self_att_ln_V_H": {
+            "axis": "f",
+            "class": "split_dims",
+            "dims": (enc_att_num_heads_dim, enc_dim_per_head_dim),
+            "from": "conformer_block_01_self_att_ln_V",
+        },
+        "conformer_block_01_self_att_ln_energy": {
+            "class": "dot",
+            "from": [
+                "conformer_block_01_self_att_ln_K_H",
+                "conformer_block_01_self_att_ln_Q_H",
+            ],
+            "reduce": enc_dim_per_head_dim,
+            "var1": "auto",
+            "var2": "auto",
+        },
+        "conformer_block_01_self_att_ln_rel_pos_enc": {
+            "class": "relative_positional_encoding",
+            "clipping": 16,
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', "
+            "scale=1.0)",
+            "from": "conformer_block_01_self_att_ln_concat",
+            "key_value_spatial_dim": concat_window_dim,
+            "out_dim": enc_dim_per_head_dim,
+            "query_offset": chunk_size_dim.dimension,
+            "query_spatial_dim": chunk_size_dim,
+        },
+        "conformer_block_01_self_att_ln_energy_rel_pos": {
+            "class": "dot",
+            "from": [
+                "conformer_block_01_self_att_ln_Q_H",
+                "conformer_block_01_self_att_ln_rel_pos_enc",
+            ],
+            "reduce": enc_dim_per_head_dim,
+            "var1": "auto",
+            "var2": "auto",
+        },
+        "conformer_block_01_self_att_ln_energy_": {
+            "allow_broadcast_all_sources": False,
+            "class": "combine",
+            "from": [
+                "conformer_block_01_self_att_ln_energy",
+                "conformer_block_01_self_att_ln_energy_rel_pos",
+            ],
+            "kind": "add",
+        },
+        "conformer_block_01_self_att_ln_weights": {
+            "class": "softmax_over_spatial",
+            "energy_factor": 1 / math.sqrt(enc_dim_per_head_dim.dimension),
+            "from": "conformer_block_01_self_att_ln_energy_",
+        },
+        "conformer_block_01_self_att_ln_weights_drop": {
+            "class": "dropout",
+            "dropout": 0.1,
+            "dropout_noise_shape": {"*": None},
+            "from": "conformer_block_01_self_att_ln_weights",
+        },
+        "conformer_block_01_self_att_ln_att0": {
+            "class": "dot",
+            "from": [
+                "conformer_block_01_self_att_ln_weights_drop",
+                "conformer_block_01_self_att_ln_V_H",
+            ],
+            "reduce": concat_window_dim,
+            "var1": "auto",
+            "var2": "auto",
+        },
+        "conformer_block_01_self_att_ln_att_": {
+            "axes": (enc_att_num_heads_dim, enc_dim_per_head_dim),
+            "class": "merge_dims",
+            "from": "conformer_block_01_self_att_ln_att0",
+        },
+        "conformer_block_01_self_att_ln_att": {
+            "class": "reinterpret_data",
+            "from": "conformer_block_01_self_att_ln_att_",
+            "set_axes": {"T": f"dim:{chunk_size_dim.dimension}"},
+        },
+        "conformer_block_01_self_att_linear": {
+            "L2": 0.0001,
+            "activation": None,
+            "class": "linear",
+            "forward_weights_init": "variance_scaling_initializer(mode='fan_avg', distribution='uniform', scale=1.0)",
+            "from": "conformer_block_01_self_att_ln_att",
+            "n_out": n_total_dim,
+            "with_bias": False,
+        },
+        "conformer_block_01_self_att_dropout": {
+            "class": "dropout",
+            "dropout": 0.1,
+            "from": "conformer_block_01_self_att_linear",
+        },
+    }
+
+    with make_scope() as session:
+        net_dict = {**net_dict_common, **net_dict_w_layer}
+        net = TFNetwork(config=Config({"extern_data": extern_data_dict}))
+        net.construct_from_dict(net_dict)
+        net.initialize_params(session=session)
+        params_serialized = net.get_params_serialized(session=session)
+
+        out = net.get_default_output_layer().output
+        k_raw = session.graph.get_tensor_by_name("conformer_block_01_self_att/qkv_1:1")  # (B,H,2*W,D//H)
+        feed_dict = make_feed_dict(net.extern_data)
+        outputs_w_layer_v = session.run(
+            {
+                "input_concat": net.layers["conformer_block_01_self_att_ln_concat"].output.placeholder,
+                "k_raw": k_raw,
+                "output": out.placeholder,
+            },
+            feed_dict=feed_dict,
+        )
+
+    # Convert params.
+    att_params = params_serialized.values_dict.pop("conformer_block_01_self_att")
+    qkv_matrix = att_params.pop("QKV")
+    assert qkv_matrix.shape == (in_feat_dim.dimension, n_total_dim * 3)
+    # Note: Just numpy.split is wrong, because SelfAttentionLayer does matmul first on all,
+    # then reshapes (separate head), then splits.
+    # In the explicit variant here, we however do separate matmuls,
+    # then reshape.
+    qkv_matrix_ = qkv_matrix.reshape((in_feat_dim.dimension, n_head, 3, n_total_dim // n_head))
+    q_mat = qkv_matrix_[:, :, 0, :].reshape((in_feat_dim.dimension, n_total_dim))
+    k_mat = qkv_matrix_[:, :, 1, :].reshape((in_feat_dim.dimension, n_total_dim))
+    v_mat = qkv_matrix_[:, :, 2, :].reshape((in_feat_dim.dimension, n_total_dim))
+    params_serialized.values_dict["conformer_block_01_self_att_ln_Q"] = {"W": q_mat}
+    params_serialized.values_dict["conformer_block_01_self_att_ln_K"] = {"W": k_mat}
+    params_serialized.values_dict["conformer_block_01_self_att_ln_V"] = {"W": v_mat}
+
+    with make_scope() as session:
+        net_dict = {**net_dict_common, **net_dict_explicit}
+        net = TFNetwork(config=Config({"extern_data": extern_data_dict}))
+        net.construct_from_dict(net_dict)
+        net.set_params_by_serialized(params_serialized, session=session)
+
+        out = net.get_default_output_layer().output
+        keys = net.layers["conformer_block_01_self_att_ln_K"].output  # (B,2*W,D)
+        k_raw = tf.reshape(
+            keys.placeholder, [batch_dim.get_dim_value(), concat_window_dim.dimension, n_head, n_total_dim // n_head]
+        )  # (B,2*W,H,D//H)
+        k_raw = tf.transpose(k_raw, [0, 2, 1, 3])  # (B,H,2*W,D//H)
+        feed_dict = make_feed_dict(net.extern_data)
+        outputs_explicit_v = session.run(
+            {
+                "input_concat": net.layers["conformer_block_01_self_att_ln_concat"].output.placeholder,
+                "k_raw": k_raw,
+                "output": out.placeholder,
+            },
+            feed_dict=feed_dict,
+        )
+
+        assert set(outputs_w_layer_v.keys()) == set(outputs_explicit_v.keys())
+        for k in outputs_w_layer_v.keys():
+            print(f"*** Compare {k} ***")
+            w_layer_v = outputs_w_layer_v[k]
+            explicit_v = outputs_explicit_v[k]
+            assert_allclose(w_layer_v, explicit_v, rtol=1e-5, atol=1e-5, err_msg=f"{k} different")
+
+
 def _build_self_attention_layer(
     d, input, output, inside_rec_layer, query_axis=None, num_heads=3, key_dim=7, value_dim=11, dropout=0.0
 ):
     """
     Essentially this does
       d[output + '_att'] = {"class": "self_attention", "num_heads": num_heads,
         "total_key_dim": num_heads * key_dim,
```

### Comparing `returnn-1.20230703.193930/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230704.111750/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TFUpdater.py` & `returnn-1.20230704.111750/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TFUtil.py` & `returnn-1.20230704.111750/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TF_determinism.py` & `returnn-1.20230704.111750/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TaskSystem.py` & `returnn-1.20230704.111750/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230704.111750/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_TranslationDataset.py` & `returnn-1.20230704.111750/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_Util.py` & `returnn-1.20230704.111750/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_demos.py` & `returnn-1.20230704.111750/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_fork_exec.py` & `returnn-1.20230704.111750/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_hdf_dump.py` & `returnn-1.20230704.111750/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_array.py` & `returnn-1.20230704.111750/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_attention.py` & `returnn-1.20230704.111750/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_base.py` & `returnn-1.20230704.111750/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_cond.py` & `returnn-1.20230704.111750/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_const.py` & `returnn-1.20230704.111750/tests/test_rf_const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_container.py` & `returnn-1.20230704.111750/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_conv.py` & `returnn-1.20230704.111750/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_encoder_conformer.py` & `returnn-1.20230704.111750/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_loop.py` & `returnn-1.20230704.111750/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_math.py` & `returnn-1.20230704.111750/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_normalization.py` & `returnn-1.20230704.111750/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_rec.py` & `returnn-1.20230704.111750/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_reduce.py` & `returnn-1.20230704.111750/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_rf_signal.py` & `returnn-1.20230704.111750/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_tensor.py` & `returnn-1.20230704.111750/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_tools.py` & `returnn-1.20230704.111750/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_torch_engine.py` & `returnn-1.20230704.111750/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_torch_frontend.py` & `returnn-1.20230704.111750/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tests/test_torch_internal_frontend.py` & `returnn-1.20230704.111750/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/analyze-dataset-batches.py` & `returnn-1.20230704.111750/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/bliss-collect-seq-lens.py` & `returnn-1.20230704.111750/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/bliss-dump-text.py` & `returnn-1.20230704.111750/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/bliss-get-segment-names.py` & `returnn-1.20230704.111750/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/bliss-to-ogg-zip.py` & `returnn-1.20230704.111750/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/bpe-create-lexicon.py` & `returnn-1.20230704.111750/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/calculate-word-error-rate.py` & `returnn-1.20230704.111750/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/cleanup-old-models.py` & `returnn-1.20230704.111750/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/collect-orth-symbols.py` & `returnn-1.20230704.111750/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/collect-words.py` & `returnn-1.20230704.111750/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/compile_native_op.py` & `returnn-1.20230704.111750/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/compile_tf_graph.py` & `returnn-1.20230704.111750/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/debug-dump-search-scores.py` & `returnn-1.20230704.111750/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/debug-plot-search-scores.py` & `returnn-1.20230704.111750/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/dump-dataset-raw-strings.py` & `returnn-1.20230704.111750/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/dump-dataset.py` & `returnn-1.20230704.111750/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/dump-forward-stats.py` & `returnn-1.20230704.111750/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/dump-forward.py` & `returnn-1.20230704.111750/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/dump-network-json.py` & `returnn-1.20230704.111750/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/dump-pickle.py` & `returnn-1.20230704.111750/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230704.111750/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/get-attention-weights.py` & `returnn-1.20230704.111750/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/get-best-model-epoch.py` & `returnn-1.20230704.111750/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/hdf_dump.py` & `returnn-1.20230704.111750/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230704.111750/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/import-blocks-mt-model.py` & `returnn-1.20230704.111750/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/import-t2t-mt-model.py` & `returnn-1.20230704.111750/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/Makefile` & `returnn-1.20230704.111750/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/README.md` & `returnn-1.20230704.111750/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/example/README.md` & `returnn-1.20230704.111750/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230704.111750/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230704.111750/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230704.111750/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/file.h` & `returnn-1.20230704.111750/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230704.111750/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230704.111750/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/main.cc` & `returnn-1.20230704.111750/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230704.111750/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230704.111750/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230704.111750/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/tf_avg_checkpoints.py` & `returnn-1.20230704.111750/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/tf_inspect_checkpoint.py` & `returnn-1.20230704.111750/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/tf_inspect_summary_log.py` & `returnn-1.20230704.111750/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.193930/tools/torch_export_to_onnx.py` & `returnn-1.20230704.111750/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

