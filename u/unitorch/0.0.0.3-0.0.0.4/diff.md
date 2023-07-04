# Comparing `tmp/unitorch-0.0.0.3.tar.gz` & `tmp/unitorch-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitorch-0.0.0.3.tar", last modified: Wed Jun 14 07:40:32 2023, max compression
+gzip compressed data, was "unitorch-0.0.0.4.tar", last modified: Tue Jul  4 07:55:37 2023, max compression
```

## Comparing `unitorch-0.0.0.3.tar` & `unitorch-0.0.0.4.tar`

### file list

```diff
@@ -1,465 +1,471 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.051503 unitorch-0.0.0.3/.pytest_cache/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-14 07:40:17.000000 unitorch-0.0.0.3/.pytest_cache/README.md
--rw-r--r--   0 root         (0) root         (0)     1085 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8985 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7956 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.051503 unitorch-0.0.0.3/benchmarks/
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/benchmarks/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.055503 unitorch-0.0.0.3/docs/search/
--rw-r--r--   0 root         (0) root         (0)  1019191 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/docs/search/search_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.059503 unitorch-0.0.0.3/examples/
--rw-r--r--   0 root         (0) root         (0)     2311 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/examples/configs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.059503 unitorch-0.0.0.3/examples/configs/caption/
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.063503 unitorch-0.0.0.3/examples/configs/classification/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)     1700 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/clip.ini
--rw-r--r--   0 root         (0) root         (0)     1688 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/image_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.063503 unitorch-0.0.0.3/examples/configs/classification/lora/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1857 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1806 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1556 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/roberta.ini
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/swin.ini
--rw-r--r--   0 root         (0) root         (0)     1636 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/text_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.067503 unitorch-0.0.0.3/examples/configs/generation/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1666 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/chatglm.ini
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/llama.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/configs/generation/lora/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/mbart.ini
--rw-r--r--   0 root         (0) root         (0)     1597 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/mt5.ini
--rw-r--r--   0 root         (0) root         (0)     1655 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/pegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1587 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/t5.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/xpegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1745 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/xprophetnet.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/configs/pretrain/
--rw-r--r--   0 root         (0) root         (0)     1266 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/pretrain/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/examples/configs/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/configs/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/services/zip_image/config.ini
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/services/zip_image/config_v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/examples/hub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/hub/caption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/hub/classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/classification/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/hub/generation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/generation/llama.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/generation/xpegasus.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/notebooks/
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/notebooks/README.md
--rw-r--r--   0 root         (0) root         (0)     1861 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/src/unitorch/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/src/unitorch/cli/
--rw-r--r--   0 root         (0) root         (0)     6024 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.079503 unitorch-0.0.0.3/src/unitorch/cli/console/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/eval.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/infer.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/script.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/service.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/train.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.079503 unitorch-0.0.0.3/src/unitorch/cli/datasets/
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12406 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/datasets/hf.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.079503 unitorch-0.0.0.3/src/unitorch/cli/loss/
--rw-r--r--   0 root         (0) root         (0)     4063 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.083503 unitorch-0.0.0.3/src/unitorch/cli/models/
--rw-r--r--   0 root         (0) root         (0)     2787 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.083503 unitorch-0.0.0.3/src/unitorch/cli/models/bart/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.087503 unitorch-0.0.0.3/src/unitorch/cli/models/beit/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.087503 unitorch-0.0.0.3/src/unitorch/cli/models/bert/
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.087503 unitorch-0.0.0.3/src/unitorch/cli/models/blip/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22703 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7788 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.091503 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13026 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8321 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.091503 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13764 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)     9143 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/classification_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.091503 unitorch-0.0.0.3/src/unitorch/cli/models/clip/
--rw-r--r--   0 root         (0) root         (0)     2514 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16125 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.095503 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/
--rw-r--r--   0 root         (0) root         (0)     4492 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing_v2.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/detection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.095503 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)     2807 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/processing_stable.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/label_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.099503 unitorch-0.0.0.3/src/unitorch/cli/models/llama/
--rw-r--r--   0 root         (0) root         (0)     1429 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14017 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8206 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.099503 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      887 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/processing.py
--rw-r--r--   0 root         (0) root         (0)    15281 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/modeling_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.099503 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7125 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5815 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.103504 unitorch-0.0.0.3/src/unitorch/cli/models/peft/
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30502 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_bloom.py
--rw-r--r--   0 root         (0) root         (0)    30560 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_llama.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.103504 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.103504 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/processing.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/random_utils.py
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/ranking_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.107504 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/segmentation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.107504 unitorch-0.0.0.3/src/unitorch/cli/models/swin/
--rw-r--r--   0 root         (0) root         (0)     3032 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.107504 unitorch-0.0.0.3/src/unitorch/cli/models/t5/
--rw-r--r--   0 root         (0) root         (0)     1282 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5811 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.111503 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)     1310 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8538 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.111503 unitorch-0.0.0.3/src/unitorch/cli/models/vit/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.111503 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)     2314 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7238 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7811 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/optim/
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/scheduler/
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/score/
--rw-r--r--   0 root         (0) root         (0)    14137 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/score/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/scripts/
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scripts/README.md
--rw-r--r--   0 root         (0) root         (0)      213 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/services/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/cli/tasks/
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26523 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/tasks/deepspeed.py
--rw-r--r--   0 root         (0) root         (0)    31557 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/tasks/supervised.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/cli/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/cli/writer/
--rw-r--r--   0 root         (0) root         (0)    10545 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/datasets/
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6832 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/datasets/hf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/loss/
--rw-r--r--   0 root         (0) root         (0)     4712 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/loss/prophetnet.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.127504 unitorch-0.0.0.3/src/unitorch/models/
--rw-r--r--   0 root         (0) root         (0)     7429 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.127504 unitorch-0.0.0.3/src/unitorch/models/bart/
--rw-r--r--   0 root         (0) root         (0)      204 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13544 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.127504 unitorch-0.0.0.3/src/unitorch/models/beit/
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.131504 unitorch-0.0.0.3/src/unitorch/models/bert/
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8355 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.131504 unitorch-0.0.0.3/src/unitorch/models/blip/
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30316 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7700 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.131504 unitorch-0.0.0.3/src/unitorch/models/bloom/
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10867 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     9140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.135504 unitorch-0.0.0.3/src/unitorch/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4201 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11157 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)    55823 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11091 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/tokenization_chatglm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.139504 unitorch-0.0.0.3/src/unitorch/models/clip/
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15100 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4393 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.139504 unitorch-0.0.0.3/src/unitorch/models/deberta/
--rw-r--r--   0 root         (0) root         (0)      424 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/processing_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/processing_stable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/llama/
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11334 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      188 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13928 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mbart/processing.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/modeling_ema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/mt5/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14219 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.147504 unitorch-0.0.0.3/src/unitorch/models/peft/
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9891 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9487 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_lora.py
--rw-r--r--   0 root         (0) root         (0)    10082 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9266 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_lora.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.147504 unitorch-0.0.0.3/src/unitorch/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13604 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.151504 unitorch-0.0.0.3/src/unitorch/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/prophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.151504 unitorch-0.0.0.3/src/unitorch/models/roberta/
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/swin/
--rw-r--r--   0 root         (0) root         (0)      193 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/t5/
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13285 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/vit/
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.159504 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.159504 unitorch-0.0.0.3/src/unitorch/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13693 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.159504 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)      212 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13514 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/modules/
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/modules/replace/
--rw-r--r--   0 root         (0) root         (0)      199 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14643 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/beam_search_v2.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/datasets_v2.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/hf_hub_v2.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/timm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/ops/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16794 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/ops/dyhead.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/ops/ngram_repeat_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/optim/
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/rl/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/rl/utils/buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/scheduler/
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/score/
--rw-r--r--   0 root         (0) root         (0)     1896 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/bleu.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/map.py
--rw-r--r--   0 root         (0) root         (0)    13291 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/rouge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/tasks/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.171504 unitorch-0.0.0.3/src/unitorch/utils/
--rw-r--r--   0 root         (0) root         (0)    13580 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/functional.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/palette.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/torch_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/src/unitorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8985 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12862 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      287 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.175505 unitorch-0.0.0.3/wiki/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.175505 unitorch-0.0.0.3/wiki/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/benchmarks/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.179504 unitorch-0.0.0.3/wiki/cli/
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/ast.md
--rw-r--r--   0 root         (0) root         (0)      173 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/csv.md
--rw-r--r--   0 root         (0) root         (0)      414 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/datatypes.md
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/deepspeed.md
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/jsonl.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/cli/models/
--rw-r--r--   0 root         (0) root         (0)      348 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/bert.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      783 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      353 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/index.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      359 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      337 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      368 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      664 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      425 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/parquet.md
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/postprocess.md
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/preprocess.md
--rw-r--r--   0 root         (0) root         (0)      192 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/supervised.md
--rw-r--r--   0 root         (0) root         (0)     4600 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/configuration.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.051503 unitorch-0.0.0.3/wiki/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/examples/caption/
--rw-r--r--   0 root         (0) root         (0)     4659 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/caption/blip.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/examples/classification/
--rw-r--r--   0 root         (0) root         (0)     4208 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/classification/clip.md
--rw-r--r--   0 root         (0) root         (0)     4130 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/classification/roberta.md
--rw-r--r--   0 root         (0) root         (0)     4525 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/classification/swin.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/examples/diffusion/
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/diffusion/controlnet.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.191505 unitorch-0.0.0.3/wiki/examples/generation/
--rw-r--r--   0 root         (0) root         (0)     4145 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/generation/bart.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.191505 unitorch-0.0.0.3/wiki/examples/service/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/service/zip_image.md
--rw-r--r--   0 root         (0) root         (0)     1346 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/index.md
--rw-r--r--   0 root         (0) root         (0)      890 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.191505 unitorch-0.0.0.3/wiki/labs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/labs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/wiki/models/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/bert.md
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      383 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/index.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      243 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      375 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)     4524 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/overview.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/.pytest_cache/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-07-04 07:55:29.000000 unitorch-0.0.0.4/.pytest_cache/README.md
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8991 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7956 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/benchmarks/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.553682 unitorch-0.0.0.4/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/docs/search/
+-rw-r--r--   0 root         (0) root         (0)  1019279 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/docs/search/search_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.573682 unitorch-0.0.0.4/examples/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/examples/configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.573682 unitorch-0.0.0.4/examples/configs/caption/
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/classification/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/clip.ini
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/image_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/classification/lora/
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/roberta.ini
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/swin.ini
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/text_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/diffusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/diffusion/controlnet/
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/controlnet/canny.ini
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/stable-v1.5.ini
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/stable-v2.1.ini
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/stable-v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.581682 unitorch-0.0.0.4/examples/configs/generation/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/chatglm.ini
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/llama.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.581682 unitorch-0.0.0.4/examples/configs/generation/lora/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/mbart.ini
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/mt5.ini
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/pegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/t5.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/xpegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/xprophetnet.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.581682 unitorch-0.0.0.4/examples/configs/pretrain/
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/pretrain/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/examples/configs/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/configs/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/services/zip_image/config.ini
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/services/zip_image/config_v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/examples/hub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/hub/caption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/hub/classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/classification/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/hub/generation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/generation/llama.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/generation/xpegasus.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/notebooks/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/notebooks/README.md
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/src/unitorch/
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/
+-rw-r--r--   0 root         (0) root         (0)     6024 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/console/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/eval.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/script.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/service.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/train.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/datasets/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12406 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/datasets/hf.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/loss/
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/bart/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/beit/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/bert/
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.601682 unitorch-0.0.0.4/src/unitorch/cli/models/blip/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22703 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7788 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.601682 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13026 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8321 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.601682 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13764 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)     9143 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/classification_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.605682 unitorch-0.0.0.4/src/unitorch/cli/models/clip/
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16125 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.605682 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/detection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3879 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/processing_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/label_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/llama/
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14017 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8206 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15281 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/modeling_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7125 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/peft/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30502 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_bloom.py
+-rw-r--r--   0 root         (0) root         (0)    30560 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_llama.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.613682 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.613682 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/processing.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/random_utils.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/ranking_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.613682 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/segmentation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/swin/
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/t5/
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8538 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/vit/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7533 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7237 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7811 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/optim/
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/score/
+-rw-r--r--   0 root         (0) root         (0)    14139 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/score/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/scripts/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scripts/README.md
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/services/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/tasks/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26512 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/tasks/deepspeed.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/tasks/supervised.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/cli/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/cli/writer/
+-rw-r--r--   0 root         (0) root         (0)    10544 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/datasets/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6832 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/datasets/hf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/loss/
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/loss/prophetnet.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/models/
+-rw-r--r--   0 root         (0) root         (0)     7474 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.633682 unitorch-0.0.0.4/src/unitorch/models/bart/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.633682 unitorch-0.0.0.4/src/unitorch/models/beit/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.633682 unitorch-0.0.0.4/src/unitorch/models/bert/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8355 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.637682 unitorch-0.0.0.4/src/unitorch/models/blip/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30316 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7700 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.637682 unitorch-0.0.0.4/src/unitorch/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     9140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.641682 unitorch-0.0.0.4/src/unitorch/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11157 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    55823 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/tokenization_chatglm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.641682 unitorch-0.0.0.4/src/unitorch/models/clip/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15100 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.641682 unitorch-0.0.0.4/src/unitorch/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/processing_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.645682 unitorch-0.0.0.4/src/unitorch/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)      548 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     8201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/processing_stable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.645682 unitorch-0.0.0.4/src/unitorch/models/llama/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.649682 unitorch-0.0.0.4/src/unitorch/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13928 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mbart/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/modeling_ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.649682 unitorch-0.0.0.4/src/unitorch/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14219 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.649682 unitorch-0.0.0.4/src/unitorch/models/peft/
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9891 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9487 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_lora.py
+-rw-r--r--   0 root         (0) root         (0)    10082 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9266 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_lora.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/prophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/swin/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/t5/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13285 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/vit/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.661682 unitorch-0.0.0.4/src/unitorch/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13710 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.661682 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13514 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.661682 unitorch-0.0.0.4/src/unitorch/modules/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/modules/replace/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14643 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/beam_search_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/datasets_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/hf_hub_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/timm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/ops/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16794 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/ops/dyhead.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/ops/ngram_repeat_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/optim/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/rl/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/rl/utils/buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.669682 unitorch-0.0.0.4/src/unitorch/score/
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/map.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/rouge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.669682 unitorch-0.0.0.4/src/unitorch/tasks/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.669682 unitorch-0.0.0.4/src/unitorch/utils/
+-rw-r--r--   0 root         (0) root         (0)    13636 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/functional.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/palette.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/torch_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/src/unitorch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8991 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13037 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      287 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.673682 unitorch-0.0.0.4/wiki/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.673682 unitorch-0.0.0.4/wiki/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/benchmarks/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.673682 unitorch-0.0.0.4/wiki/cli/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/ast.md
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/csv.md
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/datatypes.md
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/deepspeed.md
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/jsonl.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.681682 unitorch-0.0.0.4/wiki/cli/models/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/parquet.md
+-rw-r--r--   0 root         (0) root         (0)      851 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/postprocess.md
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/preprocess.md
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/supervised.md
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/wiki/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.681682 unitorch-0.0.0.4/wiki/examples/caption/
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/caption/blip.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/classification/
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/classification/clip.md
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/classification/roberta.md
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/classification/swin.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/diffusion/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/diffusion/controlnet.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/generation/
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/generation/bart.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/service/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/service/zip_image.md
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/index.md
+-rw-r--r--   0 root         (0) root         (0)      890 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/labs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/labs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/wiki/models/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/overview.md
```

### Comparing `unitorch-0.0.0.3/LICENSE` & `unitorch-0.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/PKG-INFO` & `unitorch-0.0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
+Provides-Extra: accelerate
 Provides-Extra: chatglm
-Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
```

### Comparing `unitorch-0.0.0.3/README.md` & `unitorch-0.0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/docs/search/search_index.json` & `unitorch-0.0.0.4/docs/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991302972802023%*

 * *Differences: {"'docs'": "{27: {'text': '<pre><code>infer(\\n    postprocess_fn: str,\\n    writer: str,\\n    "*

 * *           'test_batch_size: Optional[int] = 128,\\n    pin_memory: Optional[bool] = True,\\n    '*

 * *           'num_workers: Optional[int] = 4,\\n    max_size: Optional[int] = 10000,\\n    '*

 * *           'from_ckpt_dir: Optional[str] = "./from_ckpt",\\n    output_header: Optional[List] = '*

 * *           'None,\\n    output_path: Optional[str] = "./cache/predict.txt",\\n    '*

 * *           'postprocess_workers: Optional […]*

```diff
@@ -142,20 +142,20 @@
         {
             "location": "cli/deepspeed/#unitorch.cli.tasks.deepspeed.DeepspeedTask.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create a DeepspeedTask instance from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Type Description <p>A DeepspeedTask instance.</p> Source code in <code>src/unitorch/cli/tasks/deepspeed.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/task/deepspeed/supervised\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create a DeepspeedTask instance from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        A DeepspeedTask instance.\n    \"\"\"\n    try:\n        deepspeed.init_distributed(dist_backend=\"nccl\", init_method=\"env://\")\n    except:\n        logging.info(\"PyTorch is not in distributed mode\")\n\n    config.set_default_section(\"core/task/deepspeed/supervised\")\n\n    model = config.getoption(\"model\", None)\n    dataset = config.getoption(\"dataset\", None)\n\n    if model is not None:\n        model = init_registered_module(model, config, registered_model)\n\n    if dataset is not None:\n        dataset = init_registered_module(dataset, config, registered_dataset)\n\n    local_rank = config.getdefault(\n        \"core/cli\",\n        \"local_rank\",\n        get_local_rank(),\n    )\n\n    return dict(\n        configure=config,\n        model=model,\n        datasets=dataset,\n        local_rank=local_rank,\n    )\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/deepspeed/#unitorch.cli.tasks.deepspeed.DeepspeedTask.infer",
-            "text": "<pre><code>infer(\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Perform inference using the trained model.</p> <p>Parameters:</p> Name Type Description Default <code>postprocess_fn</code> <code>str</code> <p>The post-processing function for inference.</p> required <code>writer</code> <code>str</code> <p>The writer for writing the results.</p> required <code>test_batch_size</code> <code>optional</code> <p>The batch size for inference. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>max_size</code> <code>optional</code> <p>The maximum size of the dataset for inference. Defaults to 10000.</p> <code>10000</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>output_header</code> <code>optional</code> <p>The header for the output file. Defaults to None.</p> <code>None</code> <code>output_path</code> <code>optional</code> <p>The path to save the output file. Defaults to \"./cache/predict.txt\".</p> <code>'./cache/predict.txt'</code> <code>postprocess_workers</code> <code>optional</code> <p>The number of worker processes for post-processing. Defaults to 2.</p> <code>2</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/deepspeed.py</code> <pre><code>@torch.no_grad()\n@add_default_section_for_function(\"core/task/deepspeed/supervised\")\ndef infer(\n    self,\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Perform inference using the trained model.\n\n    Args:\n        postprocess_fn: The post-processing function for inference.\n        writer: The writer for writing the results.\n        test_batch_size (optional): The batch size for inference. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        max_size (optional): The maximum size of the dataset for inference. Defaults to 10000.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        output_header (optional): The header for the output file. Defaults to None.\n        output_path (optional): The path to save the output file. Defaults to \"./cache/predict.txt\".\n        postprocess_workers (optional): The number of worker processes for post-processing. Defaults to 2.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    assert self.n_gpu &lt;= 1\n    assert writer is not None\n\n    output_dir = os.path.dirname(output_path)\n    if not os.path.exists(output_dir):\n        os.makedirs(output_dir, exist_ok=True)\n\n    if postprocess_fn is not None:\n        postprocess_fn = init_registered_process(postprocess_fn, self.config)\n\n    if writer is not None:\n        writer = init_registered_module(\n            writer,\n            self.config,\n            registered_writer,\n            output_file=output_path,\n        )\n\n    skip_step = writer.skip_n_samples\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if skip_step == 0:\n        sampler = SequentialSampler\n    else:\n        sampler = SequentialSkipSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_test = self.datasets.get(\"test\")\n    else:\n        dataset_test = self.datasets.get(\"test\")\n\n    iter_test = DataLoader(\n        dataset_test,\n        sampler=sampler(dataset_test)\n        if not isinstance(dataset_test, Iterable)\n        else None,\n        batch_size=test_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if skip_step &gt; 0:\n        output_file = open(output_path, \"a\")\n    else:\n        output_file = open(output_path, \"w\")\n\n    if skip_step &gt; 0 and hasattr(dataset_test, \"set_skip_step\"):\n        dataset_test.set_skip_step(skip_step)\n\n    if skip_step &gt; 0 and hasattr(iter_test.sampler, \"set_skip_step\"):\n        iter_test.sampler.set_skip_step(skip_step)\n\n    if hasattr(dataset_test, \"dataset\"):\n        data_info = dataset_test.dataset\n        data_info = DatasetFeature(data_info)\n        iter_data = DataLoader(\n            deepcopy(data_info),\n            sampler=sampler(data_info)\n            if not isinstance(dataset_test, Iterable)\n            else None,\n            batch_size=test_batch_size,\n            shuffle=False,\n            pin_memory=pin_memory,\n            num_workers=num_workers,\n            collate_fn=None,\n        )\n    else:\n        iter_data = None\n\n    if skip_step &gt; 0 and hasattr(iter_data.sampler, \"set_skip_step\"):\n        iter_data.sampler.set_skip_step(skip_step)\n\n    self.model.eval()\n    start = time.time()\n\n    data_queue = Queue(maxsize=max_size)\n    msg_queue = Queue(maxsize=max_size)\n    postprocess_list = []\n    for _ in range(postprocess_workers):\n        p = PostProcess(\n            postprocess_fn,\n            data_queue,\n            msg_queue,\n        )\n        postprocess_list.append(p)\n        p.start()\n\n    io_process = IOProcess(msg_queue, writer=writer)\n    io_process.start()\n\n    if iter_data is None:\n        for step, (inputs, _) in enumerate(iter_test):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            data_queue.put((step, outputs))\n    else:\n        for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            if output_header is not None:\n                _infos = {k: _infos[k] for k in output_header if k in _infos}\n                outputs.set_base_dataframe(pd.DataFrame(_infos))\n            data_queue.put((step, outputs))\n\n    data_queue.put((-1, GENERATE_FINISHED))\n    for p in postprocess_list:\n        p.join()\n\n    msg_queue.put((-1, GENERATE_FINISHED))\n    io_process.join()\n\n    end = time.time()\n    ms = (end - start) * 1000\n    logging.info(\n        \"{:.2f} ms, {:.1f} sample/s\".format(\n            ms,\n            ((len(dataset_test) - skip_step) / ms * 1000),\n        )\n    )\n</code></pre>",
+            "text": "<pre><code>infer(\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Perform inference using the trained model.</p> <p>Parameters:</p> Name Type Description Default <code>postprocess_fn</code> <code>str</code> <p>The post-processing function for inference.</p> required <code>writer</code> <code>str</code> <p>The writer for writing the results.</p> required <code>test_batch_size</code> <code>optional</code> <p>The batch size for inference. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>max_size</code> <code>optional</code> <p>The maximum size of the dataset for inference. Defaults to 10000.</p> <code>10000</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>output_header</code> <code>optional</code> <p>The header for the output file. Defaults to None.</p> <code>None</code> <code>output_path</code> <code>optional</code> <p>The path to save the output file. Defaults to \"./cache/predict.txt\".</p> <code>'./cache/predict.txt'</code> <code>postprocess_workers</code> <code>optional</code> <p>The number of worker processes for post-processing. Defaults to 2.</p> <code>2</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/deepspeed.py</code> <pre><code>@torch.no_grad()\n@add_default_section_for_function(\"core/task/deepspeed/supervised\")\ndef infer(\n    self,\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Perform inference using the trained model.\n\n    Args:\n        postprocess_fn: The post-processing function for inference.\n        writer: The writer for writing the results.\n        test_batch_size (optional): The batch size for inference. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        max_size (optional): The maximum size of the dataset for inference. Defaults to 10000.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        output_header (optional): The header for the output file. Defaults to None.\n        output_path (optional): The path to save the output file. Defaults to \"./cache/predict.txt\".\n        postprocess_workers (optional): The number of worker processes for post-processing. Defaults to 2.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    assert self.n_gpu &lt;= 1\n    assert writer is not None\n\n    output_dir = os.path.dirname(output_path)\n    if not os.path.exists(output_dir):\n        os.makedirs(output_dir, exist_ok=True)\n\n    if postprocess_fn is not None:\n        postprocess_fn = init_registered_process(postprocess_fn, self.config)\n\n    if writer is not None:\n        writer = init_registered_module(\n            writer,\n            self.config,\n            registered_writer,\n            output_file=output_path,\n        )\n\n    skip_step = writer.skip_n_samples\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if skip_step == 0:\n        sampler = SequentialSampler\n    else:\n        sampler = SequentialSkipSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_test = self.datasets.get(\"test\")\n    else:\n        dataset_test = self.datasets.get(\"test\")\n\n    iter_test = DataLoader(\n        dataset_test,\n        sampler=sampler(dataset_test)\n        if not isinstance(dataset_test, Iterable)\n        else None,\n        batch_size=test_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if skip_step &gt; 0:\n        output_file = open(output_path, \"a\")\n    else:\n        output_file = open(output_path, \"w\")\n\n    if skip_step &gt; 0 and hasattr(dataset_test, \"set_skip_step\"):\n        dataset_test.set_skip_step(skip_step)\n\n    if skip_step &gt; 0 and hasattr(iter_test.sampler, \"set_skip_step\"):\n        iter_test.sampler.set_skip_step(skip_step)\n\n    if hasattr(dataset_test, \"dataset\"):\n        data_info = dataset_test.dataset\n        data_info = DatasetFeature(data_info)\n        iter_data = DataLoader(\n            deepcopy(data_info),\n            sampler=sampler(data_info)\n            if not isinstance(dataset_test, Iterable)\n            else None,\n            batch_size=test_batch_size,\n            shuffle=False,\n            pin_memory=pin_memory,\n            num_workers=num_workers,\n            collate_fn=None,\n        )\n    else:\n        iter_data = None\n\n    if skip_step &gt; 0 and hasattr(iter_data.sampler, \"set_skip_step\"):\n        iter_data.sampler.set_skip_step(skip_step)\n\n    self.model.eval()\n    start = time.time()\n\n    data_queue = Queue(maxsize=max_size)\n    msg_queue = Queue(maxsize=max_size)\n    postprocess_list = []\n    for _ in range(postprocess_workers):\n        p = PostProcess(\n            postprocess_fn,\n            data_queue,\n            msg_queue,\n        )\n        postprocess_list.append(p)\n        p.start()\n\n    io_process = IOProcess(msg_queue, writer=writer)\n    io_process.start()\n\n    if iter_data is None:\n        for step, (inputs, _) in enumerate(iter_test):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            data_queue.put((step, outputs))\n    else:\n        for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            if output_header is not None:\n                _infos = {k: _infos[k] for k in output_header if k in _infos}\n                outputs.from_pandas(pd.DataFrame(_infos))\n            data_queue.put((step, outputs))\n\n    data_queue.put((-1, GENERATE_FINISHED))\n    for p in postprocess_list:\n        p.join()\n\n    msg_queue.put((-1, GENERATE_FINISHED))\n    io_process.join()\n\n    end = time.time()\n    ms = (end - start) * 1000\n    logging.info(\n        \"{:.2f} ms, {:.1f} sample/s\".format(\n            ms,\n            ((len(dataset_test) - skip_step) / ms * 1000),\n        )\n    )\n</code></pre>",
             "title": "infer"
         },
         {
             "location": "cli/deepspeed/#unitorch.cli.tasks.deepspeed.DeepspeedTask.train",
-            "text": "<pre><code>train(\n    config_path: str,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    learning_rate: Optional[float] = None,\n    max_warmup_learning_rate: Optional[float] = None,\n    num_warmup_steps: Optional[int] = None,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Train the model using deepspeed.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the deepspeed configuration file.</p> required <code>optim</code> <code>str</code> <p>The optimizer used for training.</p> required <code>loss_fn</code> <code>str</code> <p>The loss function used for training.</p> required <code>score_fn</code> <code>str</code> <p>The score function used for evaluation.</p> required <code>monitor_fns</code> <code>optional</code> <p>The monitoring functions for evaluation. Defaults to None.</p> <code>None</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>to_ckpt_dir</code> <code>optional</code> <p>The directory path to save checkpoints to. Defaults to \"./to_ckpt\".</p> <code>'./to_ckpt'</code> <code>train_batch_size</code> <code>optional</code> <p>The batch size for training. Defaults to 128.</p> <code>128</code> <code>dev_batch_size</code> <code>optional</code> <p>The batch size for evaluation. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>save_optimizer</code> <code>optional</code> <p>Whether to save the optimizer state. Defaults to True.</p> <code>True</code> <code>save_scheduler</code> <code>optional</code> <p>Whether to save the scheduler state. Defaults to True.</p> <code>True</code> <code>log_freq</code> <code>optional</code> <p>The frequency of logging. Defaults to 100.</p> <code>100</code> <code>ckpt_freq</code> <code>optional</code> <p>The frequency of saving checkpoints. Defaults to 10000.</p> <code>10000</code> <code>grad_acc_step</code> <code>optional</code> <p>The number of gradient accumulation steps. Defaults to 1.</p> <code>1</code> <code>max_grad_norm</code> <code>optional</code> <p>The maximum gradient norm. Defaults to 1.0.</p> <code>1.0</code> <code>learning_rate</code> <code>optional</code> <p>The learning rate for the optimizer. Defaults to None.</p> <code>None</code> <code>max_warmup_learning_rate</code> <code>optional</code> <p>The maximum learning rate during warmup. Defaults to None.</p> <code>None</code> <code>num_warmup_steps</code> <code>optional</code> <p>The number of warmup steps. Defaults to None.</p> <code>None</code> <code>epochs</code> <code>optional</code> <p>The number of training epochs. Defaults to 5.</p> <code>5</code> <code>use_ema</code> <code>optional</code> <p>Whether to use exponential moving average. Defaults to False.</p> <code>False</code> <code>ema_decay</code> <code>optional</code> <p>The decay factor for exponential moving average. Defaults to 0.9999.</p> <code>0.9999</code> <code>ema_tau</code> <code>optional</code> <p>The time constant for exponential moving average. Defaults to 2000.</p> <code>2000</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/deepspeed.py</code> <pre><code>@add_default_section_for_function(\"core/task/deepspeed/supervised\")\ndef train(\n    self,\n    config_path: str,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    learning_rate: Optional[float] = None,\n    max_warmup_learning_rate: Optional[float] = None,\n    num_warmup_steps: Optional[int] = None,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Train the model using deepspeed.\n\n    Args:\n        config_path: The path to the deepspeed configuration file.\n        optim: The optimizer used for training.\n        loss_fn: The loss function used for training.\n        score_fn: The score function used for evaluation.\n        monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to \"./to_ckpt\".\n        train_batch_size (optional): The batch size for training. Defaults to 128.\n        dev_batch_size (optional): The batch size for evaluation. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        save_optimizer (optional): Whether to save the optimizer state. Defaults to True.\n        save_scheduler (optional): Whether to save the scheduler state. Defaults to True.\n        log_freq (optional): The frequency of logging. Defaults to 100.\n        ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.\n        grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.\n        max_grad_norm (optional): The maximum gradient norm. Defaults to 1.0.\n        learning_rate (optional): The learning rate for the optimizer. Defaults to None.\n        max_warmup_learning_rate (optional): The maximum learning rate during warmup. Defaults to None.\n        num_warmup_steps (optional): The number of warmup steps. Defaults to None.\n        epochs (optional): The number of training epochs. Defaults to 5.\n        use_ema (optional): Whether to use exponential moving average. Defaults to False.\n        ema_decay (optional): The decay factor for exponential moving average. Defaults to 0.9999.\n        ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:\n        os.makedirs(to_ckpt_dir, exist_ok=True)\n\n    if loss_fn is not None:\n        loss_fn = init_registered_module(loss_fn, self.config, registered_loss)\n\n    if score_fn is not None:\n        score_fn = init_registered_module(score_fn, self.config, registered_score)\n\n    if monitor_fns is not None:\n        monitor_fns = [\n            init_registered_module(monitor_fn, self.config, registered_score)\n            for monitor_fn in monitor_fns\n            if monitor_fn in registered_score\n        ]\n\n    config_file = cached_path(config_path)\n    config_dict = json.load(open(config_file, \"r\"))\n    config_dict[\"train_micro_batch_size_per_gpu\"] = train_batch_size\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if os.path.exists(to_ckpt_dir):\n        self.model.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_model_latest.bin\",\n        )\n\n    params = self.model.parameters()\n    params = filter(lambda x: x.requires_grad, params)\n\n    assert \"optimizer\" in config_dict\n\n    if \"params\" not in config_dict[\"optimizer\"]:\n        config_dict[\"optimizer\"][\"params\"] = dict()\n\n    if \"scheduler\" in config_dict:\n        if \"params\" not in config_dict[\"scheduler\"]:\n            config_dict[\"scheduler\"][\"params\"] = dict()\n\n    if learning_rate is not None:\n        config_dict[\"optimizer\"][\"params\"][\"lr\"] = learning_rate\n        if \"scheduler\" in config_dict:\n            config_dict[\"scheduler\"][\"params\"][\"warmup_max_lr\"] = learning_rate\n\n    if max_warmup_learning_rate is not None and \"scheduler\" in config_dict:\n        config_dict[\"scheduler\"][\"params\"][\n            \"warmup_max_lr\"\n        ] = max_warmup_learning_rate\n\n    if num_warmup_steps is not None and \"scheduler\" in config_dict:\n        if \"params\" not in config_dict[\"scheduler\"]:\n            config_dict[\"scheduler\"][\"params\"] = dict()\n        config_dict[\"scheduler\"][\"params\"][\"warmup_num_steps\"] = num_warmup_steps\n\n    info_path = os.path.join(to_ckpt_dir, \"info.json\")\n    if os.path.exists(info_path):\n        info = json.load(open(os.path.join(to_ckpt_dir, \"info.json\")))\n    else:\n        info = dict()\n\n    global_epoch = info.get(\"global_epoch\", 0)\n    global_step = info.get(\"global_step\", 0)\n    self.best_score = info.get(\"best_score\", self.best_score)\n\n    logging.info(f\"the best score is {self.best_score}\")\n\n    self.ema_model = None\n    if use_ema:\n        num_ema_steps = info.get(\"num_ema_steps\", 0)\n        self.ema_model = ExponentialMovingAverage(\n            self.model,\n            decay=ema_decay,\n            tau=ema_tau,\n            num_steps=num_ema_steps,\n        )\n        if os.path.exists(from_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                from_ckpt_dir,\n                weight_name=\"pytorch_ema_model.bin\",\n            )\n        if os.path.exists(to_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                to_ckpt_dir,\n                weight_name=\"pytorch_ema_model_latest.bin\",\n            )\n\n    for n, p in self.model.named_parameters():\n        logging.debug(\n            f\"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}\"\n        )\n\n    self.model, optim, _, scheduler = deepspeed.initialize(\n        model=self.model,\n        config=config_dict,\n        model_parameters=params,\n    )\n\n    global_rank = -1\n    if self.n_gpu &gt; 1:\n        global_rank = dist.get_rank()\n\n    train_sampler = DistributedSkipSampler if self.n_gpu &gt; 1 else RandomSkipSampler\n    dev_sampler = DistributedSampler if self.n_gpu &gt; 1 else SequentialSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_train = self.datasets.get(\"train\")\n            dataset_dev = self.datasets.get(\"dev\")\n    else:\n        dataset_train = self.datasets.get(\"train\")\n        dataset_dev = self.datasets.get(\"dev\")\n\n    iter_train = DataLoader(\n        dataset_train,\n        sampler=train_sampler(dataset_train)\n        if not isinstance(dataset_train, Iterable)\n        else None,\n        batch_size=train_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    iter_dev = DataLoader(\n        dataset_dev,\n        sampler=dev_sampler(dataset_dev)\n        if not isinstance(dataset_dev, Iterable)\n        else None,\n        batch_size=dev_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    log_loss = 0\n    dev_epoch = 0\n    for e in range(0, epochs):\n        torch.cuda.empty_cache()\n        if e &lt; global_epoch:\n            continue\n\n        if hasattr(dataset_train, \"set_epoch\"):\n            dataset_train.set_epoch(e)\n\n        if hasattr(dataset_train, \"set_skip_step\"):\n            dataset_train.set_skip_step(global_step * train_batch_size)\n\n        if hasattr(iter_train.sampler, \"set_epoch\"):\n            iter_train.sampler.set_epoch(e)\n\n        if hasattr(iter_train.sampler, \"set_skip_step\"):\n            iter_train.sampler.set_skip_step(global_step * train_batch_size)\n\n        self.model.train()\n        is_update_step = True\n        for step, (inputs, targets) in enumerate(iter_train):\n            step = step + global_step\n            is_update_step = False\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n                targets = targets.cuda()\n\n            if is_torch2_available():\n                with torch.cuda.amp.autocast(\n                    enabled=True\n                ) as autocast, torch.backends.cuda.sdp_kernel(\n                    enable_flash=False\n                ) as disable:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n            else:\n                with torch.cuda.amp.autocast(enabled=True) as autocast:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n\n            nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)\n            self.model.backward(loss)\n\n            log_loss += loss.data * grad_acc_step\n            if (step + 1) % grad_acc_step == 0:\n                is_update_step = True\n                optim.step()\n                if scheduler is not None:\n                    scheduler.step()\n                optim.zero_grad()\n\n                if use_ema and self.ema_model is not None:\n                    self.ema_model.step(\n                        self.model.module if self.n_gpu &gt; 1 else self.model\n                    )\n\n            if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:\n                logging.info(\n                    f\"epoch {e} step {step}: loss -- { log_loss / log_freq }\"\n                )\n                log_loss = 0\n\n            if (step + 1) % ckpt_freq == 0:\n                if hasattr(dataset_dev, \"set_epoch\"):\n                    dataset_dev.set_epoch(dev_epoch)\n\n                if hasattr(iter_dev.sampler, \"set_epoch\"):\n                    iter_dev.sampler.set_epoch(dev_epoch)\n\n                dev_epoch += 1\n                self.best_score = save_checkpoint(\n                    self.model.module if self.n_gpu &gt; 1 else self.model,\n                    to_ckpt_dir,\n                    iter_dev,\n                    score_fn,\n                    monitor_fns,\n                    optim=optim if save_optimizer else None,\n                    scheduler=scheduler if save_scheduler else None,\n                    ema_model=self.ema_ema_model if use_ema else None,\n                    best_score=self.best_score,\n                    info_path=info_path,\n                    local_rank=self.local_rank,\n                    global_epoch=e,\n                    global_step=step + 1,\n                )\n\n        if not is_update_step:\n            optim.step()\n            if scheduler is not None:\n                scheduler.step()\n            optim.zero_grad()\n\n            if use_ema and self.ema_model is not None:\n                self.ema_model.step(\n                    self.model.module if self.n_gpu &gt; 1 else self.model\n                )\n\n        log_loss = 0\n\n        if hasattr(dataset_dev, \"set_epoch\"):\n            dataset_dev.set_epoch(dev_epoch)\n\n        if hasattr(iter_dev.sampler, \"set_epoch\"):\n            iter_dev.sampler.set_epoch(dev_epoch)\n\n        dev_epoch += 1\n\n        global_step = 0\n        self.best_score = save_checkpoint(\n            self.model.module if self.n_gpu &gt; 1 else self.model,\n            to_ckpt_dir,\n            iter_dev,\n            score_fn,\n            monitor_fns,\n            optim=optim if save_optimizer else None,\n            scheduler=scheduler if save_scheduler else None,\n            ema_model=self.ema_ema_model if use_ema else None,\n            best_score=self.best_score,\n            info_path=info_path,\n            local_rank=self.local_rank,\n            global_epoch=e,\n            global_step=step + 1,\n        )\n</code></pre>",
+            "text": "<pre><code>train(\n    config_path: str,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = False,\n    save_scheduler: Optional[bool] = False,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    learning_rate: Optional[float] = None,\n    max_warmup_learning_rate: Optional[float] = None,\n    num_warmup_steps: Optional[int] = None,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Train the model using deepspeed.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the deepspeed configuration file.</p> required <code>optim</code> <code>str</code> <p>The optimizer used for training.</p> required <code>loss_fn</code> <code>str</code> <p>The loss function used for training.</p> required <code>score_fn</code> <code>str</code> <p>The score function used for evaluation.</p> required <code>monitor_fns</code> <code>optional</code> <p>The monitoring functions for evaluation. Defaults to None.</p> <code>None</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>to_ckpt_dir</code> <code>optional</code> <p>The directory path to save checkpoints to. Defaults to \"./to_ckpt\".</p> <code>'./to_ckpt'</code> <code>train_batch_size</code> <code>optional</code> <p>The batch size for training. Defaults to 128.</p> <code>128</code> <code>dev_batch_size</code> <code>optional</code> <p>The batch size for evaluation. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>save_optimizer</code> <code>optional</code> <p>Whether to save the optimizer state. Defaults to False.</p> <code>False</code> <code>save_scheduler</code> <code>optional</code> <p>Whether to save the scheduler state. Defaults to False.</p> <code>False</code> <code>log_freq</code> <code>optional</code> <p>The frequency of logging. Defaults to 100.</p> <code>100</code> <code>ckpt_freq</code> <code>optional</code> <p>The frequency of saving checkpoints. Defaults to 10000.</p> <code>10000</code> <code>grad_acc_step</code> <code>optional</code> <p>The number of gradient accumulation steps. Defaults to 1.</p> <code>1</code> <code>max_grad_norm</code> <code>optional</code> <p>The maximum gradient norm. Defaults to 1.0.</p> <code>1.0</code> <code>learning_rate</code> <code>optional</code> <p>The learning rate for the optimizer. Defaults to None.</p> <code>None</code> <code>max_warmup_learning_rate</code> <code>optional</code> <p>The maximum learning rate during warmup. Defaults to None.</p> <code>None</code> <code>num_warmup_steps</code> <code>optional</code> <p>The number of warmup steps. Defaults to None.</p> <code>None</code> <code>epochs</code> <code>optional</code> <p>The number of training epochs. Defaults to 5.</p> <code>5</code> <code>use_ema</code> <code>optional</code> <p>Whether to use exponential moving average. Defaults to False.</p> <code>False</code> <code>ema_decay</code> <code>optional</code> <p>The decay factor for exponential moving average. Defaults to 0.9999.</p> <code>0.9999</code> <code>ema_tau</code> <code>optional</code> <p>The time constant for exponential moving average. Defaults to 2000.</p> <code>2000</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/deepspeed.py</code> <pre><code>@add_default_section_for_function(\"core/task/deepspeed/supervised\")\ndef train(\n    self,\n    config_path: str,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = False,\n    save_scheduler: Optional[bool] = False,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    learning_rate: Optional[float] = None,\n    max_warmup_learning_rate: Optional[float] = None,\n    num_warmup_steps: Optional[int] = None,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Train the model using deepspeed.\n\n    Args:\n        config_path: The path to the deepspeed configuration file.\n        optim: The optimizer used for training.\n        loss_fn: The loss function used for training.\n        score_fn: The score function used for evaluation.\n        monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to \"./to_ckpt\".\n        train_batch_size (optional): The batch size for training. Defaults to 128.\n        dev_batch_size (optional): The batch size for evaluation. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        save_optimizer (optional): Whether to save the optimizer state. Defaults to False.\n        save_scheduler (optional): Whether to save the scheduler state. Defaults to False.\n        log_freq (optional): The frequency of logging. Defaults to 100.\n        ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.\n        grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.\n        max_grad_norm (optional): The maximum gradient norm. Defaults to 1.0.\n        learning_rate (optional): The learning rate for the optimizer. Defaults to None.\n        max_warmup_learning_rate (optional): The maximum learning rate during warmup. Defaults to None.\n        num_warmup_steps (optional): The number of warmup steps. Defaults to None.\n        epochs (optional): The number of training epochs. Defaults to 5.\n        use_ema (optional): Whether to use exponential moving average. Defaults to False.\n        ema_decay (optional): The decay factor for exponential moving average. Defaults to 0.9999.\n        ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:\n        os.makedirs(to_ckpt_dir, exist_ok=True)\n\n    if loss_fn is not None:\n        loss_fn = init_registered_module(loss_fn, self.config, registered_loss)\n\n    if score_fn is not None:\n        score_fn = init_registered_module(score_fn, self.config, registered_score)\n\n    if monitor_fns is not None:\n        monitor_fns = [\n            init_registered_module(monitor_fn, self.config, registered_score)\n            for monitor_fn in monitor_fns\n            if monitor_fn in registered_score\n        ]\n\n    config_file = cached_path(config_path)\n    config_dict = json.load(open(config_file, \"r\"))\n    config_dict[\"train_micro_batch_size_per_gpu\"] = train_batch_size\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if os.path.exists(to_ckpt_dir):\n        self.model.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_model_latest.bin\",\n        )\n\n    params = self.model.parameters()\n    params = filter(lambda x: x.requires_grad, params)\n\n    assert \"optimizer\" in config_dict\n\n    if \"params\" not in config_dict[\"optimizer\"]:\n        config_dict[\"optimizer\"][\"params\"] = dict()\n\n    if \"scheduler\" in config_dict:\n        if \"params\" not in config_dict[\"scheduler\"]:\n            config_dict[\"scheduler\"][\"params\"] = dict()\n\n    if learning_rate is not None:\n        config_dict[\"optimizer\"][\"params\"][\"lr\"] = learning_rate\n        if \"scheduler\" in config_dict:\n            config_dict[\"scheduler\"][\"params\"][\"warmup_max_lr\"] = learning_rate\n\n    if max_warmup_learning_rate is not None and \"scheduler\" in config_dict:\n        config_dict[\"scheduler\"][\"params\"][\n            \"warmup_max_lr\"\n        ] = max_warmup_learning_rate\n\n    if num_warmup_steps is not None and \"scheduler\" in config_dict:\n        if \"params\" not in config_dict[\"scheduler\"]:\n            config_dict[\"scheduler\"][\"params\"] = dict()\n        config_dict[\"scheduler\"][\"params\"][\"warmup_num_steps\"] = num_warmup_steps\n\n    info_path = os.path.join(to_ckpt_dir, \"info.json\")\n    if os.path.exists(info_path):\n        info = json.load(open(os.path.join(to_ckpt_dir, \"info.json\")))\n    else:\n        info = dict()\n\n    global_epoch = info.get(\"global_epoch\", 0)\n    global_step = info.get(\"global_step\", 0)\n    self.best_score = info.get(\"best_score\", self.best_score)\n\n    logging.info(f\"the best score is {self.best_score}\")\n\n    self.ema_model = None\n    if use_ema:\n        num_ema_steps = info.get(\"num_ema_steps\", 0)\n        self.ema_model = ExponentialMovingAverage(\n            self.model,\n            decay=ema_decay,\n            tau=ema_tau,\n            num_steps=num_ema_steps,\n        )\n        if os.path.exists(from_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                from_ckpt_dir,\n                weight_name=\"pytorch_ema_model.bin\",\n            )\n        if os.path.exists(to_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                to_ckpt_dir,\n                weight_name=\"pytorch_ema_model_latest.bin\",\n            )\n\n    for n, p in self.model.named_parameters():\n        logging.debug(\n            f\"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}\"\n        )\n\n    self.model, optim, _, scheduler = deepspeed.initialize(\n        model=self.model,\n        config=config_dict,\n        model_parameters=params,\n    )\n\n    global_rank = -1\n    if self.n_gpu &gt; 1:\n        global_rank = dist.get_rank()\n\n    train_sampler = DistributedSkipSampler if self.n_gpu &gt; 1 else RandomSkipSampler\n    dev_sampler = DistributedSampler if self.n_gpu &gt; 1 else SequentialSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_train = self.datasets.get(\"train\")\n            dataset_dev = self.datasets.get(\"dev\")\n    else:\n        dataset_train = self.datasets.get(\"train\")\n        dataset_dev = self.datasets.get(\"dev\")\n\n    iter_train = DataLoader(\n        dataset_train,\n        sampler=train_sampler(dataset_train)\n        if not isinstance(dataset_train, Iterable)\n        else None,\n        batch_size=train_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    iter_dev = DataLoader(\n        dataset_dev,\n        sampler=dev_sampler(dataset_dev)\n        if not isinstance(dataset_dev, Iterable)\n        else None,\n        batch_size=dev_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    log_loss = 0\n    dev_epoch = 0\n    for e in range(0, epochs):\n        torch.cuda.empty_cache()\n        if e &lt; global_epoch:\n            continue\n\n        if hasattr(dataset_train, \"set_epoch\"):\n            dataset_train.set_epoch(e)\n\n        if hasattr(dataset_train, \"set_skip_step\"):\n            dataset_train.set_skip_step(global_step * train_batch_size)\n\n        if hasattr(iter_train.sampler, \"set_epoch\"):\n            iter_train.sampler.set_epoch(e)\n\n        if hasattr(iter_train.sampler, \"set_skip_step\"):\n            iter_train.sampler.set_skip_step(global_step * train_batch_size)\n\n        self.model.train()\n        is_update_step = True\n        for step, (inputs, targets) in enumerate(iter_train):\n            step = step + global_step\n            is_update_step = False\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n                targets = targets.cuda()\n\n            if is_torch2_available():\n                with torch.cuda.amp.autocast(\n                    enabled=True\n                ) as autocast, torch.backends.cuda.sdp_kernel(\n                    enable_flash=False\n                ) as disable:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n            else:\n                with torch.cuda.amp.autocast(enabled=True) as autocast:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n\n            nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)\n            self.model.backward(loss)\n\n            log_loss += loss.data * grad_acc_step\n            if (step + 1) % grad_acc_step == 0:\n                is_update_step = True\n                optim.step()\n                if scheduler is not None:\n                    scheduler.step()\n                optim.zero_grad()\n\n                if use_ema and self.ema_model is not None:\n                    self.ema_model.step(\n                        self.model.module if self.n_gpu &gt; 1 else self.model\n                    )\n\n            if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:\n                logging.info(\n                    f\"epoch {e} step {step}: loss -- { log_loss / log_freq }\"\n                )\n                log_loss = 0\n\n            if (step + 1) % ckpt_freq == 0:\n                if hasattr(dataset_dev, \"set_epoch\"):\n                    dataset_dev.set_epoch(dev_epoch)\n\n                if hasattr(iter_dev.sampler, \"set_epoch\"):\n                    iter_dev.sampler.set_epoch(dev_epoch)\n\n                dev_epoch += 1\n                self.best_score = save_checkpoint(\n                    self.model.module if self.n_gpu &gt; 1 else self.model,\n                    to_ckpt_dir,\n                    iter_dev,\n                    score_fn,\n                    monitor_fns,\n                    optim=optim if save_optimizer else None,\n                    scheduler=scheduler if save_scheduler else None,\n                    ema_model=self.ema_model if use_ema else None,\n                    best_score=self.best_score,\n                    info_path=info_path,\n                    local_rank=self.local_rank,\n                    global_epoch=e,\n                    global_step=step + 1,\n                )\n\n        if not is_update_step:\n            optim.step()\n            if scheduler is not None:\n                scheduler.step()\n            optim.zero_grad()\n\n            if use_ema and self.ema_model is not None:\n                self.ema_model.step(\n                    self.model.module if self.n_gpu &gt; 1 else self.model\n                )\n\n        log_loss = 0\n\n        if hasattr(dataset_dev, \"set_epoch\"):\n            dataset_dev.set_epoch(dev_epoch)\n\n        if hasattr(iter_dev.sampler, \"set_epoch\"):\n            iter_dev.sampler.set_epoch(dev_epoch)\n\n        dev_epoch += 1\n\n        global_step = 0\n        self.best_score = save_checkpoint(\n            self.model.module if self.n_gpu &gt; 1 else self.model,\n            to_ckpt_dir,\n            iter_dev,\n            score_fn,\n            monitor_fns,\n            optim=optim if save_optimizer else None,\n            scheduler=scheduler if save_scheduler else None,\n            ema_model=self.ema_model if use_ema else None,\n            best_score=self.best_score,\n            info_path=info_path,\n            local_rank=self.local_rank,\n            global_epoch=e,\n            global_step=0,\n        )\n</code></pre>",
             "title": "train"
         },
         {
             "location": "cli/jsonl/",
             "text": "",
             "title": "unitorch.cli.writer"
         },
@@ -267,20 +267,20 @@
         {
             "location": "cli/supervised/#unitorch.cli.tasks.supervised.SupervisedTask.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create a SupervisedTask instance from the core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration object.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Type Description <p>A dictionary containing the configuration, model, datasets, and local rank.</p> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/task/supervised\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create a SupervisedTask instance from the core configuration.\n\n    Args:\n        config: The core configuration object.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        A dictionary containing the configuration, model, datasets, and local rank.\n    \"\"\"\n    try:\n        torch.distributed.init_process_group(backend=\"nccl\", init_method=\"env://\")\n    except:\n        logging.info(\"PyTorch is not in distributed mode\")\n\n    config.set_default_section(\"core/task/supervised\")\n\n    model = config.getoption(\"model\", None)\n    dataset = config.getoption(\"dataset\", None)\n\n    if model is not None:\n        model = init_registered_module(model, config, registered_model)\n\n    if dataset is not None:\n        dataset = init_registered_module(dataset, config, registered_dataset)\n\n    local_rank = config.getdefault(\n        \"core/cli\",\n        \"local_rank\",\n        get_local_rank(),\n    )\n\n    return dict(\n        configure=config,\n        model=model,\n        datasets=dataset,\n        local_rank=local_rank,\n    )\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/supervised/#unitorch.cli.tasks.supervised.SupervisedTask.infer",
-            "text": "<pre><code>infer(\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Perform inference using the model.</p> <p>Parameters:</p> Name Type Description Default <code>postprocess_fn</code> <code>str</code> <p>The postprocessing function for inference.</p> required <code>writer</code> <code>str</code> <p>The writer to save the inference results.</p> required <code>test_batch_size</code> <code>optional</code> <p>The batch size for inference. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>max_size</code> <code>optional</code> <p>The maximum number of samples to process. Defaults to 10000.</p> <code>10000</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>output_header</code> <code>optional</code> <p>The header for the output file. Defaults to None.</p> <code>None</code> <code>output_path</code> <code>optional</code> <p>The path to save the output file. Defaults to \"./cache/predict.txt\".</p> <code>'./cache/predict.txt'</code> <code>postprocess_workers</code> <code>optional</code> <p>The number of worker processes for postprocessing. Defaults to 2.</p> <code>2</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@torch.no_grad()\n@add_default_section_for_function(\"core/task/supervised\")\ndef infer(\n    self,\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Perform inference using the model.\n\n    Args:\n        postprocess_fn: The postprocessing function for inference.\n        writer: The writer to save the inference results.\n        test_batch_size (optional): The batch size for inference. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        max_size (optional): The maximum number of samples to process. Defaults to 10000.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        output_header (optional): The header for the output file. Defaults to None.\n        output_path (optional): The path to save the output file. Defaults to \"./cache/predict.txt\".\n        postprocess_workers (optional): The number of worker processes for postprocessing. Defaults to 2.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    assert self.n_gpu &lt;= 1\n    assert writer is not None\n\n    output_dir = os.path.dirname(output_path)\n    if not os.path.exists(output_dir):\n        os.makedirs(output_dir, exist_ok=True)\n\n    if postprocess_fn is not None:\n        postprocess_fn = init_registered_process(postprocess_fn, self.config)\n\n    if writer is not None:\n        writer = init_registered_module(\n            writer,\n            self.config,\n            registered_writer,\n            output_file=output_path,\n        )\n\n    skip_step = writer.skip_n_samples\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if skip_step == 0:\n        sampler = SequentialSampler\n    else:\n        sampler = SequentialSkipSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_test = self.datasets.get(\"test\")\n    else:\n        dataset_test = self.datasets.get(\"test\")\n\n    iter_test = DataLoader(\n        dataset_test,\n        sampler=sampler(dataset_test)\n        if not isinstance(dataset_test, Iterable)\n        else None,\n        batch_size=test_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if skip_step &gt; 0 and hasattr(dataset_test, \"set_skip_step\"):\n        dataset_test.set_skip_step(skip_step)\n\n    if skip_step &gt; 0 and hasattr(iter_test.sampler, \"set_skip_step\"):\n        iter_test.sampler.set_skip_step(skip_step)\n\n    if hasattr(dataset_test, \"dataset\"):\n        data_info = dataset_test.dataset\n        data_info = DatasetFeature(data_info)\n        iter_data = DataLoader(\n            deepcopy(data_info),\n            sampler=sampler(data_info)\n            if not isinstance(dataset_test, Iterable)\n            else None,\n            batch_size=test_batch_size,\n            shuffle=False,\n            pin_memory=pin_memory,\n            num_workers=num_workers,\n            collate_fn=None,\n        )\n    else:\n        iter_data = None\n\n    if skip_step &gt; 0 and hasattr(iter_data.sampler, \"set_skip_step\"):\n        iter_data.sampler.set_skip_step(skip_step)\n\n    self.model.eval()\n    start = time.time()\n\n    data_queue = Queue(maxsize=max_size)\n    msg_queue = Queue(maxsize=max_size)\n    postprocess_list = []\n    for _ in range(postprocess_workers):\n        p = PostProcess(\n            postprocess_fn,\n            data_queue,\n            msg_queue,\n        )\n        postprocess_list.append(p)\n        p.start()\n\n    io_process = IOProcess(msg_queue, writer=writer)\n    io_process.start()\n\n    if iter_data is None:\n        for step, (inputs, _) in enumerate(iter_test):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            data_queue.put((step, outputs))\n    else:\n        for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            if output_header is not None:\n                _infos = {k: _infos[k] for k in output_header if k in _infos}\n                outputs.set_base_dataframe(pd.DataFrame(_infos))\n            data_queue.put((step, outputs))\n\n    data_queue.put((-1, GENERATE_FINISHED))\n    for p in postprocess_list:\n        p.join()\n\n    msg_queue.put((-1, GENERATE_FINISHED))\n    io_process.join()\n\n    end = time.time()\n    ms = (end - start) * 1000\n    logging.info(\n        \"{:.2f} ms, {:.1f} sample/s\".format(\n            ms,\n            ((len(dataset_test) - skip_step) / ms * 1000),\n        )\n    )\n</code></pre>",
+            "text": "<pre><code>infer(\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Perform inference using the model.</p> <p>Parameters:</p> Name Type Description Default <code>postprocess_fn</code> <code>str</code> <p>The postprocessing function for inference.</p> required <code>writer</code> <code>str</code> <p>The writer to save the inference results.</p> required <code>test_batch_size</code> <code>optional</code> <p>The batch size for inference. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>max_size</code> <code>optional</code> <p>The maximum number of samples to process. Defaults to 10000.</p> <code>10000</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>output_header</code> <code>optional</code> <p>The header for the output file. Defaults to None.</p> <code>None</code> <code>output_path</code> <code>optional</code> <p>The path to save the output file. Defaults to \"./cache/predict.txt\".</p> <code>'./cache/predict.txt'</code> <code>postprocess_workers</code> <code>optional</code> <p>The number of worker processes for postprocessing. Defaults to 2.</p> <code>2</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@torch.no_grad()\n@add_default_section_for_function(\"core/task/supervised\")\ndef infer(\n    self,\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Perform inference using the model.\n\n    Args:\n        postprocess_fn: The postprocessing function for inference.\n        writer: The writer to save the inference results.\n        test_batch_size (optional): The batch size for inference. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        max_size (optional): The maximum number of samples to process. Defaults to 10000.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        output_header (optional): The header for the output file. Defaults to None.\n        output_path (optional): The path to save the output file. Defaults to \"./cache/predict.txt\".\n        postprocess_workers (optional): The number of worker processes for postprocessing. Defaults to 2.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    assert self.n_gpu &lt;= 1\n    assert writer is not None\n\n    output_dir = os.path.dirname(output_path)\n    if not os.path.exists(output_dir):\n        os.makedirs(output_dir, exist_ok=True)\n\n    if postprocess_fn is not None:\n        postprocess_fn = init_registered_process(postprocess_fn, self.config)\n\n    if writer is not None:\n        writer = init_registered_module(\n            writer,\n            self.config,\n            registered_writer,\n            output_file=output_path,\n        )\n\n    skip_step = writer.skip_n_samples\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if skip_step == 0:\n        sampler = SequentialSampler\n    else:\n        sampler = SequentialSkipSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_test = self.datasets.get(\"test\")\n    else:\n        dataset_test = self.datasets.get(\"test\")\n\n    iter_test = DataLoader(\n        dataset_test,\n        sampler=sampler(dataset_test)\n        if not isinstance(dataset_test, Iterable)\n        else None,\n        batch_size=test_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if skip_step &gt; 0 and hasattr(dataset_test, \"set_skip_step\"):\n        dataset_test.set_skip_step(skip_step)\n\n    if skip_step &gt; 0 and hasattr(iter_test.sampler, \"set_skip_step\"):\n        iter_test.sampler.set_skip_step(skip_step)\n\n    if hasattr(dataset_test, \"dataset\"):\n        data_info = dataset_test.dataset\n        data_info = DatasetFeature(data_info)\n        iter_data = DataLoader(\n            deepcopy(data_info),\n            sampler=sampler(data_info)\n            if not isinstance(dataset_test, Iterable)\n            else None,\n            batch_size=test_batch_size,\n            shuffle=False,\n            pin_memory=pin_memory,\n            num_workers=num_workers,\n            collate_fn=None,\n        )\n    else:\n        iter_data = None\n\n    if skip_step &gt; 0 and hasattr(iter_data.sampler, \"set_skip_step\"):\n        iter_data.sampler.set_skip_step(skip_step)\n\n    self.model.eval()\n    start = time.time()\n\n    data_queue = Queue(maxsize=max_size)\n    msg_queue = Queue(maxsize=max_size)\n    postprocess_list = []\n    for _ in range(postprocess_workers):\n        p = PostProcess(\n            postprocess_fn,\n            data_queue,\n            msg_queue,\n        )\n        postprocess_list.append(p)\n        p.start()\n\n    io_process = IOProcess(msg_queue, writer=writer)\n    io_process.start()\n\n    if iter_data is None:\n        for step, (inputs, _) in enumerate(iter_test):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            data_queue.put((step, outputs))\n    else:\n        for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            if output_header is not None:\n                _infos = {k: _infos[k] for k in output_header if k in _infos}\n                outputs.from_pandas(pd.DataFrame(_infos))\n            data_queue.put((step, outputs))\n\n    data_queue.put((-1, GENERATE_FINISHED))\n    for p in postprocess_list:\n        p.join()\n\n    msg_queue.put((-1, GENERATE_FINISHED))\n    io_process.join()\n\n    end = time.time()\n    ms = (end - start) * 1000\n    logging.info(\n        \"{:.2f} ms, {:.1f} sample/s\".format(\n            ms,\n            ((len(dataset_test) - skip_step) / ms * 1000),\n        )\n    )\n</code></pre>",
             "title": "infer"
         },
         {
             "location": "cli/supervised/#unitorch.cli.tasks.supervised.SupervisedTask.train",
-            "text": "<pre><code>train(\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Train the model.</p> <p>Parameters:</p> Name Type Description Default <code>optim</code> <code>str</code> <p>The optimizer for training.</p> required <code>loss_fn</code> <code>str</code> <p>The loss function for training.</p> required <code>score_fn</code> <code>str</code> <p>The scoring function for evaluation.</p> required <code>monitor_fns</code> <code>optional</code> <p>The monitoring functions for evaluation. Defaults to None.</p> <code>None</code> <code>scheduler</code> <code>optional</code> <p>The scheduler for adjusting the learning rate. Defaults to None.</p> <code>None</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>to_ckpt_dir</code> <code>optional</code> <p>The directory path to save checkpoints to. Defaults to \"./to_ckpt\".</p> <code>'./to_ckpt'</code> <code>train_batch_size</code> <code>optional</code> <p>The batch size for training. Defaults to 128.</p> <code>128</code> <code>dev_batch_size</code> <code>optional</code> <p>The batch size for evaluation. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>save_optimizer</code> <code>optional</code> <p>Whether to save the optimizer. Defaults to True.</p> <code>True</code> <code>save_scheduler</code> <code>optional</code> <p>Whether to save the scheduler. Defaults to True.</p> <code>True</code> <code>log_freq</code> <code>optional</code> <p>The frequency of logging training information. Defaults to 100.</p> <code>100</code> <code>ckpt_freq</code> <code>optional</code> <p>The frequency of saving checkpoints. Defaults to 10000.</p> <code>10000</code> <code>grad_acc_step</code> <code>optional</code> <p>The number of gradient accumulation steps. Defaults to 1.</p> <code>1</code> <code>max_grad_norm</code> <code>optional</code> <p>The maximum gradient norm for gradient clipping. Defaults to 1.0.</p> <code>1.0</code> <code>num_training_samples</code> <code>optional</code> <p>The number of training samples. Defaults to 1000000000.</p> <code>1000000000</code> <code>epochs</code> <code>optional</code> <p>The number of training epochs. Defaults to 5.</p> <code>5</code> <code>use_ema</code> <code>optional</code> <p>Whether to use exponential moving average. Defaults to False.</p> <code>False</code> <code>ema_decay</code> <code>optional</code> <p>The decay rate for exponential moving average. Defaults to 0.9999.</p> <code>0.9999</code> <code>ema_tau</code> <code>optional</code> <p>The time constant for exponential moving average. Defaults to 2000.</p> <code>2000</code> <code>use_amp</code> <code>optional</code> <p>Whether to use automatic mixed precision. Defaults to True.</p> <code>True</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@add_default_section_for_function(\"core/task/supervised\")\ndef train(\n    self,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Train the model.\n\n    Args:\n        optim: The optimizer for training.\n        loss_fn: The loss function for training.\n        score_fn: The scoring function for evaluation.\n        monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.\n        scheduler (optional): The scheduler for adjusting the learning rate. Defaults to None.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to \"./to_ckpt\".\n        train_batch_size (optional): The batch size for training. Defaults to 128.\n        dev_batch_size (optional): The batch size for evaluation. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        save_optimizer (optional): Whether to save the optimizer. Defaults to True.\n        save_scheduler (optional): Whether to save the scheduler. Defaults to True.\n        log_freq (optional): The frequency of logging training information. Defaults to 100.\n        ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.\n        grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.\n        max_grad_norm (optional): The maximum gradient norm for gradient clipping. Defaults to 1.0.\n        num_training_samples (optional): The number of training samples. Defaults to 1000000000.\n        epochs (optional): The number of training epochs. Defaults to 5.\n        use_ema (optional): Whether to use exponential moving average. Defaults to False.\n        ema_decay (optional): The decay rate for exponential moving average. Defaults to 0.9999.\n        ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.\n        use_amp (optional): Whether to use automatic mixed precision. Defaults to True.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:\n        os.makedirs(to_ckpt_dir, exist_ok=True)\n\n    if loss_fn is not None:\n        loss_fn = init_registered_module(loss_fn, self.config, registered_loss)\n\n    if score_fn is not None:\n        score_fn = init_registered_module(score_fn, self.config, registered_score)\n\n    if monitor_fns is not None:\n        monitor_fns = [\n            init_registered_module(monitor_fn, self.config, registered_score)\n            for monitor_fn in monitor_fns\n            if monitor_fn in registered_score\n        ]\n\n    if optim is not None and self.model is not None:\n        optim = init_registered_module(\n            optim,\n            self.config,\n            registered_optim,\n            params=self.model.parameters(),\n        )\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n        optim.from_checkpoint(from_ckpt_dir)\n\n    if os.path.exists(to_ckpt_dir):\n        self.model.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_model_latest.bin\",\n        )\n        optim.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_optim_latest.bin\",\n        )\n\n    info_path = os.path.join(to_ckpt_dir, \"info.json\")\n    if os.path.exists(info_path):\n        info = json.load(open(os.path.join(to_ckpt_dir, \"info.json\")))\n    else:\n        info = dict()\n\n    global_epoch = info.get(\"global_epoch\", 0)\n    global_step = info.get(\"global_step\", 0)\n    self.best_score = info.get(\"best_score\", self.best_score)\n\n    logging.info(f\"the best score is {self.best_score}\")\n\n    self.ema_model = None\n    if use_ema:\n        num_ema_steps = info.get(\"num_ema_steps\", 0)\n        self.ema_model = ExponentialMovingAverage(\n            self.model,\n            decay=ema_decay,\n            tau=ema_tau,\n            num_steps=num_ema_steps,\n        )\n        if os.path.exists(from_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                from_ckpt_dir,\n                weight_name=\"pytorch_ema_model.bin\",\n            )\n        if os.path.exists(to_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                to_ckpt_dir,\n                weight_name=\"pytorch_ema_model_latest.bin\",\n            )\n\n    for n, p in self.model.named_parameters():\n        logging.debug(\n            f\"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}\"\n        )\n\n    global_rank = -1\n    if self.n_gpu &gt; 1:\n        self.model = nn.parallel.DistributedDataParallel(\n            self.model,\n            device_ids=[self.local_rank],\n            output_device=self.local_rank,\n            find_unused_parameters=False,\n            broadcast_buffers=False,\n        )\n        global_rank = dist.get_rank()\n\n    train_sampler = DistributedSkipSampler if self.n_gpu &gt; 1 else RandomSkipSampler\n    dev_sampler = DistributedSampler if self.n_gpu &gt; 1 else SequentialSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_train = self.datasets.get(\"train\")\n            dataset_dev = self.datasets.get(\"dev\")\n    else:\n        dataset_train = self.datasets.get(\"train\")\n        dataset_dev = self.datasets.get(\"dev\")\n\n    iter_train = DataLoader(\n        dataset_train,\n        sampler=train_sampler(dataset_train)\n        if not isinstance(dataset_train, Iterable)\n        else None,\n        batch_size=train_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    iter_dev = DataLoader(\n        dataset_dev,\n        sampler=dev_sampler(dataset_dev)\n        if not isinstance(dataset_dev, Iterable)\n        else None,\n        batch_size=dev_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if scheduler is not None:\n        if not isinstance(dataset_train, Iterable):\n            num_training_steps = int(\n                epochs\n                * len(dataset_train)\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n        else:\n            num_training_steps = int(\n                epochs\n                * num_training_samples\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n\n        scheduler = init_registered_module(\n            scheduler,\n            self.config,\n            registered_scheduler,\n            optimizer=optim,\n            num_training_steps=num_training_steps,\n        )\n\n    if scheduler and os.path.exists(to_ckpt_dir):\n        scheduler.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_scheduler_latest.bin\",\n        )\n\n    if use_amp:\n        scaler = GradScaler()\n\n    log_loss = 0\n    dev_epoch = 0\n    for e in range(0, epochs):\n        torch.cuda.empty_cache()\n        if e &lt; global_epoch:\n            continue\n\n        if hasattr(dataset_train, \"set_epoch\"):\n            dataset_train.set_epoch(e)\n\n        if hasattr(dataset_train, \"set_skip_step\"):\n            dataset_train.set_skip_step(global_step * train_batch_size)\n\n        if hasattr(iter_train.sampler, \"set_epoch\"):\n            iter_train.sampler.set_epoch(e)\n\n        if hasattr(iter_train.sampler, \"set_skip_step\"):\n            iter_train.sampler.set_skip_step(global_step * train_batch_size)\n\n        self.model.train()\n        is_update_step = True\n        for step, (inputs, targets) in enumerate(iter_train):\n            step = step + global_step\n            is_update_step = False\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n                targets = targets.cuda()\n\n            if is_torch2_available():\n                with torch.cuda.amp.autocast(\n                    enabled=True\n                ) as autocast, torch.backends.cuda.sdp_kernel(\n                    enable_flash=False\n                ) as disable:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n            else:\n                with torch.cuda.amp.autocast(enabled=True) as autocast:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n\n            nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)\n            if use_amp:\n                scaler.scale(loss).backward()\n            else:\n                loss.backward()\n            log_loss += loss.data * grad_acc_step\n            if (step + 1) % grad_acc_step == 0:\n                is_update_step = True\n                if use_amp:\n                    scaler.step(optim)\n                    scaler.update()\n                else:\n                    optim.step()\n                if scheduler is not None:\n                    scheduler.step()\n                optim.zero_grad()\n\n                if use_ema and self.ema_model is not None:\n                    self.ema_model.step(\n                        self.model.module if self.n_gpu &gt; 1 else self.model\n                    )\n\n            if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:\n                logging.info(\n                    f\"epoch {e} step {step}: loss -- { log_loss / log_freq }\"\n                )\n                log_loss = 0\n\n            if (step + 1) % ckpt_freq == 0:\n                if hasattr(dataset_dev, \"set_epoch\"):\n                    dataset_dev.set_epoch(dev_epoch)\n\n                if hasattr(iter_dev.sampler, \"set_epoch\"):\n                    iter_dev.sampler.set_epoch(dev_epoch)\n\n                dev_epoch += 1\n                self.best_score = save_checkpoint(\n                    self.model.module if self.n_gpu &gt; 1 else self.model,\n                    to_ckpt_dir,\n                    iter_dev,\n                    score_fn,\n                    monitor_fns,\n                    optim=optim if save_optimizer else None,\n                    scheduler=scheduler if save_scheduler else None,\n                    ema_model=self.ema_ema_model if use_ema else None,\n                    best_score=self.best_score,\n                    info_path=info_path,\n                    local_rank=self.local_rank,\n                    global_epoch=e,\n                    global_step=step + 1,\n                )\n\n        if not is_update_step:\n            scaler.step(optim)\n            scaler.update()\n            if scheduler is not None:\n                scheduler.step()\n            optim.zero_grad()\n\n            if use_ema and self.ema_model is not None:\n                self.ema_model.step(\n                    self.model.module if self.n_gpu &gt; 1 else self.model\n                )\n\n        log_loss = 0\n\n        if hasattr(dataset_dev, \"set_epoch\"):\n            dataset_dev.set_epoch(dev_epoch)\n\n        if hasattr(iter_dev.sampler, \"set_epoch\"):\n            iter_dev.sampler.set_epoch(dev_epoch)\n\n        dev_epoch += 1\n\n        global_step = 0\n        self.best_score = save_checkpoint(\n            self.model.module if self.n_gpu &gt; 1 else self.model,\n            to_ckpt_dir,\n            iter_dev,\n            score_fn,\n            monitor_fns,\n            optim=optim if save_optimizer else None,\n            scheduler=scheduler if save_scheduler else None,\n            ema_model=self.ema_ema_model if use_ema else None,\n            best_score=self.best_score,\n            info_path=info_path,\n            local_rank=self.local_rank,\n            global_epoch=e,\n            global_step=step + 1,\n        )\n</code></pre>",
+            "text": "<pre><code>train(\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Train the model.</p> <p>Parameters:</p> Name Type Description Default <code>optim</code> <code>str</code> <p>The optimizer for training.</p> required <code>loss_fn</code> <code>str</code> <p>The loss function for training.</p> required <code>score_fn</code> <code>str</code> <p>The scoring function for evaluation.</p> required <code>monitor_fns</code> <code>optional</code> <p>The monitoring functions for evaluation. Defaults to None.</p> <code>None</code> <code>scheduler</code> <code>optional</code> <p>The scheduler for adjusting the learning rate. Defaults to None.</p> <code>None</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>to_ckpt_dir</code> <code>optional</code> <p>The directory path to save checkpoints to. Defaults to \"./to_ckpt\".</p> <code>'./to_ckpt'</code> <code>train_batch_size</code> <code>optional</code> <p>The batch size for training. Defaults to 128.</p> <code>128</code> <code>dev_batch_size</code> <code>optional</code> <p>The batch size for evaluation. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>save_optimizer</code> <code>optional</code> <p>Whether to save the optimizer. Defaults to True.</p> <code>True</code> <code>save_scheduler</code> <code>optional</code> <p>Whether to save the scheduler. Defaults to True.</p> <code>True</code> <code>log_freq</code> <code>optional</code> <p>The frequency of logging training information. Defaults to 100.</p> <code>100</code> <code>ckpt_freq</code> <code>optional</code> <p>The frequency of saving checkpoints. Defaults to 10000.</p> <code>10000</code> <code>grad_acc_step</code> <code>optional</code> <p>The number of gradient accumulation steps. Defaults to 1.</p> <code>1</code> <code>max_grad_norm</code> <code>optional</code> <p>The maximum gradient norm for gradient clipping. Defaults to 1.0.</p> <code>1.0</code> <code>num_training_samples</code> <code>optional</code> <p>The number of training samples. Defaults to 1000000000.</p> <code>1000000000</code> <code>epochs</code> <code>optional</code> <p>The number of training epochs. Defaults to 5.</p> <code>5</code> <code>use_ema</code> <code>optional</code> <p>Whether to use exponential moving average. Defaults to False.</p> <code>False</code> <code>ema_decay</code> <code>optional</code> <p>The decay rate for exponential moving average. Defaults to 0.9999.</p> <code>0.9999</code> <code>ema_tau</code> <code>optional</code> <p>The time constant for exponential moving average. Defaults to 2000.</p> <code>2000</code> <code>use_amp</code> <code>optional</code> <p>Whether to use automatic mixed precision. Defaults to True.</p> <code>True</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@add_default_section_for_function(\"core/task/supervised\")\ndef train(\n    self,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Train the model.\n\n    Args:\n        optim: The optimizer for training.\n        loss_fn: The loss function for training.\n        score_fn: The scoring function for evaluation.\n        monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.\n        scheduler (optional): The scheduler for adjusting the learning rate. Defaults to None.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to \"./to_ckpt\".\n        train_batch_size (optional): The batch size for training. Defaults to 128.\n        dev_batch_size (optional): The batch size for evaluation. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        save_optimizer (optional): Whether to save the optimizer. Defaults to True.\n        save_scheduler (optional): Whether to save the scheduler. Defaults to True.\n        log_freq (optional): The frequency of logging training information. Defaults to 100.\n        ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.\n        grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.\n        max_grad_norm (optional): The maximum gradient norm for gradient clipping. Defaults to 1.0.\n        num_training_samples (optional): The number of training samples. Defaults to 1000000000.\n        epochs (optional): The number of training epochs. Defaults to 5.\n        use_ema (optional): Whether to use exponential moving average. Defaults to False.\n        ema_decay (optional): The decay rate for exponential moving average. Defaults to 0.9999.\n        ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.\n        use_amp (optional): Whether to use automatic mixed precision. Defaults to True.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:\n        os.makedirs(to_ckpt_dir, exist_ok=True)\n\n    if loss_fn is not None:\n        loss_fn = init_registered_module(loss_fn, self.config, registered_loss)\n\n    if score_fn is not None:\n        score_fn = init_registered_module(score_fn, self.config, registered_score)\n\n    if monitor_fns is not None:\n        monitor_fns = [\n            init_registered_module(monitor_fn, self.config, registered_score)\n            for monitor_fn in monitor_fns\n            if monitor_fn in registered_score\n        ]\n\n    if optim is not None and self.model is not None:\n        optim = init_registered_module(\n            optim,\n            self.config,\n            registered_optim,\n            params=self.model.parameters(),\n        )\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n        optim.from_checkpoint(from_ckpt_dir, weight_name=\"pytorch_optim.bin\",)\n\n    if os.path.exists(to_ckpt_dir):\n        self.model.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_model_latest.bin\",\n        )\n        optim.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_optim_latest.bin\",\n        )\n\n    info_path = os.path.join(to_ckpt_dir, \"info.json\")\n    if os.path.exists(info_path):\n        info = json.load(open(os.path.join(to_ckpt_dir, \"info.json\")))\n    else:\n        info = dict()\n\n    global_epoch = info.get(\"global_epoch\", 0)\n    global_step = info.get(\"global_step\", 0)\n    self.best_score = info.get(\"best_score\", self.best_score)\n\n    logging.info(f\"the best score is {self.best_score}\")\n\n    self.ema_model = None\n    if use_ema:\n        num_ema_steps = info.get(\"num_ema_steps\", 0)\n        self.ema_model = ExponentialMovingAverage(\n            self.model,\n            decay=ema_decay,\n            tau=ema_tau,\n            num_steps=num_ema_steps,\n        )\n        if os.path.exists(from_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                from_ckpt_dir,\n                weight_name=\"pytorch_ema_model.bin\",\n            )\n        if os.path.exists(to_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                to_ckpt_dir,\n                weight_name=\"pytorch_ema_model_latest.bin\",\n            )\n\n    for n, p in self.model.named_parameters():\n        logging.debug(\n            f\"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}\"\n        )\n\n    global_rank = -1\n    if self.n_gpu &gt; 1:\n        self.model = nn.parallel.DistributedDataParallel(\n            self.model,\n            device_ids=[self.local_rank],\n            output_device=self.local_rank,\n            find_unused_parameters=False,\n            broadcast_buffers=False,\n        )\n        global_rank = dist.get_rank()\n\n    train_sampler = DistributedSkipSampler if self.n_gpu &gt; 1 else RandomSkipSampler\n    dev_sampler = DistributedSampler if self.n_gpu &gt; 1 else SequentialSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_train = self.datasets.get(\"train\")\n            dataset_dev = self.datasets.get(\"dev\")\n    else:\n        dataset_train = self.datasets.get(\"train\")\n        dataset_dev = self.datasets.get(\"dev\")\n\n    iter_train = DataLoader(\n        dataset_train,\n        sampler=train_sampler(dataset_train)\n        if not isinstance(dataset_train, Iterable)\n        else None,\n        batch_size=train_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    iter_dev = DataLoader(\n        dataset_dev,\n        sampler=dev_sampler(dataset_dev)\n        if not isinstance(dataset_dev, Iterable)\n        else None,\n        batch_size=dev_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if scheduler is not None:\n        if not isinstance(dataset_train, Iterable):\n            num_training_steps = int(\n                epochs\n                * len(dataset_train)\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n        else:\n            num_training_steps = int(\n                epochs\n                * num_training_samples\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n\n        scheduler = init_registered_module(\n            scheduler,\n            self.config,\n            registered_scheduler,\n            optimizer=optim,\n            num_training_steps=num_training_steps,\n        )\n\n    if scheduler and os.path.exists(to_ckpt_dir):\n        scheduler.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_scheduler_latest.bin\",\n        )\n\n    if use_amp:\n        scaler = GradScaler()\n\n    log_loss = 0\n    dev_epoch = 0\n    for e in range(0, epochs):\n        torch.cuda.empty_cache()\n        if e &lt; global_epoch:\n            continue\n\n        if hasattr(dataset_train, \"set_epoch\"):\n            dataset_train.set_epoch(e)\n\n        if hasattr(dataset_train, \"set_skip_step\"):\n            dataset_train.set_skip_step(global_step * train_batch_size)\n\n        if hasattr(iter_train.sampler, \"set_epoch\"):\n            iter_train.sampler.set_epoch(e)\n\n        if hasattr(iter_train.sampler, \"set_skip_step\"):\n            iter_train.sampler.set_skip_step(global_step * train_batch_size)\n\n        self.model.train()\n        is_update_step = True\n        for step, (inputs, targets) in enumerate(iter_train):\n            step = step + global_step\n            is_update_step = False\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n                targets = targets.cuda()\n\n            if is_torch2_available():\n                with torch.cuda.amp.autocast(\n                    enabled=True\n                ) as autocast, torch.backends.cuda.sdp_kernel(\n                    enable_flash=False\n                ) as disable:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n            else:\n                with torch.cuda.amp.autocast(enabled=True) as autocast:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n\n            nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)\n            if use_amp:\n                scaler.scale(loss).backward()\n            else:\n                loss.backward()\n            log_loss += loss.data * grad_acc_step\n            if (step + 1) % grad_acc_step == 0:\n                is_update_step = True\n                if use_amp:\n                    scaler.step(optim)\n                    scaler.update()\n                else:\n                    optim.step()\n                if scheduler is not None:\n                    scheduler.step()\n                optim.zero_grad()\n\n                if use_ema and self.ema_model is not None:\n                    self.ema_model.step(\n                        self.model.module if self.n_gpu &gt; 1 else self.model\n                    )\n\n            if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:\n                logging.info(\n                    f\"epoch {e} step {step}: loss -- { log_loss / log_freq }\"\n                )\n                log_loss = 0\n\n            if (step + 1) % ckpt_freq == 0:\n                if hasattr(dataset_dev, \"set_epoch\"):\n                    dataset_dev.set_epoch(dev_epoch)\n\n                if hasattr(iter_dev.sampler, \"set_epoch\"):\n                    iter_dev.sampler.set_epoch(dev_epoch)\n\n                dev_epoch += 1\n                self.best_score = save_checkpoint(\n                    self.model.module if self.n_gpu &gt; 1 else self.model,\n                    to_ckpt_dir,\n                    iter_dev,\n                    score_fn,\n                    monitor_fns,\n                    optim=optim if save_optimizer else None,\n                    scheduler=scheduler if save_scheduler else None,\n                    ema_model=self.ema_model if use_ema else None,\n                    best_score=self.best_score,\n                    info_path=info_path,\n                    local_rank=self.local_rank,\n                    global_epoch=e,\n                    global_step=step + 1,\n                )\n\n        if not is_update_step:\n            scaler.step(optim)\n            scaler.update()\n            if scheduler is not None:\n                scheduler.step()\n            optim.zero_grad()\n\n            if use_ema and self.ema_model is not None:\n                self.ema_model.step(\n                    self.model.module if self.n_gpu &gt; 1 else self.model\n                )\n\n        log_loss = 0\n\n        if hasattr(dataset_dev, \"set_epoch\"):\n            dataset_dev.set_epoch(dev_epoch)\n\n        if hasattr(iter_dev.sampler, \"set_epoch\"):\n            iter_dev.sampler.set_epoch(dev_epoch)\n\n        dev_epoch += 1\n\n        global_step = 0\n        self.best_score = save_checkpoint(\n            self.model.module if self.n_gpu &gt; 1 else self.model,\n            to_ckpt_dir,\n            iter_dev,\n            score_fn,\n            monitor_fns,\n            optim=optim if save_optimizer else None,\n            scheduler=scheduler if save_scheduler else None,\n            ema_model=self.ema_model if use_ema else None,\n            best_score=self.best_score,\n            info_path=info_path,\n            local_rank=self.local_rank,\n            global_epoch=e,\n            global_step=0,\n        )\n</code></pre>",
             "title": "train"
         },
         {
             "location": "cli/models/bart/",
             "text": "",
             "title": "unitorch.cli.models.bart"
         },
@@ -1622,15 +1622,15 @@
         {
             "location": "models/#unitorch.models.CheckpointMixin.from_checkpoint",
             "text": "<pre><code>from_checkpoint(\n    ckpt_dir: str,\n    weight_name: Optional[str] = None,\n    **kwargs: Optional[str]\n)\n</code></pre> <p>Load model weights from a checkpoint.</p> <p>Parameters:</p> Name Type Description Default <code>ckpt_dir</code> <code>str</code> <p>Directory path of the checkpoint.</p> required <code>weight_name</code> <code>str</code> <p>Name of the weight file.</p> <code>None</code> <p>Returns:</p> Type Description <p>None</p> Source code in <code>src/unitorch/models/__init__.py</code> <pre><code>def from_checkpoint(\n    self,\n    ckpt_dir: str,\n    weight_name: Optional[str] = None,\n    **kwargs,\n):\n\"\"\"\n    Load model weights from a checkpoint.\n\n    Args:\n        ckpt_dir (str): Directory path of the checkpoint.\n        weight_name (str): Name of the weight file.\n\n    Returns:\n        None\n    \"\"\"\n    if weight_name is None:\n        weight_name = self.checkpoint_name\n    weight_path = os.path.join(ckpt_dir, weight_name)\n    if not os.path.exists(weight_path):\n        return\n    state_dict = torch.load(weight_path, map_location=\"cpu\")\n    self.load_state_dict(state_dict)\n    logging.info(\n        f\"{type(self).__name__} model load weight from checkpoint {weight_path}\"\n    )\n</code></pre>",
             "title": "from_checkpoint"
         },
         {
             "location": "models/#unitorch.models.CheckpointMixin.from_pretrained",
-            "text": "<pre><code>from_pretrained(\n    weight_path: Union[str, List[str]] = None,\n    state_dict: Union[Dict, List[Dict]] = None,\n    replace_keys: Optional[Dict] = dict(),\n    prefix_keys: Optional[Dict] = dict(),\n)\n</code></pre> <p>Load pretrained weights into the model.</p> <p>Parameters:</p> Name Type Description Default <code>weight_path</code> <code>str or List[str]</code> <p>Path(s) to the pretrained weight file(s).</p> <code>None</code> <code>state_dict</code> <code>Dict or List[Dict]</code> <p>Pretrained state_dict(s) to load weights from.</p> <code>None</code> <code>replace_keys</code> <code>Dict</code> <p>Dictionary mapping keys in the pretrained state_dict to the model's keys.</p> <code>dict()</code> <code>prefix_keys</code> <code>Dict</code> <p>Dictionary prefix keys in the pretrained state_dict to the model's keys.</p> <code>dict()</code> <p>Returns:</p> Type Description <p>None</p> Source code in <code>src/unitorch/models/__init__.py</code> <pre><code>def from_pretrained(\n    self,\n    weight_path: Union[str, List[str]] = None,\n    state_dict: Union[Dict, List[Dict]] = None,\n    replace_keys: Optional[Dict] = dict(),\n    prefix_keys: Optional[Dict] = dict(),\n):\n\"\"\"\n    Load pretrained weights into the model.\n\n    Args:\n        weight_path (str or List[str]): Path(s) to the pretrained weight file(s).\n        state_dict (Dict or List[Dict]): Pretrained state_dict(s) to load weights from.\n        replace_keys (Dict): Dictionary mapping keys in the pretrained state_dict to the model's keys.\n        prefix_keys (Dict): Dictionary prefix keys in the pretrained state_dict to the model's keys.\n\n    Returns:\n        None\n    \"\"\"\n    assert weight_path or state_dict, \"weight_path or state_dict must be set\"\n\n    # Load state_dict(s) based on the provided weight_path or state_dict\n    if weight_path:\n        if isinstance(weight_path, str):\n            weight_path = [weight_path]\n        for path in weight_path:\n            logging.debug(f\"Loading weights from {path}\")\n        state_dicts = [\n            torch.load(hf_cached_path(path), map_location=\"cpu\")\n            for path in weight_path\n        ]\n    else:\n        state_dicts = state_dict if isinstance(state_dict, list) else [state_dict]\n\n    self_state_dict = self.state_dict()  # Get the current state_dict of the model\n    load_keys = []  # Keep track of the keys loaded from the state_dict(s)\n    non_load_keys = []  # Keep track of the keys not loaded from the state_dict(s)\n\n    if isinstance(self.replace_keys_in_state_dict, dict):\n        replace_keys = {**self.replace_keys_in_state_dict, **replace_keys}\n\n    if isinstance(self.prefix_keys_in_state_dict, dict):\n        prefix_keys = {**self.prefix_keys_in_state_dict, **prefix_keys}\n\n    # Iterate over the state_dict(s) and load the matching keys into the model's state_dict\n    for _state_dict in state_dicts:\n        if not _state_dict:\n            continue\n        for key, value in list(_state_dict.items()):\n            for rkey, prefix in prefix_keys.items():\n                if re.match(rkey, key):\n                    key = prefix + key\n                    break\n\n            for rkey, nkey in replace_keys.items():\n                key = re.sub(rkey, nkey, key)\n            if key in self_state_dict and value.shape == self_state_dict[key].shape:\n                self_state_dict[key] = value\n                load_keys.append(key)\n            else:\n                non_load_keys.append(key)\n\n    self.load_state_dict(self_state_dict, False)\n    load_percent = (\n        len(load_keys) / len(self_state_dict) * 100\n    )  # Calculate the percentage of loaded keys\n    logging.debug(f\"Non load keys in pretrain weights: {list(non_load_keys)}\")\n    logging.debug(\n        f\"{type(self).__name__} model missed keys: {list(self_state_dict.keys() - load_keys)}\"\n    )\n    logging.info(\n        f\"{type(self).__name__} model loaded weights ({int(load_percent)}%)\"\n    )\n</code></pre>",
+            "text": "<pre><code>from_pretrained(\n    weight_path: Union[str, List[str]] = None,\n    state_dict: Union[Dict, List[Dict]] = None,\n    replace_keys: Optional[Dict] = dict(),\n    prefix_keys: Optional[Dict] = dict(),\n)\n</code></pre> <p>Load pretrained weights into the model.</p> <p>Parameters:</p> Name Type Description Default <code>weight_path</code> <code>str or List[str]</code> <p>Path(s) to the pretrained weight file(s).</p> <code>None</code> <code>state_dict</code> <code>Dict or List[Dict]</code> <p>Pretrained state_dict(s) to load weights from.</p> <code>None</code> <code>replace_keys</code> <code>Dict</code> <p>Dictionary mapping keys in the pretrained state_dict to the model's keys.</p> <code>dict()</code> <code>prefix_keys</code> <code>Dict</code> <p>Dictionary prefix keys in the pretrained state_dict to the model's keys.</p> <code>dict()</code> <p>Returns:</p> Type Description <p>None</p> Source code in <code>src/unitorch/models/__init__.py</code> <pre><code>def from_pretrained(\n    self,\n    weight_path: Union[str, List[str]] = None,\n    state_dict: Union[Dict, List[Dict]] = None,\n    replace_keys: Optional[Dict] = dict(),\n    prefix_keys: Optional[Dict] = dict(),\n):\n\"\"\"\n    Load pretrained weights into the model.\n\n    Args:\n        weight_path (str or List[str]): Path(s) to the pretrained weight file(s).\n        state_dict (Dict or List[Dict]): Pretrained state_dict(s) to load weights from.\n        replace_keys (Dict): Dictionary mapping keys in the pretrained state_dict to the model's keys.\n        prefix_keys (Dict): Dictionary prefix keys in the pretrained state_dict to the model's keys.\n\n    Returns:\n        None\n    \"\"\"\n    assert weight_path or state_dict, \"weight_path or state_dict must be set\"\n\n    # Load state_dict(s) based on the provided weight_path or state_dict\n    state_dicts = []\n    if weight_path:\n        if isinstance(weight_path, str):\n            weight_path = [weight_path]\n        for path in weight_path:\n            logging.debug(f\"Loading weights from {path}\")\n        state_dicts += [\n            torch.load(hf_cached_path(path), map_location=\"cpu\")\n            for path in weight_path\n        ]\n\n    if state_dict:\n        state_dicts += state_dict if isinstance(state_dict, list) else [state_dict]\n\n    self_state_dict = self.state_dict()  # Get the current state_dict of the model\n    load_keys = []  # Keep track of the keys loaded from the state_dict(s)\n    non_load_keys = []  # Keep track of the keys not loaded from the state_dict(s)\n\n    if isinstance(self.replace_keys_in_state_dict, dict):\n        replace_keys = {**self.replace_keys_in_state_dict, **replace_keys}\n\n    if isinstance(self.prefix_keys_in_state_dict, dict):\n        prefix_keys = {**self.prefix_keys_in_state_dict, **prefix_keys}\n\n    # Iterate over the state_dict(s) and load the matching keys into the model's state_dict\n    for _state_dict in state_dicts:\n        if not _state_dict:\n            continue\n        for key, value in list(_state_dict.items()):\n            for rkey, prefix in prefix_keys.items():\n                if re.match(rkey, key):\n                    key = prefix + key\n                    break\n\n            for rkey, nkey in replace_keys.items():\n                key = re.sub(rkey, nkey, key)\n            if key in self_state_dict and value.shape == self_state_dict[key].shape:\n                self_state_dict[key] = value\n                load_keys.append(key)\n            else:\n                non_load_keys.append(key)\n\n    self.load_state_dict(self_state_dict, False)\n    load_percent = (\n        len(load_keys) / len(self_state_dict) * 100\n    )  # Calculate the percentage of loaded keys\n    logging.debug(f\"Non load keys in pretrain weights: {list(non_load_keys)}\")\n    logging.debug(\n        f\"{type(self).__name__} model missed keys: {list(self_state_dict.keys() - load_keys)}\"\n    )\n    logging.info(\n        f\"{type(self).__name__} model loaded weights ({int(load_percent)}%)\"\n    )\n</code></pre>",
             "title": "from_pretrained"
         },
         {
             "location": "models/#unitorch.models.CheckpointMixin.save_checkpoint",
             "text": "<pre><code>save_checkpoint(\n    ckpt_dir: str,\n    weight_name: Optional[str] = None,\n    **kwargs: Optional[str]\n)\n</code></pre> <p>Save the model's current state as a checkpoint.</p> <p>Parameters:</p> Name Type Description Default <code>ckpt_dir</code> <code>str</code> <p>Directory path to save the checkpoint.</p> required <code>weight_name</code> <code>str</code> <p>Name of the weight file.</p> <code>None</code> <p>Returns:</p> Type Description <p>None</p> Source code in <code>src/unitorch/models/__init__.py</code> <pre><code>def save_checkpoint(\n    self,\n    ckpt_dir: str,\n    weight_name: Optional[str] = None,\n    **kwargs,\n):\n\"\"\"\n    Save the model's current state as a checkpoint.\n\n    Args:\n        ckpt_dir (str): Directory path to save the checkpoint.\n        weight_name (str): Name of the weight file.\n\n    Returns:\n        None\n    \"\"\"\n    if weight_name is None:\n        weight_name = self.checkpoint_name\n    state_dict = self.state_dict()\n    weight_path = os.path.join(ckpt_dir, weight_name)\n    torch.save(state_dict, weight_path)\n    logging.info(f\"{type(self).__name__} model save checkpoint to {weight_path}\")\n</code></pre>",
             "title": "save_checkpoint"
         },
@@ -1722,20 +1722,20 @@
         {
             "location": "models/bart/#bartprocessor",
             "text": "<p>         Bases: <code>HfTextGenerationProcessor</code></p> <p>Processor for BART model. Inherits from HfTextGenerationProcessor.</p> <p>Initializes the BartProcessor.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_path</code> <code>str</code> <p>Path to the vocabulary file.</p> required <code>merge_path</code> <code>str</code> <p>Path to the BPE merge file.</p> required <code>special_input_ids</code> <code>Optional[Dict]</code> <p>Optional dictionary of special input IDs.</p> <code>dict()</code> <code>max_seq_length</code> <code>Optional[int]</code> <p>Maximum sequence length.</p> <code>128</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>Maximum generation sequence length.</p> <code>48</code> Source code in <code>src/unitorch/models/bart/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_path: str,\n    merge_path: str,\n    special_input_ids: Optional[Dict] = dict(),\n    max_seq_length: Optional[int] = 128,\n    max_gen_seq_length: Optional[int] = 48,\n):\n\"\"\"\n    Initializes the BartProcessor.\n\n    Args:\n        vocab_path (str): Path to the vocabulary file.\n        merge_path (str): Path to the BPE merge file.\n        special_input_ids (Optional[Dict]): Optional dictionary of special input IDs.\n        max_seq_length (Optional[int]): Maximum sequence length.\n        max_gen_seq_length (Optional[int]): Maximum generation sequence length.\n    \"\"\"\n    tokenizer = get_bart_tokenizer(\n        vocab_path,\n        merge_path,\n        special_input_ids=special_input_ids,\n    )\n    super().__init__(\n        tokenizer=tokenizer,\n        max_seq_length=max_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n    )\n</code></pre>",
             "title": "BartProcessor"
         },
         {
             "location": "models/bart/#bartforgeneration",
-            "text": "<p>         Bases: <code>GenericModel</code></p> <p>BART model for text generation.</p> <p>Initializes a BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>Path to the BART model configuration file.</p> required <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes a BartForGeneration model.\n\n    Args:\n        config_path (str): Path to the BART model configuration file.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.config = BartConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.model = BartForConditionalGeneration(self.config)\n    self.init_weights()\n</code></pre>",
+            "text": "<p>         Bases: <code>GenericModel</code></p> <p>BART model for text generation.</p> <p>Initializes a BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>Path to the BART model configuration file.</p> required <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes a BartForGeneration model.\n\n    Args:\n        config_path (str): Path to the BART model configuration file.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.config = BartConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.config.forced_bos_token_id = None\n    self.model = BartForConditionalGeneration(self.config)\n    self.init_weights()\n</code></pre>",
             "title": "BartForGeneration"
         },
         {
             "location": "models/bart/#unitorch.models.bart.modeling.BartForGeneration.forward",
-            "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which tokens should be attended to.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which decoder tokens should be attended to.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Output logits of the model.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor indicating which tokens should be attended to.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor indicating which decoder tokens should be attended to.\n\n    Returns:\n        (torch.Tensor): Output logits of the model.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
+            "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which tokens should be attended to.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which decoder tokens should be attended to.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Output logits of the model.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor indicating which tokens should be attended to.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor indicating which decoder tokens should be attended to.\n\n    Returns:\n        (torch.Tensor): Output logits of the model.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    print(\"model :\", logits[0, 0, 0].item(), logits[0, 0, 41552].item())\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/bart/#unitorch.models.bart.modeling.BartForGeneration.generate",
             "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates text using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling during generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates text using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling during generation. Defaults to False.\n        temperature (float, optional): Temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): Value for top-k sampling. Defaults to 50.\n        top_p (float, optional): Value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
             "title": "generate"
         },
@@ -1767,15 +1767,15 @@
         {
             "location": "models/bert/#bertprocessor",
             "text": "<p>         Bases: <code>HfTextClassificationProcessor</code></p> <p>Initializes the BertProcessor.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_path</code> <code>str</code> <p>The path to the vocabulary file.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length. Defaults to 128.</p> <code>128</code> <code>special_input_ids</code> <code>Optional[Dict]</code> <p>Special input IDs mapping. Defaults to an empty dictionary.</p> <code>dict()</code> <code>do_lower_case</code> <code>Optional[bool]</code> <p>Whether to perform lowercase tokenization. Defaults to True.</p> <code>True</code> <code>do_basic_tokenize</code> <code>Optional[bool]</code> <p>Whether to perform basic tokenization. Defaults to True.</p> <code>True</code> <code>do_whole_word_mask</code> <code>Optional[bool]</code> <p>Whether to perform whole word masking. Defaults to True.</p> <code>True</code> <code>masked_lm_prob</code> <code>Optional[float]</code> <p>The probability of masking a token for pretraining. Defaults to 0.15.</p> <code>0.15</code> <code>max_predictions_per_seq</code> <code>Optional[int]</code> <p>The maximum number of masked tokens per sequence for pretraining. Defaults to 20.</p> <code>20</code> Source code in <code>src/unitorch/models/bert/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_path: str,\n    max_seq_length: Optional[int] = 128,\n    special_input_ids: Optional[Dict] = dict(),\n    do_lower_case: Optional[bool] = True,\n    do_basic_tokenize: Optional[bool] = True,\n    do_whole_word_mask: Optional[bool] = True,\n    masked_lm_prob: Optional[float] = 0.15,\n    max_predictions_per_seq: Optional[int] = 20,\n):\n\"\"\"\n    Initializes the BertProcessor.\n\n    Args:\n        vocab_path (str): The path to the vocabulary file.\n        max_seq_length (Optional[int], optional): The maximum sequence length. Defaults to 128.\n        special_input_ids (Optional[Dict], optional): Special input IDs mapping. Defaults to an empty dictionary.\n        do_lower_case (Optional[bool], optional): Whether to perform lowercase tokenization. Defaults to True.\n        do_basic_tokenize (Optional[bool], optional): Whether to perform basic tokenization. Defaults to True.\n        do_whole_word_mask (Optional[bool], optional): Whether to perform whole word masking. Defaults to True.\n        masked_lm_prob (Optional[float], optional): The probability of masking a token for pretraining. Defaults to 0.15.\n        max_predictions_per_seq (Optional[int], optional): The maximum number of masked tokens per sequence for pretraining. Defaults to 20.\n    \"\"\"\n    tokenizer = get_bert_tokenizer(\n        vocab_path,\n        do_lower_case=do_lower_case,\n        do_basic_tokenize=do_basic_tokenize,\n        special_input_ids=special_input_ids,\n    )\n    super().__init__(\n        tokenizer=tokenizer,\n        max_seq_length=max_seq_length,\n    )\n    self.do_whole_word_mask = do_whole_word_mask\n    self.masked_lm_prob = masked_lm_prob\n    self.max_predictions_per_seq = max_predictions_per_seq\n    self.vocab_words = list(self.tokenizer.vocab.keys())\n</code></pre>",
             "title": "BertProcessor"
         },
         {
             "location": "models/bert/#unitorch.models.bert.processing.BertProcessor.pretrain",
-            "text": "<pre><code>pretrain(\n    text: str,\n    text_pair: str,\n    nsp_label: int,\n    max_seq_length: Optional[int] = None,\n    masked_lm_prob: Optional[float] = None,\n    do_whole_word_mask: Optional[bool] = None,\n    max_predictions_per_seq: Optional[int] = None,\n)\n</code></pre> <p>The Bert pretrain processor on the given text and text pair.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>The input text.</p> required <code>text_pair</code> <code>str</code> <p>The input text pair.</p> required <code>nsp_label</code> <code>int</code> <p>The next sentence prediction label.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length. Defaults to None.</p> <code>None</code> <code>masked_lm_prob</code> <code>Optional[float]</code> <p>The probability of masking a token for pretraining. Defaults to None.</p> <code>None</code> <code>do_whole_word_mask</code> <code>Optional[bool]</code> <p>Whether to perform whole word masking. Defaults to None.</p> <code>None</code> <code>max_predictions_per_seq</code> <code>Optional[int]</code> <p>The maximum number of masked tokens per sequence for pretraining. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>pretrain processing outputs.</p> Source code in <code>src/unitorch/models/bert/processing.py</code> <pre><code>def pretrain(\n    self,\n    text: str,\n    text_pair: str,\n    nsp_label: int,\n    max_seq_length: Optional[int] = None,\n    masked_lm_prob: Optional[float] = None,\n    do_whole_word_mask: Optional[bool] = None,\n    max_predictions_per_seq: Optional[int] = None,\n):\n\"\"\"\n    The Bert pretrain processor on the given text and text pair.\n\n    Args:\n        text (str): The input text.\n        text_pair (str): The input text pair.\n        nsp_label (int): The next sentence prediction label.\n        max_seq_length (Optional[int], optional): The maximum sequence length. Defaults to None.\n        masked_lm_prob (Optional[float], optional): The probability of masking a token for pretraining. Defaults to None.\n        do_whole_word_mask (Optional[bool], optional): Whether to perform whole word masking. Defaults to None.\n        max_predictions_per_seq (Optional[int], optional): The maximum number of masked tokens per sequence for pretraining. Defaults to None.\n\n    Returns:\n        GenericOutputs: pretrain processing outputs.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n\n    masked_lm_prob = pop_value(\n        masked_lm_prob,\n        self.masked_lm_prob,\n    )\n\n    do_whole_word_mask = pop_value(\n        do_whole_word_mask,\n        self.do_whole_word_mask,\n    )\n\n    max_predictions_per_seq = pop_value(\n        max_predictions_per_seq,\n        self.max_predictions_per_seq,\n    )\n\n    tokens = self.tokenizer.tokenize(str(text))\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))\n    truncate_sequence_pair(tokens, tokens_pair, max_seq_length - 3)\n    tokens = (\n        [self.cls_token]\n        + tokens\n        + [self.sep_token]\n        + tokens_pair\n        + [self.sep_token]\n    )\n\n    covered_indexes = get_random_mask_indexes(\n        tokens,\n        masked_lm_prob,\n        do_whole_word_mask,\n        max_predictions_per_seq,\n        special_tokens=[self.cls_token, self.sep_token],\n    )\n    label = [\n        tokens[pos] if pos in covered_indexes else self.pad_token\n        for pos in range(max_seq_length)\n    ]\n    label_mask = [\n        1 if pos in covered_indexes else 0 for pos in range(max_seq_length)\n    ]\n    label = self.tokenizer.convert_tokens_to_ids(label)\n\n    for index in covered_indexes:\n        mask_token = None\n        if random.random() &lt; 0.8:\n            mask_token = self.mask_token\n        else:\n            mask_token = (\n                tokens[index]\n                if random.random() &lt; 0.5\n                else get_random_word(self.vocab_words)\n            )\n        tokens[index] = mask_token\n\n    input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n    token_type_ids = [0] + [0] * len(tokens) + [0] + [1] * len(tokens_pair) + [1]\n    attention_mask = [1] * len(input_ids)\n\n    padding = [0] * (max_seq_length - len(input_ids))\n    input_ids += len(padding) * [self.pad_token_id]\n    attention_mask += padding\n    token_type_ids += len(padding) * [1]\n\n    assert len(input_ids) == max_seq_length\n    assert len(attention_mask) == max_seq_length\n    assert len(token_type_ids) == max_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        token_type_ids=torch.tensor(token_type_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n        position_ids=torch.tensor(list(range(max_seq_length)), dtype=torch.long),\n        nsp_label=torch.tensor(int(nsp_label), dtype=torch.long),\n        mlm_label=torch.tensor(label, dtype=torch.long),\n        mlm_label_mask=torch.tensor(label_mask, dtype=torch.long),\n    )\n</code></pre>",
+            "text": "<pre><code>pretrain(\n    text: str,\n    text_pair: str,\n    nsp_label: int,\n    max_seq_length: Optional[int] = None,\n    masked_lm_prob: Optional[float] = None,\n    do_whole_word_mask: Optional[bool] = None,\n    max_predictions_per_seq: Optional[int] = None,\n)\n</code></pre> <p>The Bert pretrain processor on the given text and text pair.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>The input text.</p> required <code>text_pair</code> <code>str</code> <p>The input text pair.</p> required <code>nsp_label</code> <code>int</code> <p>The next sentence prediction label.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length. Defaults to None.</p> <code>None</code> <code>masked_lm_prob</code> <code>Optional[float]</code> <p>The probability of masking a token for pretraining. Defaults to None.</p> <code>None</code> <code>do_whole_word_mask</code> <code>Optional[bool]</code> <p>Whether to perform whole word masking. Defaults to None.</p> <code>None</code> <code>max_predictions_per_seq</code> <code>Optional[int]</code> <p>The maximum number of masked tokens per sequence for pretraining. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>pretrain processing outputs.</p> Source code in <code>src/unitorch/models/bert/processing.py</code> <pre><code>def pretrain(\n    self,\n    text: str,\n    text_pair: str,\n    nsp_label: int,\n    max_seq_length: Optional[int] = None,\n    masked_lm_prob: Optional[float] = None,\n    do_whole_word_mask: Optional[bool] = None,\n    max_predictions_per_seq: Optional[int] = None,\n):\n\"\"\"\n    The Bert pretrain processor on the given text and text pair.\n\n    Args:\n        text (str): The input text.\n        text_pair (str): The input text pair.\n        nsp_label (int): The next sentence prediction label.\n        max_seq_length (Optional[int], optional): The maximum sequence length. Defaults to None.\n        masked_lm_prob (Optional[float], optional): The probability of masking a token for pretraining. Defaults to None.\n        do_whole_word_mask (Optional[bool], optional): Whether to perform whole word masking. Defaults to None.\n        max_predictions_per_seq (Optional[int], optional): The maximum number of masked tokens per sequence for pretraining. Defaults to None.\n\n    Returns:\n        GenericOutputs: pretrain processing outputs.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n\n    masked_lm_prob = pop_value(\n        masked_lm_prob,\n        self.masked_lm_prob,\n    )\n\n    do_whole_word_mask = pop_value(\n        do_whole_word_mask,\n        self.do_whole_word_mask,\n    )\n\n    max_predictions_per_seq = pop_value(\n        max_predictions_per_seq,\n        self.max_predictions_per_seq,\n    )\n\n    _tokens = self.tokenizer.tokenize(str(text))\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))\n    truncate_sequence_pair(_tokens, tokens_pair, max_seq_length - 3)\n    tokens = (\n        [self.cls_token]\n        + _tokens\n        + [self.sep_token]\n        + tokens_pair\n        + [self.sep_token]\n    )\n\n    covered_indexes = get_random_mask_indexes(\n        tokens,\n        masked_lm_prob,\n        do_whole_word_mask,\n        max_predictions_per_seq,\n        special_tokens=[self.cls_token, self.sep_token],\n    )\n    label = [\n        tokens[pos] if pos in covered_indexes else self.pad_token\n        for pos in range(max_seq_length)\n    ]\n    label_mask = [\n        1 if pos in covered_indexes else 0 for pos in range(max_seq_length)\n    ]\n    label = self.tokenizer.convert_tokens_to_ids(label)\n\n    for index in covered_indexes:\n        mask_token = None\n        if random.random() &lt; 0.8:\n            mask_token = self.mask_token\n        else:\n            mask_token = (\n                tokens[index]\n                if random.random() &lt; 0.5\n                else get_random_word(self.vocab_words)\n            )\n        tokens[index] = mask_token\n\n    input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n    token_type_ids = [0] + [0] * len(_tokens) + [0] + [1] * len(tokens_pair) + [1]\n    attention_mask = [1] * len(input_ids)\n\n    padding = [0] * (max_seq_length - len(input_ids))\n    input_ids += len(padding) * [self.pad_token_id]\n    attention_mask += padding\n    token_type_ids += len(padding) * [1]\n\n    assert len(input_ids) == max_seq_length\n    assert len(attention_mask) == max_seq_length\n    assert len(token_type_ids) == max_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        token_type_ids=torch.tensor(token_type_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n        position_ids=torch.tensor(list(range(max_seq_length)), dtype=torch.long),\n        nsp_label=torch.tensor(int(nsp_label), dtype=torch.long),\n        mlm_label=torch.tensor(label, dtype=torch.long),\n        mlm_label_mask=torch.tensor(label_mask, dtype=torch.long),\n    )\n</code></pre>",
             "title": "pretrain"
         },
         {
             "location": "models/bert/#bertforclassification",
             "text": "<p>         Bases: <code>GenericModel</code></p> <p>Initializes the BertForClassification model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the configuration file.</p> required <code>num_classes</code> <code>Optional[int]</code> <p>The number of classes for classification. Defaults to 1.</p> <code>1</code> <code>gradient_checkpointing</code> <code>Optional[bool]</code> <p>Whether to use gradient checkpointing. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/bert/modeling.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    num_classes: Optional[int] = 1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes the BertForClassification model.\n\n    Args:\n        config_path (str): The path to the configuration file.\n        num_classes (Optional[int], optional): The number of classes for classification. Defaults to 1.\n        gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.config = BertConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.bert = BertModel(self.config)\n    self.dropout = nn.Dropout(self.config.hidden_dropout_prob)\n    self.classifier = nn.Linear(self.config.hidden_size, num_classes)\n    self.init_weights()\n</code></pre>",
             "title": "BertForClassification"
         },
@@ -2137,20 +2137,20 @@
         {
             "location": "models/diffusers/#bartprocessor",
             "text": "<p>         Bases: <code>HfTextGenerationProcessor</code></p> <p>Processor for BART model. Inherits from HfTextGenerationProcessor.</p> <p>Initializes the BartProcessor.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_path</code> <code>str</code> <p>Path to the vocabulary file.</p> required <code>merge_path</code> <code>str</code> <p>Path to the BPE merge file.</p> required <code>special_input_ids</code> <code>Optional[Dict]</code> <p>Optional dictionary of special input IDs.</p> <code>dict()</code> <code>max_seq_length</code> <code>Optional[int]</code> <p>Maximum sequence length.</p> <code>128</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>Maximum generation sequence length.</p> <code>48</code> Source code in <code>src/unitorch/models/bart/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_path: str,\n    merge_path: str,\n    special_input_ids: Optional[Dict] = dict(),\n    max_seq_length: Optional[int] = 128,\n    max_gen_seq_length: Optional[int] = 48,\n):\n\"\"\"\n    Initializes the BartProcessor.\n\n    Args:\n        vocab_path (str): Path to the vocabulary file.\n        merge_path (str): Path to the BPE merge file.\n        special_input_ids (Optional[Dict]): Optional dictionary of special input IDs.\n        max_seq_length (Optional[int]): Maximum sequence length.\n        max_gen_seq_length (Optional[int]): Maximum generation sequence length.\n    \"\"\"\n    tokenizer = get_bart_tokenizer(\n        vocab_path,\n        merge_path,\n        special_input_ids=special_input_ids,\n    )\n    super().__init__(\n        tokenizer=tokenizer,\n        max_seq_length=max_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n    )\n</code></pre>",
             "title": "BartProcessor"
         },
         {
             "location": "models/diffusers/#bartforgeneration",
-            "text": "<p>         Bases: <code>GenericModel</code></p> <p>BART model for text generation.</p> <p>Initializes a BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>Path to the BART model configuration file.</p> required <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes a BartForGeneration model.\n\n    Args:\n        config_path (str): Path to the BART model configuration file.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.config = BartConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.model = BartForConditionalGeneration(self.config)\n    self.init_weights()\n</code></pre>",
+            "text": "<p>         Bases: <code>GenericModel</code></p> <p>BART model for text generation.</p> <p>Initializes a BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>Path to the BART model configuration file.</p> required <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes a BartForGeneration model.\n\n    Args:\n        config_path (str): Path to the BART model configuration file.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.config = BartConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.config.forced_bos_token_id = None\n    self.model = BartForConditionalGeneration(self.config)\n    self.init_weights()\n</code></pre>",
             "title": "BartForGeneration"
         },
         {
             "location": "models/diffusers/#unitorch.models.bart.modeling.BartForGeneration.forward",
-            "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which tokens should be attended to.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which decoder tokens should be attended to.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Output logits of the model.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor indicating which tokens should be attended to.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor indicating which decoder tokens should be attended to.\n\n    Returns:\n        (torch.Tensor): Output logits of the model.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
+            "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which tokens should be attended to.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which decoder tokens should be attended to.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Output logits of the model.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor indicating which tokens should be attended to.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor indicating which decoder tokens should be attended to.\n\n    Returns:\n        (torch.Tensor): Output logits of the model.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    print(\"model :\", logits[0, 0, 0].item(), logits[0, 0, 41552].item())\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/diffusers/#unitorch.models.bart.modeling.BartForGeneration.generate",
             "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates text using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling during generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates text using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling during generation. Defaults to False.\n        temperature (float, optional): Temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): Value for top-k sampling. Defaults to 50.\n        top_p (float, optional): Value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
             "title": "generate"
         },
@@ -2492,15 +2492,15 @@
         {
             "location": "models/visualbert/",
             "text": "",
             "title": "unitorch.models.visualbert"
         },
         {
             "location": "models/visualbert/#visualbertprocessor",
-            "text": "<p>         Bases: <code>BertProcessor</code></p> <p>Processor for VisualBERT-based models.</p> <p>Initializes the VisualBertProcessor.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_path</code> <code>str</code> <p>Path to the vocabulary file.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>Maximum sequence length. Defaults to 128.</p> <code>128</code> <code>special_input_ids</code> <code>Optional[Dict]</code> <p>Special input IDs. Defaults to an empty dictionary.</p> <code>dict()</code> <code>do_lower_case</code> <code>Optional[bool]</code> <p>Whether to convert text to lowercase. Defaults to True.</p> <code>True</code> <code>do_basic_tokenize</code> <code>Optional[bool]</code> <p>Whether to perform basic tokenization. Defaults to True.</p> <code>True</code> <code>do_whole_word_mask</code> <code>Optional[bool]</code> <p>Whether to use whole word masking. Defaults to True.</p> <code>True</code> <code>masked_lm_prob</code> <code>Optional[float]</code> <p>Probability for masked LM. Defaults to 0.15.</p> <code>0.15</code> <code>max_predictions_per_seq</code> <code>Optional[int]</code> <p>Maximum number of masked LM predictions per sequence. Defaults to 20.</p> <code>20</code> Source code in <code>src/unitorch/models/visualbert/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_path,\n    max_seq_length: Optional[int] = 128,\n    special_input_ids: Optional[Dict] = dict(),\n    do_lower_case: Optional[bool] = True,\n    do_basic_tokenize: Optional[bool] = True,\n    do_whole_word_mask: Optional[bool] = True,\n    masked_lm_prob: Optional[float] = 0.15,\n    max_predictions_per_seq: Optional[int] = 20,\n):\n\"\"\"\n    Initializes the VisualBertProcessor.\n\n    Args:\n        vocab_path (str): Path to the vocabulary file.\n        max_seq_length (Optional[int]): Maximum sequence length. Defaults to 128.\n        special_input_ids (Optional[Dict]): Special input IDs. Defaults to an empty dictionary.\n        do_lower_case (Optional[bool]): Whether to convert text to lowercase. Defaults to True.\n        do_basic_tokenize (Optional[bool]): Whether to perform basic tokenization. Defaults to True.\n        do_whole_word_mask (Optional[bool]): Whether to use whole word masking. Defaults to True.\n        masked_lm_prob (Optional[float]): Probability for masked LM. Defaults to 0.15.\n        max_predictions_per_seq (Optional[int]): Maximum number of masked LM predictions per sequence. Defaults to 20.\n    \"\"\"\n    tokenizer = get_bert_tokenizer(\n        vocab_path,\n        do_lower_case=do_lower_case,\n        do_basic_tokenize=do_basic_tokenize,\n        special_input_ids=special_input_ids,\n    )\n    super().__init__(\n        tokenizer=tokenizer,\n        max_seq_length=max_seq_length,\n        do_lower_case=do_lower_case,\n        do_basic_tokenize=do_basic_tokenize,\n        do_whole_word_mask=do_whole_word_mask,\n        masked_lm_prob=masked_lm_prob,\n        max_predictions_per_seq=max_predictions_per_seq,\n    )\n</code></pre>",
+            "text": "<p>         Bases: <code>BertProcessor</code></p> <p>Processor for VisualBERT-based models.</p> <p>Initializes the VisualBertProcessor.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_path</code> <code>str</code> <p>Path to the vocabulary file.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>Maximum sequence length. Defaults to 128.</p> <code>128</code> <code>special_input_ids</code> <code>Optional[Dict]</code> <p>Special input IDs. Defaults to an empty dictionary.</p> <code>dict()</code> <code>do_lower_case</code> <code>Optional[bool]</code> <p>Whether to convert text to lowercase. Defaults to True.</p> <code>True</code> <code>do_basic_tokenize</code> <code>Optional[bool]</code> <p>Whether to perform basic tokenization. Defaults to True.</p> <code>True</code> <code>do_whole_word_mask</code> <code>Optional[bool]</code> <p>Whether to use whole word masking. Defaults to True.</p> <code>True</code> <code>masked_lm_prob</code> <code>Optional[float]</code> <p>Probability for masked LM. Defaults to 0.15.</p> <code>0.15</code> <code>max_predictions_per_seq</code> <code>Optional[int]</code> <p>Maximum number of masked LM predictions per sequence. Defaults to 20.</p> <code>20</code> Source code in <code>src/unitorch/models/visualbert/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_path,\n    max_seq_length: Optional[int] = 128,\n    special_input_ids: Optional[Dict] = dict(),\n    do_lower_case: Optional[bool] = True,\n    do_basic_tokenize: Optional[bool] = True,\n    do_whole_word_mask: Optional[bool] = True,\n    masked_lm_prob: Optional[float] = 0.15,\n    max_predictions_per_seq: Optional[int] = 20,\n):\n\"\"\"\n    Initializes the VisualBertProcessor.\n\n    Args:\n        vocab_path (str): Path to the vocabulary file.\n        max_seq_length (Optional[int]): Maximum sequence length. Defaults to 128.\n        special_input_ids (Optional[Dict]): Special input IDs. Defaults to an empty dictionary.\n        do_lower_case (Optional[bool]): Whether to convert text to lowercase. Defaults to True.\n        do_basic_tokenize (Optional[bool]): Whether to perform basic tokenization. Defaults to True.\n        do_whole_word_mask (Optional[bool]): Whether to use whole word masking. Defaults to True.\n        masked_lm_prob (Optional[float]): Probability for masked LM. Defaults to 0.15.\n        max_predictions_per_seq (Optional[int]): Maximum number of masked LM predictions per sequence. Defaults to 20.\n    \"\"\"\n    super().__init__(\n        vocab_path=vocab_path,\n        max_seq_length=max_seq_length,\n        do_lower_case=do_lower_case,\n        do_basic_tokenize=do_basic_tokenize,\n        do_whole_word_mask=do_whole_word_mask,\n        masked_lm_prob=masked_lm_prob,\n        max_predictions_per_seq=max_predictions_per_seq,\n    )\n</code></pre>",
             "title": "VisualBertProcessor"
         },
         {
             "location": "models/visualbert/#visualbertforclassification",
             "text": "<p>         Bases: <code>GenericModel</code></p> <p>VisualBERT model for classification tasks.</p> <p>Initialize the VisualBertForClassification model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the VisualBERT model config file.</p> required <code>num_classes</code> <code>int</code> <p>The number of output classes for classification. Defaults to 1.</p> <code>1</code> <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/visualbert/modeling.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    num_classes: Optional[int] = 1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initialize the VisualBertForClassification model.\n\n    Args:\n        config_path (str): The path to the VisualBERT model config file.\n        num_classes (int, optional): The number of output classes for classification. Defaults to 1.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.config = VisualBertConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.visual_bert = VisualBertModel(self.config)\n    self.dropout = nn.Dropout(self.config.hidden_dropout_prob)\n    self.classifier = nn.Linear(self.config.hidden_size, num_classes)\n    self.init_weights()\n</code></pre>",
             "title": "VisualBertForClassification"
         },
```

### Comparing `unitorch-0.0.0.3/examples/README.md` & `unitorch-0.0.0.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/caption/blip.ini` & `unitorch-0.0.0.4/examples/configs/caption/blip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/bert.ini` & `unitorch-0.0.0.4/examples/configs/classification/bert.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/clip.ini` & `unitorch-0.0.0.4/examples/configs/classification/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/image_clip.ini` & `unitorch-0.0.0.4/examples/configs/classification/image_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/lora/bloom.ini` & `unitorch-0.0.0.4/examples/configs/classification/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/lora/bloom_ds.ini` & `unitorch-0.0.0.4/examples/configs/classification/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/lora/llama.ini` & `unitorch-0.0.0.4/examples/configs/classification/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/lora/llama_ds.ini` & `unitorch-0.0.0.4/examples/configs/classification/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/roberta.ini` & `unitorch-0.0.0.4/examples/configs/classification/roberta.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/swin.ini` & `unitorch-0.0.0.4/examples/configs/classification/swin.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/classification/text_clip.ini` & `unitorch-0.0.0.4/examples/configs/classification/text_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/bart.ini` & `unitorch-0.0.0.4/examples/configs/generation/bart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/bloom.ini` & `unitorch-0.0.0.4/examples/configs/generation/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/chatglm.ini` & `unitorch-0.0.0.4/examples/configs/generation/chatglm.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/llama.ini` & `unitorch-0.0.0.4/examples/configs/generation/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/lora/bloom.ini` & `unitorch-0.0.0.4/examples/configs/generation/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/lora/bloom_ds.ini` & `unitorch-0.0.0.4/examples/configs/generation/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/lora/llama.ini` & `unitorch-0.0.0.4/examples/configs/generation/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/lora/llama_ds.ini` & `unitorch-0.0.0.4/examples/configs/generation/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/mbart.ini` & `unitorch-0.0.0.4/examples/configs/generation/mbart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/mt5.ini` & `unitorch-0.0.0.4/examples/configs/generation/mt5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/pegasus.ini` & `unitorch-0.0.0.4/examples/configs/generation/pegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/t5.ini` & `unitorch-0.0.0.4/examples/configs/generation/t5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/xpegasus.ini` & `unitorch-0.0.0.4/examples/configs/generation/xpegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/generation/xprophetnet.ini` & `unitorch-0.0.0.4/examples/configs/generation/xprophetnet.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/examples/configs/pretrain/clip.ini` & `unitorch-0.0.0.4/examples/configs/pretrain/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/pyproject.toml` & `unitorch-0.0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,17 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["version", "dependencies"]
 
 [project.optional-dependencies]
 deepspeed = ["deepspeed==0.9.0", "mpi4py==3.1.4"]
 diffusers = ["diffusers==0.16.1"]
+accelerate = ["accelerate==0.20.3"]
 chatglm = ["protobuf==3.20.0", "icetk==0.0.4", "cpm_kernels==1.0.11"]
-docs = ["mkdocstrings[python]>=0.18", "mkdocs-material", "markdown-exec", "mkdocs-gen-files", "mkdocs-coverage"]
-all = ["unitorch[deepspeed,diffusers,chatglm,docs]"]
+all = ["unitorch[deepspeed,diffusers,accelerate,chatglm]"]
 
 [project.scripts]
 unitorch-train = "unitorch.cli.console.train:cli_main"
 unitorch-eval = "unitorch.cli.console.eval:cli_main"
 unitorch-infer = "unitorch.cli.console.infer:cli_main"
 unitorch-script= "unitorch.cli.console.script:cli_main"
 unitorch-service = "unitorch.cli.console.service:cli_main"
```

### Comparing `unitorch-0.0.0.3/setup.py` & `unitorch-0.0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/__init__.py` & `unitorch-0.0.0.4/src/unitorch/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_cache_home():
     return UNITORCH_CACHE
 
 
 ### version
-VERSION = "0.0.0.3"
+VERSION = "0.0.0.4"
 
 ### is offline mode
 UNITORCH_OFFLINE = os.environ.get("UNITORCH_OFFLINE", "0").upper()
 
 
 def is_offline_mode():
     return UNITORCH_OFFLINE in ENV_VARS_TRUE_VALUES
@@ -84,14 +84,16 @@
         torch.cuda.manual_seed_all(seed)
 
 
 # useful functions
 from unitorch.utils import cached_path as hf_cached_path
 from unitorch.utils import (
     is_deepspeed_available,
+    is_accelerate_available,
+    is_megatron_available,
     is_diffusers_available,
     is_torch_available,
     is_torch2_available,
 )
 
 # imports from other files
 import unitorch.datasets
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/console/eval.py` & `unitorch-0.0.0.4/src/unitorch/cli/console/eval.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/console/infer.py` & `unitorch-0.0.0.4/src/unitorch/cli/console/infer.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/console/script.py` & `unitorch-0.0.0.4/src/unitorch/cli/console/script.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/console/service.py` & `unitorch-0.0.0.4/src/unitorch/cli/console/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,18 @@
     main_service_cls = registered_service.get(service_name)
     if main_service_cls is None:
         raise ValueError(f"service {service_name} not found")
 
     if gpu_mode:
         with ActiveGPUJob() as _:
             service_inst = main_service_cls["obj"](config)
-    else:
+    elif service_action in ["start", "restart"]:
         service_inst = main_service_cls["obj"](config)
+    else:
+        service_inst = None
 
     hexsha = config.hexsha(6)
     service_name = service_name + f"@{hexsha}"
     if service_action == "start":
         start(service_name, service_inst, daemon_mode)
     elif service_action == "stop":
         stop(service_name, service_inst)
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/console/train.py` & `unitorch-0.0.0.4/src/unitorch/cli/console/train.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/core.py` & `unitorch-0.0.0.4/src/unitorch/cli/core.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/datasets/hf.py` & `unitorch-0.0.0.4/src/unitorch/cli/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/decorators.py` & `unitorch-0.0.0.4/src/unitorch/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/loss/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/loss/ranking.py` & `unitorch-0.0.0.4/src/unitorch/cli/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 import unitorch.cli.models.image_utils
 import unitorch.cli.models.random_utils
 import unitorch.cli.models.label_utils
 import unitorch.cli.models.processing_utils
 
 if is_diffusers_available():
     from unitorch.cli.models.diffusion_utils import DiffusionOutputs, DiffusionTargets
+    from unitorch.cli.models.diffusion_utils import diffusion_model_decorator
     import unitorch.cli.models.diffusers
 
 # import model classes & process functions
 import unitorch.cli.models.bart
 import unitorch.cli.models.bert
 import unitorch.cli.models.beit
 import unitorch.cli.models.blip
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bart/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bart/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bart/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/beit/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/beit/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/beit/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bert/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bert/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bert/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/blip/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/blip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/blip/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/blip/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bloom/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bloom/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/bloom/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/classification_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/classification_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/clip/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/clip/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/clip/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling_v2.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing_v2.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/detection_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/detection_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,47 +15,39 @@
     "vae": {
         "config": f"https://huggingface.co/{name}/resolve/main/vae/config.json",
         "weight": f"https://huggingface.co/{name}/resolve/main/vae/diffusion_pytorch_model.bin",
     },
     "scheduler": f"https://huggingface.co/{name}/resolve/main/scheduler/scheduler_config.json",
 }
 
-__hf_hub_stable_controlnet_dict__ = lambda name: {
+__hf_hub_controlnet_dict__ = lambda name: {
     **__hf_hub_stable_dict__("runwayml/stable-diffusion-v1-5"),
     **{
         "controlnet": {
             "config": f"https://huggingface.co/{name}/resolve/main/config.json",
             "weight": f"https://huggingface.co/{name}/resolve/main/diffusion_pytorch_model.bin",
         }
     },
 }
 
 pretrained_diffusers_infos = {
     "ddpm-ema-pokemon-64": {
         "config": "https://huggingface.co/anton-l/ddpm-ema-pokemon-64/resolve/main/unet/config.json",
         "weight": "https://huggingface.co/anton-l/ddpm-ema-pokemon-64/resolve/main/unet/diffusion_pytorch_model.bin",
     },
-    "stable-diffusion-v1.5": __hf_hub_stable_dict__("runwayml/stable-diffusion-v1-5"),
-    "stable-diffusion-v2": __hf_hub_stable_dict__("stabilityai/stable-diffusion-2"),
-    "stable-diffusion-v2.1": __hf_hub_stable_dict__("stabilityai/stable-diffusion-2-1"),
-    "stable-diffusion-v2-inpainting": __hf_hub_stable_dict__(
-        "stabilityai/stable-diffusion-2-inpainting"
-    ),
-    "stable-diffusion-x4-upscaler": __hf_hub_stable_dict__(
+    "stable-v1.5": __hf_hub_stable_dict__("runwayml/stable-diffusion-v1-5"),
+    "stable-v2": __hf_hub_stable_dict__("stabilityai/stable-diffusion-2"),
+    "stable-v2.1": __hf_hub_stable_dict__("stabilityai/stable-diffusion-2-1"),
+    "stable-x4-upscaler": __hf_hub_stable_dict__(
         "stabilityai/stable-diffusion-x4-upscaler"
     ),
-    "stable-diffusion-controlnet-canny": __hf_hub_stable_controlnet_dict__(
-        "lllyasviel/sd-controlnet-canny"
-    ),
-    "stable-diffusion-controlnet-openpose": __hf_hub_stable_controlnet_dict__(
+    "controlnet-canny": __hf_hub_controlnet_dict__("lllyasviel/sd-controlnet-canny"),
+    "controlnet-openpose": __hf_hub_controlnet_dict__(
         "lllyasviel/sd-controlnet-openpose"
     ),
-    "stable-diffusion-controlnet-depth": __hf_hub_stable_controlnet_dict__(
-        "lllyasviel/sd-controlnet-depth"
-    ),
 }
 from unitorch import is_diffusers_available
 
 if is_diffusers_available():
     import unitorch.cli.models.diffusers.modeling_controlnet
     import unitorch.cli.models.diffusers.modeling_stable
     import unitorch.cli.models.diffusers.processing_controlnet
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/diffusion_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/diffusion_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 import os
 import torch
+import torch.nn as nn
 import hashlib
 from PIL import Image
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from diffusers.utils import numpy_to_pil
 from unitorch.cli import WriterMixin, WriterOutputs
 from unitorch.cli import (
@@ -50,11 +51,49 @@
     @register_process("core/postprocess/diffusion")
     def _diffusion(
         self,
         outputs: DiffusionOutputs,
     ):
         results = outputs.to_pandas()
         assert results.shape[0] == 0 or results.shape[0] == outputs.outputs.shape[0]
-        images = outputs.outputs.numpy().transpose(0, 2, 3, 1)
+        images = outputs.outputs.numpy()
         images = numpy_to_pil(images)
         results["diffusion"] = [self.save(image) for image in images]
         return WriterOutputs(results)
+
+
+def diffusion_model_decorator(cls):
+    class DiffusionModel(nn.Module):
+        def __init__(self, *args, **kwargs):
+            super().__init__()
+            if "__diffusion_model__" in kwargs:
+                self.model = kwargs.pop("__diffusion_model__")
+            else:
+                self.model = cls(*args, **kwargs)
+
+            __more_attrs__ = [
+                "load_state_dict",
+                "state_dict",
+                "save_checkpoint",
+                "from_checkpoint",
+                "from_pretrained",
+            ]
+            for __more_attr__ in __more_attrs__:
+                setattr(self, __more_attr__, getattr(self.model, __more_attr__))
+
+            self.model.register_forward_hook(self._hook)
+            self.__in_training__ = False
+
+        def _hook(self, module, inputs, outputs):
+            self.__in_training__ = True
+
+        def forward(self, *args, **kwargs):
+            if self.training or self.__in_training__:
+                return self.model(*args, **kwargs)
+            return self.model.generate(*args, **kwargs)
+
+        @classmethod
+        def from_core_configure(_cls, cfg, **kwargs):
+            model = cls.from_core_configure(cfg, **kwargs)
+            return _cls(__diffusion_model__=model)
+
+    return DiffusionModel
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/generation_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/image_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/label_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/label_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/llama/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/llama/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,38 @@
         "config": "https://huggingface.co/decapoda-research/llama-7b-hf/resolve/main/config.json",
         "vocab": "https://huggingface.co/decapoda-research/llama-7b-hf/resolve/main/tokenizer.model",
         "weight": [
             f"https://huggingface.co/decapoda-research/llama-7b-hf/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00033.bin"
             for i in range(1, 34)
         ],
     },
+    "llama-13b-hf": {
+        "config": "https://huggingface.co/decapoda-research/llama-13b-hf/resolve/main/config.json",
+        "vocab": "https://huggingface.co/decapoda-research/llama-13b-hf/resolve/main/tokenizer.model",
+        "weight": [
+            f"https://huggingface.co/decapoda-research/llama-13b-hf/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00041.bin"
+            for i in range(0, 42)
+        ],
+    },
     "llama-7b": {
         "config": "https://huggingface.co/huggyllama/llama-7b/resolve/main/config.json",
         "vocab": "https://huggingface.co/huggyllama/llama-7b/resolve/main/tokenizer.model",
         "weight": [
             f"https://huggingface.co/huggyllama/llama-7b/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00002.bin"
             for i in range(1, 3)
         ],
     },
+    "llama-13b": {
+        "config": "https://huggingface.co/huggyllama/llama-13b/resolve/main/config.json",
+        "vocab": "https://huggingface.co/huggyllama/llama-13b/resolve/main/tokenizer.model",
+        "weight": [
+            f"https://huggingface.co/huggyllama/llama-13b/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00003.bin"
+            for i in range(1, 4)
+        ],
+    },
 }
 
 import unitorch.cli.models.llama.modeling
 import unitorch.cli.models.llama.processing
 from unitorch.cli.models.llama.modeling import (
     LlamaForClassification,
     LlamaForPretrain,
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/llama/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/llama/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/mbart/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/mbart/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/mbart/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/modeling_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/mt5/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/mt5/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/mt5/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/peft/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_bloom.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_llama.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/processing_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/random_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/ranking_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/ranking_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/roberta/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/roberta/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/roberta/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/segmentation_utils.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/swin/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/swin/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/swin/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/swin/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/t5/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/t5/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/t5/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/vit/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/vit/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/vit/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         )
         if weight_path is not None:
             weight_path = cached_path(weight_path)
             inst.from_pretrained(weight_path)
 
         return inst
 
-    # @autocast()
+    #@autocast()
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: torch.Tensor,
         decoder_input_ids: torch.Tensor,
         decoder_attention_mask: torch.Tensor,
     ):
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/modeling.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/processing.py` & `unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/optim/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/optim/lion.py` & `unitorch-0.0.0.4/src/unitorch/cli/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/scheduler/warmup.py` & `unitorch-0.0.0.4/src/unitorch/cli/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/score/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/score/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,15 @@
         if targets.dim() == 2 and targets.size(-1) == 1:
             targets = targets[:, 0]
 
         assert outputs.dim() == 1 and targets.dim() == 1
 
         return matthews_corrcoef(targets, outputs)
 
+
 @register_score("core/score/pearsonr_corr")
 class PearsonrCorrScore(Score):
     def __init__(
         self,
     ):
         super().__init__()
 
@@ -326,14 +327,15 @@
         outputs = outputs.view(-1)
         targets = targets.view(-1)
 
         assert outputs.numel() == targets.numel()
 
         return pearsonr(targets, outputs)
 
+
 @register_score("core/score/bleu")
 class BleuScore(Score):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/service.py` & `unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/tasks/deepspeed.py` & `unitorch-0.0.0.4/src/unitorch/cli/tasks/deepspeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         monitor_fns: Optional[Union[str, List[str]]] = None,
         from_ckpt_dir: Optional[str] = "./from_ckpt",
         to_ckpt_dir: Optional[str] = "./to_ckpt",
         train_batch_size: Optional[int] = 128,
         dev_batch_size: Optional[int] = 128,
         pin_memory: Optional[bool] = True,
         num_workers: Optional[int] = 4,
-        save_optimizer: Optional[bool] = True,
-        save_scheduler: Optional[bool] = True,
+        save_optimizer: Optional[bool] = False,
+        save_scheduler: Optional[bool] = False,
         log_freq: Optional[int] = 100,
         ckpt_freq: Optional[int] = 10000,
         grad_acc_step: Optional[int] = 1,
         max_grad_norm: Optional[float] = 1.0,
         learning_rate: Optional[float] = None,
         max_warmup_learning_rate: Optional[float] = None,
         num_warmup_steps: Optional[int] = None,
@@ -187,16 +187,16 @@
             monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.
             from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
             to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to "./to_ckpt".
             train_batch_size (optional): The batch size for training. Defaults to 128.
             dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
             pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
             num_workers (optional): The number of worker processes for data loading. Defaults to 4.
-            save_optimizer (optional): Whether to save the optimizer state. Defaults to True.
-            save_scheduler (optional): Whether to save the scheduler state. Defaults to True.
+            save_optimizer (optional): Whether to save the optimizer state. Defaults to False.
+            save_scheduler (optional): Whether to save the scheduler state. Defaults to False.
             log_freq (optional): The frequency of logging. Defaults to 100.
             ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.
             grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.
             max_grad_norm (optional): The maximum gradient norm. Defaults to 1.0.
             learning_rate (optional): The learning rate for the optimizer. Defaults to None.
             max_warmup_learning_rate (optional): The maximum learning rate during warmup. Defaults to None.
             num_warmup_steps (optional): The number of warmup steps. Defaults to None.
@@ -431,15 +431,15 @@
                         self.model.module if self.n_gpu > 1 else self.model,
                         to_ckpt_dir,
                         iter_dev,
                         score_fn,
                         monitor_fns,
                         optim=optim if save_optimizer else None,
                         scheduler=scheduler if save_scheduler else None,
-                        ema_model=self.ema_ema_model if use_ema else None,
+                        ema_model=self.ema_model if use_ema else None,
                         best_score=self.best_score,
                         info_path=info_path,
                         local_rank=self.local_rank,
                         global_epoch=e,
                         global_step=step + 1,
                     )
 
@@ -469,15 +469,15 @@
                 self.model.module if self.n_gpu > 1 else self.model,
                 to_ckpt_dir,
                 iter_dev,
                 score_fn,
                 monitor_fns,
                 optim=optim if save_optimizer else None,
                 scheduler=scheduler if save_scheduler else None,
-                ema_model=self.ema_ema_model if use_ema else None,
+                ema_model=self.ema_model if use_ema else None,
                 best_score=self.best_score,
                 info_path=info_path,
                 local_rank=self.local_rank,
                 global_epoch=e,
                 global_step=0,
             )
 
@@ -687,15 +687,15 @@
             for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):
                 if torch.cuda.is_available():
                     inputs = inputs.cuda()
                 outputs = self.model(**inputs.dict())
                 outputs = outputs.cpu()
                 if output_header is not None:
                     _infos = {k: _infos[k] for k in output_header if k in _infos}
-                    outputs.set_base_dataframe(pd.DataFrame(_infos))
+                    outputs.from_pandas(pd.DataFrame(_infos))
                 data_queue.put((step, outputs))
 
         data_queue.put((-1, GENERATE_FINISHED))
         for p in postprocess_list:
             p.join()
 
         msg_queue.put((-1, GENERATE_FINISHED))
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/tasks/supervised.py` & `unitorch-0.0.0.4/src/unitorch/cli/tasks/supervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
                 self.config,
                 registered_optim,
                 params=self.model.parameters(),
             )
 
         if os.path.exists(from_ckpt_dir):
             self.model.from_checkpoint(from_ckpt_dir)
-            optim.from_checkpoint(from_ckpt_dir)
+            optim.from_checkpoint(from_ckpt_dir, weight_name="pytorch_optim.bin",)
 
         if os.path.exists(to_ckpt_dir):
             self.model.from_checkpoint(
                 to_ckpt_dir,
                 weight_name="pytorch_model_latest.bin",
             )
             optim.from_checkpoint(
@@ -602,15 +602,15 @@
                         self.model.module if self.n_gpu > 1 else self.model,
                         to_ckpt_dir,
                         iter_dev,
                         score_fn,
                         monitor_fns,
                         optim=optim if save_optimizer else None,
                         scheduler=scheduler if save_scheduler else None,
-                        ema_model=self.ema_ema_model if use_ema else None,
+                        ema_model=self.ema_model if use_ema else None,
                         best_score=self.best_score,
                         info_path=info_path,
                         local_rank=self.local_rank,
                         global_epoch=e,
                         global_step=step + 1,
                     )
 
@@ -641,15 +641,15 @@
                 self.model.module if self.n_gpu > 1 else self.model,
                 to_ckpt_dir,
                 iter_dev,
                 score_fn,
                 monitor_fns,
                 optim=optim if save_optimizer else None,
                 scheduler=scheduler if save_scheduler else None,
-                ema_model=self.ema_ema_model if use_ema else None,
+                ema_model=self.ema_model if use_ema else None,
                 best_score=self.best_score,
                 info_path=info_path,
                 local_rank=self.local_rank,
                 global_epoch=e,
                 global_step=0,
             )
 
@@ -854,15 +854,15 @@
             for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):
                 if torch.cuda.is_available():
                     inputs = inputs.cuda()
                 outputs = self.model(**inputs.dict())
                 outputs = outputs.cpu()
                 if output_header is not None:
                     _infos = {k: _infos[k] for k in output_header if k in _infos}
-                    outputs.set_base_dataframe(pd.DataFrame(_infos))
+                    outputs.from_pandas(pd.DataFrame(_infos))
                 data_queue.put((step, outputs))
 
         data_queue.put((-1, GENERATE_FINISHED))
         for p in postprocess_list:
             p.join()
 
         msg_queue.put((-1, GENERATE_FINISHED))
```

### Comparing `unitorch-0.0.0.3/src/unitorch/cli/writer/__init__.py` & `unitorch-0.0.0.4/src/unitorch/cli/writer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import pyarrow.parquet as pq
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from unitorch.utils.io import GenericWriter
 from unitorch.cli import add_default_section_for_init, register_writer
 
 
 class WriterMixin:
-    def set_base_dataframe(self, df: pd.DataFrame):
-        self.__base_dataframe__ = df
+    def from_pandas(self, df: pd.DataFrame):
+        self.__pandas_dataframe__ = df
 
     def to_pandas(self):
-        if hasattr(self, "__base_dataframe__"):
-            return pd.DataFrame(self.__base_dataframe__)
+        if hasattr(self, "__pandas_dataframe__"):
+            return pd.DataFrame(self.__pandas_dataframe__)
         return pd.DataFrame()
 
 
 class WriterOutputs:
     def __init__(
         self,
         process_outputs: pd.DataFrame,
```

### Comparing `unitorch-0.0.0.3/src/unitorch/datasets/hf.py` & `unitorch-0.0.0.4/src/unitorch/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/loss/__init__.py` & `unitorch-0.0.0.4/src/unitorch/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/loss/prophetnet.py` & `unitorch-0.0.0.4/src/unitorch/loss/prophetnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/loss/ranking.py` & `unitorch-0.0.0.4/src/unitorch/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/__init__.py` & `unitorch-0.0.0.4/src/unitorch/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,27 @@
 
         Returns:
             None
         """
         assert weight_path or state_dict, "weight_path or state_dict must be set"
 
         # Load state_dict(s) based on the provided weight_path or state_dict
+        state_dicts = []
         if weight_path:
             if isinstance(weight_path, str):
                 weight_path = [weight_path]
             for path in weight_path:
                 logging.debug(f"Loading weights from {path}")
-            state_dicts = [
+            state_dicts += [
                 torch.load(hf_cached_path(path), map_location="cpu")
                 for path in weight_path
             ]
-        else:
-            state_dicts = state_dict if isinstance(state_dict, list) else [state_dict]
+        
+        if state_dict:
+            state_dicts += state_dict if isinstance(state_dict, list) else [state_dict]
 
         self_state_dict = self.state_dict()  # Get the current state_dict of the model
         load_keys = []  # Keep track of the keys loaded from the state_dict(s)
         non_load_keys = []  # Keep track of the keys not loaded from the state_dict(s)
 
         if isinstance(self.replace_keys_in_state_dict, dict):
             replace_keys = {**self.replace_keys_in_state_dict, **replace_keys}
```

### Comparing `unitorch-0.0.0.3/src/unitorch/models/bart/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/bart/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
 
 class BartForGeneration(GenericModel):
     """
     BART model for text generation.
     """
 
-    prefix_keys_in_state_dict = {"^(?!model\.model\.).*": "model.model."}
+    prefix_keys_in_state_dict = {"^(?!model\.model\.|model\.).*": "model.model."}
 
     def __init__(
         self,
         config_path: str,
         gradient_checkpointing: Optional[bool] = False,
     ):
         """
@@ -193,14 +193,15 @@
         Args:
             config_path (str): Path to the BART model configuration file.
             gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.
         """
         super().__init__()
         self.config = BartConfig.from_json_file(config_path)
         self.config.gradient_checkpointing = gradient_checkpointing
+        self.config.forced_bos_token_id = None
         self.model = BartForConditionalGeneration(self.config)
         self.init_weights()
 
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: torch.Tensor,
@@ -223,14 +224,15 @@
             input_ids=input_ids,
             attention_mask=attention_mask,
             decoder_input_ids=decoder_input_ids,
             decoder_attention_mask=decoder_attention_mask,
             return_dict=True,
         )
         logits = outputs.logits
+        print("model :", logits[0, 0, 0].item(), logits[0, 0, 41552].item())
         return logits
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
```

### Comparing `unitorch-0.0.0.3/src/unitorch/models/bart/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/beit/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/beit/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/bert/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/bert/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/blip/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/blip/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/bloom/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/bloom/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/chatglm/configuration_chatglm.py` & `unitorch-0.0.0.4/src/unitorch/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling_chatglm.py` & `unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/chatglm/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/chatglm/quantization.py` & `unitorch-0.0.0.4/src/unitorch/models/chatglm/quantization.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/chatglm/tokenization_chatglm.py` & `unitorch-0.0.0.4/src/unitorch/models/chatglm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/clip/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/clip/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/deberta/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/deberta/modeling_v2.py` & `unitorch-0.0.0.4/src/unitorch/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/deberta/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/deberta/processing_v2.py` & `unitorch-0.0.0.4/src/unitorch/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/llama/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/llama/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/mbart/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/mbart/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/modeling_ema.py` & `unitorch-0.0.0.4/src/unitorch/models/modeling_ema.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/mt5/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/mt5/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/peft/__init__.py` & `unitorch-0.0.0.4/src/unitorch/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_adalora.py` & `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_adalora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_lora.py` & `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_lora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_adalora.py` & `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_adalora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_lora.py` & `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_lora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/pegasus/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/pegasus/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/processing_utils.py` & `unitorch-0.0.0.4/src/unitorch/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/prophetnet/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/prophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/prophetnet/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/prophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/roberta/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/roberta/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/swin/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/swin/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/t5/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/t5/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/visualbert/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/visualbert/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/vit/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/vit/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/xpegasus/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/xpegasus/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 class XPegasusForGeneration(GenericModel):
     """
     XPegasus model for text generation tasks.
     """
 
     prefix_keys_in_state_dict = {
-        "^(?!model\.model\.)model\.": "model.",
+        "^(?!model\.model\.|model\.lm_head\.)model\.": "model.",
         "^lm_head.": "model.",
     }
 
     def __init__(
         self,
         config_path: str,
         gradient_checkpointing: Optional[bool] = False,
```

### Comparing `unitorch-0.0.0.3/src/unitorch/models/xpegasus/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/xprophetnet/modeling.py` & `unitorch-0.0.0.4/src/unitorch/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/models/xprophetnet/processing.py` & `unitorch-0.0.0.4/src/unitorch/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/modules/classifier.py` & `unitorch-0.0.0.4/src/unitorch/modules/classifier.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/modules/replace/beam_search_v2.py` & `unitorch-0.0.0.4/src/unitorch/modules/replace/beam_search_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/modules/replace/datasets_v2.py` & `unitorch-0.0.0.4/src/unitorch/modules/replace/datasets_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/modules/replace/hf_hub_v2.py` & `unitorch-0.0.0.4/src/unitorch/modules/replace/hf_hub_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/modules/timm.py` & `unitorch-0.0.0.4/src/unitorch/modules/timm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/ops/dyhead.py` & `unitorch-0.0.0.4/src/unitorch/ops/dyhead.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/ops/ngram_repeat_block.py` & `unitorch-0.0.0.4/src/unitorch/ops/ngram_repeat_block.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/optim/lion.py` & `unitorch-0.0.0.4/src/unitorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/scheduler/warmup.py` & `unitorch-0.0.0.4/src/unitorch/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/score/__init__.py` & `unitorch-0.0.0.4/src/unitorch/score/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         }
     elif isinstance(inputs, frozenset):
         return frozenset(
             remove_strings_ignore_tokens(element, ignore_tokens) for element in inputs
         )
     else:
         return inputs
-    
+
 
 pearsonr = lambda y_true, y_pred: np.corrcoef(y_true, y_pred)[0, 1]
 
 
 from unitorch.score.bleu import bleu_score
 from unitorch.score.rouge import rouge1_score, rouge2_score, rougel_score
 from unitorch.score.map import map_score, map50_score
```

### Comparing `unitorch-0.0.0.3/src/unitorch/score/bleu.py` & `unitorch-0.0.0.4/src/unitorch/score/bleu.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/score/map.py` & `unitorch-0.0.0.4/src/unitorch/score/map.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/score/rouge.py` & `unitorch-0.0.0.4/src/unitorch/score/rouge.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/__init__.py` & `unitorch-0.0.0.4/src/unitorch/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     rpartial,
     truncate_sequence_pair,
     nested_dict_value,
 )
 from unitorch.utils.image_utils import make_grid
 from unitorch.utils.import_utils import (
     is_deepspeed_available,
+    is_accelerate_available,
+    is_megatron_available,
     is_diffusers_available,
     is_torch_available,
     is_torch2_available,
 )
 from unitorch.utils.io import GenericWriter, IOProcess, PostProcess, GENERATE_FINISHED
 from unitorch.utils.torch_utils import get_local_rank
 from unitorch.utils.torch_utils import (
```

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/decorators.py` & `unitorch-0.0.0.4/src/unitorch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/functional.py` & `unitorch-0.0.0.4/src/unitorch/utils/functional.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/image_utils.py` & `unitorch-0.0.0.4/src/unitorch/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/import_utils.py` & `unitorch-0.0.0.4/src/unitorch/utils/import_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,40 @@
     _deepspeed_available = False
 
 
 def is_deepspeed_available():
     return _deepspeed_available or is_offline_debug_mode()
 
 
+# accelerate
+_accelerate_available = importlib.util.find_spec("accelerate") is not None
+try:
+    _accelerate_version = importlib_metadata.version("accelerate")
+    logging.debug(f"Successfully imported accelerate version {_accelerate_version}")
+except importlib_metadata.PackageNotFoundError:
+    _accelerate_available = False
+
+
+def is_accelerate_available():
+    return _accelerate_available or is_offline_debug_mode()
+
+
+# megatron
+_megatron_available = importlib.util.find_spec("megatron") is not None
+try:
+    _megatron_version = importlib_metadata.version("megatron")
+    logging.debug(f"Successfully imported megatron version {_megatron_version}")
+except importlib_metadata.PackageNotFoundError:
+    _megatron_available = False
+
+
+def is_megatron_available():
+    return _megatron_available or is_offline_debug_mode()
+
+
 # diffusers
 _diffusers_available = importlib.util.find_spec("diffusers") is not None
 try:
     _diffusers_version = importlib_metadata.version("diffusers")
     logging.debug(f"Successfully imported diffusers version {_diffusers_version}")
 except importlib_metadata.PackageNotFoundError:
     _diffusers_available = False
```

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/io.py` & `unitorch-0.0.0.4/src/unitorch/utils/io.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/palette.py` & `unitorch-0.0.0.4/src/unitorch/utils/palette.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch/utils/torch_utils.py` & `unitorch-0.0.0.4/src/unitorch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/src/unitorch.egg-info/PKG-INFO` & `unitorch-0.0.0.4/src/unitorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
+Provides-Extra: accelerate
 Provides-Extra: chatglm
-Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
```

### Comparing `unitorch-0.0.0.3/src/unitorch.egg-info/SOURCES.txt` & `unitorch-0.0.0.4/src/unitorch.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 examples/configs/classification/roberta.ini
 examples/configs/classification/swin.ini
 examples/configs/classification/text_clip.ini
 examples/configs/classification/lora/bloom.ini
 examples/configs/classification/lora/bloom_ds.ini
 examples/configs/classification/lora/llama.ini
 examples/configs/classification/lora/llama_ds.ini
+examples/configs/diffusion/stable-v1.5.ini
+examples/configs/diffusion/stable-v2.1.ini
+examples/configs/diffusion/stable-v2.ini
+examples/configs/diffusion/controlnet/canny.ini
 examples/configs/generation/bart.ini
 examples/configs/generation/bloom.ini
 examples/configs/generation/chatglm.ini
 examples/configs/generation/llama.ini
 examples/configs/generation/mbart.ini
 examples/configs/generation/mt5.ini
 examples/configs/generation/pegasus.ini
```

### Comparing `unitorch-0.0.0.3/wiki/cli/models/blip.md` & `unitorch-0.0.0.4/wiki/cli/models/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/bloom.md` & `unitorch-0.0.0.4/wiki/cli/models/bloom.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/chatglm.md` & `unitorch-0.0.0.4/wiki/cli/models/chatglm.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/clip.md` & `unitorch-0.0.0.4/wiki/cli/models/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/deberta.md` & `unitorch-0.0.0.4/wiki/cli/models/deberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/llama.md` & `unitorch-0.0.0.4/wiki/cli/models/llama.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/peft.md` & `unitorch-0.0.0.4/wiki/cli/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/visualbert.md` & `unitorch-0.0.0.4/wiki/cli/models/visualbert.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/models/xlm_roberta.md` & `unitorch-0.0.0.4/wiki/cli/models/xlm_roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/cli/postprocess.md` & `unitorch-0.0.0.4/wiki/cli/postprocess.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/configuration.md` & `unitorch-0.0.0.4/wiki/configuration.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/examples/caption/blip.md` & `unitorch-0.0.0.4/wiki/examples/caption/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/examples/classification/clip.md` & `unitorch-0.0.0.4/wiki/examples/classification/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/examples/classification/roberta.md` & `unitorch-0.0.0.4/wiki/examples/classification/roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/examples/classification/swin.md` & `unitorch-0.0.0.4/wiki/examples/classification/swin.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/examples/generation/bart.md` & `unitorch-0.0.0.4/wiki/examples/generation/bart.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/examples/service/zip_image.md` & `unitorch-0.0.0.4/wiki/examples/service/zip_image.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/index.md` & `unitorch-0.0.0.4/wiki/index.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/installation.md` & `unitorch-0.0.0.4/wiki/installation.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/models/peft.md` & `unitorch-0.0.0.4/wiki/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.3/wiki/overview.md` & `unitorch-0.0.0.4/wiki/overview.md`

 * *Files identical despite different names*

