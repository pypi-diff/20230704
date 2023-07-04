# Comparing `tmp/mmocr-1.0.0rc6.tar.gz` & `tmp/mmocr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmocr-1.0.0rc6.tar", last modified: Tue Mar  7 12:27:59 2023, max compression
+gzip compressed data, was "dist/mmocr-1.0.1.tar", last modified: Tue Jul  4 07:12:10 2023, max compression
```

## Comparing `mmocr-1.0.0rc6.tar` & `mmocr-1.0.1.tar`

### file list

```diff
@@ -1,566 +1,569 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/backbone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/backbone/oclip/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/backbone/oclip/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/datasets/wildreceipt-openset.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/datasets/wildreceipt.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/schedules/schedule_adam_60e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_novisual.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_unet16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt-openset.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/sdmgr_unet16_60e_wildreceipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/icdar2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/synthtext.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/totaltext.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/toy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/default_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/pretrain_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/schedules/schedule_adam_600e.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_100k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_1200e.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet18_fpnc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet50-dcnv2_fpnc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_100k_synthtext.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_totaltext.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_100k_synthtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-oclip_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/_base_dbnetpp_resnet50-dcnv2_fpnc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_100k_synthtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-oclip_fpnc_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50_fpnc_1200e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/_base_drrg_resnet50_fpn-unet.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/drrg_resnet50-oclip_fpn-unet_1200e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/drrg_resnet50_fpn-unet_1200e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50-dcnv2_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-dcnv2_fpn_1500e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-oclip_fpn_1500e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-oclip_fpn_1500e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_totaltext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/_base_mask-rcnn_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50-oclip_fpn_160e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50-oclip_fpn_160e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_icdar2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/_base_panet_resnet18_fpem-ffm.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/_base_panet_resnet50_fpem-ffm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/panet_resnet50_fpem-ffm_600e_icdar2017.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/_base_psenet_resnet50_fpnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50-oclip_fpnf_600e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50-oclip_fpnf_600e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2017.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/_base_textsnake_resnet50_fpn-unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/textsnake_resnet50-oclip_fpn-unet_1200e_ctw1500.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/textsnake_resnet50_fpn-unet_1200e_ctw1500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/coco_text_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/cute80.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2011.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2013.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/iiit5k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/mjsynth.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/svt.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/svtp.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/synthtext.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/synthtext_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/totaltext.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/toy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adadelta_5e.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adam_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adam_step_5e.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adamw_cos_6e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/_base_abinet-vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/_base_abinet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/abinet-vision_20e_st-an_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/abinet_20e_st-an_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/_base_aster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/aster_resnet45_6e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/_base_crnn_mini-vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_toy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/_base_master_resnet31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_st_mj_sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_toy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_modality-transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_resnet31.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_toy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_resnet31-1by16-1by8_6e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_resnet31-1by8-1by4_6e_st_mj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/_base_robustscanner_resnet31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_st-sub_mj-sub_sa_real.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_toy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4109 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/_base_sar_resnet31_parallel-decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_st-sub_mj-sub_sa_real.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_toy.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/sar_resnet31_sequential-decoder_5e_st-sub_mj-sub_sa_real.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/_base_satrn_shallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/satrn_shallow-small_5e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/satrn_shallow_5e_st_mj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/_base_svtr-tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/svtr-base_20e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/svtr-large_20e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/svtr-small_20e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/svtr-tiny_20e_st_mj.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/get_flops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/offline_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/print_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/common/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/common/curvedsyntext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/common/extract_kaist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/kie/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/kie/closeset_to_openset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/prepare_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/art_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/bid_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/coco_to_line_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/cocotext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ctw1500_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/data_migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/detext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/funsd_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/hiertext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ic11_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ic13_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/icdar_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ilst_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/imgur_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/kaist_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/lsvt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/lv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/mtwi_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/naf_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/rctw_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/rects_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/sroie_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/synthtext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/textocr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/totaltext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/vintext_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/art_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/bid_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/cocotext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/data_migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/detext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/funsd_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/hiertext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/ic11_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/ic13_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/ilst_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/imgur_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/kaist_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/lmdb_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/lsvt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/lv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/mtwi_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/naf_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/openvino_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/rctw_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/rects_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/sroie_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/svt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/synthtext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/textocr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/totaltext_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/vintext_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/dist_train.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/model_converters/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/model_converters/publish_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/slurm_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/slurm_train.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4985 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4006 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/.mim/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/base_mmocr_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/kie_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/mmocr_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/textdet_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/textrec_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/apis/inferencers/textspot_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/icdar_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/ocr_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/textdet_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/textrecog_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/textspotting_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/data_preparer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/json_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/lmdb_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/wild_receipt_openset_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/mono_gatherer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/naf_gatherer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/pair_gatherer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/obtainers/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/obtainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/obtainers/naive_data_obtainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/textdet_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/textrecog_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/textspotting_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/wildreceipt_packer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/coco_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/funsd_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/icdar_txt_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/naf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/sroie_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/svt_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/totaltext_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/wildreceipt_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/recog_lmdb_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/recog_text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/samplers/batch_aug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)    28656 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/ocr_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/textdet_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    23383 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/textrecog_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/transforms/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/datasets/wildreceipt_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/evaluation/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/evaluator/multi_datasets_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/evaluation/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/functional/hmean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/metrics/f_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/metrics/hmean_iou_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/evaluation/metrics/recog_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/backbones/clip_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/backbones/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/dictionary/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/layers/transformer_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/losses/bce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/losses/ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/losses/l1_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/modules/transformer_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/common/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/common/plugins/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/kie/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/kie/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/extractors/sdmgr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/kie/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/heads/sdmgr_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/kie/module_losses/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/module_losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/module_losses/sdmgr_module_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/kie/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/kie/postprocessors/sdmgr_postprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/data_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/data_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/data_preprocessors/data_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/dbnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/drrg.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/fcenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/mmdet_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/panet.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/psenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/single_stage_text_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/detectors/textsnake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/db_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    50385 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/drrg_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/fce_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/pan_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/pse_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/heads/textsnake_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/db_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    33570 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/drrg_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/fce_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/pan_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/pse_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/seg_based_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    27634 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/textsnake_module_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpem_ffm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpn_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpn_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpnf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/db_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/drrg_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/fce_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/pan_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/pse_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/textsnake_postprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/mini_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/resnet31_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/resnet_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/shallow_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/data_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/data_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/data_preprocessors/data_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/abi_fuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/abi_language_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/abi_vision_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/aster_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/crnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/master_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/nrtr_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/position_attention_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/robust_scanner_fuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22509 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/sar_decoder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5459 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/sequence_attention_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/svtr_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/aster_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/channel_reduction_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/nrtr_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/sar_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/satrn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    24406 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/svtr_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/conv_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/dot_product_attention_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/lstm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/position_aware_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/layers/satrn_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/abi_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/ce_module_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/ctc_module_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/plugins/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/attn_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/ctc_postprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/preprocessors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/preprocessors/tps_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/abinet.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/aster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/crnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/master.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/nrtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/robust_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/satrn.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/svtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/structures/kie_data_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/structures/textdet_data_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/structures/textrecog_data_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/structures/textspotting_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/testing/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/bbox_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/bezier_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/check_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/data_converter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/point_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/polygon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/transform_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/utils/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/visualization/base_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/visualization/kie_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/visualization/textdet_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/visualization/textrecog_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/mmocr/visualization/textspotting_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/mmocr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/albu.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-07 12:27:59.000000 mmocr-1.0.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-03-07 12:27:54.000000 mmocr-1.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-04 07:12:05.000000 mmocr-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17168 2023-07-04 07:12:10.000000 mmocr-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-04 07:12:05.000000 mmocr-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/backbone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/backbone/oclip/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/backbone/oclip/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/datasets/wildreceipt-openset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/datasets/wildreceipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/schedules/schedule_adam_60e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_novisual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_unet16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt-openset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/sdmgr_unet16_60e_wildreceipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/icdar2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/synthtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/totaltext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/toy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/default_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/pretrain_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/schedules/schedule_adam_600e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_100k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_1200e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet18_fpnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet50-dcnv2_fpnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_100k_synthtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_totaltext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_100k_synthtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-oclip_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/_base_dbnetpp_resnet50-dcnv2_fpnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_100k_synthtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-oclip_fpnc_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50_fpnc_1200e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/_base_drrg_resnet50_fpn-unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/drrg_resnet50-oclip_fpn-unet_1200e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/drrg_resnet50_fpn-unet_1200e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50-dcnv2_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-dcnv2_fpn_1500e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-oclip_fpn_1500e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-oclip_fpn_1500e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_totaltext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/_base_mask-rcnn_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50-oclip_fpn_160e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50-oclip_fpn_160e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_icdar2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/_base_panet_resnet18_fpem-ffm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/_base_panet_resnet50_fpem-ffm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/panet_resnet50_fpem-ffm_600e_icdar2017.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/_base_psenet_resnet50_fpnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50-oclip_fpnf_600e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50-oclip_fpnf_600e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2017.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/_base_textsnake_resnet50_fpn-unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/textsnake_resnet50-oclip_fpn-unet_1200e_ctw1500.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/textsnake_resnet50_fpn-unet_1200e_ctw1500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/coco_text_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/cute80.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2013.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/iiit5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/mjsynth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/svt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/svtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/synthtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/synthtext_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/totaltext.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/toy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adadelta_5e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adam_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adam_step_5e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adamw_cos_6e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/_base_abinet-vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/_base_abinet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/abinet-vision_20e_st-an_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/abinet_20e_st-an_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/_base_aster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/aster_resnet45_6e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/_base_crnn_mini-vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_toy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/_base_master_resnet31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_st_mj_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_toy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_modality-transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_resnet31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_toy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_resnet31-1by16-1by8_6e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_resnet31-1by8-1by4_6e_st_mj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/_base_robustscanner_resnet31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_st-sub_mj-sub_sa_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_toy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3931 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/_base_sar_resnet31_parallel-decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_st-sub_mj-sub_sa_real.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_toy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/sar_resnet31_sequential-decoder_5e_st-sub_mj-sub_sa_real.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/_base_satrn_shallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/satrn_shallow-small_5e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/satrn_shallow_5e_st_mj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/_base_svtr-tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/svtr-base_20e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/svtr-large_20e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/svtr-small_20e_st_mj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/svtr-tiny_20e_st_mj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/dicts/
+-rw-r--r--   0 runner    (1001) docker     (123)    45284 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/chinese_english_digits.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/english_digits_symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/english_digits_symbols_space.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/korean_english_digits_symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/lower_english_digits.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/lower_english_digits_space.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/dicts/sdmgr_dict.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/get_flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/offline_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/print_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/common/curvedsyntext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/common/extract_kaist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/kie/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/kie/closeset_to_openset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/prepare_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/art_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/bid_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/coco_to_line_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/cocotext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/data_migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/detext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/funsd_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/hiertext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/ic11_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/ilst_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/imgur_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/kaist_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/lsvt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/lv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/mtwi_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/naf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/rctw_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/rects_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/sroie_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/vintext_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/art_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/bid_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/cocotext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/data_migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/detext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/funsd_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/hiertext_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/ic11_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/ilst_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/imgur_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/kaist_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/lmdb_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/lsvt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/lv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/mtwi_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/naf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/openvino_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/rctw_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/rects_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/sroie_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/vintext_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/dist_train.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/model_converters/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/model_converters/publish_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/slurm_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/slurm_train.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5172 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4194 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/.mim/tools/visualizations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/visualizations/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/.mim/tools/visualizations/vis_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/apis/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/base_mmocr_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/kie_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/mmocr_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/textdet_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/textrec_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/apis/inferencers/textspot_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/icdar_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/ocr_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/config_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/config_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/config_generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/config_generators/textdet_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/config_generators/textrecog_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/config_generators/textspotting_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/data_preparer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/dumpers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/dumpers/json_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/dumpers/lmdb_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/dumpers/wild_receipt_openset_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/gatherers/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/gatherers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/gatherers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/gatherers/mono_gatherer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/gatherers/naf_gatherer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/gatherers/pair_gatherer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/obtainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/obtainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/obtainers/aws_s3_obtainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/obtainers/naive_data_obtainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/textdet_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/textrecog_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/textspotting_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/packers/wildreceipt_packer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/coco_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/ctw1500_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/funsd_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/icdar_txt_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/mjsynth_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/naf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/sroie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/svt_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/synthtext_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/totaltext_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/preparers/parsers/wildreceipt_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/recog_lmdb_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/recog_text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/samplers/batch_aug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28656 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/ocr_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/textdet_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23383 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/textrecog_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/transforms/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/datasets/wildreceipt_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/evaluation/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/evaluator/multi_datasets_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/evaluation/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/functional/hmean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/metrics/f_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/metrics/hmean_iou_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/evaluation/metrics/recog_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/backbones/clip_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/backbones/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/dictionary/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/layers/transformer_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/losses/bce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/losses/ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/losses/l1_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/modules/transformer_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/common/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/common/plugins/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/kie/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/kie/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/extractors/sdmgr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/kie/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/heads/sdmgr_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/kie/module_losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/module_losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/module_losses/sdmgr_module_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/kie/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/kie/postprocessors/sdmgr_postprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/data_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/data_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/data_preprocessors/data_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/dbnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/drrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/fcenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/mmdet_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/panet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/psenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/single_stage_text_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/detectors/textsnake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/db_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50609 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/drrg_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/fce_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/pan_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/pse_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/heads/textsnake_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/db_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33782 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/drrg_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/fce_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/pan_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/pse_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/seg_based_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27634 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/module_losses/textsnake_module_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/necks/fpem_ffm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/necks/fpn_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/necks/fpn_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/necks/fpnf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/db_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/drrg_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/fce_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/pan_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/pse_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textdet/postprocessors/textsnake_postprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/mini_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/resnet31_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/resnet_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/backbones/shallow_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/data_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/data_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/data_preprocessors/data_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/abi_fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/abi_language_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/abi_vision_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/aster_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/crnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/master_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/nrtr_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/position_attention_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/robust_scanner_fuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22509 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/sar_decoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5459 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/sequence_attention_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/decoders/svtr_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/aster_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/channel_reduction_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/nrtr_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/sar_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/satrn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24406 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/encoders/svtr_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/conv_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/dot_product_attention_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/lstm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/position_aware_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/layers/satrn_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/module_losses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/module_losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/module_losses/abi_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/module_losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/module_losses/ce_module_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/module_losses/ctc_module_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/plugins/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/postprocessors/attn_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/postprocessors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/postprocessors/ctc_postprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/preprocessors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/preprocessors/tps_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/abinet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/aster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/crnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/nrtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/robust_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/satrn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/models/textrecog/recognizers/svtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/structures/kie_data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/structures/textdet_data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/structures/textrecog_data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/structures/textspotting_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/testing/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/bezier_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/check_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/data_converter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/point_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/polygon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/utils/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/mmocr/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/visualization/base_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19584 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/visualization/kie_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/visualization/textdet_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/visualization/textrecog_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-04 07:12:05.000000 mmocr-1.0.1/mmocr/visualization/textspotting_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17168 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 07:12:09.000000 mmocr-1.0.1/mmocr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:12:10.000000 mmocr-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/albu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 07:12:05.000000 mmocr-1.0.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 07:12:10.000000 mmocr-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-04 07:12:05.000000 mmocr-1.0.1/setup.py
```

### Comparing `mmocr-1.0.0rc6/PKG-INFO` & `mmocr-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmocr
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: OpenMMLab Text Detection, OCR, and NLP Toolbox
 Home-page: https://github.com/open-mmlab/mmocr
 Maintainer: MMOCR Authors
 Maintainer-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmocr-logo.png" width="500px"/>
@@ -46,42 +46,44 @@
         <div align="center">
         
         English | [简体中文](README_zh-CN.md)
         
         </div>
         <div align="center">
           <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218352562-cdded397-b0f3-4ca1-b8dd-a60df8dca75b.png" width="3%" alt="" /></a>
+            <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## Latest Updates
         
-        **The default branch has been switched to `1.x` from `main`, and we encourage
-        users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html) for more
-        details.**
-        
-        v1.0.0rc6 was released in 2023-03-07.
-        
-        1. Two new models, ABCNet v2 (inference only) and SPTS are added to `projects/` folder.
-        2. Announcing `Inferencer`, a unified inference interface in OpenMMLab for everyone's easy access and quick inference with all the pre-trained weights. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/inference.html)
-        3. Users can use test-time augmentation for text recognition tasks. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/train_test.html#test-time-augmentation)
-        4. Support [batch augmentation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf) through [`BatchAugSampler`](https://github.com/open-mmlab/mmocr/pull/1757), which is a technique used in SPTS.
-        5. Dataset Preparer has been refactored to allow more flexible configurations. Besides, users are now able to prepare text recognition datasets in LMDB formats. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/dataset_preparer.html#lmdb-format)
-        6. Some textspotting datasets have been revised to enhance the correctness and consistency with the common practice.
-        7. Potential spurious warnings from `shapely` have been eliminated.
+        **The default branch is now `main` and the code on the branch has been upgraded to v1.0.0. The old `main` branch (v0.6.3) code now exists on the `0.x` branch.** If you have been using the `main` branch and encounter upgrade issues, please read the [Migration Guide](https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html) and notes on [Branches](https://mmocr.readthedocs.io/en/dev-1.x/migration/branches.html) .
+        
+        v1.0.0 was released in 2023-04-06. Major updates from 1.0.0rc6 include:
+        
+        1. Support for SCUT-CTW1500, SynthText, and MJSynth datasets in Dataset Preparer
+        2. Updated FAQ and documentation
+        3. Deprecation of file_client_args in favor of backend_args
+        4. Added a new MMOCR tutorial notebook
         
+        To know more about the updates in MMOCR 1.0, please refer to [What's New in MMOCR 1.x](https://mmocr.readthedocs.io/en/dev-1.x/migration/news.html), or
         Read [Changelog](https://mmocr.readthedocs.io/en/dev-1.x/notes/changelog.html) for more details!
         
         ## Introduction
         
         MMOCR is an open-source toolbox based on PyTorch and mmdetection for text detection, text recognition, and the corresponding downstream tasks including key information extraction. It is part of the [OpenMMLab](https://openmmlab.com/) project.
         
         The main branch works with **PyTorch 1.6+**.
@@ -104,49 +106,27 @@
         
           The modular design of MMOCR enables users to define their own optimizers, data preprocessors, and model components such as backbones, necks and heads as well as losses. Please refer to [Overview](https://mmocr.readthedocs.io/en/dev-1.x/get_started/overview.html) for how to construct a customized model.
         
         - **Numerous Utilities**
         
           The toolbox provides a comprehensive set of utilities which can help users assess the performance of models. It includes visualizers which allow visualization of images, ground truths as well as predicted bounding boxes, and a validation tool for evaluating checkpoints during training.  It also includes data converters to demonstrate how to convert your own data to the annotation files which the toolbox supports.
         
-        ## What's New in MMOCR 1.0
-        
-        1. **New engines**. MMOCR 1.x is based on [MMEngine](https://github.com/open-mmlab/mmengine), which provides a general and powerful runner that allows more flexible customizations and significantly simplifies the entrypoints of high-level interfaces.
-        
-        2. **Unified interfaces**. As a part of the OpenMMLab 2.0 projects, MMOCR 1.x unifies and refactors the interfaces and internal logics of train, testing, datasets, models, evaluation, and visualization. All the OpenMMLab 2.0 projects share the same design in those interfaces and logics to allow the emergence of multi-task/modality algorithms.
-        
-        3. **Cross project calling**. Benefiting from the unified design, you can use the models implemented in other OpenMMLab projects, such as MMDet. We provide an example of how to use MMDetection's Mask R-CNN through `MMDetWrapper`. Check our documents for more details. More wrappers will be released in the future.
-        
-        4. **Stronger visualization**. We provide a series of useful tools which are mostly based on brand-new visualizers. As a result, it is more convenient for the users to explore the models and datasets now.
-        
-        5. **More documentation and tutorials**. We add a bunch of documentation and tutorials to help users get started more smoothly. Read it [here](https://mmocr.readthedocs.io/en/dev-1.x/).
-        
-        6. **One-stop Dataset Preparaion**. Multiple datasets are instantly ready with only one line of command, via our [Dataset Preparer](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/dataset_preparer.html).
-        
-        7. **Embracing more `projects/`**: We now introduce `projects/` folder, where some experimental features, frameworks and models can be placed, only needed to satisfy the minimum requirement on the code quality. Everyone is welcome to post their implementation of any great ideas in this folder! Learn more from our [example project](https://github.com/open-mmlab/mmocr/blob/dev-1.x/projects/example_project/).
-        
-        8. **More models**. MMOCR 1.0 supports more tasks and more state-of-the-art models!
-        
         ## Installation
         
         MMOCR depends on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-mmlab/mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection](https://github.com/open-mmlab/mmdetection).
         Below are quick steps for installation.
         Please refer to [Install Guide](https://mmocr.readthedocs.io/en/dev-1.x/get_started/install.html) for more detailed instruction.
         
         ```shell
         conda create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -y
         conda activate open-mmlab
         pip3 install openmim
-        mim install mmengine
-        mim install 'mmcv>=2.0.0rc1'
-        mim install 'mmdet>=3.0.0rc0'
         git clone https://github.com/open-mmlab/mmocr.git
         cd mmocr
-        git checkout 1.x
-        pip3 install -e .
+        mim install -e .
         ```
         
         ## Get Started
         
         Please see [Quick Run](https://mmocr.readthedocs.io/en/dev-1.x/get_started/quick_run.html) for the basic usage of MMOCR.
         
         ## [Model Zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html)
@@ -202,14 +182,18 @@
         - [x] [ABCNetV2](projects/ABCNet/README_V2.md) (TPAMI'2021)
         - [x] [SPTS](projects/SPTS/README.md) (ACM MM'2022)
         
         </details>
         
         Please refer to [model_zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more details.
         
+        ## Projects
+        
+        [Here](projects/README.md) are some implementations of SOTA models and solutions built on MMOCR, which are supported and maintained by community users. These projects demonstrate the best practices based on MMOCR for research and product development. We welcome and appreciate all the contributions to OpenMMLab ecosystem.
+        
         ## Contributing
         
         We appreciate all contributions to improve MMOCR. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guidelines.
         
         ## Acknowledgement
         
         MMOCR is an open-source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
@@ -228,15 +212,15 @@
         }
         ```
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE).
         
-        ## Projects in OpenMMLab
+        ## OpenMMLab Family
         
         - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
         - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
         - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
         - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmocr Version: 1.0.0rc6 Summary: OpenMMLab Text
+Metadata-Version: 2.1 Name: mmocr Version: 1.0.1 Summary: OpenMMLab Text
 Detection, OCR, and NLP Toolbox Home-page: https://github.com/open-mmlab/mmocr
 Maintainer: MMOCR Authors Maintainer-email: openmmlab@gmail.com License: Apache
 License 2.0 Description:
                           [resources/mmocr-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
@@ -22,35 +22,26 @@
       mmocr.readthedocs.io/en/dev-1.x/) | [ð ï¸Installation](https://
   mmocr.readthedocs.io/en/dev-1.x/get_started/install.html) | [ðModel Zoo]
   (https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) | [ðUpdate News]
 (https://mmocr.readthedocs.io/en/dev-1.x/notes/changelog.html) | [ð¤Reporting
         Issues](https://github.com/open-mmlab/mmocr/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## Latest Updates **The default branch has been switched to `1.x` from `main`,
-and we encourage users to migrate to the latest version, though it comes with
-some cost. Please refer to [Migration Guide](https://mmocr.readthedocs.io/en/
-dev-1.x/migration/overview.html) for more details.** v1.0.0rc6 was released in
-2023-03-07. 1. Two new models, ABCNet v2 (inference only) and SPTS are added to
-`projects/` folder. 2. Announcing `Inferencer`, a unified inference interface
-in OpenMMLab for everyone's easy access and quick inference with all the pre-
-trained weights. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/
-inference.html) 3. Users can use test-time augmentation for text recognition
-tasks. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/
-train_test.html#test-time-augmentation) 4. Support [batch augmentation](https:/
-/openaccess.thecvf.com/content_CVPR_2020/papers/
-Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf)
-through [`BatchAugSampler`](https://github.com/open-mmlab/mmocr/pull/1757),
-which is a technique used in SPTS. 5. Dataset Preparer has been refactored to
-allow more flexible configurations. Besides, users are now able to prepare text
-recognition datasets in LMDB formats. [Docs](https://mmocr.readthedocs.io/en/
-dev-1.x/user_guides/data_prepare/dataset_preparer.html#lmdb-format) 6. Some
-textspotting datasets have been revised to enhance the correctness and
-consistency with the common practice. 7. Potential spurious warnings from
-`shapely` have been eliminated. Read [Changelog](https://mmocr.readthedocs.io/
+## Latest Updates **The default branch is now `main` and the code on the branch
+has been upgraded to v1.0.0. The old `main` branch (v0.6.3) code now exists on
+the `0.x` branch.** If you have been using the `main` branch and encounter
+upgrade issues, please read the [Migration Guide](https://mmocr.readthedocs.io/
+en/dev-1.x/migration/overview.html) and notes on [Branches](https://
+mmocr.readthedocs.io/en/dev-1.x/migration/branches.html) . v1.0.0 was released
+in 2023-04-06. Major updates from 1.0.0rc6 include: 1. Support for SCUT-
+CTW1500, SynthText, and MJSynth datasets in Dataset Preparer 2. Updated FAQ and
+documentation 3. Deprecation of file_client_args in favor of backend_args 4.
+Added a new MMOCR tutorial notebook To know more about the updates in MMOCR
+1.0, please refer to [What's New in MMOCR 1.x](https://mmocr.readthedocs.io/en/
+dev-1.x/migration/news.html), or Read [Changelog](https://mmocr.readthedocs.io/
 en/dev-1.x/notes/changelog.html) for more details! ## Introduction MMOCR is an
 open-source toolbox based on PyTorch and mmdetection for text detection, text
 recognition, and the corresponding downstream tasks including key information
 extraction. It is part of the [OpenMMLab](https://openmmlab.com/) project. The
 main branch works with **PyTorch 1.6+**.
  [https://user-images.githubusercontent.com/24622904/187838618-1fdc61c0-2d46-
                           49f9-8502-976ffdf01f28.png]
@@ -64,126 +55,102 @@
 to [Overview](https://mmocr.readthedocs.io/en/dev-1.x/get_started/
 overview.html) for how to construct a customized model. - **Numerous
 Utilities** The toolbox provides a comprehensive set of utilities which can
 help users assess the performance of models. It includes visualizers which
 allow visualization of images, ground truths as well as predicted bounding
 boxes, and a validation tool for evaluating checkpoints during training. It
 also includes data converters to demonstrate how to convert your own data to
-the annotation files which the toolbox supports. ## What's New in MMOCR 1.0 1.
-**New engines**. MMOCR 1.x is based on [MMEngine](https://github.com/open-
-mmlab/mmengine), which provides a general and powerful runner that allows more
-flexible customizations and significantly simplifies the entrypoints of high-
-level interfaces. 2. **Unified interfaces**. As a part of the OpenMMLab 2.0
-projects, MMOCR 1.x unifies and refactors the interfaces and internal logics of
-train, testing, datasets, models, evaluation, and visualization. All the
-OpenMMLab 2.0 projects share the same design in those interfaces and logics to
-allow the emergence of multi-task/modality algorithms. 3. **Cross project
-calling**. Benefiting from the unified design, you can use the models
-implemented in other OpenMMLab projects, such as MMDet. We provide an example
-of how to use MMDetection's Mask R-CNN through `MMDetWrapper`. Check our
-documents for more details. More wrappers will be released in the future. 4.
-**Stronger visualization**. We provide a series of useful tools which are
-mostly based on brand-new visualizers. As a result, it is more convenient for
-the users to explore the models and datasets now. 5. **More documentation and
-tutorials**. We add a bunch of documentation and tutorials to help users get
-started more smoothly. Read it [here](https://mmocr.readthedocs.io/en/dev-1.x/
-). 6. **One-stop Dataset Preparaion**. Multiple datasets are instantly ready
-with only one line of command, via our [Dataset Preparer](https://
-mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/
-dataset_preparer.html). 7. **Embracing more `projects/`**: We now introduce
-`projects/` folder, where some experimental features, frameworks and models can
-be placed, only needed to satisfy the minimum requirement on the code quality.
-Everyone is welcome to post their implementation of any great ideas in this
-folder! Learn more from our [example project](https://github.com/open-mmlab/
-mmocr/blob/dev-1.x/projects/example_project/). 8. **More models**. MMOCR 1.0
-supports more tasks and more state-of-the-art models! ## Installation MMOCR
-depends on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-
-mmlab/mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection]
-(https://github.com/open-mmlab/mmdetection). Below are quick steps for
-installation. Please refer to [Install Guide](https://mmocr.readthedocs.io/en/
-dev-1.x/get_started/install.html) for more detailed instruction. ```shell conda
-create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -
-c pytorch -y conda activate open-mmlab pip3 install openmim mim install
-mmengine mim install 'mmcv>=2.0.0rc1' mim install 'mmdet>=3.0.0rc0' git clone
-https://github.com/open-mmlab/mmocr.git cd mmocr git checkout 1.x pip3 install
--e . ``` ## Get Started Please see [Quick Run](https://mmocr.readthedocs.io/en/
-dev-1.x/get_started/quick_run.html) for the basic usage of MMOCR. ## [Model
-Zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) Supported
-algorithms:  BackBone - [x] [oCLIP](configs/backbone/oclip/README.md)
-(ECCV'2022)   Text Detection - [x] [DBNet](configs/textdet/dbnet/README.md)
-(AAAI'2020) / [DBNet++](configs/textdet/dbnetpp/README.md) (TPAMI'2022) - [x]
-[Mask R-CNN](configs/textdet/maskrcnn/README.md) (ICCV'2017) - [x] [PANet]
-(configs/textdet/panet/README.md) (ICCV'2019) - [x] [PSENet](configs/textdet/
-psenet/README.md) (CVPR'2019) - [x] [TextSnake](configs/textdet/textsnake/
-README.md) (ECCV'2018) - [x] [DRRG](configs/textdet/drrg/README.md) (CVPR'2020)
-- [x] [FCENet](configs/textdet/fcenet/README.md) (CVPR'2021)   Text Recognition
-- [x] [ABINet](configs/textrecog/abinet/README.md) (CVPR'2021) - [x] [ASTER]
-(configs/textrecog/aster/README.md) (TPAMI'2018) - [x] [CRNN](configs/
-textrecog/crnn/README.md) (TPAMI'2016) - [x] [MASTER](configs/textrecog/master/
-README.md) (PR'2021) - [x] [NRTR](configs/textrecog/nrtr/README.md)
-(ICDAR'2019) - [x] [RobustScanner](configs/textrecog/robust_scanner/README.md)
-(ECCV'2020) - [x] [SAR](configs/textrecog/sar/README.md) (AAAI'2019) - [x]
-[SATRN](configs/textrecog/satrn/README.md) (CVPR'2020 Workshop on Text and
-Documents in the Deep Learning Era) - [x] [SVTR](configs/textrecog/svtr/
-README.md) (IJCAI'2022)   Key Information Extraction - [x] [SDMG-R](configs/
-kie/sdmgr/README.md) (ArXiv'2021)   Text Spotting - [x] [ABCNet](projects/
-ABCNet/README.md) (CVPR'2020) - [x] [ABCNetV2](projects/ABCNet/README_V2.md)
-(TPAMI'2021) - [x] [SPTS](projects/SPTS/README.md) (ACM MM'2022)  Please refer
-to [model_zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more
-details. ## Contributing We appreciate all contributions to improve MMOCR.
-Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
-guidelines. ## Acknowledgement MMOCR is an open-source project that is
-contributed by researchers and engineers from various colleges and companies.
-We appreciate all the contributors who implement their methods or add new
-features, as well as users who give valuable feedbacks. We hope the toolbox and
-benchmark could serve the growing research community by providing a flexible
-toolkit to reimplement existing methods and develop their own new OCR methods.
-## Citation If you find this project useful in your research, please consider
-cite: ```bibtex @article{mmocr2021, title={MMOCR: A Comprehensive Toolbox for
-Text Detection, Recognition and Understanding}, author={Kuang, Zhanghui and
-Sun, Hongbin and Li, Zhizhong and Yue, Xiaoyu and Lin, Tsui Hin and Chen,
-Jianyong and Wei, Huaqiang and Zhu, Yiqin and Gao, Tong and Zhang, Wenwei and
-Chen, Kai and Zhang, Wayne and Lin, Dahua}, journal= {arXiv preprint arXiv:
-2108.06543}, year={2021} } ``` ## License This project is released under the
-[Apache 2.0 license](LICENSE). ## Projects in OpenMMLab - [MMEngine](https://
-github.com/open-mmlab/mmengine): OpenMMLab foundational library for training
-deep learning models - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab
-foundational library for computer vision. - [MIM](https://github.com/open-
-mmlab/mim): MIM installs OpenMMLab packages. - [MMClassification](https://
-github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox
-and benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection):
-OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
-github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
-general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
-mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
-[MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab
-semantic segmentation toolbox and benchmark. - [MMOCR](https://github.com/open-
-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation
-toolbox and benchmark. - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d):
-OpenMMLab 3D human parametric model toolbox and benchmark. - [MMSelfSup](https:
-//github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox
-and benchmark. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab
-model compression toolbox and benchmark. - [MMFewShot](https://github.com/open-
-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark. -
-[MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-
-generation action understanding toolbox and benchmark. - [MMTracking](https://
-github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and
-benchmark. - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical
-flow toolbox and benchmark. - [MMEditing](https://github.com/open-mmlab/
-mmediting): OpenMMLab image and video editing toolbox. - [MMGeneration](https:/
-/github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative
-models toolbox. - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab
-model deployment framework. ## Welcome to the OpenMMLab community Scan the QR
-code below to follow the OpenMMLab team's [**Zhihu Official Account**](https://
-www.zhihu.com/people/openmmlab) and join the OpenMMLab team's [**QQ Group**]
-(https://jq.qq.com/?_wv=1027&k=aCvMxdr3), or join the official communication
-WeChat group by adding the WeChat, or join our [**Slack**](https://
-join.slack.com/t/mmocrworkspace/shared_invite/zt-1ifqhfla8-
-yKnLO_aKhVA2h71OrK8GZw)
+the annotation files which the toolbox supports. ## Installation MMOCR depends
+on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-mmlab/
+mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection](https:/
+/github.com/open-mmlab/mmdetection). Below are quick steps for installation.
+Please refer to [Install Guide](https://mmocr.readthedocs.io/en/dev-1.x/
+get_started/install.html) for more detailed instruction. ```shell conda create
+-n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -
+y conda activate open-mmlab pip3 install openmim git clone https://github.com/
+open-mmlab/mmocr.git cd mmocr mim install -e . ``` ## Get Started Please see
+[Quick Run](https://mmocr.readthedocs.io/en/dev-1.x/get_started/quick_run.html)
+for the basic usage of MMOCR. ## [Model Zoo](https://mmocr.readthedocs.io/en/
+dev-1.x/modelzoo.html) Supported algorithms:  BackBone - [x] [oCLIP](configs/
+backbone/oclip/README.md) (ECCV'2022)   Text Detection - [x] [DBNet](configs/
+textdet/dbnet/README.md) (AAAI'2020) / [DBNet++](configs/textdet/dbnetpp/
+README.md) (TPAMI'2022) - [x] [Mask R-CNN](configs/textdet/maskrcnn/README.md)
+(ICCV'2017) - [x] [PANet](configs/textdet/panet/README.md) (ICCV'2019) - [x]
+[PSENet](configs/textdet/psenet/README.md) (CVPR'2019) - [x] [TextSnake]
+(configs/textdet/textsnake/README.md) (ECCV'2018) - [x] [DRRG](configs/textdet/
+drrg/README.md) (CVPR'2020) - [x] [FCENet](configs/textdet/fcenet/README.md)
+(CVPR'2021)   Text Recognition - [x] [ABINet](configs/textrecog/abinet/
+README.md) (CVPR'2021) - [x] [ASTER](configs/textrecog/aster/README.md)
+(TPAMI'2018) - [x] [CRNN](configs/textrecog/crnn/README.md) (TPAMI'2016) - [x]
+[MASTER](configs/textrecog/master/README.md) (PR'2021) - [x] [NRTR](configs/
+textrecog/nrtr/README.md) (ICDAR'2019) - [x] [RobustScanner](configs/textrecog/
+robust_scanner/README.md) (ECCV'2020) - [x] [SAR](configs/textrecog/sar/
+README.md) (AAAI'2019) - [x] [SATRN](configs/textrecog/satrn/README.md)
+(CVPR'2020 Workshop on Text and Documents in the Deep Learning Era) - [x]
+[SVTR](configs/textrecog/svtr/README.md) (IJCAI'2022)   Key Information
+Extraction - [x] [SDMG-R](configs/kie/sdmgr/README.md) (ArXiv'2021)   Text
+Spotting - [x] [ABCNet](projects/ABCNet/README.md) (CVPR'2020) - [x] [ABCNetV2]
+(projects/ABCNet/README_V2.md) (TPAMI'2021) - [x] [SPTS](projects/SPTS/
+README.md) (ACM MM'2022)  Please refer to [model_zoo](https://
+mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more details. ## Projects
+[Here](projects/README.md) are some implementations of SOTA models and
+solutions built on MMOCR, which are supported and maintained by community
+users. These projects demonstrate the best practices based on MMOCR for
+research and product development. We welcome and appreciate all the
+contributions to OpenMMLab ecosystem. ## Contributing We appreciate all
+contributions to improve MMOCR. Please refer to [CONTRIBUTING.md](.github/
+CONTRIBUTING.md) for the contributing guidelines. ## Acknowledgement MMOCR is
+an open-source project that is contributed by researchers and engineers from
+various colleges and companies. We appreciate all the contributors who
+implement their methods or add new features, as well as users who give valuable
+feedbacks. We hope the toolbox and benchmark could serve the growing research
+community by providing a flexible toolkit to reimplement existing methods and
+develop their own new OCR methods. ## Citation If you find this project useful
+in your research, please consider cite: ```bibtex @article{mmocr2021, title=
+{MMOCR: A Comprehensive Toolbox for Text Detection, Recognition and
+Understanding}, author={Kuang, Zhanghui and Sun, Hongbin and Li, Zhizhong and
+Yue, Xiaoyu and Lin, Tsui Hin and Chen, Jianyong and Wei, Huaqiang and Zhu,
+Yiqin and Gao, Tong and Zhang, Wenwei and Chen, Kai and Zhang, Wayne and Lin,
+Dahua}, journal= {arXiv preprint arXiv:2108.06543}, year={2021} } ``` ##
+License This project is released under the [Apache 2.0 license](LICENSE). ##
+OpenMMLab Family - [MMEngine](https://github.com/open-mmlab/mmengine):
+OpenMMLab foundational library for training deep learning models - [MMCV]
+(https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for
+computer vision. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [MMClassification](https://github.com/open-mmlab/
+mmclassification): OpenMMLab image classification toolbox and benchmark. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMDetection3D](https://github.com/open-mmlab/
+mmdetection3d): OpenMMLab's next-generation platform for general 3D object
+detection. - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab
+rotated object detection toolbox and benchmark. - [MMSegmentation](https://
+github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox
+and benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text
+detection, recognition, and understanding toolbox. - [MMPose](https://
+github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human
+parametric model toolbox and benchmark. - [MMSelfSup](https://github.com/open-
+mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark. -
+[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
+toolbox and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
+OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
+github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
+understanding toolbox and benchmark. - [MMTracking](https://github.com/open-
+mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark. - [MMFlow]
+(https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and
+benchmark. - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab
+image and video editing toolbox. - [MMGeneration](https://github.com/open-
+mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. ## Welcome to the OpenMMLab community Scan the QR code below to
+follow the OpenMMLab team's [**Zhihu Official Account**](https://www.zhihu.com/
+people/openmmlab) and join the OpenMMLab team's [**QQ Group**](https://
+jq.qq.com/?_wv=1027&k=aCvMxdr3), or join the official communication WeChat
+group by adding the WeChat, or join our [**Slack**](https://join.slack.com/t/
+mmocrworkspace/shared_invite/zt-1ifqhfla8-yKnLO_aKhVA2h71OrK8GZw)
   [https://raw.githubusercontent.com/open-mmlab/mmcv/master/docs/en/_static/
  zhihu_qrcode.jpg] [https://raw.githubusercontent.com/open-mmlab/mmcv/master/
  docs/en/_static/qq_group_qrcode.jpg] [https://raw.githubusercontent.com/open-
              mmlab/mmcv/master/docs/en/_static/wechat_qrcode.jpg]
 We will provide you with the OpenMMLab community - ð¢ share the latest core
 technologies of AI frameworks - ð» Explaining PyTorch common module source
 Code - ð° News related to the release of OpenMMLab - ð Introduction of
```

### Comparing `mmocr-1.0.0rc6/README.md` & `mmocr-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -38,42 +38,44 @@
 <div align="center">
 
 English | [简体中文](README_zh-CN.md)
 
 </div>
 <div align="center">
   <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218352562-cdded397-b0f3-4ca1-b8dd-a60df8dca75b.png" width="3%" alt="" /></a>
+    <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
   <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
   <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
     <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
 </div>
 
 ## Latest Updates
 
-**The default branch has been switched to `1.x` from `main`, and we encourage
-users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html) for more
-details.**
-
-v1.0.0rc6 was released in 2023-03-07.
-
-1. Two new models, ABCNet v2 (inference only) and SPTS are added to `projects/` folder.
-2. Announcing `Inferencer`, a unified inference interface in OpenMMLab for everyone's easy access and quick inference with all the pre-trained weights. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/inference.html)
-3. Users can use test-time augmentation for text recognition tasks. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/train_test.html#test-time-augmentation)
-4. Support [batch augmentation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf) through [`BatchAugSampler`](https://github.com/open-mmlab/mmocr/pull/1757), which is a technique used in SPTS.
-5. Dataset Preparer has been refactored to allow more flexible configurations. Besides, users are now able to prepare text recognition datasets in LMDB formats. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/dataset_preparer.html#lmdb-format)
-6. Some textspotting datasets have been revised to enhance the correctness and consistency with the common practice.
-7. Potential spurious warnings from `shapely` have been eliminated.
+**The default branch is now `main` and the code on the branch has been upgraded to v1.0.0. The old `main` branch (v0.6.3) code now exists on the `0.x` branch.** If you have been using the `main` branch and encounter upgrade issues, please read the [Migration Guide](https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html) and notes on [Branches](https://mmocr.readthedocs.io/en/dev-1.x/migration/branches.html) .
+
+v1.0.0 was released in 2023-04-06. Major updates from 1.0.0rc6 include:
+
+1. Support for SCUT-CTW1500, SynthText, and MJSynth datasets in Dataset Preparer
+2. Updated FAQ and documentation
+3. Deprecation of file_client_args in favor of backend_args
+4. Added a new MMOCR tutorial notebook
 
+To know more about the updates in MMOCR 1.0, please refer to [What's New in MMOCR 1.x](https://mmocr.readthedocs.io/en/dev-1.x/migration/news.html), or
 Read [Changelog](https://mmocr.readthedocs.io/en/dev-1.x/notes/changelog.html) for more details!
 
 ## Introduction
 
 MMOCR is an open-source toolbox based on PyTorch and mmdetection for text detection, text recognition, and the corresponding downstream tasks including key information extraction. It is part of the [OpenMMLab](https://openmmlab.com/) project.
 
 The main branch works with **PyTorch 1.6+**.
@@ -96,49 +98,27 @@
 
   The modular design of MMOCR enables users to define their own optimizers, data preprocessors, and model components such as backbones, necks and heads as well as losses. Please refer to [Overview](https://mmocr.readthedocs.io/en/dev-1.x/get_started/overview.html) for how to construct a customized model.
 
 - **Numerous Utilities**
 
   The toolbox provides a comprehensive set of utilities which can help users assess the performance of models. It includes visualizers which allow visualization of images, ground truths as well as predicted bounding boxes, and a validation tool for evaluating checkpoints during training.  It also includes data converters to demonstrate how to convert your own data to the annotation files which the toolbox supports.
 
-## What's New in MMOCR 1.0
-
-1. **New engines**. MMOCR 1.x is based on [MMEngine](https://github.com/open-mmlab/mmengine), which provides a general and powerful runner that allows more flexible customizations and significantly simplifies the entrypoints of high-level interfaces.
-
-2. **Unified interfaces**. As a part of the OpenMMLab 2.0 projects, MMOCR 1.x unifies and refactors the interfaces and internal logics of train, testing, datasets, models, evaluation, and visualization. All the OpenMMLab 2.0 projects share the same design in those interfaces and logics to allow the emergence of multi-task/modality algorithms.
-
-3. **Cross project calling**. Benefiting from the unified design, you can use the models implemented in other OpenMMLab projects, such as MMDet. We provide an example of how to use MMDetection's Mask R-CNN through `MMDetWrapper`. Check our documents for more details. More wrappers will be released in the future.
-
-4. **Stronger visualization**. We provide a series of useful tools which are mostly based on brand-new visualizers. As a result, it is more convenient for the users to explore the models and datasets now.
-
-5. **More documentation and tutorials**. We add a bunch of documentation and tutorials to help users get started more smoothly. Read it [here](https://mmocr.readthedocs.io/en/dev-1.x/).
-
-6. **One-stop Dataset Preparaion**. Multiple datasets are instantly ready with only one line of command, via our [Dataset Preparer](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/dataset_preparer.html).
-
-7. **Embracing more `projects/`**: We now introduce `projects/` folder, where some experimental features, frameworks and models can be placed, only needed to satisfy the minimum requirement on the code quality. Everyone is welcome to post their implementation of any great ideas in this folder! Learn more from our [example project](https://github.com/open-mmlab/mmocr/blob/dev-1.x/projects/example_project/).
-
-8. **More models**. MMOCR 1.0 supports more tasks and more state-of-the-art models!
-
 ## Installation
 
 MMOCR depends on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-mmlab/mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection](https://github.com/open-mmlab/mmdetection).
 Below are quick steps for installation.
 Please refer to [Install Guide](https://mmocr.readthedocs.io/en/dev-1.x/get_started/install.html) for more detailed instruction.
 
 ```shell
 conda create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -y
 conda activate open-mmlab
 pip3 install openmim
-mim install mmengine
-mim install 'mmcv>=2.0.0rc1'
-mim install 'mmdet>=3.0.0rc0'
 git clone https://github.com/open-mmlab/mmocr.git
 cd mmocr
-git checkout 1.x
-pip3 install -e .
+mim install -e .
 ```
 
 ## Get Started
 
 Please see [Quick Run](https://mmocr.readthedocs.io/en/dev-1.x/get_started/quick_run.html) for the basic usage of MMOCR.
 
 ## [Model Zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html)
@@ -194,14 +174,18 @@
 - [x] [ABCNetV2](projects/ABCNet/README_V2.md) (TPAMI'2021)
 - [x] [SPTS](projects/SPTS/README.md) (ACM MM'2022)
 
 </details>
 
 Please refer to [model_zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more details.
 
+## Projects
+
+[Here](projects/README.md) are some implementations of SOTA models and solutions built on MMOCR, which are supported and maintained by community users. These projects demonstrate the best practices based on MMOCR for research and product development. We welcome and appreciate all the contributions to OpenMMLab ecosystem.
+
 ## Contributing
 
 We appreciate all contributions to improve MMOCR. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guidelines.
 
 ## Acknowledgement
 
 MMOCR is an open-source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
@@ -220,15 +204,15 @@
 }
 ```
 
 ## License
 
 This project is released under the [Apache 2.0 license](LICENSE).
 
-## Projects in OpenMMLab
+## OpenMMLab Family
 
 - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models
 - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
 - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
 - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
 - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
 - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
```

#### html2text {}

```diff
@@ -18,35 +18,26 @@
       mmocr.readthedocs.io/en/dev-1.x/) | [ð ï¸Installation](https://
   mmocr.readthedocs.io/en/dev-1.x/get_started/install.html) | [ðModel Zoo]
   (https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) | [ðUpdate News]
 (https://mmocr.readthedocs.io/en/dev-1.x/notes/changelog.html) | [ð¤Reporting
         Issues](https://github.com/open-mmlab/mmocr/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## Latest Updates **The default branch has been switched to `1.x` from `main`,
-and we encourage users to migrate to the latest version, though it comes with
-some cost. Please refer to [Migration Guide](https://mmocr.readthedocs.io/en/
-dev-1.x/migration/overview.html) for more details.** v1.0.0rc6 was released in
-2023-03-07. 1. Two new models, ABCNet v2 (inference only) and SPTS are added to
-`projects/` folder. 2. Announcing `Inferencer`, a unified inference interface
-in OpenMMLab for everyone's easy access and quick inference with all the pre-
-trained weights. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/
-inference.html) 3. Users can use test-time augmentation for text recognition
-tasks. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/
-train_test.html#test-time-augmentation) 4. Support [batch augmentation](https:/
-/openaccess.thecvf.com/content_CVPR_2020/papers/
-Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf)
-through [`BatchAugSampler`](https://github.com/open-mmlab/mmocr/pull/1757),
-which is a technique used in SPTS. 5. Dataset Preparer has been refactored to
-allow more flexible configurations. Besides, users are now able to prepare text
-recognition datasets in LMDB formats. [Docs](https://mmocr.readthedocs.io/en/
-dev-1.x/user_guides/data_prepare/dataset_preparer.html#lmdb-format) 6. Some
-textspotting datasets have been revised to enhance the correctness and
-consistency with the common practice. 7. Potential spurious warnings from
-`shapely` have been eliminated. Read [Changelog](https://mmocr.readthedocs.io/
+## Latest Updates **The default branch is now `main` and the code on the branch
+has been upgraded to v1.0.0. The old `main` branch (v0.6.3) code now exists on
+the `0.x` branch.** If you have been using the `main` branch and encounter
+upgrade issues, please read the [Migration Guide](https://mmocr.readthedocs.io/
+en/dev-1.x/migration/overview.html) and notes on [Branches](https://
+mmocr.readthedocs.io/en/dev-1.x/migration/branches.html) . v1.0.0 was released
+in 2023-04-06. Major updates from 1.0.0rc6 include: 1. Support for SCUT-
+CTW1500, SynthText, and MJSynth datasets in Dataset Preparer 2. Updated FAQ and
+documentation 3. Deprecation of file_client_args in favor of backend_args 4.
+Added a new MMOCR tutorial notebook To know more about the updates in MMOCR
+1.0, please refer to [What's New in MMOCR 1.x](https://mmocr.readthedocs.io/en/
+dev-1.x/migration/news.html), or Read [Changelog](https://mmocr.readthedocs.io/
 en/dev-1.x/notes/changelog.html) for more details! ## Introduction MMOCR is an
 open-source toolbox based on PyTorch and mmdetection for text detection, text
 recognition, and the corresponding downstream tasks including key information
 extraction. It is part of the [OpenMMLab](https://openmmlab.com/) project. The
 main branch works with **PyTorch 1.6+**.
  [https://user-images.githubusercontent.com/24622904/187838618-1fdc61c0-2d46-
                           49f9-8502-976ffdf01f28.png]
@@ -60,126 +51,102 @@
 to [Overview](https://mmocr.readthedocs.io/en/dev-1.x/get_started/
 overview.html) for how to construct a customized model. - **Numerous
 Utilities** The toolbox provides a comprehensive set of utilities which can
 help users assess the performance of models. It includes visualizers which
 allow visualization of images, ground truths as well as predicted bounding
 boxes, and a validation tool for evaluating checkpoints during training. It
 also includes data converters to demonstrate how to convert your own data to
-the annotation files which the toolbox supports. ## What's New in MMOCR 1.0 1.
-**New engines**. MMOCR 1.x is based on [MMEngine](https://github.com/open-
-mmlab/mmengine), which provides a general and powerful runner that allows more
-flexible customizations and significantly simplifies the entrypoints of high-
-level interfaces. 2. **Unified interfaces**. As a part of the OpenMMLab 2.0
-projects, MMOCR 1.x unifies and refactors the interfaces and internal logics of
-train, testing, datasets, models, evaluation, and visualization. All the
-OpenMMLab 2.0 projects share the same design in those interfaces and logics to
-allow the emergence of multi-task/modality algorithms. 3. **Cross project
-calling**. Benefiting from the unified design, you can use the models
-implemented in other OpenMMLab projects, such as MMDet. We provide an example
-of how to use MMDetection's Mask R-CNN through `MMDetWrapper`. Check our
-documents for more details. More wrappers will be released in the future. 4.
-**Stronger visualization**. We provide a series of useful tools which are
-mostly based on brand-new visualizers. As a result, it is more convenient for
-the users to explore the models and datasets now. 5. **More documentation and
-tutorials**. We add a bunch of documentation and tutorials to help users get
-started more smoothly. Read it [here](https://mmocr.readthedocs.io/en/dev-1.x/
-). 6. **One-stop Dataset Preparaion**. Multiple datasets are instantly ready
-with only one line of command, via our [Dataset Preparer](https://
-mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/
-dataset_preparer.html). 7. **Embracing more `projects/`**: We now introduce
-`projects/` folder, where some experimental features, frameworks and models can
-be placed, only needed to satisfy the minimum requirement on the code quality.
-Everyone is welcome to post their implementation of any great ideas in this
-folder! Learn more from our [example project](https://github.com/open-mmlab/
-mmocr/blob/dev-1.x/projects/example_project/). 8. **More models**. MMOCR 1.0
-supports more tasks and more state-of-the-art models! ## Installation MMOCR
-depends on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-
-mmlab/mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection]
-(https://github.com/open-mmlab/mmdetection). Below are quick steps for
-installation. Please refer to [Install Guide](https://mmocr.readthedocs.io/en/
-dev-1.x/get_started/install.html) for more detailed instruction. ```shell conda
-create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -
-c pytorch -y conda activate open-mmlab pip3 install openmim mim install
-mmengine mim install 'mmcv>=2.0.0rc1' mim install 'mmdet>=3.0.0rc0' git clone
-https://github.com/open-mmlab/mmocr.git cd mmocr git checkout 1.x pip3 install
--e . ``` ## Get Started Please see [Quick Run](https://mmocr.readthedocs.io/en/
-dev-1.x/get_started/quick_run.html) for the basic usage of MMOCR. ## [Model
-Zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) Supported
-algorithms:  BackBone - [x] [oCLIP](configs/backbone/oclip/README.md)
-(ECCV'2022)   Text Detection - [x] [DBNet](configs/textdet/dbnet/README.md)
-(AAAI'2020) / [DBNet++](configs/textdet/dbnetpp/README.md) (TPAMI'2022) - [x]
-[Mask R-CNN](configs/textdet/maskrcnn/README.md) (ICCV'2017) - [x] [PANet]
-(configs/textdet/panet/README.md) (ICCV'2019) - [x] [PSENet](configs/textdet/
-psenet/README.md) (CVPR'2019) - [x] [TextSnake](configs/textdet/textsnake/
-README.md) (ECCV'2018) - [x] [DRRG](configs/textdet/drrg/README.md) (CVPR'2020)
-- [x] [FCENet](configs/textdet/fcenet/README.md) (CVPR'2021)   Text Recognition
-- [x] [ABINet](configs/textrecog/abinet/README.md) (CVPR'2021) - [x] [ASTER]
-(configs/textrecog/aster/README.md) (TPAMI'2018) - [x] [CRNN](configs/
-textrecog/crnn/README.md) (TPAMI'2016) - [x] [MASTER](configs/textrecog/master/
-README.md) (PR'2021) - [x] [NRTR](configs/textrecog/nrtr/README.md)
-(ICDAR'2019) - [x] [RobustScanner](configs/textrecog/robust_scanner/README.md)
-(ECCV'2020) - [x] [SAR](configs/textrecog/sar/README.md) (AAAI'2019) - [x]
-[SATRN](configs/textrecog/satrn/README.md) (CVPR'2020 Workshop on Text and
-Documents in the Deep Learning Era) - [x] [SVTR](configs/textrecog/svtr/
-README.md) (IJCAI'2022)   Key Information Extraction - [x] [SDMG-R](configs/
-kie/sdmgr/README.md) (ArXiv'2021)   Text Spotting - [x] [ABCNet](projects/
-ABCNet/README.md) (CVPR'2020) - [x] [ABCNetV2](projects/ABCNet/README_V2.md)
-(TPAMI'2021) - [x] [SPTS](projects/SPTS/README.md) (ACM MM'2022)  Please refer
-to [model_zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more
-details. ## Contributing We appreciate all contributions to improve MMOCR.
-Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
-guidelines. ## Acknowledgement MMOCR is an open-source project that is
-contributed by researchers and engineers from various colleges and companies.
-We appreciate all the contributors who implement their methods or add new
-features, as well as users who give valuable feedbacks. We hope the toolbox and
-benchmark could serve the growing research community by providing a flexible
-toolkit to reimplement existing methods and develop their own new OCR methods.
-## Citation If you find this project useful in your research, please consider
-cite: ```bibtex @article{mmocr2021, title={MMOCR: A Comprehensive Toolbox for
-Text Detection, Recognition and Understanding}, author={Kuang, Zhanghui and
-Sun, Hongbin and Li, Zhizhong and Yue, Xiaoyu and Lin, Tsui Hin and Chen,
-Jianyong and Wei, Huaqiang and Zhu, Yiqin and Gao, Tong and Zhang, Wenwei and
-Chen, Kai and Zhang, Wayne and Lin, Dahua}, journal= {arXiv preprint arXiv:
-2108.06543}, year={2021} } ``` ## License This project is released under the
-[Apache 2.0 license](LICENSE). ## Projects in OpenMMLab - [MMEngine](https://
-github.com/open-mmlab/mmengine): OpenMMLab foundational library for training
-deep learning models - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab
-foundational library for computer vision. - [MIM](https://github.com/open-
-mmlab/mim): MIM installs OpenMMLab packages. - [MMClassification](https://
-github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox
-and benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection):
-OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
-github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
-general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
-mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
-[MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab
-semantic segmentation toolbox and benchmark. - [MMOCR](https://github.com/open-
-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation
-toolbox and benchmark. - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d):
-OpenMMLab 3D human parametric model toolbox and benchmark. - [MMSelfSup](https:
-//github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox
-and benchmark. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab
-model compression toolbox and benchmark. - [MMFewShot](https://github.com/open-
-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark. -
-[MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-
-generation action understanding toolbox and benchmark. - [MMTracking](https://
-github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and
-benchmark. - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical
-flow toolbox and benchmark. - [MMEditing](https://github.com/open-mmlab/
-mmediting): OpenMMLab image and video editing toolbox. - [MMGeneration](https:/
-/github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative
-models toolbox. - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab
-model deployment framework. ## Welcome to the OpenMMLab community Scan the QR
-code below to follow the OpenMMLab team's [**Zhihu Official Account**](https://
-www.zhihu.com/people/openmmlab) and join the OpenMMLab team's [**QQ Group**]
-(https://jq.qq.com/?_wv=1027&k=aCvMxdr3), or join the official communication
-WeChat group by adding the WeChat, or join our [**Slack**](https://
-join.slack.com/t/mmocrworkspace/shared_invite/zt-1ifqhfla8-
-yKnLO_aKhVA2h71OrK8GZw)
+the annotation files which the toolbox supports. ## Installation MMOCR depends
+on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-mmlab/
+mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection](https:/
+/github.com/open-mmlab/mmdetection). Below are quick steps for installation.
+Please refer to [Install Guide](https://mmocr.readthedocs.io/en/dev-1.x/
+get_started/install.html) for more detailed instruction. ```shell conda create
+-n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -
+y conda activate open-mmlab pip3 install openmim git clone https://github.com/
+open-mmlab/mmocr.git cd mmocr mim install -e . ``` ## Get Started Please see
+[Quick Run](https://mmocr.readthedocs.io/en/dev-1.x/get_started/quick_run.html)
+for the basic usage of MMOCR. ## [Model Zoo](https://mmocr.readthedocs.io/en/
+dev-1.x/modelzoo.html) Supported algorithms:  BackBone - [x] [oCLIP](configs/
+backbone/oclip/README.md) (ECCV'2022)   Text Detection - [x] [DBNet](configs/
+textdet/dbnet/README.md) (AAAI'2020) / [DBNet++](configs/textdet/dbnetpp/
+README.md) (TPAMI'2022) - [x] [Mask R-CNN](configs/textdet/maskrcnn/README.md)
+(ICCV'2017) - [x] [PANet](configs/textdet/panet/README.md) (ICCV'2019) - [x]
+[PSENet](configs/textdet/psenet/README.md) (CVPR'2019) - [x] [TextSnake]
+(configs/textdet/textsnake/README.md) (ECCV'2018) - [x] [DRRG](configs/textdet/
+drrg/README.md) (CVPR'2020) - [x] [FCENet](configs/textdet/fcenet/README.md)
+(CVPR'2021)   Text Recognition - [x] [ABINet](configs/textrecog/abinet/
+README.md) (CVPR'2021) - [x] [ASTER](configs/textrecog/aster/README.md)
+(TPAMI'2018) - [x] [CRNN](configs/textrecog/crnn/README.md) (TPAMI'2016) - [x]
+[MASTER](configs/textrecog/master/README.md) (PR'2021) - [x] [NRTR](configs/
+textrecog/nrtr/README.md) (ICDAR'2019) - [x] [RobustScanner](configs/textrecog/
+robust_scanner/README.md) (ECCV'2020) - [x] [SAR](configs/textrecog/sar/
+README.md) (AAAI'2019) - [x] [SATRN](configs/textrecog/satrn/README.md)
+(CVPR'2020 Workshop on Text and Documents in the Deep Learning Era) - [x]
+[SVTR](configs/textrecog/svtr/README.md) (IJCAI'2022)   Key Information
+Extraction - [x] [SDMG-R](configs/kie/sdmgr/README.md) (ArXiv'2021)   Text
+Spotting - [x] [ABCNet](projects/ABCNet/README.md) (CVPR'2020) - [x] [ABCNetV2]
+(projects/ABCNet/README_V2.md) (TPAMI'2021) - [x] [SPTS](projects/SPTS/
+README.md) (ACM MM'2022)  Please refer to [model_zoo](https://
+mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more details. ## Projects
+[Here](projects/README.md) are some implementations of SOTA models and
+solutions built on MMOCR, which are supported and maintained by community
+users. These projects demonstrate the best practices based on MMOCR for
+research and product development. We welcome and appreciate all the
+contributions to OpenMMLab ecosystem. ## Contributing We appreciate all
+contributions to improve MMOCR. Please refer to [CONTRIBUTING.md](.github/
+CONTRIBUTING.md) for the contributing guidelines. ## Acknowledgement MMOCR is
+an open-source project that is contributed by researchers and engineers from
+various colleges and companies. We appreciate all the contributors who
+implement their methods or add new features, as well as users who give valuable
+feedbacks. We hope the toolbox and benchmark could serve the growing research
+community by providing a flexible toolkit to reimplement existing methods and
+develop their own new OCR methods. ## Citation If you find this project useful
+in your research, please consider cite: ```bibtex @article{mmocr2021, title=
+{MMOCR: A Comprehensive Toolbox for Text Detection, Recognition and
+Understanding}, author={Kuang, Zhanghui and Sun, Hongbin and Li, Zhizhong and
+Yue, Xiaoyu and Lin, Tsui Hin and Chen, Jianyong and Wei, Huaqiang and Zhu,
+Yiqin and Gao, Tong and Zhang, Wenwei and Chen, Kai and Zhang, Wayne and Lin,
+Dahua}, journal= {arXiv preprint arXiv:2108.06543}, year={2021} } ``` ##
+License This project is released under the [Apache 2.0 license](LICENSE). ##
+OpenMMLab Family - [MMEngine](https://github.com/open-mmlab/mmengine):
+OpenMMLab foundational library for training deep learning models - [MMCV]
+(https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for
+computer vision. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [MMClassification](https://github.com/open-mmlab/
+mmclassification): OpenMMLab image classification toolbox and benchmark. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMDetection3D](https://github.com/open-mmlab/
+mmdetection3d): OpenMMLab's next-generation platform for general 3D object
+detection. - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab
+rotated object detection toolbox and benchmark. - [MMSegmentation](https://
+github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox
+and benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text
+detection, recognition, and understanding toolbox. - [MMPose](https://
+github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human
+parametric model toolbox and benchmark. - [MMSelfSup](https://github.com/open-
+mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark. -
+[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
+toolbox and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
+OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
+github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
+understanding toolbox and benchmark. - [MMTracking](https://github.com/open-
+mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark. - [MMFlow]
+(https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and
+benchmark. - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab
+image and video editing toolbox. - [MMGeneration](https://github.com/open-
+mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. ## Welcome to the OpenMMLab community Scan the QR code below to
+follow the OpenMMLab team's [**Zhihu Official Account**](https://www.zhihu.com/
+people/openmmlab) and join the OpenMMLab team's [**QQ Group**](https://
+jq.qq.com/?_wv=1027&k=aCvMxdr3), or join the official communication WeChat
+group by adding the WeChat, or join our [**Slack**](https://join.slack.com/t/
+mmocrworkspace/shared_invite/zt-1ifqhfla8-yKnLO_aKhVA2h71OrK8GZw)
   [https://raw.githubusercontent.com/open-mmlab/mmcv/master/docs/en/_static/
  zhihu_qrcode.jpg] [https://raw.githubusercontent.com/open-mmlab/mmcv/master/
  docs/en/_static/qq_group_qrcode.jpg] [https://raw.githubusercontent.com/open-
              mmlab/mmcv/master/docs/en/_static/wechat_qrcode.jpg]
 We will provide you with the OpenMMLab community - ð¢ share the latest core
 technologies of AI frameworks - ð» Explaining PyTorch common module source
 Code - ð° News related to the release of OpenMMLab - ð Introduction of
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/datasets/wildreceipt-openset.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/datasets/wildreceipt-openset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/_base_/default_runtime.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_novisual.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_novisual.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_unet16.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/_base_sdmgr_unet16.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt-openset.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt-openset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/sdmgr_novisual_60e_wildreceipt.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/kie/sdmgr/sdmgr_unet16_60e_wildreceipt.py` & `mmocr-1.0.1/mmocr/.mim/configs/kie/sdmgr/sdmgr_unet16_60e_wildreceipt.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/datasets/icdar2017.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/datasets/icdar2017.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/default_runtime.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_base.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/_base_/schedules/schedule_sgd_base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet18_fpnc.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/_base_dbnetpp_resnet50-dcnv2_fpnc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-file_client_args = dict(backend='disk')
-
 model = dict(
     type='DBNet',
     backbone=dict(
         type='mmdet.ResNet',
-        depth=18,
+        depth=50,
         num_stages=4,
         out_indices=(0, 1, 2, 3),
         frozen_stages=-1,
         norm_cfg=dict(type='BN', requires_grad=True),
-        init_cfg=dict(type='Pretrained', checkpoint='torchvision://resnet18'),
         norm_eval=False,
-        style='caffe'),
+        style='pytorch',
+        dcn=dict(type='DCNv2', deform_groups=1, fallback_on_stride=False),
+        init_cfg=dict(type='Pretrained', checkpoint='torchvision://resnet50'),
+        stage_with_dcn=(False, True, True, True)),
     neck=dict(
-        type='FPNC', in_channels=[64, 128, 256, 512], lateral_channels=256),
+        type='FPNC',
+        in_channels=[256, 512, 1024, 2048],
+        lateral_channels=256,
+        asf_cfg=dict(attention_type='ScaleChannelSpatial')),
     det_head=dict(
         type='DBHead',
         in_channels=256,
         module_loss=dict(type='DBModuleLoss'),
-        postprocessor=dict(type='DBPostprocessor', text_repr_type='quad')),
+        postprocessor=dict(
+            type='DBPostprocessor', text_repr_type='quad',
+            epsilon_ratio=0.002)),
     data_preprocessor=dict(
         type='TextDetDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375],
         bgr_to_rgb=True,
         pad_size_divisor=32))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
-        with_polygon=True,
         with_bbox=True,
+        with_polygon=True,
         with_label=True,
     ),
     dict(
         type='TorchVisionWrapper',
         op='ColorJitter',
         brightness=32.0 / 255,
         saturation=0.5),
@@ -51,22 +53,20 @@
     dict(type='Pad', size=(640, 640)),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
-    dict(type='Resize', scale=(1333, 736), keep_ratio=True),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
+    dict(type='Resize', scale=(4068, 1024), keep_ratio=True),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(
         type='PackTextDetInputs',
-        meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
+        meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor',
+                   'instances'))
 ]
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet50-dcnv2_fpnc.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/_base_textsnake_resnet50_fpn-unet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,82 @@
-file_client_args = dict(backend='disk')
-
 model = dict(
-    type='DBNet',
+    type='TextSnake',
     backbone=dict(
         type='mmdet.ResNet',
         depth=50,
         num_stages=4,
         out_indices=(0, 1, 2, 3),
         frozen_stages=-1,
         norm_cfg=dict(type='BN', requires_grad=True),
-        norm_eval=False,
-        style='pytorch',
-        dcn=dict(type='DCNv2', deform_groups=1, fallback_on_stride=False),
         init_cfg=dict(type='Pretrained', checkpoint='torchvision://resnet50'),
-        stage_with_dcn=(False, True, True, True)),
+        norm_eval=True,
+        style='caffe'),
     neck=dict(
-        type='FPNC', in_channels=[256, 512, 1024, 2048], lateral_channels=256),
+        type='FPN_UNet', in_channels=[256, 512, 1024, 2048], out_channels=32),
     det_head=dict(
-        type='DBHead',
-        in_channels=256,
-        module_loss=dict(type='DBModuleLoss'),
-        postprocessor=dict(type='DBPostprocessor', text_repr_type='quad')),
+        type='TextSnakeHead',
+        in_channels=32,
+        module_loss=dict(type='TextSnakeModuleLoss'),
+        postprocessor=dict(
+            type='TextSnakePostprocessor', text_repr_type='poly')),
     data_preprocessor=dict(
         type='TextDetDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375],
         bgr_to_rgb=True,
         pad_size_divisor=32))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_bbox=True,
         with_polygon=True,
-        with_label=True,
-    ),
+        with_label=True),
     dict(
         type='TorchVisionWrapper',
         op='ColorJitter',
         brightness=32.0 / 255,
         saturation=0.5),
     dict(
-        type='ImgAugWrapper',
-        args=[['Fliplr', 0.5],
-              dict(cls='Affine', rotate=[-10, 10]), ['Resize', [0.5, 3.0]]]),
-    dict(type='RandomCrop', min_side_ratio=0.1),
-    dict(type='Resize', scale=(640, 640), keep_ratio=True),
-    dict(type='Pad', size=(640, 640)),
+        type='RandomApply',
+        transforms=[dict(type='RandomCrop', min_side_ratio=0.3)],
+        prob=0.65),
+    dict(
+        type='RandomRotate',
+        max_angle=20,
+        pad_with_fixed_color=False,
+        use_canvas=True),
+    dict(
+        type='BoundedScaleAspectJitter',
+        long_size_bound=800,
+        short_size_bound=480,
+        ratio_range=(0.7, 1.3),
+        aspect_ratio_range=(0.9, 1.1)),
+    dict(
+        type='RandomChoice',
+        transforms=[[
+            dict(type='Resize', scale=800, keep_ratio=True),
+            dict(type='SourceImagePad', target_scale=800)
+        ],
+                    dict(type='Resize', scale=800, keep_ratio=False)],
+        prob=[0.4, 0.6]),
+    dict(type='RandomFlip', prob=0.5, direction='horizontal'),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
-    dict(type='Resize', scale=(4068, 1024), keep_ratio=True),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
+    dict(type='Resize', scale=(1333, 736), keep_ratio=True),
+    # add loading annotation after ``Resize`` because ground truth
+    # does not need to do resize data transform
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
-        with_label=True,
-    ),
+        with_label=True),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_100k_synthtext.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_100k_synthtext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 _base_ = [
     '_base_dbnet_resnet18_fpnc.py',
     '../_base_/datasets/synthtext.py',
     '../_base_/pretrain_runtime.py',
     '../_base_/schedules/schedule_sgd_100k.py',
 ]
 
-file_client_args = dict(backend='disk')
-
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(type='FixInvalidPolygon'),
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_totaltext.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet18_fpnc_1200e_totaltext.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 _base_ = [
     '_base_dbnet_resnet18_fpnc.py',
     '../_base_/datasets/totaltext.py',
     '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_sgd_1200e.py',
 ]
 
-file_client_args = dict(backend='disk')
-
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(type='FixInvalidPolygon', min_poly_points=4),
@@ -33,18 +28,15 @@
     dict(type='Pad', size=(640, 640)),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(type='Resize', scale=(1333, 736), keep_ratio=True),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_100k_synthtext.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_100k_synthtext.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-dcnv2_fpnc_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-oclip_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50-oclip_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/dbnet_resnet50_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnet/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/_base_dbnetpp_resnet50-dcnv2_fpnc.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnet/_base_dbnet_resnet50-dcnv2_fpnc.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,20 @@
         norm_cfg=dict(type='BN', requires_grad=True),
         norm_eval=False,
         style='pytorch',
         dcn=dict(type='DCNv2', deform_groups=1, fallback_on_stride=False),
         init_cfg=dict(type='Pretrained', checkpoint='torchvision://resnet50'),
         stage_with_dcn=(False, True, True, True)),
     neck=dict(
-        type='FPNC',
-        in_channels=[256, 512, 1024, 2048],
-        lateral_channels=256,
-        asf_cfg=dict(attention_type='ScaleChannelSpatial')),
+        type='FPNC', in_channels=[256, 512, 1024, 2048], lateral_channels=256),
     det_head=dict(
         type='DBHead',
         in_channels=256,
         module_loss=dict(type='DBModuleLoss'),
-        postprocessor=dict(
-            type='DBPostprocessor', text_repr_type='quad',
-            epsilon_ratio=0.002)),
+        postprocessor=dict(type='DBPostprocessor', text_repr_type='quad')),
     data_preprocessor=dict(
         type='TextDetDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375],
         bgr_to_rgb=True,
         pad_size_divisor=32))
 
@@ -63,10 +58,9 @@
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(
         type='PackTextDetInputs',
-        meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor',
-                   'instances'))
+        meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_100k_synthtext.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_100k_synthtext.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-dcnv2_fpnc_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-oclip_fpnc_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50-oclip_fpnc_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50_fpnc_1200e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/dbnetpp_resnet50_fpnc_1200e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/dbnetpp/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/dbnetpp/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/_base_drrg_resnet50_fpn-unet.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/_base_drrg_resnet50_fpn-unet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-file_client_args = dict(backend='disk')
-
 model = dict(
     type='DRRG',
     backbone=dict(
         type='mmdet.ResNet',
         depth=50,
         num_stages=4,
         out_indices=(0, 1, 2, 3),
@@ -25,18 +23,15 @@
         type='TextDetDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375],
         bgr_to_rgb=True,
         pad_size_divisor=32))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_bbox=True,
         with_polygon=True,
         with_label=True),
     dict(
         type='TorchVisionWrapper',
@@ -78,18 +73,15 @@
     dict(type='RandomFlip', prob=0.5, direction='horizontal'),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(type='Resize', scale=(1024, 640), keep_ratio=True),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/drrg_resnet50_fpn-unet_1200e_ctw1500.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/drrg_resnet50_fpn-unet_1200e_ctw1500.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/drrg/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/drrg/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50-dcnv2_fpn.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50-dcnv2_fpn.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50_fpn.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/_base_fcenet_resnet50_fpn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-file_client_args = dict(backend='disk')
-
 model = dict(
     type='FCENet',
     backbone=dict(
         type='mmdet.ResNet',
         depth=50,
         num_stages=4,
         out_indices=(1, 2, 3),
@@ -37,18 +35,15 @@
         type='TextDetDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375],
         bgr_to_rgb=True,
         pad_size_divisor=32))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(
@@ -92,18 +87,15 @@
         contrast=0.5),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(type='Resize', scale=(2260, 2260), keep_ratio=True),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-dcnv2_fpn_1500e_ctw1500.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50-dcnv2_fpn_1500e_ctw1500.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 optim_wrapper = dict(optimizer=dict(lr=1e-3, weight_decay=5e-4))
 train_cfg = dict(max_epochs=1500)
 # learning policy
 param_scheduler = [
     dict(type='PolyLR', power=0.9, eta_min=1e-7, end=1500),
 ]
 
-file_client_args = dict(backend='disk')
 # dataset settings
 ctw1500_textdet_train = _base_.ctw1500_textdet_train
 ctw1500_textdet_test = _base_.ctw1500_textdet_test
 
 # test pipeline for CTW1500
 ctw_test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(type='Resize', scale=(1080, 736), keep_ratio=True),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_totaltext.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/fcenet_resnet50_fpn_1500e_totaltext.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/fcenet/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/fcenet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/_base_mask-rcnn_resnet50_fpn.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/_base_mask-rcnn_resnet50_fpn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 _base_ = ['mmdet::_base_/models/mask-rcnn_r50_fpn.py']
 
-file_client_args = dict(backend='disk')
-
 mask_rcnn = _base_.pop('model')
 # Adapt Mask R-CNN model to OCR task
 mask_rcnn.update(
     dict(
         data_preprocessor=dict(pad_mask=False),
         rpn_head=dict(
             anchor_generator=dict(
@@ -14,18 +12,15 @@
             bbox_head=dict(num_classes=1),
             mask_head=dict(num_classes=1),
         )))
 
 model = dict(type='MMDetWrapper', text_repr_type='poly', cfg=mask_rcnn)
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(
@@ -45,18 +40,15 @@
     dict(
         type='mmdet.PackDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'flip',
                    'scale_factor', 'flip_direction'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(type='Resize', scale=(1920, 1920), keep_ratio=True),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True),
     dict(
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_ctw1500.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_ctw1500.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 
 # dataset settings
 ctw1500_textdet_train = _base_.ctw1500_textdet_train
 ctw1500_textdet_test = _base_.ctw1500_textdet_test
 
 # test pipeline for CTW1500
 ctw_test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=dict(backend='disk'),
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(type='Resize', scale=(1600, 1600), keep_ratio=True),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/mask-rcnn_resnet50_fpn_160e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/maskrcnn/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/maskrcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/_base_panet_resnet18_fpem-ffm.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/_base_panet_resnet18_fpem-ffm.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,16 @@
         module_loss=dict(
             type='PANModuleLoss',
             loss_text=dict(type='MaskedSquareDiceLoss'),
             loss_kernel=dict(type='MaskedSquareDiceLoss'),
         ),
         postprocessor=dict(type='PANPostprocessor', text_repr_type='quad')))
 
-file_client_args = dict(backend='disk')
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(type='ShortScaleAspectJitter', short_size=736, scale_divisor=32),
@@ -56,18 +52,15 @@
         saturation=0.5),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     # TODO Replace with mmcv.RescaleToShort when it's ready
     dict(
         type='ShortScaleAspectJitter',
         short_size=736,
         scale_divisor=1,
         ratio_range=(1.0, 1.0),
         aspect_ratio_range=(1.0, 1.0)),
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/_base_panet_resnet50_fpem-ffm.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/_base_panet_resnet50_fpem-ffm.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_ctw1500.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_ctw1500.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,16 @@
     '_base_panet_resnet18_fpem-ffm.py',
 ]
 
 model = dict(det_head=dict(module_loss=dict(shrink_ratio=(1, 0.7))))
 
 default_hooks = dict(checkpoint=dict(type='CheckpointHook', interval=20), )
 
-file_client_args = dict(backend='disk')
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True,
     ),
     dict(type='ShortScaleAspectJitter', short_size=640, scale_divisor=32),
@@ -33,18 +29,15 @@
         saturation=0.5),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     # TODO Replace with mmcv.RescaleToShort when it's ready
     dict(
         type='ShortScaleAspectJitter',
         short_size=640,
         scale_divisor=1,
         ratio_range=(1.0, 1.0),
         aspect_ratio_range=(1.0, 1.0)),
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/panet/panet_resnet18_fpem-ffm_600e_icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/panet/panet_resnet50_fpem-ffm_600e_icdar2017.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/_base_psenet_resnet50_fpnf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,66 @@
-_base_ = [
-    '../_base_/datasets/icdar2017.py',
-    '../_base_/default_runtime.py',
-    '../_base_/schedules/schedule_adam_600e.py',
-    '_base_panet_resnet50_fpem-ffm.py',
-]
-
-default_hooks = dict(checkpoint=dict(type='CheckpointHook', interval=20), )
+model = dict(
+    type='PSENet',
+    backbone=dict(
+        type='mmdet.ResNet',
+        depth=50,
+        num_stages=4,
+        out_indices=(0, 1, 2, 3),
+        frozen_stages=-1,
+        norm_cfg=dict(type='SyncBN', requires_grad=True),
+        init_cfg=dict(type='Pretrained', checkpoint='torchvision://resnet50'),
+        norm_eval=True,
+        style='caffe'),
+    neck=dict(
+        type='FPNF',
+        in_channels=[256, 512, 1024, 2048],
+        out_channels=256,
+        fusion_type='concat'),
+    det_head=dict(
+        type='PSEHead',
+        in_channels=[256],
+        hidden_dim=256,
+        out_channel=7,
+        module_loss=dict(type='PSEModuleLoss'),
+        postprocessor=dict(type='PSEPostprocessor', text_repr_type='poly')),
+    data_preprocessor=dict(
+        type='TextDetDataPreprocessor',
+        mean=[123.675, 116.28, 103.53],
+        std=[58.395, 57.12, 57.375],
+        bgr_to_rgb=True,
+        pad_size_divisor=32))
 
-file_client_args = dict(backend='disk')
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
-        with_label=True,
-    ),
-    dict(type='ShortScaleAspectJitter', short_size=800, scale_divisor=32),
-    dict(type='RandomFlip', prob=0.5, direction='horizontal'),
-    dict(type='RandomRotate', max_angle=10),
-    dict(type='TextDetRandomCrop', target_size=(800, 800)),
-    dict(type='Pad', size=(800, 800)),
+        with_label=True),
     dict(
         type='TorchVisionWrapper',
         op='ColorJitter',
         brightness=32.0 / 255,
         saturation=0.5),
+    dict(type='FixInvalidPolygon'),
+    dict(type='ShortScaleAspectJitter', short_size=736, scale_divisor=32),
+    dict(type='RandomFlip', prob=0.5, direction='horizontal'),
+    dict(type='RandomRotate', max_angle=10),
+    dict(type='TextDetRandomCrop', target_size=(736, 736)),
+    dict(type='Pad', size=(736, 736)),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
-    # TODO Replace with mmcv.RescaleToShort when it's ready
-    dict(
-        type='ShortScaleAspectJitter',
-        short_size=800,
-        scale_divisor=1,
-        ratio_range=(1.0, 1.0),
-        aspect_ratio_range=(1.0, 1.0)),
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
+    dict(type='Resize', scale=(2240, 2240), keep_ratio=True),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
-icdar2017_textdet_train = _base_.icdar2017_textdet_train
-icdar2017_textdet_test = _base_.icdar2017_textdet_test
-# pipeline settings
-icdar2017_textdet_train.pipeline = train_pipeline
-icdar2017_textdet_test.pipeline = test_pipeline
-train_dataloader = dict(
-    batch_size=64,
-    num_workers=8,
-    persistent_workers=True,
-    sampler=dict(type='DefaultSampler', shuffle=True),
-    dataset=icdar2017_textdet_train)
-val_dataloader = dict(
-    batch_size=1,
-    num_workers=4,
-    persistent_workers=True,
-    sampler=dict(type='DefaultSampler', shuffle=False),
-    dataset=icdar2017_textdet_test)
-test_dataloader = val_dataloader
-
-val_evaluator = dict(
-    type='HmeanIOUMetric', pred_score_thrs=dict(start=0.3, stop=1, step=0.05))
-test_evaluator = val_evaluator
-
-auto_scale_lr = dict(base_batch_size=64)
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/_base_psenet_resnet50_fpnf.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_ctw1500.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,52 @@
-file_client_args = dict(backend='disk')
-
-model = dict(
-    type='PSENet',
-    backbone=dict(
-        type='mmdet.ResNet',
-        depth=50,
-        num_stages=4,
-        out_indices=(0, 1, 2, 3),
-        frozen_stages=-1,
-        norm_cfg=dict(type='SyncBN', requires_grad=True),
-        init_cfg=dict(type='Pretrained', checkpoint='torchvision://resnet50'),
-        norm_eval=True,
-        style='caffe'),
-    neck=dict(
-        type='FPNF',
-        in_channels=[256, 512, 1024, 2048],
-        out_channels=256,
-        fusion_type='concat'),
-    det_head=dict(
-        type='PSEHead',
-        in_channels=[256],
-        hidden_dim=256,
-        out_channel=7,
-        module_loss=dict(type='PSEModuleLoss'),
-        postprocessor=dict(type='PSEPostprocessor', text_repr_type='poly')),
-    data_preprocessor=dict(
-        type='TextDetDataPreprocessor',
-        mean=[123.675, 116.28, 103.53],
-        std=[58.395, 57.12, 57.375],
-        bgr_to_rgb=True,
-        pad_size_divisor=32))
+_base_ = [
+    '_base_psenet_resnet50_fpnf.py',
+    '../_base_/datasets/ctw1500.py',
+    '../_base_/default_runtime.py',
+    '../_base_/schedules/schedule_adam_600e.py',
+]
 
-train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
-    dict(
-        type='LoadOCRAnnotations',
-        with_polygon=True,
-        with_bbox=True,
-        with_label=True),
-    dict(
-        type='TorchVisionWrapper',
-        op='ColorJitter',
-        brightness=32.0 / 255,
-        saturation=0.5),
-    dict(type='FixInvalidPolygon'),
-    dict(type='ShortScaleAspectJitter', short_size=736, scale_divisor=32),
-    dict(type='RandomFlip', prob=0.5, direction='horizontal'),
-    dict(type='RandomRotate', max_angle=10),
-    dict(type='TextDetRandomCrop', target_size=(736, 736)),
-    dict(type='Pad', size=(736, 736)),
-    dict(
-        type='PackTextDetInputs',
-        meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
+# optimizer
+optim_wrapper = dict(optimizer=dict(lr=1e-4))
+train_cfg = dict(val_interval=40)
+param_scheduler = [
+    dict(type='MultiStepLR', milestones=[200, 400], end=600),
 ]
 
-test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        color_type='color_ignore_orientation'),
-    dict(type='Resize', scale=(2240, 2240), keep_ratio=True),
+# dataset settings
+ctw1500_textdet_train = _base_.ctw1500_textdet_train
+ctw1500_textdet_test = _base_.ctw1500_textdet_test
+
+test_pipeline_ctw = [
+    dict(type='LoadImageFromFile', color_type='color_ignore_orientation'),
+    dict(type='Resize', scale=(1280, 1280), keep_ratio=True),
     dict(
         type='LoadOCRAnnotations',
         with_polygon=True,
         with_bbox=True,
         with_label=True),
     dict(
         type='PackTextDetInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
 ]
+
+# pipeline settings
+ctw1500_textdet_train.pipeline = _base_.train_pipeline
+ctw1500_textdet_test.pipeline = test_pipeline_ctw
+
+train_dataloader = dict(
+    batch_size=16,
+    num_workers=8,
+    persistent_workers=False,
+    sampler=dict(type='DefaultSampler', shuffle=True),
+    dataset=ctw1500_textdet_train)
+
+val_dataloader = dict(
+    batch_size=1,
+    num_workers=1,
+    persistent_workers=False,
+    sampler=dict(type='DefaultSampler', shuffle=False),
+    dataset=ctw1500_textdet_test)
+
+test_dataloader = val_dataloader
+
+auto_scale_lr = dict(base_batch_size=64 * 4)
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/metafile.yml`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     Metadata:
       Training Data: ICDAR2015
     Results:
       - Task: Text Detection
         Dataset: ICDAR2015
         Metrics:
           hmean-iou: 0.7998
-    Weights:
+    Weights: https://download.openmmlab.com/mmocr/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2015/psenet_resnet50_fpnf_600e_icdar2015_20220825_222709-b6741ec3.pth
 
   - Name: psenet_resnet50-oclip_fpnf_600e_icdar2015
     Alias: PSENet
     In Collection: PSENet
     Config: configs/textdet/psenet/psenet_resnet50-oclip_fpnf_600e_icdar2015.py
     Metadata:
       Training Data: ICDAR2015
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_ctw1500.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2015.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 _base_ = [
     '_base_psenet_resnet50_fpnf.py',
-    '../_base_/datasets/ctw1500.py',
+    '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_adam_600e.py',
 ]
 
 # optimizer
 optim_wrapper = dict(optimizer=dict(lr=1e-4))
 train_cfg = dict(val_interval=40)
 param_scheduler = [
     dict(type='MultiStepLR', milestones=[200, 400], end=600),
 ]
 
 # dataset settings
-ctw1500_textdet_train = _base_.ctw1500_textdet_train
-ctw1500_textdet_test = _base_.ctw1500_textdet_test
+icdar2015_textdet_train = _base_.icdar2015_textdet_train
+icdar2015_textdet_test = _base_.icdar2015_textdet_test
 
-test_pipeline_ctw = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=_base_.file_client_args,
-        color_type='color_ignore_orientation'),
-    dict(type='Resize', scale=(1280, 1280), keep_ratio=True),
-    dict(
-        type='LoadOCRAnnotations',
-        with_polygon=True,
-        with_bbox=True,
-        with_label=True),
-    dict(
-        type='PackTextDetInputs',
-        meta_keys=('img_path', 'ori_shape', 'img_shape', 'scale_factor'))
-]
+# use quadrilaterals for icdar2015
+model = dict(
+    backbone=dict(style='pytorch'),
+    det_head=dict(postprocessor=dict(text_repr_type='quad')))
 
 # pipeline settings
-ctw1500_textdet_train.pipeline = _base_.train_pipeline
-ctw1500_textdet_test.pipeline = test_pipeline_ctw
+icdar2015_textdet_train.pipeline = _base_.train_pipeline
+icdar2015_textdet_test.pipeline = _base_.test_pipeline
 
 train_dataloader = dict(
     batch_size=16,
     num_workers=8,
     persistent_workers=False,
     sampler=dict(type='DefaultSampler', shuffle=True),
-    dataset=ctw1500_textdet_train)
+    dataset=icdar2015_textdet_train)
 
 val_dataloader = dict(
     batch_size=1,
     num_workers=1,
     persistent_workers=False,
     sampler=dict(type='DefaultSampler', shuffle=False),
-    dataset=ctw1500_textdet_test)
+    dataset=icdar2015_textdet_test)
 
 test_dataloader = val_dataloader
 
 auto_scale_lr = dict(base_batch_size=64 * 4)
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_resnet31-1by16-1by8_6e_st_mj.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 _base_ = [
-    '_base_psenet_resnet50_fpnf.py',
+    '../_base_/datasets/mjsynth.py',
+    '../_base_/datasets/synthtext.py',
+    '../_base_/datasets/cute80.py',
+    '../_base_/datasets/iiit5k.py',
+    '../_base_/datasets/svt.py',
+    '../_base_/datasets/svtp.py',
+    '../_base_/datasets/icdar2013.py',
     '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
-    '../_base_/schedules/schedule_adam_600e.py',
+    '../_base_/schedules/schedule_adam_base.py',
+    '_base_nrtr_resnet31.py',
 ]
 
-# optimizer
-optim_wrapper = dict(optimizer=dict(lr=1e-4))
-train_cfg = dict(val_interval=40)
+# optimizer settings
+train_cfg = dict(max_epochs=6)
+# learning policy
 param_scheduler = [
-    dict(type='MultiStepLR', milestones=[200, 400], end=600),
+    dict(type='MultiStepLR', milestones=[3, 4], end=6),
 ]
 
 # dataset settings
-icdar2015_textdet_train = _base_.icdar2015_textdet_train
-icdar2015_textdet_test = _base_.icdar2015_textdet_test
+train_list = [_base_.mjsynth_textrecog_train, _base_.synthtext_textrecog_train]
+test_list = [
+    _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
+    _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
+    _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
+]
 
-# use quadrilaterals for icdar2015
-model = dict(
-    backbone=dict(style='pytorch'),
-    det_head=dict(postprocessor=dict(text_repr_type='quad')))
-
-# pipeline settings
-icdar2015_textdet_train.pipeline = _base_.train_pipeline
-icdar2015_textdet_test.pipeline = _base_.test_pipeline
+train_dataset = dict(
+    type='ConcatDataset', datasets=train_list, pipeline=_base_.train_pipeline)
+test_dataset = dict(
+    type='ConcatDataset', datasets=test_list, pipeline=_base_.test_pipeline)
 
 train_dataloader = dict(
-    batch_size=16,
-    num_workers=8,
-    persistent_workers=False,
+    batch_size=384,
+    num_workers=24,
+    persistent_workers=True,
     sampler=dict(type='DefaultSampler', shuffle=True),
-    dataset=icdar2015_textdet_train)
+    dataset=train_dataset)
 
-val_dataloader = dict(
+test_dataloader = dict(
     batch_size=1,
-    num_workers=1,
-    persistent_workers=False,
+    num_workers=4,
+    persistent_workers=True,
+    drop_last=False,
     sampler=dict(type='DefaultSampler', shuffle=False),
-    dataset=icdar2015_textdet_test)
+    dataset=test_dataset)
+
+val_dataloader = test_dataloader
 
-test_dataloader = val_dataloader
+val_evaluator = dict(
+    dataset_prefixes=['CUTE80', 'IIIT5K', 'SVT', 'SVTP', 'IC13', 'IC15'])
+test_evaluator = val_evaluator
 
-auto_scale_lr = dict(base_batch_size=64 * 4)
+auto_scale_lr = dict(base_batch_size=384)
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2017.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/psenet/psenet_resnet50_fpnf_600e_icdar2017.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textdet/textsnake/textsnake_resnet50_fpn-unet_1200e_ctw1500.py` & `mmocr-1.0.1/mmocr/.mim/configs/textdet/textsnake/textsnake_resnet50_fpn-unet_1200e_ctw1500.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2013.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2013.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2015.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/datasets/icdar2015.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/default_runtime.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adam_base.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/_base_/schedules/schedule_adam_base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/_base_abinet-vision.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/_base_abinet-vision.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,22 +35,16 @@
         max_seq_len=26,
     ),
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375]))
 
-file_client_args = dict(backend='disk')
-
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(type='Resize', scale=(128, 32)),
     dict(
         type='RandomApply',
         prob=0.5,
         transforms=[
             dict(
@@ -82,15 +76,15 @@
         prob=0.25,
         transforms=[
             dict(type='PyramidRescale'),
             dict(
                 type='mmdet.Albu',
                 transforms=[
                     dict(type='GaussNoise', var_limit=(20, 20), p=0.5),
-                    dict(type='MotionBlur', blur_limit=6, p=0.5),
+                    dict(type='MotionBlur', blur_limit=7, p=0.5),
                 ]),
         ]),
     dict(
         type='RandomApply',
         prob=0.25,
         transforms=[
             dict(
@@ -103,26 +97,26 @@
         ]),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(type='Resize', scale=(128, 32)),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/abinet-vision_20e_st-an_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/abinet_20e_st-an_mj.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,44 +5,46 @@
     '../_base_/datasets/iiit5k.py',
     '../_base_/datasets/svt.py',
     '../_base_/datasets/svtp.py',
     '../_base_/datasets/icdar2013.py',
     '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_adam_base.py',
-    '_base_abinet-vision.py',
+    '_base_abinet.py',
 ]
 
+load_from = 'https://download.openmmlab.com/mmocr/textrecog/abinet/abinet_pretrain-45deac15.pth'  # noqa
+
 optim_wrapper = dict(optimizer=dict(lr=1e-4))
 train_cfg = dict(max_epochs=20)
 # learning policy
 param_scheduler = [
     dict(
         type='LinearLR', end=2, start_factor=0.001,
         convert_to_iter_based=True),
     dict(type='MultiStepLR', milestones=[16, 18], end=20),
 ]
 
 # dataset settings
 train_list = [
-    _base_.mjsynth_textrecog_test, _base_.synthtext_an_textrecog_train
+    _base_.mjsynth_textrecog_train, _base_.synthtext_an_textrecog_train
 ]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
 
 train_dataset = dict(
     type='ConcatDataset', datasets=train_list, pipeline=_base_.train_pipeline)
 test_dataset = dict(
     type='ConcatDataset', datasets=test_list, pipeline=_base_.test_pipeline)
 
 train_dataloader = dict(
-    batch_size=192 * 4,
+    batch_size=192,
     num_workers=32,
     persistent_workers=True,
     sampler=dict(type='DefaultSampler', shuffle=True),
     dataset=train_dataset)
 
 test_dataloader = dict(
     batch_size=1,
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/abinet_20e_st-an_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/abinet-vision_20e_st-an_mj.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,46 +5,44 @@
     '../_base_/datasets/iiit5k.py',
     '../_base_/datasets/svt.py',
     '../_base_/datasets/svtp.py',
     '../_base_/datasets/icdar2013.py',
     '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_adam_base.py',
-    '_base_abinet.py',
+    '_base_abinet-vision.py',
 ]
 
-load_from = 'https://download.openmmlab.com/mmocr/textrecog/abinet/abinet_pretrain-45deac15.pth'  # noqa
-
 optim_wrapper = dict(optimizer=dict(lr=1e-4))
 train_cfg = dict(max_epochs=20)
 # learning policy
 param_scheduler = [
     dict(
         type='LinearLR', end=2, start_factor=0.001,
         convert_to_iter_based=True),
     dict(type='MultiStepLR', milestones=[16, 18], end=20),
 ]
 
 # dataset settings
 train_list = [
-    _base_.mjsynth_textrecog_test, _base_.synthtext_an_textrecog_train
+    _base_.mjsynth_textrecog_train, _base_.synthtext_an_textrecog_train
 ]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
 
 train_dataset = dict(
     type='ConcatDataset', datasets=train_list, pipeline=_base_.train_pipeline)
 test_dataset = dict(
     type='ConcatDataset', datasets=test_list, pipeline=_base_.test_pipeline)
 
 train_dataloader = dict(
-    batch_size=192,
+    batch_size=192 * 4,
     num_workers=32,
     persistent_workers=True,
     sampler=dict(type='DefaultSampler', shuffle=True),
     dataset=train_dataset)
 
 test_dataloader = dict(
     batch_size=1,
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/abinet/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/abinet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/_base_aster.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/_base_aster.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-file_client_args = dict(backend='disk')
-
 dictionary = dict(
     type='Dictionary',
     dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
     with_padding=True,
     with_unknown=True,
     same_start_end=True,
     with_start=True,
@@ -44,38 +42,34 @@
     ),
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor',
         mean=[127.5, 127.5, 127.5],
         std=[127.5, 127.5, 127.5]))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=5),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=5),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(type='Resize', scale=(256, 64)),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(type='Resize', scale=(256, 64)),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio',
                    'instances'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[[
             dict(
                 type='ConditionApply',
                 true_transforms=[
                     dict(
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/aster_resnet45_6e_st_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/aster_resnet45_6e_st_mj.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_adamw_cos_6e.py',
 ]
 
 # dataset settings
 train_list = [
-    _base_.mjsynth_textrecog_test,
+    _base_.mjsynth_textrecog_train,
     _base_.synthtext_textrecog_train,
 ]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/aster/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/aster/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/_base_crnn_mini-vgg.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_modality-transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 dictionary = dict(
     type='Dictionary',
-    dict_file='{{ fileDirname }}/../../../dicts/lower_english_digits.txt',
-    with_padding=True)
+    dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
+    with_padding=True,
+    with_unknown=True,
+    same_start_end=True,
+    with_start=True,
+    with_end=True)
 
 model = dict(
-    type='CRNN',
-    preprocessor=None,
-    backbone=dict(type='MiniVGG', leaky_relu=False, input_channels=1),
-    encoder=None,
+    type='NRTR',
+    backbone=dict(type='NRTRModalityTransform'),
+    encoder=dict(type='NRTREncoder', n_layers=12),
     decoder=dict(
-        type='CRNNDecoder',
-        in_channels=512,
-        rnn_flag=True,
-        module_loss=dict(type='CTCModuleLoss', letter_case='lower'),
-        postprocessor=dict(type='CTCPostProcessor'),
-        dictionary=dictionary),
+        type='NRTRDecoder',
+        module_loss=dict(
+            type='CEModuleLoss', ignore_first_char=True, flatten=True),
+        postprocessor=dict(type='AttentionPostprocessor'),
+        dictionary=dictionary,
+        max_seq_len=30),
     data_preprocessor=dict(
-        type='TextRecogDataPreprocessor', mean=[127], std=[127]))
+        type='TextRecogDataPreprocessor',
+        mean=[123.675, 116.28, 103.53],
+        std=[58.395, 57.12, 57.375]))
 
-file_client_args = dict(backend='disk')
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        color_type='grayscale',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
-    dict(type='Resize', scale=(100, 32), keep_ratio=False),
+    dict(
+        type='RescaleToHeight',
+        height=32,
+        min_width=32,
+        max_width=160,
+        width_divisor=4),
+    dict(type='PadToWidth', width=160),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        color_type='grayscale',
-        file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='RescaleToHeight',
         height=32,
         min_width=32,
-        max_width=None,
+        max_width=160,
         width_divisor=16),
+    dict(type='PadToWidth', width=160),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        color_type='grayscale',
-        file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
@@ -90,17 +90,18 @@
                 ),
             ],
             [
                 dict(
                     type='RescaleToHeight',
                     height=32,
                     min_width=32,
-                    max_width=None,
+                    max_width=160,
                     width_divisor=16)
             ],
+            [dict(type='PadToWidth', width=160)],
             # add loading annotation after ``Resize`` because ground truth
             # does not need to do resize data transform
             [dict(type='LoadOCRAnnotations', with_text=True)],
             [
                 dict(
                     type='PackTextRecogInputs',
                     meta_keys=('img_path', 'ori_shape', 'img_shape',
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_mj.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     '../_base_/datasets/icdar2013.py',
     '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_adadelta_5e.py',
     '_base_crnn_mini-vgg.py',
 ]
 # dataset settings
-train_list = [_base_.mjsynth_textrecog_test]
+train_list = [_base_.mjsynth_textrecog_train]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
 
 default_hooks = dict(logger=dict(type='LoggerHook', interval=50), )
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_toy.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/crnn_mini-vgg_5e_toy.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/crnn/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/_base_master_resnet31.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/_base_master_resnet31.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-file_client_args = dict(backend='disk')
-
 dictionary = dict(
     type='Dictionary',
     dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
     with_padding=True,
     with_unknown=True,
     same_start_end=True,
     with_start=True,
@@ -71,34 +69,30 @@
         dictionary=dictionary),
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor',
         mean=[127.5, 127.5, 127.5],
         std=[127.5, 127.5, 127.5]))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='RescaleToHeight',
         height=48,
         min_width=48,
         max_width=160,
         width_divisor=16),
     dict(type='PadToWidth', width=160),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='RescaleToHeight',
         height=48,
         min_width=48,
         max_width=160,
         width_divisor=16),
     dict(type='PadToWidth', width=160),
@@ -107,15 +101,15 @@
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_st_mj_sa.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_st_mj_sa.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 param_scheduler = [
     dict(type='LinearLR', end=100, by_epoch=False),
     dict(type='MultiStepLR', milestones=[11], end=12),
 ]
 
 # dataset settings
 train_list = [
-    _base_.mjsynth_textrecog_test, _base_.synthtext_textrecog_train,
+    _base_.mjsynth_textrecog_train, _base_.synthtext_textrecog_train,
     _base_.synthtext_add_textrecog_train
 ]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_toy.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/master_resnet31_12e_toy.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/master/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/master/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_modality-transform.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/_base_robustscanner_resnet31.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-file_client_args = dict(backend='disk')
-
 dictionary = dict(
     type='Dictionary',
     dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
-    with_padding=True,
-    with_unknown=True,
-    same_start_end=True,
     with_start=True,
-    with_end=True)
+    with_end=True,
+    same_start_end=True,
+    with_padding=True,
+    with_unknown=True)
 
 model = dict(
-    type='NRTR',
-    backbone=dict(type='NRTRModalityTransform'),
-    encoder=dict(type='NRTREncoder', n_layers=12),
+    type='RobustScanner',
+    data_preprocessor=dict(
+        type='TextRecogDataPreprocessor',
+        mean=[127, 127, 127],
+        std=[127, 127, 127]),
+    backbone=dict(type='ResNet31OCR'),
+    encoder=dict(
+        type='ChannelReductionEncoder', in_channels=512, out_channels=128),
     decoder=dict(
-        type='NRTRDecoder',
-        module_loss=dict(
-            type='CEModuleLoss', ignore_first_char=True, flatten=True),
+        type='RobustScannerFuser',
+        hybrid_decoder=dict(
+            type='SequenceAttentionDecoder', dim_input=512, dim_model=128),
+        position_decoder=dict(
+            type='PositionAttentionDecoder', dim_input=512, dim_model=128),
+        in_channels=[512, 512],
         postprocessor=dict(type='AttentionPostprocessor'),
+        module_loss=dict(
+            type='CEModuleLoss', ignore_first_char=True, reduction='mean'),
         dictionary=dictionary,
-        max_seq_len=30),
-    data_preprocessor=dict(
-        type='TextRecogDataPreprocessor',
-        mean=[123.675, 116.28, 103.53],
-        std=[58.395, 57.12, 57.375]))
+        max_seq_len=30))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='RescaleToHeight',
-        height=32,
-        min_width=32,
+        height=48,
+        min_width=48,
         max_width=160,
         width_divisor=4),
     dict(type='PadToWidth', width=160),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='RescaleToHeight',
-        height=32,
-        min_width=32,
+        height=48,
+        min_width=48,
         max_width=160,
-        width_divisor=16),
+        width_divisor=4),
     dict(type='PadToWidth', width=160),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
@@ -94,18 +94,18 @@
                     ],
                     condition="results['img_shape'][1]<results['img_shape'][0]"
                 ),
             ],
             [
                 dict(
                     type='RescaleToHeight',
-                    height=32,
-                    min_width=32,
+                    height=48,
+                    min_width=48,
                     max_width=160,
-                    width_divisor=16)
+                    width_divisor=4),
             ],
             [dict(type='PadToWidth', width=160)],
             # add loading annotation after ``Resize`` because ground truth
             # does not need to do resize data transform
             [dict(type='LoadOCRAnnotations', with_text=True)],
             [
                 dict(
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_resnet31.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/_base_nrtr_resnet31.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-file_client_args = dict(backend='disk')
-
 dictionary = dict(
     type='Dictionary',
     dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
     with_padding=True,
     with_unknown=True,
     same_start_end=True,
     with_start=True,
@@ -28,34 +26,30 @@
     ),
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375]))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='RescaleToHeight',
         height=32,
         min_width=32,
         max_width=160,
         width_divisor=4),
     dict(type='PadToWidth', width=160),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='RescaleToHeight',
         height=32,
         min_width=32,
         max_width=160,
         width_divisor=16),
     dict(type='PadToWidth', width=160),
@@ -64,15 +58,15 @@
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_st_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_st_mj.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 train_cfg = dict(max_epochs=6)
 # learning policy
 param_scheduler = [
     dict(type='MultiStepLR', milestones=[3, 4], end=6),
 ]
 
 # dataset settings
-train_list = [_base_.mjsynth_textrecog_test, _base_.synthtext_textrecog_train]
+train_list = [_base_.mjsynth_textrecog_train, _base_.synthtext_textrecog_train]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
 
 train_dataset = dict(
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_toy.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/nrtr/nrtr_modality-transform_6e_toy.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/nrtr/nrtr_resnet31-1by16-1by8_6e_st_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/satrn_shallow_5e_st_mj.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,40 +4,38 @@
     '../_base_/datasets/cute80.py',
     '../_base_/datasets/iiit5k.py',
     '../_base_/datasets/svt.py',
     '../_base_/datasets/svtp.py',
     '../_base_/datasets/icdar2013.py',
     '../_base_/datasets/icdar2015.py',
     '../_base_/default_runtime.py',
-    '../_base_/schedules/schedule_adam_base.py',
-    '_base_nrtr_resnet31.py',
+    '../_base_/schedules/schedule_adam_step_5e.py',
+    '_base_satrn_shallow.py',
 ]
 
-# optimizer settings
-train_cfg = dict(max_epochs=6)
-# learning policy
-param_scheduler = [
-    dict(type='MultiStepLR', milestones=[3, 4], end=6),
-]
+train_cfg = dict(type='EpochBasedTrainLoop', max_epochs=20, val_interval=1)
 
 # dataset settings
-train_list = [_base_.mjsynth_textrecog_test, _base_.synthtext_textrecog_train]
+train_list = [_base_.mjsynth_textrecog_train, _base_.synthtext_textrecog_train]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
 
 train_dataset = dict(
     type='ConcatDataset', datasets=train_list, pipeline=_base_.train_pipeline)
 test_dataset = dict(
     type='ConcatDataset', datasets=test_list, pipeline=_base_.test_pipeline)
 
+# optimizer
+optim_wrapper = dict(type='OptimWrapper', optimizer=dict(type='Adam', lr=3e-4))
+
 train_dataloader = dict(
-    batch_size=384,
+    batch_size=128,
     num_workers=24,
     persistent_workers=True,
     sampler=dict(type='DefaultSampler', shuffle=True),
     dataset=train_dataset)
 
 test_dataloader = dict(
     batch_size=1,
@@ -49,8 +47,8 @@
 
 val_dataloader = test_dataloader
 
 val_evaluator = dict(
     dataset_prefixes=['CUTE80', 'IIIT5K', 'SVT', 'SVTP', 'IC13', 'IC15'])
 test_evaluator = val_evaluator
 
-auto_scale_lr = dict(base_batch_size=384)
+auto_scale_lr = dict(base_batch_size=64 * 8)
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/_base_robustscanner_resnet31.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/_base_sar_resnet31_parallel-decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,58 +4,58 @@
     with_start=True,
     with_end=True,
     same_start_end=True,
     with_padding=True,
     with_unknown=True)
 
 model = dict(
-    type='RobustScanner',
+    type='SARNet',
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor',
         mean=[127, 127, 127],
         std=[127, 127, 127]),
     backbone=dict(type='ResNet31OCR'),
     encoder=dict(
-        type='ChannelReductionEncoder', in_channels=512, out_channels=128),
+        type='SAREncoder',
+        enc_bi_rnn=False,
+        enc_do_rnn=0.1,
+        enc_gru=False,
+    ),
     decoder=dict(
-        type='RobustScannerFuser',
-        hybrid_decoder=dict(
-            type='SequenceAttentionDecoder', dim_input=512, dim_model=128),
-        position_decoder=dict(
-            type='PositionAttentionDecoder', dim_input=512, dim_model=128),
-        in_channels=[512, 512],
+        type='ParallelSARDecoder',
+        enc_bi_rnn=False,
+        dec_bi_rnn=False,
+        dec_do_rnn=0,
+        dec_gru=False,
+        pred_dropout=0.1,
+        d_k=512,
+        pred_concat=True,
         postprocessor=dict(type='AttentionPostprocessor'),
         module_loss=dict(
             type='CEModuleLoss', ignore_first_char=True, reduction='mean'),
         dictionary=dictionary,
         max_seq_len=30))
 
-file_client_args = dict(backend='disk')
-
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='RescaleToHeight',
         height=48,
         min_width=48,
         max_width=160,
         width_divisor=4),
     dict(type='PadToWidth', width=160),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='RescaleToHeight',
         height=48,
         min_width=48,
         max_width=160,
         width_divisor=4),
     dict(type='PadToWidth', width=160),
@@ -64,15 +64,15 @@
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
@@ -103,15 +103,15 @@
             ],
             [
                 dict(
                     type='RescaleToHeight',
                     height=48,
                     min_width=48,
                     max_width=160,
-                    width_divisor=4),
+                    width_divisor=4)
             ],
             [dict(type='PadToWidth', width=160)],
             # add loading annotation after ``Resize`` because ground truth
             # does not need to do resize data transform
             [dict(type='LoadOCRAnnotations', with_text=True)],
             [
                 dict(
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_st-sub_mj-sub_sa_real.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_st-sub_mj-sub_sa_real.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_toy.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/robust_scanner/robustscanner_resnet31_5e_toy.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/_base_sar_resnet31_parallel-decoder.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/crnn/_base_crnn_mini-vgg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,58 @@
 dictionary = dict(
     type='Dictionary',
-    dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
-    with_start=True,
-    with_end=True,
-    same_start_end=True,
-    with_padding=True,
-    with_unknown=True)
+    dict_file='{{ fileDirname }}/../../../dicts/lower_english_digits.txt',
+    with_padding=True)
 
 model = dict(
-    type='SARNet',
-    data_preprocessor=dict(
-        type='TextRecogDataPreprocessor',
-        mean=[127, 127, 127],
-        std=[127, 127, 127]),
-    backbone=dict(type='ResNet31OCR'),
-    encoder=dict(
-        type='SAREncoder',
-        enc_bi_rnn=False,
-        enc_do_rnn=0.1,
-        enc_gru=False,
-    ),
+    type='CRNN',
+    preprocessor=None,
+    backbone=dict(type='MiniVGG', leaky_relu=False, input_channels=1),
+    encoder=None,
     decoder=dict(
-        type='ParallelSARDecoder',
-        enc_bi_rnn=False,
-        dec_bi_rnn=False,
-        dec_do_rnn=0,
-        dec_gru=False,
-        pred_dropout=0.1,
-        d_k=512,
-        pred_concat=True,
-        postprocessor=dict(type='AttentionPostprocessor'),
-        module_loss=dict(
-            type='CEModuleLoss', ignore_first_char=True, reduction='mean'),
-        dictionary=dictionary,
-        max_seq_len=30))
+        type='CRNNDecoder',
+        in_channels=512,
+        rnn_flag=True,
+        module_loss=dict(type='CTCModuleLoss', letter_case='lower'),
+        postprocessor=dict(type='CTCPostProcessor'),
+        dictionary=dictionary),
+    data_preprocessor=dict(
+        type='TextRecogDataPreprocessor', mean=[127], std=[127]))
 
-file_client_args = dict(backend='disk')
 train_pipeline = [
     dict(
         type='LoadImageFromFile',
-        file_client_args=file_client_args,
+        color_type='grayscale',
         ignore_empty=True,
         min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
-    dict(
-        type='RescaleToHeight',
-        height=48,
-        min_width=48,
-        max_width=160,
-        width_divisor=4),
-    dict(type='PadToWidth', width=160),
+    dict(type='Resize', scale=(100, 32), keep_ratio=False),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile', color_type='grayscale'),
     dict(
         type='RescaleToHeight',
-        height=48,
-        min_width=48,
-        max_width=160,
-        width_divisor=4),
-    dict(type='PadToWidth', width=160),
+        height=32,
+        min_width=32,
+        max_width=None,
+        width_divisor=16),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile', color_type='grayscale'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
@@ -105,20 +80,19 @@
                     ],
                     condition="results['img_shape'][1]<results['img_shape'][0]"
                 ),
             ],
             [
                 dict(
                     type='RescaleToHeight',
-                    height=48,
-                    min_width=48,
-                    max_width=160,
-                    width_divisor=4)
+                    height=32,
+                    min_width=32,
+                    max_width=None,
+                    width_divisor=16)
             ],
-            [dict(type='PadToWidth', width=160)],
             # add loading annotation after ``Resize`` because ground truth
             # does not need to do resize data transform
             [dict(type='LoadOCRAnnotations', with_text=True)],
             [
                 dict(
                     type='PackTextRecogInputs',
                     meta_keys=('img_path', 'ori_shape', 'img_shape',
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_st-sub_mj-sub_sa_real.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_st-sub_mj-sub_sa_real.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_toy.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/sar/sar_resnet31_parallel-decoder_5e_toy.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/_base_satrn_shallow.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/_base_satrn_shallow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-file_client_args = dict(backend='disk')
-
 dictionary = dict(
     type='Dictionary',
     dict_file='{{ fileDirname }}/../../../dicts/english_digits_symbols.txt',
     with_padding=True,
     with_unknown=True,
     same_start_end=True,
     with_start=True,
@@ -38,39 +36,35 @@
         postprocessor=dict(type='AttentionPostprocessor')),
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor',
         mean=[123.675, 116.28, 103.53],
         std=[58.395, 57.12, 57.375]))
 
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=2),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(type='Resize', scale=(100, 32), keep_ratio=False),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(type='Resize', scale=(100, 32), keep_ratio=False),
     # add loading annotation after ``Resize`` because ground truth
     # does not need to do resize data transform
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[
             [
                 dict(
                     type='ConditionApply',
                     true_transforms=[
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/satrn_shallow-small_5e_st_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/satrn/satrn_shallow-small_5e_st_mj.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/satrn/satrn_shallow_5e_st_mj.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/svtr-tiny_20e_st_mj.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 _base_ = [
+    '_base_svtr-tiny.py',
+    '../_base_/default_runtime.py',
     '../_base_/datasets/mjsynth.py',
     '../_base_/datasets/synthtext.py',
     '../_base_/datasets/cute80.py',
     '../_base_/datasets/iiit5k.py',
     '../_base_/datasets/svt.py',
     '../_base_/datasets/svtp.py',
     '../_base_/datasets/icdar2013.py',
     '../_base_/datasets/icdar2015.py',
-    '../_base_/default_runtime.py',
-    '../_base_/schedules/schedule_adam_step_5e.py',
-    '_base_satrn_shallow.py',
+    '../_base_/schedules/schedule_adam_base.py',
+]
+
+train_cfg = dict(type='EpochBasedTrainLoop', max_epochs=20, val_interval=1)
+
+optim_wrapper = dict(
+    type='OptimWrapper',
+    optimizer=dict(
+        type='AdamW',
+        lr=5 / (10**4) * 2048 / 2048,
+        betas=(0.9, 0.99),
+        eps=8e-8,
+        weight_decay=0.05))
+
+param_scheduler = [
+    dict(
+        type='LinearLR',
+        start_factor=0.5,
+        end_factor=1.,
+        end=2,
+        verbose=False,
+        convert_to_iter_based=True),
+    dict(
+        type='CosineAnnealingLR',
+        T_max=19,
+        begin=2,
+        end=20,
+        verbose=False,
+        convert_to_iter_based=True),
 ]
 
 # dataset settings
-train_list = [_base_.mjsynth_textrecog_test, _base_.synthtext_textrecog_train]
+train_list = [_base_.mjsynth_textrecog_train, _base_.synthtext_textrecog_train]
 test_list = [
     _base_.cute80_textrecog_test, _base_.iiit5k_textrecog_test,
     _base_.svt_textrecog_test, _base_.svtp_textrecog_test,
     _base_.icdar2013_textrecog_test, _base_.icdar2015_textrecog_test
 ]
 
-train_dataset = dict(
-    type='ConcatDataset', datasets=train_list, pipeline=_base_.train_pipeline)
-test_dataset = dict(
-    type='ConcatDataset', datasets=test_list, pipeline=_base_.test_pipeline)
-
-# optimizer
-optim_wrapper = dict(type='OptimWrapper', optimizer=dict(type='Adam', lr=3e-4))
+val_evaluator = dict(
+    dataset_prefixes=['CUTE80', 'IIIT5K', 'SVT', 'SVTP', 'IC13', 'IC15'])
+test_evaluator = val_evaluator
 
 train_dataloader = dict(
-    batch_size=128,
+    batch_size=512,
     num_workers=24,
     persistent_workers=True,
+    pin_memory=True,
     sampler=dict(type='DefaultSampler', shuffle=True),
-    dataset=train_dataset)
+    dataset=dict(
+        type='ConcatDataset',
+        datasets=train_list,
+        pipeline=_base_.train_pipeline))
 
-test_dataloader = dict(
-    batch_size=1,
-    num_workers=4,
+val_dataloader = dict(
+    batch_size=128,
+    num_workers=8,
     persistent_workers=True,
+    pin_memory=True,
     drop_last=False,
     sampler=dict(type='DefaultSampler', shuffle=False),
-    dataset=test_dataset)
-
-val_dataloader = test_dataloader
-
-val_evaluator = dict(
-    dataset_prefixes=['CUTE80', 'IIIT5K', 'SVT', 'SVTP', 'IC13', 'IC15'])
-test_evaluator = val_evaluator
+    dataset=dict(
+        type='ConcatDataset',
+        datasets=test_list,
+        pipeline=_base_.test_pipeline))
 
-auto_scale_lr = dict(base_batch_size=64 * 8)
+test_dataloader = val_dataloader
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/_base_svtr-tiny.py` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/_base_svtr-tiny.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,16 @@
         module_loss=dict(
             type='CTCModuleLoss', letter_case='lower', zero_infinity=True),
         postprocessor=dict(type='CTCPostProcessor'),
         dictionary=dictionary),
     data_preprocessor=dict(
         type='TextRecogDataPreprocessor', mean=[127.5], std=[127.5]))
 
-file_client_args = dict(backend='disk')
-
 train_pipeline = [
-    dict(
-        type='LoadImageFromFile',
-        file_client_args=file_client_args,
-        ignore_empty=True,
-        min_size=5),
+    dict(type='LoadImageFromFile', ignore_empty=True, min_size=5),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='RandomApply',
         prob=0.4,
         transforms=[
             dict(type='TextRecogGeneralAug', ),
         ],
@@ -113,24 +107,24 @@
     dict(type='Resize', scale=(256, 64)),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 test_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(type='Resize', scale=(256, 64)),
     dict(type='LoadOCRAnnotations', with_text=True),
     dict(
         type='PackTextRecogInputs',
         meta_keys=('img_path', 'ori_shape', 'img_shape', 'valid_ratio'))
 ]
 
 tta_pipeline = [
-    dict(type='LoadImageFromFile', file_client_args=file_client_args),
+    dict(type='LoadImageFromFile'),
     dict(
         type='TestTimeAug',
         transforms=[[
             dict(
                 type='ConditionApply',
                 true_transforms=[
                     dict(
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/configs/textrecog/svtr/metafile.yml` & `mmocr-1.0.1/mmocr/.mim/configs/textrecog/svtr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/model-index.yml` & `mmocr-1.0.1/mmocr/.mim/model-index.yml`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/browse_dataset.py` & `mmocr-1.0.1/mmocr/.mim/tools/visualizations/browse_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,14 @@
             visualizer=dict(
                 type='TextDetLocalVisualizer',
                 name='visualizer',
                 vis_backends=[dict(type='LocalVisBackend')]),
             pipeline=[
                 dict(
                     type='LoadImageFromFile',
-                    file_client_args=dict(backend='disk'),
                     color_type='color_ignore_orientation'),
                 dict(
                     type='LoadOCRAnnotations',
                     with_polygon=True,
                     with_bbox=True,
                     with_label=True,
                 ),
@@ -273,19 +272,15 @@
             ]),
         textrecog=dict(
             visualizer=dict(
                 type='TextRecogLocalVisualizer',
                 name='visualizer',
                 vis_backends=[dict(type='LocalVisBackend')]),
             pipeline=[
-                dict(
-                    type='LoadImageFromFile',
-                    file_client_args=dict(backend='disk'),
-                    ignore_empty=True,
-                    min_size=2),
+                dict(type='LoadImageFromFile', ignore_empty=True, min_size=2),
                 dict(type='LoadOCRAnnotations', with_text=True),
                 dict(
                     type='PackTextRecogInputs',
                     meta_keys=('img_path', 'ori_shape', 'img_shape',
                                'valid_ratio'))
             ]),
     )
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/get_flops.py` & `mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/offline_eval.py` & `mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/offline_eval.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/analysis_tools/print_config.py` & `mmocr-1.0.1/mmocr/.mim/tools/analysis_tools/print_config.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/common/curvedsyntext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/common/curvedsyntext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/common/extract_kaist.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/common/extract_kaist.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/kie/closeset_to_openset.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/kie/closeset_to_openset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/prepare_dataset.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/art_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/art_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/bid_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/bid_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/coco_to_line_dict.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/coco_to_line_dict.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/cocotext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/cocotext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ctw1500_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/ilst_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,233 +1,206 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import glob
+import os
 import os.path as osp
 import xml.etree.ElementTree as ET
-from functools import partial
 
 import mmcv
 import mmengine
-import numpy as np
-from shapely.geometry import Polygon
 
-from mmocr.utils import dump_ocr_data, list_from_file
+from mmocr.utils import dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, split):
+def collect_files(img_dir, gt_dir):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
-        img_dir(str): The image directory
-        gt_dir(str): The groundtruth directory
-        split(str): The split of dataset. Namely: training or test
+        img_dir (str): The image directory
+        gt_dir (str): The groundtruth directory
 
     Returns:
-        files(list): The list of tuples (img_file, groundtruth_file)
+        files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
 
-    # note that we handle png and jpg only. Pls convert others such as gif to
-    # jpg or png offline
-    suffixes = ['.png', '.PNG', '.jpg', '.JPG', '.jpeg', '.JPEG']
-
-    imgs_list = []
-    for suffix in suffixes:
-        imgs_list.extend(glob.glob(osp.join(img_dir, '*' + suffix)))
-
-    files = []
-    if split == 'training':
-        for img_file in imgs_list:
-            gt_file = gt_dir + '/' + osp.splitext(
-                osp.basename(img_file))[0] + '.xml'
-            files.append((img_file, gt_file))
-        assert len(files), f'No images found in {img_dir}'
-        print(f'Loaded {len(files)} images from {img_dir}')
-    elif split == 'test':
-        for img_file in imgs_list:
-            gt_file = gt_dir + '/000' + osp.splitext(
-                osp.basename(img_file))[0] + '.txt'
-            files.append((img_file, gt_file))
-        assert len(files), f'No images found in {img_dir}'
-        print(f'Loaded {len(files)} images from {img_dir}')
+    ann_list, imgs_list = [], []
+    for img_file in os.listdir(img_dir):
+        ann_path = osp.join(gt_dir, img_file.split('.')[0] + '.xml')
+        if os.path.exists(ann_path):
+            ann_list.append(ann_path)
+            imgs_list.append(osp.join(img_dir, img_file))
+
+    files = list(zip(imgs_list, ann_list))
+    assert len(files), f'No images found in {img_dir}'
+    print(f'Loaded {len(files)} images from {img_dir}')
 
     return files
 
 
-def collect_annotations(files, split, nproc=1):
+def collect_annotations(files, nproc=1):
     """Collect the annotation information.
 
     Args:
-        files(list): The list of tuples (image_file, groundtruth_file)
-        split(str): The split of dataset. Namely: training or test
-        nproc(int): The number of process to collect annotations
+        files (list): The list of tuples (image_file, groundtruth_file)
+        nproc (int): The number of process to collect annotations
 
     Returns:
-        images(list): The list of image information dicts
+        images (list): The list of image information dicts
     """
     assert isinstance(files, list)
-    assert isinstance(split, str)
     assert isinstance(nproc, int)
 
-    load_img_info_with_split = partial(load_img_info, split=split)
     if nproc > 1:
         images = mmengine.track_parallel_progress(
-            load_img_info_with_split, files, nproc=nproc)
+            load_img_info, files, nproc=nproc)
     else:
-        images = mmengine.track_progress(load_img_info_with_split, files)
+        images = mmengine.track_progress(load_img_info, files)
 
     return images
 
 
-def load_txt_info(gt_file, img_info):
-    anno_info = []
-    for line in list_from_file(gt_file):
-        # each line has one ploygen (n vetices), and one text.
-        # e.g., 695,885,866,888,867,1146,696,1143,####Latin 9
-        line = line.strip()
-        strs = line.split(',')
-        category_id = 1
-        assert strs[28][0] == '#'
-        xy = [int(x) for x in strs[0:28]]
-        assert len(xy) == 28
-        coordinates = np.array(xy).reshape(-1, 2)
-        polygon = Polygon(coordinates)
-        iscrowd = 0
-        area = polygon.area
-        # convert to COCO style XYWH format
-        min_x, min_y, max_x, max_y = polygon.bounds
-        bbox = [min_x, min_y, max_x - min_x, max_y - min_y]
-        text = strs[28][4:]
+def load_img_info(files):
+    """Load the information of one image.
+
+    Args:
+        files (tuple): The tuple of (img_file, groundtruth_file)
+
+    Returns:
+        img_info (dict): The dict of the img and annotation information
+    """
+    assert isinstance(files, tuple)
+
+    img_file, gt_file = files
+    assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
+        '.')[0]
+    # read imgs while ignoring orientations
+    img = mmcv.imread(img_file, 'unchanged')
+
+    try:
+        img_info = dict(
+            file_name=osp.join(osp.basename(img_file)),
+            height=img.shape[0],
+            width=img.shape[1],
+            segm_file=osp.join(osp.basename(gt_file)))
+    except AttributeError:
+        print(f'Skip broken img {img_file}')
+        return None
+
+    if osp.splitext(gt_file)[1] == '.xml':
+        img_info = load_xml_info(gt_file, img_info)
+    else:
+        raise NotImplementedError
 
-        anno = dict(
-            iscrowd=iscrowd,
-            category_id=category_id,
-            bbox=bbox,
-            area=area,
-            text=text,
-            segmentation=[xy])
-        anno_info.append(anno)
-    img_info.update(anno_info=anno_info)
     return img_info
 
 
 def load_xml_info(gt_file, img_info):
+    """Collect the annotation information.
+
+    The annotation format is as the following:
+    <annotations>
+    ...
+        <object>
+            <name>SMT</name>
+            <pose>Unspecified</pose>
+            <truncated>0</truncated>
+            <difficult>0</difficult>
+            <bndbox>
+                <xmin>157</xmin>
+                <ymin>294</ymin>
+                <xmax>237</xmax>
+                <ymax>357</ymax>
+            </bndbox>
+        <object>
 
+    Args:
+        gt_file (str): The path to ground-truth
+        img_info (dict): The dict of the img and annotation information
+
+    Returns:
+        img_info (dict): The dict of the img and annotation information
+    """
     obj = ET.parse(gt_file)
+    root = obj.getroot()
     anno_info = []
-    for image in obj.getroot():  # image
-        for box in image:  # image
-            h = box.attrib['height']
-            w = box.attrib['width']
-            x = box.attrib['left']
-            y = box.attrib['top']
-            text = box[0].text
-            segs = box[1].text
-            pts = segs.strip().split(',')
-            pts = [int(x) for x in pts]
-            assert len(pts) == 28
-            # pts = []
-            # for iter in range(2,len(box)):
-            #    pts.extend([int(box[iter].attrib['x']),
-            #  int(box[iter].attrib['y'])])
-            iscrowd = 0
-            category_id = 1
-            bbox = [int(x), int(y), int(w), int(h)]
-
-            coordinates = np.array(pts).reshape(-1, 2)
-            polygon = Polygon(coordinates)
-            area = polygon.area
-            anno = dict(
-                iscrowd=iscrowd,
-                category_id=category_id,
-                bbox=bbox,
-                area=area,
-                text=text,
-                segmentation=[pts])
-            anno_info.append(anno)
+    for object in root.iter('object'):
+        word = object.find('name').text
+        iscrowd = 1 if len(word) == 0 else 0
+        x1 = int(object.find('bndbox').find('xmin').text)
+        y1 = int(object.find('bndbox').find('ymin').text)
+        x2 = int(object.find('bndbox').find('xmax').text)
+        y2 = int(object.find('bndbox').find('ymax').text)
+
+        x = max(0, min(x1, x2))
+        y = max(0, min(y1, y2))
+        w, h = abs(x2 - x1), abs(y2 - y1)
+        bbox = [x1, y1, w, h]
+        segmentation = [x, y, x + w, y, x + w, y + h, x, y + h]
+        anno = dict(
+            iscrowd=iscrowd,
+            category_id=1,
+            bbox=bbox,
+            area=w * h,
+            segmentation=[segmentation])
+        anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
-def load_img_info(files, split):
-    """Load the information of one image.
+def split_train_val_list(full_list, val_ratio):
+    """Split list by val_ratio.
 
     Args:
-        files(tuple): The tuple of (img_file, groundtruth_file)
-        split(str): The split of dataset: training or test
+        full_list (list): List to be split
+        val_ratio (float): Split ratio for val set
 
-    Returns:
-        img_info(dict): The dict of the img and annotation information
+    return:
+        list(list, list): Train_list and val_list
     """
-    assert isinstance(files, tuple)
-    assert isinstance(split, str)
 
-    img_file, gt_file = files
-    # read imgs with ignoring orientations
-    img = mmcv.imread(img_file, 'unchanged')
-
-    split_name = osp.basename(osp.dirname(img_file))
-    img_info = dict(
-        # remove img_prefix for filename
-        file_name=osp.join(split_name, osp.basename(img_file)),
-        height=img.shape[0],
-        width=img.shape[1],
-        # anno_info=anno_info,
-        segm_file=osp.join(split_name, osp.basename(gt_file)))
-
-    if split == 'training':
-        img_info = load_xml_info(gt_file, img_info)
-    elif split == 'test':
-        img_info = load_txt_info(gt_file, img_info)
-    else:
-        raise NotImplementedError
-
-    return img_info
+    n_total = len(full_list)
+    offset = int(n_total * val_ratio)
+    if n_total == 0 or offset < 1:
+        return [], full_list
+    val_list = full_list[:offset]
+    train_list = full_list[offset:]
+    return [train_list, val_list]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Convert ctw1500 annotations to COCO format')
-    parser.add_argument('root_path', help='ctw1500 root path')
-    parser.add_argument('-o', '--out-dir', help='output path')
+        description='Generate training and val set of ILST ')
+    parser.add_argument('root_path', help='Root dir path of ILST')
     parser.add_argument(
-        '--split-list',
-        nargs='+',
-        help='a list of splits. e.g., "--split-list training test"')
-
+        '--val-ratio', help='Split ratio for val set', default=0., type=float)
     parser.add_argument(
-        '--nproc', default=1, type=int, help='number of process')
+        '--nproc', default=1, type=int, help='Number of processes')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    out_dir = args.out_dir if args.out_dir else root_path
-    mmengine.mkdir_or_exist(out_dir)
-
-    img_dir = osp.join(root_path, 'imgs')
-    gt_dir = osp.join(root_path, 'annotations')
-
-    set_name = {}
-    for split in args.split_list:
-        set_name.update({split: 'instances_' + split + '.json'})
-        assert osp.exists(osp.join(img_dir, split))
-
-    for split, json_name in set_name.items():
-        print(f'Converting {split} into {json_name}')
-        with mmengine.Timer(
-                print_tmpl='It takes {}s to convert icdar annotation'):
-            files = collect_files(
-                osp.join(img_dir, split), osp.join(gt_dir, split), split)
-            image_infos = collect_annotations(files, split, nproc=args.nproc)
-            dump_ocr_data(image_infos, osp.join(out_dir, json_name), 'textdet')
+    with mmengine.Timer(print_tmpl='It takes {}s to convert ILST annotation'):
+        files = collect_files(
+            osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'))
+        image_infos = collect_annotations(files, nproc=args.nproc)
+        if args.val_ratio:
+            image_infos = split_train_val_list(image_infos, args.val_ratio)
+            splits = ['training', 'val']
+        else:
+            image_infos = [image_infos]
+            splits = ['training']
+        for i, split in enumerate(splits):
+            dump_ocr_data(
+                list(filter(None, image_infos[i])),
+                osp.join(root_path, 'instances_' + split + '.json'), 'textdet')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/data_migrator.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/data_migrator.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/detext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/detext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/funsd_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/funsd_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/hiertext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/hiertext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ic11_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/ic11_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ic13_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/sroie_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
 import os
 import os.path as osp
 
 import mmcv
 import mmengine
+import numpy as np
 
 from mmocr.utils import dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, split):
+def collect_files(img_dir, gt_dir):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
+
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
 
-    ann_list, imgs_list, splits = [], [], []
-    for img in os.listdir(img_dir):
-        img_path = osp.join(img_dir, img)
-        imgs_list.append(img_path)
-        ann_list.append(osp.join(gt_dir, 'gt_' + img.split('.')[0] + '.txt'))
-        splits.append(split)
+    ann_list, imgs_list = [], []
+    for gt_file in os.listdir(gt_dir):
+        # Filtering repeated and missing images
+        if '(' in gt_file or gt_file == 'X51006619570.txt':
+            continue
+        ann_list.append(osp.join(gt_dir, gt_file))
+        imgs_list.append(osp.join(img_dir, gt_file.replace('.txt', '.jpg')))
 
-    files = list(zip(sorted(imgs_list), sorted(ann_list), splits))
+    files = list(zip(sorted(imgs_list), sorted(ann_list)))
     assert len(files), f'No images found in {img_dir}'
+
     print(f'Loaded {len(files)} images from {img_dir}')
 
     return files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
@@ -44,14 +48,15 @@
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
         nproc (int): The number of process to collect annotations
 
     Returns:
         images (list): The list of image information dicts
     """
+
     assert isinstance(files, list)
     assert isinstance(nproc, int)
 
     if nproc > 1:
         images = mmengine.track_parallel_progress(
             load_img_info, files, nproc=nproc)
     else:
@@ -60,107 +65,103 @@
     return images
 
 
 def load_img_info(files):
     """Load the information of one image.
 
     Args:
-        files (tuple): The tuple of (img_file, groundtruth_file, split)
+        files (tuple): The tuple of (img_file, groundtruth_file)
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
+
     assert isinstance(files, tuple)
 
-    img_file, gt_file, split = files
+    img_file, gt_file = files
+    assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
+        '.')[0]
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
     img_info = dict(
         file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
-    # IC13 uses different separator in gt files
-    if split == 'training':
-        separator = ' '
-    elif split == 'test':
-        separator = ','
-    else:
-        raise NotImplementedError
     if osp.splitext(gt_file)[1] == '.txt':
-        img_info = load_txt_info(gt_file, img_info, separator)
+        img_info = load_txt_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
-def load_txt_info(gt_file, img_info, separator):
+def load_txt_info(gt_file, img_info):
     """Collect the annotation information.
 
-    The annotation format is as the following:
-    [train]
-    left top right bottom "transcription"
-    [test]
-    left, top, right, bottom, "transcription"
-
     Args:
-        gt_file (str): The path to ground-truth
-        img_info (dict): The dict of the img and annotation information
+        gt_file (list): The list of tuples (image_file, groundtruth_file)
+        img_info (int): The dict of the img and annotation information
 
     Returns:
-        img_info (dict): The dict of the img and annotation information
+        img_info (list): The dict of the img and annotation information
     """
-    anno_info = []
-    with open(gt_file) as f:
-        lines = f.readlines()
-        for line in lines:
-            xmin, ymin, xmax, ymax = line.split(separator)[0:4]
-            x = max(0, int(xmin))
-            y = max(0, int(ymin))
-            w = int(xmax) - x
-            h = int(ymax) - y
+
+    with open(gt_file, encoding='unicode_escape') as f:
+        anno_info = []
+        for ann in f.readlines():
+
+            # annotation format [x1, y1, x2, y2, x3, y3, x4, y4, transcript]
+            try:
+                ann_box = np.array(ann.split(',')[0:8]).astype(int).tolist()
+            except ValueError:
+                # skip invalid annotation line
+                continue
+            x = max(0, min(ann_box[0::2]))
+            y = max(0, min(ann_box[1::2]))
+            w, h = max(ann_box[0::2]) - x, max(ann_box[1::2]) - y
             bbox = [x, y, w, h]
-            segmentation = [x, y, x + w, y, x + w, y + h, x, y + h]
+            segmentation = ann_box
 
             anno = dict(
                 iscrowd=0,
                 category_id=1,
                 bbox=bbox,
                 area=w * h,
                 segmentation=[segmentation])
             anno_info.append(anno)
+
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and test set of IC13')
-    parser.add_argument('root_path', help='Root dir path of IC13')
+        description='Generate training and test set of SROIE')
+    parser.add_argument('root_path', help='Root dir path of SROIE')
     parser.add_argument(
         '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
 
     for split in ['training', 'test']:
         print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert IC13 annotation'):
+                print_tmpl='It takes {}s to convert SROIE annotation'):
             files = collect_files(
                 osp.join(root_path, 'imgs', split),
-                osp.join(root_path, 'annotations', split), split)
+                osp.join(root_path, 'annotations', split))
             image_infos = collect_annotations(files, nproc=args.nproc)
             dump_ocr_data(image_infos,
                           osp.join(root_path, 'instances_' + split + '.json'),
                           'textdet')
 
 
 if __name__ == '__main__':
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/icdar_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/mtwi_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,185 +1,203 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import glob
+import math
+import os
 import os.path as osp
-from functools import partial
 
+import cv2
 import mmcv
 import mmengine
-import numpy as np
-from shapely.geometry import Polygon
+from PIL import Image
 
-from mmocr.utils import dump_ocr_data, list_from_file
+from mmocr.utils import dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir):
+def collect_files(img_dir, gt_dir, ratio):
     """Collect all images and their corresponding groundtruth files.
-
     Args:
-        img_dir(str): The image directory
-        gt_dir(str): The groundtruth directory
+        img_dir (str): The image directory
+        gt_dir (str): The groundtruth directory
+        ratio (float): Split ratio for val set
 
     Returns:
-        files(list): The list of tuples (img_file, groundtruth_file)
+        files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
+    assert isinstance(ratio, float)
+    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
+
+    ann_list, imgs_list = [], []
+    for ann_file in os.listdir(gt_dir):
+        img_file = osp.join(img_dir, ann_file.replace('txt', 'jpg'))
+        # This dataset contains some images obtained from .gif,
+        # which cannot be loaded by mmcv.imread(), convert them
+        # to RGB mode.
+        try:
+            if mmcv.imread(img_file) is None:
+                print(f'Convert {img_file} to RGB mode.')
+                img = Image.open(img_file)
+                img = img.convert('RGB')
+                img.save(img_file)
+        except cv2.error:
+            print(f'Skip broken img {img_file}')
+            continue
+
+        ann_list.append(osp.join(gt_dir, ann_file))
+        imgs_list.append(img_file)
+
+    all_files = list(zip(imgs_list, ann_list))
+    assert len(all_files), f'No images found in {img_dir}'
+    print(f'Loaded {len(all_files)} images from {img_dir}')
+
+    trn_files, val_files = [], []
+    if ratio > 0:
+        for i, file in enumerate(all_files):
+            if i % math.floor(1 / ratio):
+                trn_files.append(file)
+            else:
+                val_files.append(file)
+    else:
+        trn_files, val_files = all_files, []
 
-    # note that we handle png and jpg only. Pls convert others such as gif to
-    # jpg or png offline
-    suffixes = ['.png', '.PNG', '.jpg', '.JPG', '.jpeg', '.JPEG']
-    imgs_list = []
-    for suffix in suffixes:
-        imgs_list.extend(glob.glob(osp.join(img_dir, '*' + suffix)))
-
-    files = []
-    for img_file in imgs_list:
-        gt_file = gt_dir + '/gt_' + osp.splitext(
-            osp.basename(img_file))[0] + '.txt'
-        files.append((img_file, gt_file))
-    assert len(files), f'No images found in {img_dir}'
-    print(f'Loaded {len(files)} images from {img_dir}')
+    print(f'training #{len(trn_files)}, val #{len(val_files)}')
 
-    return files
+    return trn_files, val_files
 
 
-def collect_annotations(files, dataset, nproc=1):
+def collect_annotations(files, nproc=1):
     """Collect the annotation information.
-
     Args:
-        files(list): The list of tuples (image_file, groundtruth_file)
-        dataset(str): The dataset name, icdar2015 or icdar2017
-        nproc(int): The number of process to collect annotations
+        files (list): The list of tuples (image_file, groundtruth_file)
+        nproc (int): The number of process to collect annotations
 
     Returns:
-        images(list): The list of image information dicts
+        images (list): The list of image information dicts
     """
     assert isinstance(files, list)
-    assert isinstance(dataset, str)
-    assert dataset
     assert isinstance(nproc, int)
 
-    load_img_info_with_dataset = partial(load_img_info, dataset=dataset)
     if nproc > 1:
         images = mmengine.track_parallel_progress(
-            load_img_info_with_dataset, files, nproc=nproc)
+            load_img_info, files, nproc=nproc)
     else:
-        images = mmengine.track_progress(load_img_info_with_dataset, files)
+        images = mmengine.track_progress(load_img_info, files)
 
     return images
 
 
-def load_img_info(files, dataset):
+def load_img_info(files):
     """Load the information of one image.
-
     Args:
-        files(tuple): The tuple of (img_file, groundtruth_file)
-        dataset(str): Dataset name, icdar2015 or icdar2017
+        files (tuple): The tuple of (img_file, groundtruth_file)
 
     Returns:
-        img_info(dict): The dict of the img and annotation information
+        img_info (dict): The dict of the img and annotation information
     """
     assert isinstance(files, tuple)
-    assert isinstance(dataset, str)
-    assert dataset
 
     img_file, gt_file = files
-    # read imgs with ignoring orientations
-    img = mmcv.imread(img_file, 'unchanged')
+    assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
+        '.')[0]
+    # read imgs while ignoring orientations
+    img = mmcv.imread(img_file)
 
-    if dataset == 'icdar2017':
-        gt_list = list_from_file(gt_file)
-    elif dataset == 'icdar2015':
-        gt_list = list_from_file(gt_file, encoding='utf-8-sig')
+    img_info = dict(
+        file_name=osp.join(osp.basename(img_file)),
+        height=img.shape[0],
+        width=img.shape[1],
+        segm_file=osp.join(osp.basename(gt_file)))
+
+    if osp.splitext(gt_file)[1] == '.txt':
+        img_info = load_txt_info(gt_file, img_info)
     else:
-        raise NotImplementedError(f'Not support {dataset}')
+        raise NotImplementedError
+
+    return img_info
+
+
+def load_txt_info(gt_file, img_info):
+    """Collect the annotation information.
+
+    The annotation format is as the following:
+    x1,y1,x2,y2,x3,y3,x4,y4,text
+
+    45.45,226.83,11.87,181.79,183.84,13.1,233.79,49.95,时尚袋袋
+    345.98,311.18,345.98,347.21,462.26,347.21,462.26,311.18,73774
+    462.26,292.34,461.44,299.71,502.39,299.71,502.39,292.34,73/74/737
+
+    Args:
+        gt_file (str): The path to ground-truth
+        img_info (dict): The dict of the img and annotation information
+
+    Returns:
+        img_info (dict): The dict of the img and annotation information
+    """
 
     anno_info = []
-    for line in gt_list:
-        # each line has one ploygen (4 vetices), and others.
-        # e.g., 695,885,866,888,867,1146,696,1143,Latin,9
-        line = line.strip()
-        strs = line.split(',')
-        category_id = 1
-        xy = [int(x) for x in strs[0:8]]
-        coordinates = np.array(xy).reshape(-1, 2)
-        polygon = Polygon(coordinates)
-        iscrowd = 0
-        # set iscrowd to 1 to ignore 1.
-        if (dataset == 'icdar2015'
-                and strs[8] == '###') or (dataset == 'icdar2017'
-                                          and strs[9] == '###'):
-            iscrowd = 1
-            print('ignore text')
-
-        area = polygon.area
-        # convert to COCO style XYWH format
-        min_x, min_y, max_x, max_y = polygon.bounds
-        bbox = [min_x, min_y, max_x - min_x, max_y - min_y]
+    with open(gt_file) as f:
+        lines = f.readlines()
+    for line in lines:
+        points = line.split(',')[0:8]
+        word = line.split(',')[8].rstrip('\n')
+        segmentation = [math.floor(float(pt)) for pt in points]
+        x = max(0, min(segmentation[0::2]))
+        y = max(0, min(segmentation[1::2]))
+        w = abs(max(segmentation[0::2]) - x)
+        h = abs(max(segmentation[1::2]) - y)
+        bbox = [x, y, w, h]
 
         anno = dict(
-            iscrowd=iscrowd,
-            category_id=category_id,
+            iscrowd=1 if word == '###' else 0,
+            category_id=1,
             bbox=bbox,
-            area=area,
-            segmentation=[xy])
+            area=w * h,
+            segmentation=[segmentation])
         anno_info.append(anno)
-    split_name = osp.basename(osp.dirname(img_file))
-    img_info = dict(
-        # remove img_prefix for filename
-        file_name=osp.join(split_name, osp.basename(img_file)),
-        height=img.shape[0],
-        width=img.shape[1],
-        anno_info=anno_info,
-        segm_file=osp.join(split_name, osp.basename(gt_file)))
+
+    img_info.update(anno_info=anno_info)
+
     return img_info
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Convert Icdar2015 or Icdar2017 annotations to COCO format'
-    )
-    parser.add_argument('icdar_path', help='icdar root path')
-    parser.add_argument('-o', '--out-dir', help='output path')
+        description='Generate training and val set of MTWI.')
+    parser.add_argument('root_path', help='Root dir path of MTWI')
     parser.add_argument(
-        '-d', '--dataset', required=True, help='icdar2017 or icdar2015')
+        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
     parser.add_argument(
-        '--split-list',
-        nargs='+',
-        help='a list of splits. e.g., "--split-list training test"')
-
-    parser.add_argument(
-        '--nproc', default=1, type=int, help='number of process')
+        '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
-    icdar_path = args.icdar_path
-    out_dir = args.out_dir if args.out_dir else icdar_path
-    mmengine.mkdir_or_exist(out_dir)
-
-    img_dir = osp.join(icdar_path, 'imgs')
-    gt_dir = osp.join(icdar_path, 'annotations')
-
-    set_name = {}
-    for split in args.split_list:
-        set_name.update({split: 'instances_' + split + '.json'})
-        assert osp.exists(osp.join(img_dir, split))
+    root_path = args.root_path
+    ratio = args.val_ratio
+
+    trn_files, val_files = collect_files(
+        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
 
-    for split, json_name in set_name.items():
-        print(f'Converting {split} into {json_name}')
+    # Train set
+    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
+    with mmengine.Timer(
+            print_tmpl='It takes {}s to convert MTWI Training annotation'):
+        dump_ocr_data(trn_infos, osp.join(root_path,
+                                          'instances_training.json'),
+                      'textdet')
+
+    # Val set
+    if len(val_files) > 0:
+        val_infos = collect_annotations(val_files, nproc=args.nproc)
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert icdar annotation'):
-            files = collect_files(
-                osp.join(img_dir, split), osp.join(gt_dir, split))
-            image_infos = collect_annotations(
-                files, args.dataset, nproc=args.nproc)
-            dump_ocr_data(image_infos, osp.join(out_dir, json_name), 'textdet')
+                print_tmpl='It takes {}s to convert MTWI Val annotation'):
+            dump_ocr_data(val_infos, osp.join(root_path, 'instances_val.json'),
+                          'textdet')
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/ilst_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/kaist_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
+import math
 import os
 import os.path as osp
 import xml.etree.ElementTree as ET
 
 import mmcv
 import mmengine
 
 from mmocr.utils import dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir):
+def collect_files(img_dir, gt_dir, ratio):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
+        ratio (float): Split ratio for val set
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
+    assert isinstance(ratio, float)
+    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
 
     ann_list, imgs_list = [], []
     for img_file in os.listdir(img_dir):
-        ann_path = osp.join(gt_dir, img_file.split('.')[0] + '.xml')
-        if os.path.exists(ann_path):
-            ann_list.append(ann_path)
-            imgs_list.append(osp.join(img_dir, img_file))
-
-    files = list(zip(imgs_list, ann_list))
-    assert len(files), f'No images found in {img_dir}'
-    print(f'Loaded {len(files)} images from {img_dir}')
+        ann_list.append(osp.join(gt_dir, img_file.split('.')[0] + '.xml'))
+        imgs_list.append(osp.join(img_dir, img_file))
 
-    return files
+    all_files = list(zip(sorted(imgs_list), sorted(ann_list)))
+    assert len(all_files), f'No images found in {img_dir}'
+    print(f'Loaded {len(all_files)} images from {img_dir}')
+
+    trn_files, val_files = [], []
+    if ratio > 0:
+        for i, file in enumerate(all_files):
+            if i % math.floor(1 / ratio):
+                trn_files.append(file)
+            else:
+                val_files.append(file)
+    else:
+        trn_files, val_files = all_files, []
+
+    print(f'training #{len(trn_files)}, val #{len(val_files)}')
+
+    return trn_files, val_files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
 
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
@@ -74,133 +88,114 @@
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
-    try:
-        img_info = dict(
-            file_name=osp.join(osp.basename(img_file)),
-            height=img.shape[0],
-            width=img.shape[1],
-            segm_file=osp.join(osp.basename(gt_file)))
-    except AttributeError:
-        print(f'Skip broken img {img_file}')
-        return None
+    img_info = dict(
+        file_name=osp.join(osp.basename(img_file)),
+        height=img.shape[0],
+        width=img.shape[1],
+        segm_file=osp.join(osp.basename(gt_file)))
 
     if osp.splitext(gt_file)[1] == '.xml':
         img_info = load_xml_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
 def load_xml_info(gt_file, img_info):
     """Collect the annotation information.
 
-    The annotation format is as the following:
-    <annotations>
-    ...
-        <object>
-            <name>SMT</name>
-            <pose>Unspecified</pose>
-            <truncated>0</truncated>
-            <difficult>0</difficult>
-            <bndbox>
-                <xmin>157</xmin>
-                <ymin>294</ymin>
-                <xmax>237</xmax>
-                <ymax>357</ymax>
-            </bndbox>
-        <object>
+    Annotation Format
+    <image>
+        <imageName>DSC02306.JPG</imageName>
+        <resolution x="640" y="480" />
+        <words>
+            <word x="61" y="140" width="566" height="107">
+                <character x="61" y="147" width="75" height="94" char="C" />
+                <character x="173" y="147" width="77" height="93" char="L" />
+                <character x="251" y="146" width="83" height="96" char="A" />
+                <character x="335" y="146" width="75" height="97" char="V" />
+                <character x="409" y="140" width="52" height="105" char="I" />
+                <character x="464" y="147" width="76" height="96" char="T" />
+                <character x="538" y="154" width="89" height="93" char="A" />
+            </word>
+        </words>
+        <illumination>no</illumination>
+        <difficulty>2</difficulty>
+        <tag>
+        </tag>
+    </image>
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
+
     obj = ET.parse(gt_file)
     root = obj.getroot()
     anno_info = []
-    for object in root.iter('object'):
-        word = object.find('name').text
-        iscrowd = 1 if len(word) == 0 else 0
-        x1 = int(object.find('bndbox').find('xmin').text)
-        y1 = int(object.find('bndbox').find('ymin').text)
-        x2 = int(object.find('bndbox').find('xmax').text)
-        y2 = int(object.find('bndbox').find('ymax').text)
-
-        x = max(0, min(x1, x2))
-        y = max(0, min(y1, y2))
-        w, h = abs(x2 - x1), abs(y2 - y1)
-        bbox = [x1, y1, w, h]
+    for word in root.iter('word'):
+        x, y = max(0, int(word.attrib['x'])), max(0, int(word.attrib['y']))
+        w, h = int(word.attrib['width']), int(word.attrib['height'])
+        bbox = [x, y, w, h]
         segmentation = [x, y, x + w, y, x + w, y + h, x, y + h]
+
         anno = dict(
-            iscrowd=iscrowd,
+            iscrowd=0,
             category_id=1,
             bbox=bbox,
             area=w * h,
             segmentation=[segmentation])
         anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
-def split_train_val_list(full_list, val_ratio):
-    """Split list by val_ratio.
-
-    Args:
-        full_list (list): List to be split
-        val_ratio (float): Split ratio for val set
-
-    return:
-        list(list, list): Train_list and val_list
-    """
-
-    n_total = len(full_list)
-    offset = int(n_total * val_ratio)
-    if n_total == 0 or offset < 1:
-        return [], full_list
-    val_list = full_list[:offset]
-    train_list = full_list[offset:]
-    return [train_list, val_list]
-
-
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of ILST ')
-    parser.add_argument('root_path', help='Root dir path of ILST')
+        description='Generate training and val set of KAIST ')
+    parser.add_argument('root_path', help='Root dir path of KAIST')
     parser.add_argument(
-        '--val-ratio', help='Split ratio for val set', default=0., type=float)
+        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
     parser.add_argument(
-        '--nproc', default=1, type=int, help='Number of processes')
+        '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    with mmengine.Timer(print_tmpl='It takes {}s to convert ILST annotation'):
-        files = collect_files(
-            osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'))
-        image_infos = collect_annotations(files, nproc=args.nproc)
-        if args.val_ratio:
-            image_infos = split_train_val_list(image_infos, args.val_ratio)
-            splits = ['training', 'val']
-        else:
-            image_infos = [image_infos]
-            splits = ['training']
-        for i, split in enumerate(splits):
-            dump_ocr_data(
-                list(filter(None, image_infos[i])),
-                osp.join(root_path, 'instances_' + split + '.json'), 'textdet')
+    ratio = args.val_ratio
+
+    trn_files, val_files = collect_files(
+        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
+
+    # Train set
+    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
+    with mmengine.Timer(
+            print_tmpl='It takes {}s to convert KAIST Training annotation'):
+        dump_ocr_data(trn_infos, osp.join(root_path,
+                                          'instances_training.json'),
+                      'textdet')
+
+    # Val set
+    if len(val_files) > 0:
+        val_infos = collect_annotations(val_files, nproc=args.nproc)
+        with mmengine.Timer(
+                print_tmpl='It takes {}s to convert KAIST Val annotation'):
+            dump_ocr_data(val_infos, osp.join(root_path, 'instances_val.json'),
+                          'textdet')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/imgur_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/imgur_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/kaist_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/lv_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import math
 import os
 import os.path as osp
 import xml.etree.ElementTree as ET
 
 import mmcv
 import mmengine
 
 from mmocr.utils import dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, ratio):
+def collect_files(data_dir):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
-        img_dir (str): The image directory
-        gt_dir (str): The groundtruth directory
-        ratio (float): Split ratio for val set
+        data_dir (str): The directory to dataset
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
-    assert isinstance(img_dir, str)
-    assert img_dir
-    assert isinstance(gt_dir, str)
-    assert gt_dir
-    assert isinstance(ratio, float)
-    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
+    assert isinstance(data_dir, str)
+    assert data_dir
 
     ann_list, imgs_list = [], []
-    for img_file in os.listdir(img_dir):
-        ann_list.append(osp.join(gt_dir, img_file.split('.')[0] + '.xml'))
-        imgs_list.append(osp.join(img_dir, img_file))
-
-    all_files = list(zip(sorted(imgs_list), sorted(ann_list)))
-    assert len(all_files), f'No images found in {img_dir}'
-    print(f'Loaded {len(all_files)} images from {img_dir}')
-
-    trn_files, val_files = [], []
-    if ratio > 0:
-        for i, file in enumerate(all_files):
-            if i % math.floor(1 / ratio):
-                trn_files.append(file)
-            else:
-                val_files.append(file)
-    else:
-        trn_files, val_files = all_files, []
-
-    print(f'training #{len(trn_files)}, val #{len(val_files)}')
+    for video_dir in os.listdir(data_dir):
+        for frame_dir in os.listdir(osp.join(data_dir, video_dir)):
+            crt_dir = osp.join(data_dir, video_dir, frame_dir)
+            if not osp.isdir(crt_dir):
+                continue
+            for crt_file in os.listdir(crt_dir):
+                if crt_file.endswith('xml'):
+                    ann_path = osp.join(crt_dir, crt_file)
+                    img_path = osp.join(crt_dir,
+                                        crt_file.replace('xml', 'png'))
+                    if os.path.exists(img_path):
+                        ann_list.append(ann_path)
+                        imgs_list.append(img_path)
+                    else:
+                        continue
+
+    files = list(zip(imgs_list, ann_list))
+    assert len(files), f'No images found in {data_dir}'
+    print(f'Loaded {len(files)} images from {data_dir}')
 
-    return trn_files, val_files
+    return files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
 
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
@@ -87,17 +80,18 @@
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
+    img_file = os.path.split(img_file)[-1]
 
     img_info = dict(
-        file_name=osp.join(osp.basename(img_file)),
+        file_name=img_file,
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
     if osp.splitext(gt_file)[1] == '.xml':
         img_info = load_xml_info(gt_file, img_info)
     else:
@@ -105,49 +99,48 @@
 
     return img_info
 
 
 def load_xml_info(gt_file, img_info):
     """Collect the annotation information.
 
-    Annotation Format
-    <image>
-        <imageName>DSC02306.JPG</imageName>
-        <resolution x="640" y="480" />
-        <words>
-            <word x="61" y="140" width="566" height="107">
-                <character x="61" y="147" width="75" height="94" char="C" />
-                <character x="173" y="147" width="77" height="93" char="L" />
-                <character x="251" y="146" width="83" height="96" char="A" />
-                <character x="335" y="146" width="75" height="97" char="V" />
-                <character x="409" y="140" width="52" height="105" char="I" />
-                <character x="464" y="147" width="76" height="96" char="T" />
-                <character x="538" y="154" width="89" height="93" char="A" />
-            </word>
-        </words>
-        <illumination>no</illumination>
-        <difficulty>2</difficulty>
-        <tag>
-        </tag>
-    </image>
+    The annotation format is as the following:
+    <annotation>
+        <object>
+            <name>hierarchy</name>
+            <pose>Unspecified</pose>
+            <truncated>0</truncated>
+            <difficult>0</difficult>
+            <bndbox>
+                <xmin>657</xmin>
+                <ymin>467</ymin>
+                <xmax>839</xmax>
+                <ymax>557</ymax>
+            </bndbox>
+        </object>
+    </annotation>
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
 
     obj = ET.parse(gt_file)
     root = obj.getroot()
     anno_info = []
-    for word in root.iter('word'):
-        x, y = max(0, int(word.attrib['x'])), max(0, int(word.attrib['y']))
-        w, h = int(word.attrib['width']), int(word.attrib['height'])
+    for obj in root.iter('object'):
+        x = max(0, int(obj.find('bndbox').find('xmin').text))
+        y = max(0, int(obj.find('bndbox').find('ymin').text))
+        xmax = int(obj.find('bndbox').find('xmax').text)
+        ymax = int(obj.find('bndbox').find('ymax').text)
+
+        w, h = abs(xmax - x), abs(ymax - y)
         bbox = [x, y, w, h]
         segmentation = [x, y, x + w, y, x + w, y + h, x, y + h]
 
         anno = dict(
             iscrowd=0,
             category_id=1,
             bbox=bbox,
@@ -158,44 +151,32 @@
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of KAIST ')
-    parser.add_argument('root_path', help='Root dir path of KAIST')
+        description='Generate training, val and test set of Lecture Video DB ')
+    parser.add_argument('root_path', help='Root dir path of Lecture Video DB')
     parser.add_argument(
-        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
-    parser.add_argument(
-        '--nproc', default=1, type=int, help='Number of process')
+        '--nproc', default=1, type=int, help='number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    ratio = args.val_ratio
-
-    trn_files, val_files = collect_files(
-        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
 
-    # Train set
-    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
-    with mmengine.Timer(
-            print_tmpl='It takes {}s to convert KAIST Training annotation'):
-        dump_ocr_data(trn_infos, osp.join(root_path,
-                                          'instances_training.json'),
-                      'textdet')
-
-    # Val set
-    if len(val_files) > 0:
-        val_infos = collect_annotations(val_files, nproc=args.nproc)
+    for split in ['train', 'val', 'test']:
+        print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert KAIST Val annotation'):
-            dump_ocr_data(val_infos, osp.join(root_path, 'instances_val.json'),
+                print_tmpl='It takes {}s to convert LV annotation'):
+            files = collect_files(osp.join(root_path, 'imgs', split))
+            image_infos = collect_annotations(files, nproc=args.nproc)
+            dump_ocr_data(image_infos,
+                          osp.join(root_path, 'instances_' + split + '.json'),
                           'textdet')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/lsvt_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/lsvt_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/lv_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/naf_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import os
 import os.path as osp
-import xml.etree.ElementTree as ET
 
 import mmcv
 import mmengine
 
 from mmocr.utils import dump_ocr_data
 
 
-def collect_files(data_dir):
+def collect_files(img_dir, gt_dir, split_info):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
-        data_dir (str): The directory to dataset
+        img_dir (str): The image directory
+        gt_dir (str): The groundtruth directory
+        split_info (dict): The split information for train/val/test
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
-    assert isinstance(data_dir, str)
-    assert data_dir
+    assert isinstance(img_dir, str)
+    assert img_dir
+    assert isinstance(gt_dir, str)
+    assert gt_dir
+    assert isinstance(split_info, dict)
+    assert split_info
 
     ann_list, imgs_list = [], []
-    for video_dir in os.listdir(data_dir):
-        for frame_dir in os.listdir(osp.join(data_dir, video_dir)):
-            crt_dir = osp.join(data_dir, video_dir, frame_dir)
-            if not osp.isdir(crt_dir):
+    for group in split_info:
+        for img in split_info[group]:
+            image_path = osp.join(img_dir, img)
+            anno_path = osp.join(gt_dir, 'groups', group,
+                                 img.replace('jpg', 'json'))
+
+            # Filtering out the missing images
+            if not osp.exists(image_path) or not osp.exists(anno_path):
                 continue
-            for crt_file in os.listdir(crt_dir):
-                if crt_file.endswith('xml'):
-                    ann_path = osp.join(crt_dir, crt_file)
-                    img_path = osp.join(crt_dir,
-                                        crt_file.replace('xml', 'png'))
-                    if os.path.exists(img_path):
-                        ann_list.append(ann_path)
-                        imgs_list.append(img_path)
-                    else:
-                        continue
+
+            imgs_list.append(image_path)
+            ann_list.append(anno_path)
 
     files = list(zip(imgs_list, ann_list))
-    assert len(files), f'No images found in {data_dir}'
-    print(f'Loaded {len(files)} images from {data_dir}')
+    assert len(files), f'No images found in {img_dir}'
+    print(f'Loaded {len(files)} images from {img_dir}')
 
     return files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
 
@@ -78,104 +79,118 @@
         img_info (dict): The dict of the img and annotation information
     """
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
-    # read imgs while ignoring orientations
+    # Read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
-    img_file = os.path.split(img_file)[-1]
 
     img_info = dict(
-        file_name=img_file,
+        file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
-    if osp.splitext(gt_file)[1] == '.xml':
-        img_info = load_xml_info(gt_file, img_info)
+    if osp.splitext(gt_file)[1] == '.json':
+        img_info = load_json_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
-def load_xml_info(gt_file, img_info):
+def load_json_info(gt_file, img_info):
     """Collect the annotation information.
 
-    The annotation format is as the following:
-    <annotation>
-        <object>
-            <name>hierarchy</name>
-            <pose>Unspecified</pose>
-            <truncated>0</truncated>
-            <difficult>0</difficult>
-            <bndbox>
-                <xmin>657</xmin>
-                <ymin>467</ymin>
-                <xmax>839</xmax>
-                <ymax>557</ymax>
-            </bndbox>
-        </object>
-    </annotation>
+    Annotation Format
+    {
+        'textBBs': [{
+            'poly_points': [[435,1406], [466,1406], [466,1439], [435,1439]],
+            "type": "text",
+            "id": "t1",
+        }], ...
+    }
+
+    Some special characters are used in the transcription:
+    "«text»" indicates that "text" had a strikethrough
+    "¿" indicates the transcriber could not read a character
+    "§" indicates the whole line or word was illegible
+    "" (empty string) is if the field was blank
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
+    assert isinstance(gt_file, str)
+    assert isinstance(img_info, dict)
 
-    obj = ET.parse(gt_file)
-    root = obj.getroot()
+    annotation = mmengine.load(gt_file)
     anno_info = []
-    for obj in root.iter('object'):
-        x = max(0, int(obj.find('bndbox').find('xmin').text))
-        y = max(0, int(obj.find('bndbox').find('ymin').text))
-        xmax = int(obj.find('bndbox').find('xmax').text)
-        ymax = int(obj.find('bndbox').find('ymax').text)
-
-        w, h = abs(xmax - x), abs(ymax - y)
-        bbox = [x, y, w, h]
-        segmentation = [x, y, x + w, y, x + w, y + h, x, y + h]
-
-        anno = dict(
-            iscrowd=0,
-            category_id=1,
-            bbox=bbox,
-            area=w * h,
-            segmentation=[segmentation])
-        anno_info.append(anno)
+
+    # 'textBBs' contains the printed texts of the table while 'fieldBBs'
+    #  contains the text filled by human.
+    for box_type in ['textBBs', 'fieldBBs']:
+        for anno in annotation[box_type]:
+            # Skip blanks
+            if box_type == 'fieldBBs':
+                if anno['type'] == 'blank':
+                    continue
+
+            xs, ys, segmentation = [], [], []
+            for p in anno['poly_points']:
+                xs.append(p[0])
+                ys.append(p[1])
+                segmentation.append(p[0])
+                segmentation.append(p[1])
+            x, y = max(0, min(xs)), max(0, min(ys))
+            w, h = max(xs) - x, max(ys) - y
+            bbox = [x, y, w, h]
+
+            anno = dict(
+                iscrowd=0,
+                category_id=1,
+                bbox=bbox,
+                area=w * h,
+                segmentation=[segmentation])
+            anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training, val and test set of Lecture Video DB ')
-    parser.add_argument('root_path', help='Root dir path of Lecture Video DB')
+        description='Generate training, val, and test set of NAF ')
+    parser.add_argument('root_path', help='Root dir path of NAF')
     parser.add_argument(
-        '--nproc', default=1, type=int, help='number of process')
+        '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-
-    for split in ['train', 'val', 'test']:
+    split_info = mmengine.load(
+        osp.join(root_path, 'annotations', 'train_valid_test_split.json'))
+    split_info['training'] = split_info.pop('train')
+    split_info['val'] = split_info.pop('valid')
+    for split in ['training', 'val', 'test']:
         print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert LV annotation'):
-            files = collect_files(osp.join(root_path, 'imgs', split))
+                print_tmpl='It takes {}s to convert NAF annotation'):
+            files = collect_files(
+                osp.join(root_path, 'imgs'),
+                osp.join(root_path, 'annotations'), split_info[split])
             image_infos = collect_annotations(files, nproc=args.nproc)
             dump_ocr_data(image_infos,
                           osp.join(root_path, 'instances_' + split + '.json'),
                           'textdet')
 
 
 if __name__ == '__main__':
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/mtwi_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/rctw_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
 import math
 import os
 import os.path as osp
 
-import cv2
 import mmcv
 import mmengine
-from PIL import Image
 
 from mmocr.utils import dump_ocr_data
 
 
 def collect_files(img_dir, gt_dir, ratio):
     """Collect all images and their corresponding groundtruth files.
     Args:
@@ -27,30 +25,16 @@
     assert isinstance(gt_dir, str)
     assert gt_dir
     assert isinstance(ratio, float)
     assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
 
     ann_list, imgs_list = [], []
     for ann_file in os.listdir(gt_dir):
-        img_file = osp.join(img_dir, ann_file.replace('txt', 'jpg'))
-        # This dataset contains some images obtained from .gif,
-        # which cannot be loaded by mmcv.imread(), convert them
-        # to RGB mode.
-        try:
-            if mmcv.imread(img_file) is None:
-                print(f'Convert {img_file} to RGB mode.')
-                img = Image.open(img_file)
-                img = img.convert('RGB')
-                img.save(img_file)
-        except cv2.error:
-            print(f'Skip broken img {img_file}')
-            continue
-
         ann_list.append(osp.join(gt_dir, ann_file))
-        imgs_list.append(img_file)
+        imgs_list.append(osp.join(img_dir, ann_file.replace('txt', 'jpg')))
 
     all_files = list(zip(imgs_list, ann_list))
     assert len(all_files), f'No images found in {img_dir}'
     print(f'Loaded {len(all_files)} images from {img_dir}')
 
     trn_files, val_files = [], []
     if ratio > 0:
@@ -118,58 +102,64 @@
     return img_info
 
 
 def load_txt_info(gt_file, img_info):
     """Collect the annotation information.
 
     The annotation format is as the following:
-    x1,y1,x2,y2,x3,y3,x4,y4,text
+    x1, y1, x2, y2, x3, y3, x4, y4, difficult, text
 
-    45.45,226.83,11.87,181.79,183.84,13.1,233.79,49.95,时尚袋袋
-    345.98,311.18,345.98,347.21,462.26,347.21,462.26,311.18,73774
-    462.26,292.34,461.44,299.71,502.39,299.71,502.39,292.34,73/74/737
+    390,902,1856,902,1856,1225,390,1225,0,"金氏眼镜"
+    1875,1170,2149,1170,2149,1245,1875,1245,0,"创于1989"
+    2054,1277,2190,1277,2190,1323,2054,1323,0,"城建店"
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
 
     anno_info = []
-    with open(gt_file) as f:
+    with open(gt_file, encoding='utf-8-sig') as f:
         lines = f.readlines()
     for line in lines:
         points = line.split(',')[0:8]
-        word = line.split(',')[8].rstrip('\n')
-        segmentation = [math.floor(float(pt)) for pt in points]
+        word = line.split(',')[9].rstrip('\n').strip('"')
+        difficult = 1 if line.split(',')[8] != '0' else 0
+        segmentation = [int(pt) for pt in points]
         x = max(0, min(segmentation[0::2]))
         y = max(0, min(segmentation[1::2]))
         w = abs(max(segmentation[0::2]) - x)
         h = abs(max(segmentation[1::2]) - y)
         bbox = [x, y, w, h]
 
+        if word == '###' or difficult == 1:
+            iscrowd = 1
+        else:
+            iscrowd = 0
+
         anno = dict(
-            iscrowd=1 if word == '###' else 0,
+            iscrowd=iscrowd,
             category_id=1,
             bbox=bbox,
             area=w * h,
             segmentation=[segmentation])
         anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of MTWI.')
-    parser.add_argument('root_path', help='Root dir path of MTWI')
+        description='Generate training and val set of RCTW.')
+    parser.add_argument('root_path', help='Root dir path of RCTW')
     parser.add_argument(
         '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
     parser.add_argument(
         '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
@@ -179,25 +169,25 @@
     root_path = args.root_path
     ratio = args.val_ratio
 
     trn_files, val_files = collect_files(
         osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
 
     # Train set
-    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
     with mmengine.Timer(
-            print_tmpl='It takes {}s to convert MTWI Training annotation'):
+            print_tmpl='It takes {}s to convert RCTW Training annotation'):
+        trn_infos = collect_annotations(trn_files, nproc=args.nproc)
         dump_ocr_data(trn_infos, osp.join(root_path,
                                           'instances_training.json'),
                       'textdet')
 
     # Val set
     if len(val_files) > 0:
-        val_infos = collect_annotations(val_files, nproc=args.nproc)
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert MTWI Val annotation'):
+                print_tmpl='It takes {}s to convert RCTW Val annotation'):
+            val_infos = collect_annotations(val_files, nproc=args.nproc)
             dump_ocr_data(val_infos, osp.join(root_path, 'instances_val.json'),
                           'textdet')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/naf_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/funsd_converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
+import math
+import os
 import os.path as osp
 
 import mmcv
 import mmengine
 
-from mmocr.utils import dump_ocr_data
+from mmocr.utils import crop_img, dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, split_info):
+def collect_files(img_dir, gt_dir):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
-        split_info (dict): The split information for train/val/test
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
-    assert isinstance(split_info, dict)
-    assert split_info
 
     ann_list, imgs_list = [], []
-    for group in split_info:
-        for img in split_info[group]:
-            image_path = osp.join(img_dir, img)
-            anno_path = osp.join(gt_dir, 'groups', group,
-                                 img.replace('jpg', 'json'))
+    for gt_file in os.listdir(gt_dir):
+        ann_list.append(osp.join(gt_dir, gt_file))
+        imgs_list.append(osp.join(img_dir, gt_file.replace('.json', '.png')))
 
-            # Filtering out the missing images
-            if not osp.exists(image_path) or not osp.exists(anno_path):
-                continue
-
-            imgs_list.append(image_path)
-            ann_list.append(anno_path)
-
-    files = list(zip(imgs_list, ann_list))
+    files = list(zip(sorted(imgs_list), sorted(ann_list)))
     assert len(files), f'No images found in {img_dir}'
     print(f'Loaded {len(files)} images from {img_dir}')
 
     return files
 
 
 def collect_annotations(files, nproc=1):
@@ -79,15 +69,15 @@
         img_info (dict): The dict of the img and annotation information
     """
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
-    # Read imgs while ignoring orientations
+    # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
     img_info = dict(
         file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
@@ -99,99 +89,122 @@
 
     return img_info
 
 
 def load_json_info(gt_file, img_info):
     """Collect the annotation information.
 
-    Annotation Format
-    {
-        'textBBs': [{
-            'poly_points': [[435,1406], [466,1406], [466,1439], [435,1439]],
-            "type": "text",
-            "id": "t1",
-        }], ...
-    }
-
-    Some special characters are used in the transcription:
-    "«text»" indicates that "text" had a strikethrough
-    "¿" indicates the transcriber could not read a character
-    "§" indicates the whole line or word was illegible
-    "" (empty string) is if the field was blank
-
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
-    assert isinstance(gt_file, str)
-    assert isinstance(img_info, dict)
 
     annotation = mmengine.load(gt_file)
     anno_info = []
+    for form in annotation['form']:
+        for ann in form['words']:
+
+            # Ignore illegible samples
+            if len(ann['text']) == 0:
+                continue
+
+            x1, y1, x2, y2 = ann['box']
+            x = max(0, min(math.floor(x1), math.floor(x2)))
+            y = max(0, min(math.floor(y1), math.floor(y2)))
+            w, h = math.ceil(abs(x2 - x1)), math.ceil(abs(y2 - y1))
+            bbox = [x, y, x + w, y, x + w, y + h, x, y + h]
+            word = ann['text']
 
-    # 'textBBs' contains the printed texts of the table while 'fieldBBs'
-    #  contains the text filled by human.
-    for box_type in ['textBBs', 'fieldBBs']:
-        for anno in annotation[box_type]:
-            # Skip blanks
-            if box_type == 'fieldBBs':
-                if anno['type'] == 'blank':
-                    continue
-
-            xs, ys, segmentation = [], [], []
-            for p in anno['poly_points']:
-                xs.append(p[0])
-                ys.append(p[1])
-                segmentation.append(p[0])
-                segmentation.append(p[1])
-            x, y = max(0, min(xs)), max(0, min(ys))
-            w, h = max(xs) - x, max(ys) - y
-            bbox = [x, y, w, h]
-
-            anno = dict(
-                iscrowd=0,
-                category_id=1,
-                bbox=bbox,
-                area=w * h,
-                segmentation=[segmentation])
+            anno = dict(bbox=bbox, word=word)
             anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
+def generate_ann(root_path, split, image_infos, preserve_vertical):
+    """Generate cropped annotations and label txt file.
+
+    Args:
+        root_path (str): The root path of the dataset
+        split (str): The split of dataset. Namely: training or test
+        image_infos (list[dict]): A list of dicts of the img and
+            annotation information
+        preserve_vertical (bool): Whether to preserve vertical texts
+    """
+
+    dst_image_root = osp.join(root_path, 'crops', split)
+    if split == 'training':
+        dst_label_file = osp.join(root_path, 'train_label.json')
+    elif split == 'test':
+        dst_label_file = osp.join(root_path, 'test_label.json')
+    os.makedirs(dst_image_root, exist_ok=True)
+
+    img_info = []
+    for image_info in image_infos:
+        index = 1
+        src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
+        image = mmcv.imread(src_img_path)
+        src_img_root = image_info['file_name'].split('.')[0]
+
+        for anno in image_info['anno_info']:
+            word = anno['word']
+            dst_img = crop_img(image, anno['bbox'])
+            h, w, _ = dst_img.shape
+
+            # Skip invalid annotations
+            if min(dst_img.shape) == 0:
+                continue
+            # Skip vertical texts
+            if not preserve_vertical and h / w > 2:
+                continue
+
+            dst_img_name = f'{src_img_root}_{index}.png'
+            index += 1
+            dst_img_path = osp.join(dst_image_root, dst_img_name)
+            mmcv.imwrite(dst_img, dst_img_path)
+
+            img_info.append({
+                'file_name': dst_img_name,
+                'anno_info': [{
+                    'text': word
+                }]
+            })
+
+    dump_ocr_data(img_info, dst_label_file, 'textrecog')
+
+
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training, val, and test set of NAF ')
-    parser.add_argument('root_path', help='Root dir path of NAF')
+        description='Generate training and test set of FUNSD ')
+    parser.add_argument('root_path', help='Root dir path of FUNSD')
     parser.add_argument(
-        '--nproc', default=1, type=int, help='Number of process')
+        '--preserve_vertical',
+        help='Preserve samples containing vertical texts',
+        action='store_true')
+    parser.add_argument(
+        '--nproc', default=1, type=int, help='Number of processes')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    split_info = mmengine.load(
-        osp.join(root_path, 'annotations', 'train_valid_test_split.json'))
-    split_info['training'] = split_info.pop('train')
-    split_info['val'] = split_info.pop('valid')
-    for split in ['training', 'val', 'test']:
+
+    for split in ['training', 'test']:
         print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert NAF annotation'):
+                print_tmpl='It takes {}s to convert FUNSD annotation'):
             files = collect_files(
                 osp.join(root_path, 'imgs'),
-                osp.join(root_path, 'annotations'), split_info[split])
+                osp.join(root_path, 'annotations', split))
             image_infos = collect_annotations(files, nproc=args.nproc)
-            dump_ocr_data(image_infos,
-                          osp.join(root_path, 'instances_' + split + '.json'),
-                          'textdet')
+            generate_ann(root_path, split, image_infos, args.preserve_vertical)
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/rctw_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/sroie_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,91 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import math
 import os
 import os.path as osp
 
 import mmcv
 import mmengine
+import numpy as np
 
-from mmocr.utils import dump_ocr_data
+from mmocr.utils import crop_img, dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, ratio):
+def collect_files(img_dir, gt_dir):
     """Collect all images and their corresponding groundtruth files.
+
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
-        ratio (float): Split ratio for val set
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
+
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
-    assert isinstance(ratio, float)
-    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
 
     ann_list, imgs_list = [], []
-    for ann_file in os.listdir(gt_dir):
-        ann_list.append(osp.join(gt_dir, ann_file))
-        imgs_list.append(osp.join(img_dir, ann_file.replace('txt', 'jpg')))
-
-    all_files = list(zip(imgs_list, ann_list))
-    assert len(all_files), f'No images found in {img_dir}'
-    print(f'Loaded {len(all_files)} images from {img_dir}')
-
-    trn_files, val_files = [], []
-    if ratio > 0:
-        for i, file in enumerate(all_files):
-            if i % math.floor(1 / ratio):
-                trn_files.append(file)
-            else:
-                val_files.append(file)
-    else:
-        trn_files, val_files = all_files, []
+    for gt_file in os.listdir(gt_dir):
+        # Filtering repeated and missing images
+        if '(' in gt_file or gt_file == 'X51006619570.txt':
+            continue
+        ann_list.append(osp.join(gt_dir, gt_file))
+        imgs_list.append(osp.join(img_dir, gt_file.replace('.txt', '.jpg')))
 
-    print(f'training #{len(trn_files)}, val #{len(val_files)}')
+    files = list(zip(sorted(imgs_list), sorted(ann_list)))
+    assert len(files), f'No images found in {img_dir}'
 
-    return trn_files, val_files
+    print(f'Loaded {len(files)} images from {img_dir}')
+
+    return files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
+
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
         nproc (int): The number of process to collect annotations
 
     Returns:
         images (list): The list of image information dicts
     """
+
     assert isinstance(files, list)
     assert isinstance(nproc, int)
 
     if nproc > 1:
         images = mmengine.track_parallel_progress(
             load_img_info, files, nproc=nproc)
     else:
         images = mmengine.track_progress(load_img_info, files)
 
     return images
 
 
 def load_img_info(files):
     """Load the information of one image.
+
     Args:
         files (tuple): The tuple of (img_file, groundtruth_file)
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
+
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
     # read imgs while ignoring orientations
-    img = mmcv.imread(img_file)
+    img = mmcv.imread(img_file, 'unchanged')
 
     img_info = dict(
         file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
@@ -101,93 +96,112 @@
 
     return img_info
 
 
 def load_txt_info(gt_file, img_info):
     """Collect the annotation information.
 
-    The annotation format is as the following:
-    x1, y1, x2, y2, x3, y3, x4, y4, difficult, text
-
-    390,902,1856,902,1856,1225,390,1225,0,"金氏眼镜"
-    1875,1170,2149,1170,2149,1245,1875,1245,0,"创于1989"
-    2054,1277,2190,1277,2190,1323,2054,1323,0,"城建店"
+    Annotation Format
+    x1, y1, x2, y2, x3, y3, x4, y4, transcript
 
     Args:
-        gt_file (str): The path to ground-truth
-        img_info (dict): The dict of the img and annotation information
+        gt_file (list): The list of tuples (image_file, groundtruth_file)
+        img_info (int): The dict of the img and annotation information
 
     Returns:
-        img_info (dict): The dict of the img and annotation information
+        img_info (list): The dict of the img and annotation information
     """
 
-    anno_info = []
-    with open(gt_file, encoding='utf-8-sig') as f:
-        lines = f.readlines()
-    for line in lines:
-        points = line.split(',')[0:8]
-        word = line.split(',')[9].rstrip('\n').strip('"')
-        difficult = 1 if line.split(',')[8] != '0' else 0
-        segmentation = [int(pt) for pt in points]
-        x = max(0, min(segmentation[0::2]))
-        y = max(0, min(segmentation[1::2]))
-        w = abs(max(segmentation[0::2]) - x)
-        h = abs(max(segmentation[1::2]) - y)
-        bbox = [x, y, w, h]
-
-        if word == '###' or difficult == 1:
-            iscrowd = 1
-        else:
-            iscrowd = 0
-
-        anno = dict(
-            iscrowd=iscrowd,
-            category_id=1,
-            bbox=bbox,
-            area=w * h,
-            segmentation=[segmentation])
-        anno_info.append(anno)
+    with open(gt_file, encoding='unicode_escape') as f:
+        anno_info = []
+        for ann in f.readlines():
+            # skip invalid annotation line
+            try:
+                bbox = np.array(ann.split(',')[0:8]).astype(int).tolist()
+            except ValueError:
+
+                continue
+            word = ann.split(',')[-1].replace('\n', '').strip()
+
+            anno = dict(bbox=bbox, word=word)
+            anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
+def generate_ann(root_path, split, image_infos):
+    """Generate cropped annotations and label txt file.
+
+    Args:
+        root_path (str): The root path of the dataset
+        split (str): The split of dataset. Namely: training or test
+        image_infos (list[dict]): A list of dicts of the img and
+            annotation information
+    """
+
+    dst_image_root = osp.join(root_path, 'crops', split)
+    if split == 'training':
+        dst_label_file = osp.join(root_path, 'train_label.json')
+    elif split == 'test':
+        dst_label_file = osp.join(root_path, 'test_label.json')
+    os.makedirs(dst_image_root, exist_ok=True)
+
+    img_info = []
+    for image_info in image_infos:
+        index = 1
+        src_img_path = osp.join(root_path, 'imgs', split,
+                                image_info['file_name'])
+        image = mmcv.imread(src_img_path)
+        src_img_root = image_info['file_name'].split('.')[0]
+
+        for anno in image_info['anno_info']:
+            word = anno['word']
+            dst_img = crop_img(image, anno['bbox'], 0, 0)
+
+            # Skip invalid annotations
+            if min(dst_img.shape) == 0 or len(word) == 0:
+                continue
+
+            dst_img_name = f'{src_img_root}_{index}.png'
+            index += 1
+            dst_img_path = osp.join(dst_image_root, dst_img_name)
+            mmcv.imwrite(dst_img, dst_img_path)
+
+            img_info.append({
+                'file_name': dst_img_name,
+                'anno_info': [{
+                    'text': word
+                }]
+            })
+
+    dump_ocr_data(img_info, dst_label_file, 'textrecog')
+
+
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of RCTW.')
-    parser.add_argument('root_path', help='Root dir path of RCTW')
-    parser.add_argument(
-        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
+        description='Generate training and test set of SROIE')
+    parser.add_argument('root_path', help='Root dir path of SROIE')
     parser.add_argument(
         '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    ratio = args.val_ratio
-
-    trn_files, val_files = collect_files(
-        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
-
-    # Train set
-    with mmengine.Timer(
-            print_tmpl='It takes {}s to convert RCTW Training annotation'):
-        trn_infos = collect_annotations(trn_files, nproc=args.nproc)
-        dump_ocr_data(trn_infos, osp.join(root_path,
-                                          'instances_training.json'),
-                      'textdet')
 
-    # Val set
-    if len(val_files) > 0:
+    for split in ['training', 'test']:
+        print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert RCTW Val annotation'):
-            val_infos = collect_annotations(val_files, nproc=args.nproc)
-            dump_ocr_data(val_infos, osp.join(root_path, 'instances_val.json'),
-                          'textdet')
+                print_tmpl='It takes {}s to convert SROIE annotation'):
+            files = collect_files(
+                osp.join(root_path, 'imgs', split),
+                osp.join(root_path, 'annotations', split))
+            image_infos = collect_annotations(files, nproc=args.nproc)
+            generate_ann(root_path, split, image_infos)
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/rects_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/rects_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/sroie_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textdet/vintext_converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
 import os
 import os.path as osp
 
 import mmcv
 import mmengine
-import numpy as np
 
 from mmocr.utils import dump_ocr_data
 
 
 def collect_files(img_dir, gt_dir):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
-
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
 
     ann_list, imgs_list = [], []
-    for gt_file in os.listdir(gt_dir):
-        # Filtering repeated and missing images
-        if '(' in gt_file or gt_file == 'X51006619570.txt':
-            continue
-        ann_list.append(osp.join(gt_dir, gt_file))
-        imgs_list.append(osp.join(img_dir, gt_file.replace('.txt', '.jpg')))
+    for img_file in os.listdir(img_dir):
+        ann_file = 'gt_' + str(int(img_file[2:6])) + '.txt'
+        ann_list.append(osp.join(gt_dir, ann_file))
+        imgs_list.append(osp.join(img_dir, img_file))
 
-    files = list(zip(sorted(imgs_list), sorted(ann_list)))
+    files = list(zip(imgs_list, ann_list))
     assert len(files), f'No images found in {img_dir}'
-
     print(f'Loaded {len(files)} images from {img_dir}')
 
     return files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
@@ -48,15 +43,14 @@
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
         nproc (int): The number of process to collect annotations
 
     Returns:
         images (list): The list of image information dicts
     """
-
     assert isinstance(files, list)
     assert isinstance(nproc, int)
 
     if nproc > 1:
         images = mmengine.track_parallel_progress(
             load_img_info, files, nproc=nproc)
     else:
@@ -70,98 +64,107 @@
 
     Args:
         files (tuple): The tuple of (img_file, groundtruth_file)
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
-
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
-    assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
-        '.')[0]
+    assert int(osp.basename(gt_file)[3:-4]) == int(
+        osp.basename(img_file)[2:-4])
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
     img_info = dict(
-        file_name=osp.join(osp.basename(img_file)),
+        file_name=osp.basename(img_file),
         height=img.shape[0],
         width=img.shape[1],
-        segm_file=osp.join(osp.basename(gt_file)))
+        segm_file=osp.basename(gt_file))
 
     if osp.splitext(gt_file)[1] == '.txt':
         img_info = load_txt_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
 def load_txt_info(gt_file, img_info):
     """Collect the annotation information.
 
+    The annotation format is as the following:
+    x1,y1,x2,y2,x3,y3,x4,y4,text
+    118,15,147,15,148,46,118,46,LƯỢNG
+    149,9,165,9,165,43,150,43,TỐT
+    167,9,180,9,179,43,167,42,ĐỂ
+    181,12,193,12,193,43,181,43,CÓ
+    195,13,215,14,215,46,196,46,VIỆC
+    217,13,237,14,239,47,217,46,LÀM,
+
     Args:
-        gt_file (list): The list of tuples (image_file, groundtruth_file)
-        img_info (int): The dict of the img and annotation information
+        gt_file (str): The path to ground-truth
+        img_info (dict): The dict of the img and annotation information
 
     Returns:
-        img_info (list): The dict of the img and annotation information
+        img_info (dict): The dict of the img and annotation information
     """
 
-    with open(gt_file, encoding='unicode_escape') as f:
+    with open(gt_file, encoding='utf-8') as f:
         anno_info = []
-        for ann in f.readlines():
-
-            # annotation format [x1, y1, x2, y2, x3, y3, x4, y4, transcript]
-            try:
-                ann_box = np.array(ann.split(',')[0:8]).astype(int).tolist()
-            except ValueError:
-                # skip invalid annotation line
-                continue
-            x = max(0, min(ann_box[0::2]))
-            y = max(0, min(ann_box[1::2]))
-            w, h = max(ann_box[0::2]) - x, max(ann_box[1::2]) - y
-            bbox = [x, y, w, h]
-            segmentation = ann_box
+        for line in f:
+            line = line.strip('\n')
+            ann = line.split(',')
+            bbox = ann[0:8]
+            word = line[len(','.join(bbox)) + 1:]
+            bbox = [int(coord) for coord in bbox]
+            segmentation = bbox
+            x_min = min(bbox[0], bbox[2], bbox[4], bbox[6])
+            x_max = max(bbox[0], bbox[2], bbox[4], bbox[6])
+            y_min = min(bbox[1], bbox[3], bbox[5], bbox[7])
+            y_max = max(bbox[1], bbox[3], bbox[5], bbox[7])
+            w = x_max - x_min
+            h = y_max - y_min
+            bbox = [x_min, y_min, w, h]
+            iscrowd = 1 if word == '###' else 0
 
             anno = dict(
-                iscrowd=0,
+                iscrowd=iscrowd,
                 category_id=1,
                 bbox=bbox,
                 area=w * h,
                 segmentation=[segmentation])
             anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and test set of SROIE')
-    parser.add_argument('root_path', help='Root dir path of SROIE')
+        description='Generate training and test set of VinText ')
+    parser.add_argument('root_path', help='Root dir path of VinText')
     parser.add_argument(
-        '--nproc', default=1, type=int, help='Number of process')
+        '--nproc', default=1, type=int, help='Number of processes')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-
-    for split in ['training', 'test']:
+    for split in ['training', 'test', 'unseen_test']:
         print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert SROIE annotation'):
+                print_tmpl='It takes {}s to convert VinText annotation'):
             files = collect_files(
                 osp.join(root_path, 'imgs', split),
-                osp.join(root_path, 'annotations', split))
+                osp.join(root_path, 'annotations'))
             image_infos = collect_annotations(files, nproc=args.nproc)
             dump_ocr_data(image_infos,
                           osp.join(root_path, 'instances_' + split + '.json'),
                           'textdet')
 
 
 if __name__ == '__main__':
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textdet/vintext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/vintext_converter.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import os
 import os.path as osp
 
 import mmcv
 import mmengine
 
-from mmocr.utils import dump_ocr_data
+from mmocr.utils import crop_img, dump_ocr_data
 
 
 def collect_files(img_dir, gt_dir):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
@@ -73,18 +73,18 @@
     img_file, gt_file = files
     assert int(osp.basename(gt_file)[3:-4]) == int(
         osp.basename(img_file)[2:-4])
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
     img_info = dict(
-        file_name=osp.basename(img_file),
+        file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
-        segm_file=osp.basename(gt_file))
+        segm_file=osp.join(osp.basename(gt_file)))
 
     if osp.splitext(gt_file)[1] == '.txt':
         img_info = load_txt_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
@@ -114,42 +114,90 @@
         anno_info = []
         for line in f:
             line = line.strip('\n')
             ann = line.split(',')
             bbox = ann[0:8]
             word = line[len(','.join(bbox)) + 1:]
             bbox = [int(coord) for coord in bbox]
-            segmentation = bbox
-            x_min = min(bbox[0], bbox[2], bbox[4], bbox[6])
-            x_max = max(bbox[0], bbox[2], bbox[4], bbox[6])
-            y_min = min(bbox[1], bbox[3], bbox[5], bbox[7])
-            y_max = max(bbox[1], bbox[3], bbox[5], bbox[7])
-            w = x_max - x_min
-            h = y_max - y_min
-            bbox = [x_min, y_min, w, h]
-            iscrowd = 1 if word == '###' else 0
-
-            anno = dict(
-                iscrowd=iscrowd,
-                category_id=1,
-                bbox=bbox,
-                area=w * h,
-                segmentation=[segmentation])
+            # Ignore hard samples
+            if word == '###':
+                continue
+            assert len(bbox) == 8
+            anno = dict(bbox=bbox, word=word)
             anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
+def generate_ann(root_path, split, image_infos, preserve_vertical):
+    """Generate cropped annotations and label txt file.
+
+    Args:
+        root_path (str): The root path of the dataset
+        split (str): The split of dataset. Namely: training or test
+        image_infos (list[dict]): A list of dicts of the img and
+            annotation information
+        preserve_vertical (bool): Whether to preserve vertical texts
+    """
+    dst_image_root = osp.join(root_path, 'crops', split)
+    ignore_image_root = osp.join(root_path, 'ignores', split)
+    if split == 'training':
+        dst_label_file = osp.join(root_path, 'train_label.json')
+    elif split == 'test':
+        dst_label_file = osp.join(root_path, 'test_label.json')
+    elif split == 'unseen_test':
+        dst_label_file = osp.join(root_path, 'unseen_test_label.json')
+    os.makedirs(dst_image_root, exist_ok=True)
+
+    img_info = []
+    for image_info in image_infos:
+        index = 1
+        src_img_path = osp.join(root_path, 'imgs', split,
+                                image_info['file_name'])
+        image = mmcv.imread(src_img_path)
+        src_img_root = image_info['file_name'].split('.')[0]
+
+        for anno in image_info['anno_info']:
+            word = anno['word']
+            dst_img = crop_img(image, anno['bbox'], 0, 0)
+            h, w, _ = dst_img.shape
+
+            dst_img_name = f'{src_img_root}_{index}.png'
+            index += 1
+            # Skip invalid annotations
+            if min(dst_img.shape) == 0:
+                continue
+            # Skip vertical texts
+            if not preserve_vertical and h / w > 2 and split == 'training':
+                dst_img_path = osp.join(ignore_image_root, dst_img_name)
+                mmcv.imwrite(dst_img, dst_img_path)
+                continue
+
+            dst_img_path = osp.join(dst_image_root, dst_img_name)
+            mmcv.imwrite(dst_img, dst_img_path)
+            img_info.append({
+                'file_name': dst_img_name,
+                'anno_info': [{
+                    'text': word
+                }]
+            })
+    dump_ocr_data(img_info, dst_label_file, 'textrecog')
+
+
 def parse_args():
     parser = argparse.ArgumentParser(
         description='Generate training and test set of VinText ')
     parser.add_argument('root_path', help='Root dir path of VinText')
     parser.add_argument(
+        '--preserve-vertical',
+        help='Preserve samples containing vertical texts',
+        action='store_true')
+    parser.add_argument(
         '--nproc', default=1, type=int, help='Number of processes')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
@@ -158,14 +206,12 @@
         print(f'Processing {split} set...')
         with mmengine.Timer(
                 print_tmpl='It takes {}s to convert VinText annotation'):
             files = collect_files(
                 osp.join(root_path, 'imgs', split),
                 osp.join(root_path, 'annotations'))
             image_infos = collect_annotations(files, nproc=args.nproc)
-            dump_ocr_data(image_infos,
-                          osp.join(root_path, 'instances_' + split + '.json'),
-                          'textdet')
+            generate_ann(root_path, split, image_infos, args.preserve_vertical)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/art_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/art_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/bid_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/bid_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/cocotext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/cocotext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/data_migrator.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/data_migrator.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/detext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/detext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/funsd_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/ilst_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import math
 import os
 import os.path as osp
+import xml.etree.ElementTree as ET
 
 import mmcv
 import mmengine
 
 from mmocr.utils import crop_img, dump_ocr_data
 
 
@@ -22,19 +22,21 @@
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
 
     ann_list, imgs_list = [], []
-    for gt_file in os.listdir(gt_dir):
-        ann_list.append(osp.join(gt_dir, gt_file))
-        imgs_list.append(osp.join(img_dir, gt_file.replace('.json', '.png')))
+    for img_file in os.listdir(img_dir):
+        ann_path = osp.join(gt_dir, img_file.split('.')[0] + '.xml')
+        if os.path.exists(ann_path):
+            ann_list.append(ann_path)
+            imgs_list.append(osp.join(img_dir, img_file))
 
-    files = list(zip(sorted(imgs_list), sorted(ann_list)))
+    files = list(zip(imgs_list, ann_list))
     assert len(files), f'No images found in {img_dir}'
     print(f'Loaded {len(files)} images from {img_dir}')
 
     return files
 
 
 def collect_annotations(files, nproc=1):
@@ -72,139 +74,187 @@
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
-    img_info = dict(
-        file_name=osp.join(osp.basename(img_file)),
-        height=img.shape[0],
-        width=img.shape[1],
-        segm_file=osp.join(osp.basename(gt_file)))
+    try:
+        img_info = dict(
+            file_name=osp.join(osp.basename(img_file)),
+            height=img.shape[0],
+            width=img.shape[1],
+            segm_file=osp.join(osp.basename(gt_file)))
+    except AttributeError:
+        print(f'Skip broken img {img_file}')
+        return None
 
-    if osp.splitext(gt_file)[1] == '.json':
-        img_info = load_json_info(gt_file, img_info)
+    if osp.splitext(gt_file)[1] == '.xml':
+        img_info = load_xml_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
-def load_json_info(gt_file, img_info):
+def load_xml_info(gt_file, img_info):
     """Collect the annotation information.
 
+    The annotation format is as the following:
+    <annotations>
+    ...
+        <object>
+            <name>SMT</name>
+            <pose>Unspecified</pose>
+            <truncated>0</truncated>
+            <difficult>0</difficult>
+            <bndbox>
+                <xmin>157</xmin>
+                <ymin>294</ymin>
+                <xmax>237</xmax>
+                <ymax>357</ymax>
+            </bndbox>
+        <object>
+
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
-
-    annotation = mmengine.load(gt_file)
+    obj = ET.parse(gt_file)
+    root = obj.getroot()
     anno_info = []
-    for form in annotation['form']:
-        for ann in form['words']:
-
-            # Ignore illegible samples
-            if len(ann['text']) == 0:
-                continue
-
-            x1, y1, x2, y2 = ann['box']
-            x = max(0, min(math.floor(x1), math.floor(x2)))
-            y = max(0, min(math.floor(y1), math.floor(y2)))
-            w, h = math.ceil(abs(x2 - x1)), math.ceil(abs(y2 - y1))
-            bbox = [x, y, x + w, y, x + w, y + h, x, y + h]
-            word = ann['text']
-
-            anno = dict(bbox=bbox, word=word)
-            anno_info.append(anno)
+    for object in root.iter('object'):
+        word = object.find('name').text
+        x1 = int(object.find('bndbox').find('xmin').text)
+        y1 = int(object.find('bndbox').find('ymin').text)
+        x2 = int(object.find('bndbox').find('xmax').text)
+        y2 = int(object.find('bndbox').find('ymax').text)
+
+        x = max(0, min(x1, x2))
+        y = max(0, min(y1, y2))
+        w, h = abs(x2 - x1), abs(y2 - y1)
+        bbox = [x, y, x + w, y, x + w, y + h, x, y + h]
+        anno = dict(bbox=bbox, word=word)
+        anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
-def generate_ann(root_path, split, image_infos, preserve_vertical):
+def split_train_val_list(full_list, val_ratio):
+    """Split list by val_ratio.
+
+    Args:
+        full_list (list): List to be splited
+        val_ratio (float): Split ratio for val set
+
+    return:
+        list(list, list): Train_list and val_list
+    """
+    n_total = len(full_list)
+    offset = int(n_total * val_ratio)
+    if n_total == 0 or offset < 1:
+        return [], full_list
+    val_list = full_list[:offset]
+    train_list = full_list[offset:]
+    return [train_list, val_list]
+
+
+def generate_ann(root_path, image_infos, preserve_vertical, val_ratio):
     """Generate cropped annotations and label txt file.
 
     Args:
         root_path (str): The root path of the dataset
         split (str): The split of dataset. Namely: training or test
         image_infos (list[dict]): A list of dicts of the img and
             annotation information
         preserve_vertical (bool): Whether to preserve vertical texts
+        val_ratio (float): Split ratio for val set
     """
 
-    dst_image_root = osp.join(root_path, 'crops', split)
-    if split == 'training':
-        dst_label_file = osp.join(root_path, 'train_label.json')
-    elif split == 'test':
-        dst_label_file = osp.join(root_path, 'test_label.json')
-    os.makedirs(dst_image_root, exist_ok=True)
-
-    img_info = []
-    for image_info in image_infos:
-        index = 1
-        src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
-        image = mmcv.imread(src_img_path)
-        src_img_root = image_info['file_name'].split('.')[0]
-
-        for anno in image_info['anno_info']:
-            word = anno['word']
-            dst_img = crop_img(image, anno['bbox'])
-            h, w, _ = dst_img.shape
-
-            # Skip invalid annotations
-            if min(dst_img.shape) == 0:
-                continue
-            # Skip vertical texts
-            if not preserve_vertical and h / w > 2:
-                continue
-
-            dst_img_name = f'{src_img_root}_{index}.png'
-            index += 1
-            dst_img_path = osp.join(dst_image_root, dst_img_name)
-            mmcv.imwrite(dst_img, dst_img_path)
-
-            img_info.append({
-                'file_name': dst_img_name,
-                'anno_info': [{
-                    'text': word
-                }]
-            })
+    assert val_ratio <= 1.
+
+    if val_ratio:
+        image_infos = split_train_val_list(image_infos, val_ratio)
+        splits = ['training', 'val']
+
+    else:
+        image_infos = [image_infos]
+        splits = ['training']
+
+    for i, split in enumerate(splits):
+        dst_image_root = osp.join(root_path, 'crops', split)
+        ignore_image_root = osp.join(root_path, 'ignores', split)
+        dst_label_file = osp.join(root_path, f'{split}_label.json')
+        os.makedirs(dst_image_root, exist_ok=True)
+
+        img_info = []
+        for image_info in image_infos[i]:
+            index = 1
+            src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
+            image = mmcv.imread(src_img_path)
+            src_img_root = image_info['file_name'].split('.')[0]
+
+            for anno in image_info['anno_info']:
+                word = anno['word']
+                dst_img = crop_img(image, anno['bbox'], 0, 0)
+                h, w, _ = dst_img.shape
+
+                dst_img_name = f'{src_img_root}_{index}.png'
+                index += 1
+                # Skip invalid annotations
+                if min(dst_img.shape) == 0:
+                    continue
+                # Skip vertical texts
+                if not preserve_vertical and h / w > 2 and split == 'training':
+                    dst_img_path = osp.join(ignore_image_root, dst_img_name)
+                    mmcv.imwrite(dst_img, dst_img_path)
+                    continue
+
+                dst_img_path = osp.join(dst_image_root, dst_img_name)
+                mmcv.imwrite(dst_img, dst_img_path)
+                img_info.append({
+                    'file_name': dst_img_name,
+                    'anno_info': [{
+                        'text': word
+                    }]
+                })
 
-    dump_ocr_data(img_info, dst_label_file, 'textrecog')
+        ensure_ascii = dict(ensure_ascii=False)
+        dump_ocr_data(img_info, dst_label_file, 'textrecog', **ensure_ascii)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and test set of FUNSD ')
-    parser.add_argument('root_path', help='Root dir path of FUNSD')
+        description='Generate training and val set of ILST ')
+    parser.add_argument('root_path', help='Root dir path of ILST')
     parser.add_argument(
-        '--preserve_vertical',
+        '--preserve-vertical',
         help='Preserve samples containing vertical texts',
         action='store_true')
     parser.add_argument(
+        '--val-ratio', help='Split ratio for val set', default=0., type=float)
+    parser.add_argument(
         '--nproc', default=1, type=int, help='Number of processes')
-    args = parser.parse_args()
+    args = parser.parse_args(['data/IIIT-ILST'])
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-
-    for split in ['training', 'test']:
-        print(f'Processing {split} set...')
-        with mmengine.Timer(
-                print_tmpl='It takes {}s to convert FUNSD annotation'):
-            files = collect_files(
-                osp.join(root_path, 'imgs'),
-                osp.join(root_path, 'annotations', split))
-            image_infos = collect_annotations(files, nproc=args.nproc)
-            generate_ann(root_path, split, image_infos, args.preserve_vertical)
+    with mmengine.Timer(print_tmpl='It takes {}s to convert ILST annotation'):
+        files = collect_files(
+            osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'))
+        image_infos = collect_annotations(files, nproc=args.nproc)
+        # filter broken images
+        image_infos = list(filter(None, image_infos))
+        generate_ann(root_path, image_infos, args.preserve_vertical,
+                     args.val_ratio)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/hiertext_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/hiertext_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/ic11_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/ic11_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/ic13_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/lv_converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,63 +5,64 @@
 from mmocr.utils import dump_ocr_data
 
 
 def convert_annotations(root_path, split):
     """Convert original annotations to mmocr format.
 
     The annotation format is as the following:
-        word_1.png, "flying"
-        word_2.png, "today"
-        word_3.png, "means"
-    See the format of converted annotation in mmocr.utils.dump_ocr_data.
+        Crops/val/11/1/1.png weighted
+        Crops/val/11/1/2.png 26
+        Crops/val/11/1/3.png casting
+        Crops/val/11/1/4.png 28
+    After this module, the annotation has been changed to the format below:
+        jsonl:
+        {'filename': 'Crops/val/11/1/1.png', 'text': 'weighted'}
+        {'filename': 'Crops/val/11/1/1.png', 'text': '26'}
+        {'filename': 'Crops/val/11/1/1.png', 'text': 'casting'}
+        {'filename': 'Crops/val/11/1/1.png', 'text': '28'}
 
     Args:
         root_path (str): The root path of the dataset
         split (str): The split of dataset. Namely: training or test
     """
     assert isinstance(root_path, str)
     assert isinstance(split, str)
 
     img_info = []
     with open(
-            osp.join(root_path, 'annotations',
-                     f'Challenge2_{split}_Task3_GT.txt'),
+            osp.join(root_path, f'{split}_label.txt'),
             encoding='"utf-8-sig') as f:
         annos = f.readlines()
     for anno in annos:
-        seg = ' ' if split == 'Test1015' else ', "'
-        # text may contain comma ','
-        dst_img_name, word = anno.split(seg)
-        word = word.replace('"\n', '')
-
-        img_info.append({
-            'file_name': osp.basename(dst_img_name),
-            'anno_info': [{
-                'text': word
-            }]
-        })
-
-    return img_info
+        if anno:
+            # Text may contain spaces
+            dst_img_name, word = anno.split('png ')
+            word = word.strip('\n')
+            img_info.append({
+                'file_name': dst_img_name + 'png',
+                'anno_info': [{
+                    'text': word
+                }]
+            })
+    dump_ocr_data(img_info, osp.join(root_path, f'{split.lower()}_label.json'),
+                  'textrecog')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and test set of IC13')
-    parser.add_argument('root_path', help='Root dir path of IC13')
+        description='Generate training and test set of Lecture Video DB')
+    parser.add_argument('root_path', help='Root dir path of Lecture Video DB')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
 
-    for split in ['Train', 'Test', 'Test1015']:
-        img_info = convert_annotations(root_path, split)
-        dump_ocr_data(img_info,
-                      osp.join(root_path, f'{split.lower()}_label.json'),
-                      'textrecog')
+    for split in ['train', 'val', 'test']:
+        convert_annotations(root_path, split)
         print(f'{split} split converted.')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/ilst_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/kaist_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
+import math
 import os
 import os.path as osp
 import xml.etree.ElementTree as ET
 
 import mmcv
 import mmengine
 
 from mmocr.utils import crop_img, dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir):
+def collect_files(img_dir, gt_dir, ratio):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
+        ratio (float): Split ratio for val set
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
+    assert isinstance(ratio, float)
+    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
 
     ann_list, imgs_list = [], []
     for img_file in os.listdir(img_dir):
-        ann_path = osp.join(gt_dir, img_file.split('.')[0] + '.xml')
-        if os.path.exists(ann_path):
-            ann_list.append(ann_path)
-            imgs_list.append(osp.join(img_dir, img_file))
-
-    files = list(zip(imgs_list, ann_list))
-    assert len(files), f'No images found in {img_dir}'
-    print(f'Loaded {len(files)} images from {img_dir}')
+        ann_list.append(osp.join(gt_dir, img_file.split('.')[0] + '.xml'))
+        imgs_list.append(osp.join(img_dir, img_file))
 
-    return files
+    all_files = list(zip(sorted(imgs_list), sorted(ann_list)))
+    assert len(all_files), f'No images found in {img_dir}'
+    print(f'Loaded {len(all_files)} images from {img_dir}')
+
+    trn_files, val_files = [], []
+    if ratio > 0:
+        for i, file in enumerate(all_files):
+            if i % math.floor(1 / ratio):
+                trn_files.append(file)
+            else:
+                val_files.append(file)
+    else:
+        trn_files, val_files = all_files, []
+
+    print(f'training #{len(trn_files)}, val #{len(val_files)}')
+
+    return trn_files, val_files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
 
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
@@ -74,187 +88,172 @@
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
     # read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
-    try:
-        img_info = dict(
-            file_name=osp.join(osp.basename(img_file)),
-            height=img.shape[0],
-            width=img.shape[1],
-            segm_file=osp.join(osp.basename(gt_file)))
-    except AttributeError:
-        print(f'Skip broken img {img_file}')
-        return None
+    img_info = dict(
+        file_name=osp.join(osp.basename(img_file)),
+        height=img.shape[0],
+        width=img.shape[1],
+        segm_file=osp.join(osp.basename(gt_file)))
 
     if osp.splitext(gt_file)[1] == '.xml':
         img_info = load_xml_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
 def load_xml_info(gt_file, img_info):
     """Collect the annotation information.
 
-    The annotation format is as the following:
-    <annotations>
-    ...
-        <object>
-            <name>SMT</name>
-            <pose>Unspecified</pose>
-            <truncated>0</truncated>
-            <difficult>0</difficult>
-            <bndbox>
-                <xmin>157</xmin>
-                <ymin>294</ymin>
-                <xmax>237</xmax>
-                <ymax>357</ymax>
-            </bndbox>
-        <object>
+    Annotation Format
+    <image>
+        <imageName>DSC02306.JPG</imageName>
+        <resolution x="640" y="480" />
+        <words>
+            <word x="61" y="140" width="566" height="107">
+                <character x="61" y="147" width="75" height="94" char="C" />
+                <character x="173" y="147" width="77" height="93" char="L" />
+                <character x="251" y="146" width="83" height="96" char="A" />
+                <character x="335" y="146" width="75" height="97" char="V" />
+                <character x="409" y="140" width="52" height="105" char="I" />
+                <character x="464" y="147" width="76" height="96" char="T" />
+                <character x="538" y="154" width="89" height="93" char="A" />
+            </word>
+        </words>
+        <illumination>no</illumination>
+        <difficulty>2</difficulty>
+        <tag>
+        </tag>
+    </image>
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
+
     obj = ET.parse(gt_file)
     root = obj.getroot()
     anno_info = []
-    for object in root.iter('object'):
-        word = object.find('name').text
-        x1 = int(object.find('bndbox').find('xmin').text)
-        y1 = int(object.find('bndbox').find('ymin').text)
-        x2 = int(object.find('bndbox').find('xmax').text)
-        y2 = int(object.find('bndbox').find('ymax').text)
-
-        x = max(0, min(x1, x2))
-        y = max(0, min(y1, y2))
-        w, h = abs(x2 - x1), abs(y2 - y1)
+    for word in root.iter('word'):
+        x, y = max(0, int(word.attrib['x'])), max(0, int(word.attrib['y']))
+        w, h = int(word.attrib['width']), int(word.attrib['height'])
         bbox = [x, y, x + w, y, x + w, y + h, x, y + h]
+        chars = []
+        for character in word.iter('character'):
+            chars.append(character.attrib['char'])
+        word = ''.join(chars)
+        if len(word) == 0:
+            continue
         anno = dict(bbox=bbox, word=word)
         anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
-def split_train_val_list(full_list, val_ratio):
-    """Split list by val_ratio.
-
-    Args:
-        full_list (list): List to be splited
-        val_ratio (float): Split ratio for val set
-
-    return:
-        list(list, list): Train_list and val_list
-    """
-    n_total = len(full_list)
-    offset = int(n_total * val_ratio)
-    if n_total == 0 or offset < 1:
-        return [], full_list
-    val_list = full_list[:offset]
-    train_list = full_list[offset:]
-    return [train_list, val_list]
-
-
-def generate_ann(root_path, image_infos, preserve_vertical, val_ratio):
+def generate_ann(root_path, split, image_infos, preserve_vertical):
     """Generate cropped annotations and label txt file.
 
     Args:
         root_path (str): The root path of the dataset
         split (str): The split of dataset. Namely: training or test
         image_infos (list[dict]): A list of dicts of the img and
             annotation information
         preserve_vertical (bool): Whether to preserve vertical texts
-        val_ratio (float): Split ratio for val set
+        format (str): Annotation format, should be either 'txt' or 'jsonl'
     """
 
-    assert val_ratio <= 1.
-
-    if val_ratio:
-        image_infos = split_train_val_list(image_infos, val_ratio)
-        splits = ['training', 'val']
-
-    else:
-        image_infos = [image_infos]
-        splits = ['training']
+    dst_image_root = osp.join(root_path, 'crops', split)
+    ignore_image_root = osp.join(root_path, 'ignores', split)
+    if split == 'training':
+        dst_label_file = osp.join(root_path, 'train_label.json')
+    elif split == 'val':
+        dst_label_file = osp.join(root_path, 'val_label.json')
+    mmengine.mkdir_or_exist(dst_image_root)
+    mmengine.mkdir_or_exist(ignore_image_root)
+
+    img_info = []
+    for image_info in image_infos:
+        index = 1
+        src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
+        image = mmcv.imread(src_img_path)
+        src_img_root = image_info['file_name'].split('.')[0]
+
+        for anno in image_info['anno_info']:
+            word = anno['word']
+            dst_img = crop_img(image, anno['bbox'], 0, 0)
+            h, w, _ = dst_img.shape
+
+            dst_img_name = f'{src_img_root}_{index}.png'
+            index += 1
+            # Skip invalid annotations
+            if min(dst_img.shape) == 0:
+                continue
+            # Filter out vertical texts
+            if not preserve_vertical and h / w > 2:
+                dst_img_path = osp.join(ignore_image_root, dst_img_name)
+                mmcv.imwrite(dst_img, dst_img_path)
+                continue
 
-    for i, split in enumerate(splits):
-        dst_image_root = osp.join(root_path, 'crops', split)
-        ignore_image_root = osp.join(root_path, 'ignores', split)
-        dst_label_file = osp.join(root_path, f'{split}_label.json')
-        os.makedirs(dst_image_root, exist_ok=True)
-
-        img_info = []
-        for image_info in image_infos[i]:
-            index = 1
-            src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
-            image = mmcv.imread(src_img_path)
-            src_img_root = image_info['file_name'].split('.')[0]
-
-            for anno in image_info['anno_info']:
-                word = anno['word']
-                dst_img = crop_img(image, anno['bbox'], 0, 0)
-                h, w, _ = dst_img.shape
-
-                dst_img_name = f'{src_img_root}_{index}.png'
-                index += 1
-                # Skip invalid annotations
-                if min(dst_img.shape) == 0:
-                    continue
-                # Skip vertical texts
-                if not preserve_vertical and h / w > 2 and split == 'training':
-                    dst_img_path = osp.join(ignore_image_root, dst_img_name)
-                    mmcv.imwrite(dst_img, dst_img_path)
-                    continue
+            dst_img_path = osp.join(dst_image_root, dst_img_name)
+            mmcv.imwrite(dst_img, dst_img_path)
 
-                dst_img_path = osp.join(dst_image_root, dst_img_name)
-                mmcv.imwrite(dst_img, dst_img_path)
-                img_info.append({
-                    'file_name': dst_img_name,
-                    'anno_info': [{
-                        'text': word
-                    }]
-                })
+            img_info.append({
+                'file_name': dst_img_name,
+                'anno_info': [{
+                    'text': word
+                }]
+            })
 
-        ensure_ascii = dict(ensure_ascii=False)
-        dump_ocr_data(img_info, dst_label_file, 'textrecog', **ensure_ascii)
+    ensure_ascii = dict(ensure_ascii=False)
+    dump_ocr_data(img_info, dst_label_file, 'textrecog', **ensure_ascii)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of ILST ')
-    parser.add_argument('root_path', help='Root dir path of ILST')
+        description='Generate training and val set of KAIST ')
+    parser.add_argument('root_path', help='Root dir path of KAIST')
+    parser.add_argument(
+        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
     parser.add_argument(
         '--preserve-vertical',
         help='Preserve samples containing vertical texts',
         action='store_true')
     parser.add_argument(
-        '--val-ratio', help='Split ratio for val set', default=0., type=float)
-    parser.add_argument(
-        '--nproc', default=1, type=int, help='Number of processes')
-    args = parser.parse_args(['data/IIIT-ILST'])
+        '--nproc', default=1, type=int, help='Number of process')
+    args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    with mmengine.Timer(print_tmpl='It takes {}s to convert ILST annotation'):
-        files = collect_files(
-            osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'))
-        image_infos = collect_annotations(files, nproc=args.nproc)
-        # filter broken images
-        image_infos = list(filter(None, image_infos))
-        generate_ann(root_path, image_infos, args.preserve_vertical,
-                     args.val_ratio)
+    ratio = args.val_ratio
+
+    trn_files, val_files = collect_files(
+        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
+
+    # Train set
+    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
+    with mmengine.Timer(
+            print_tmpl='It takes {}s to convert KAIST Training annotation'):
+        generate_ann(root_path, 'training', trn_infos, args.preserve_vertical)
+
+    # Val set
+    if len(val_files) > 0:
+        val_infos = collect_annotations(val_files, nproc=args.nproc)
+        with mmengine.Timer(
+                print_tmpl='It takes {}s to convert KAIST Val annotation'):
+            generate_ann(root_path, 'val', val_infos, args.preserve_vertical)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/imgur_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/imgur_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/kaist_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/naf_converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
-import math
-import os
 import os.path as osp
-import xml.etree.ElementTree as ET
 
 import mmcv
 import mmengine
+import numpy as np
 
 from mmocr.utils import crop_img, dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, ratio):
+def collect_files(img_dir, gt_dir, split_info):
     """Collect all images and their corresponding groundtruth files.
 
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
-        ratio (float): Split ratio for val set
+        split_info (dict): The split information for train/val/test
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
-    assert isinstance(ratio, float)
-    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
+    assert isinstance(split_info, dict)
+    assert split_info
 
     ann_list, imgs_list = [], []
-    for img_file in os.listdir(img_dir):
-        ann_list.append(osp.join(gt_dir, img_file.split('.')[0] + '.xml'))
-        imgs_list.append(osp.join(img_dir, img_file))
-
-    all_files = list(zip(sorted(imgs_list), sorted(ann_list)))
-    assert len(all_files), f'No images found in {img_dir}'
-    print(f'Loaded {len(all_files)} images from {img_dir}')
-
-    trn_files, val_files = [], []
-    if ratio > 0:
-        for i, file in enumerate(all_files):
-            if i % math.floor(1 / ratio):
-                trn_files.append(file)
-            else:
-                val_files.append(file)
-    else:
-        trn_files, val_files = all_files, []
+    for group in split_info:
+        for img in split_info[group]:
+            image_path = osp.join(img_dir, img)
+            anno_path = osp.join(gt_dir, 'groups', group,
+                                 img.replace('jpg', 'json'))
+
+            # Filtering out the missing images
+            if not osp.exists(image_path) or not osp.exists(anno_path):
+                continue
+
+            imgs_list.append(image_path)
+            ann_list.append(anno_path)
 
-    print(f'training #{len(trn_files)}, val #{len(val_files)}')
+    files = list(zip(imgs_list, ann_list))
+    assert len(files), f'No images found in {img_dir}'
+    print(f'Loaded {len(files)} images from {img_dir}')
 
-    return trn_files, val_files
+    return files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
 
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
@@ -85,78 +80,94 @@
         img_info (dict): The dict of the img and annotation information
     """
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
-    # read imgs while ignoring orientations
+    # Read imgs while ignoring orientations
     img = mmcv.imread(img_file, 'unchanged')
 
     img_info = dict(
         file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
-    if osp.splitext(gt_file)[1] == '.xml':
-        img_info = load_xml_info(gt_file, img_info)
+    if osp.splitext(gt_file)[1] == '.json':
+        img_info = load_json_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
-def load_xml_info(gt_file, img_info):
+def load_json_info(gt_file, img_info):
     """Collect the annotation information.
 
     Annotation Format
-    <image>
-        <imageName>DSC02306.JPG</imageName>
-        <resolution x="640" y="480" />
-        <words>
-            <word x="61" y="140" width="566" height="107">
-                <character x="61" y="147" width="75" height="94" char="C" />
-                <character x="173" y="147" width="77" height="93" char="L" />
-                <character x="251" y="146" width="83" height="96" char="A" />
-                <character x="335" y="146" width="75" height="97" char="V" />
-                <character x="409" y="140" width="52" height="105" char="I" />
-                <character x="464" y="147" width="76" height="96" char="T" />
-                <character x="538" y="154" width="89" height="93" char="A" />
-            </word>
-        </words>
-        <illumination>no</illumination>
-        <difficulty>2</difficulty>
-        <tag>
-        </tag>
-    </image>
+    {
+        'filedBBs': [{
+            'poly_points': [[435,1406], [466,1406], [466,1439], [435,1439]],
+            "type": "fieldCheckBox",
+            "id": "f0",
+            "isBlank": 1, # 0:text,1:handwriting,2:print,3:blank,4:signature,
+        }], ...
+        "transcriptions":{
+            "f38": "CASE NUMBER",
+            "f29": "July 1, 1949",
+            "t20": "RANK",
+            "t19": "COMPANY",
+            ...
+        }
+    }
+
+    Some special characters are used in the transcription:
+    "«text»" indicates that "text" had a strikethrough
+    "¿" indicates the transcriber could not read a character
+    "§" indicates the whole line or word was illegible
+    "" (empty string) is if the field was blank
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
+    assert isinstance(gt_file, str)
+    assert isinstance(img_info, dict)
 
-    obj = ET.parse(gt_file)
-    root = obj.getroot()
+    annotation = mmengine.load(gt_file)
     anno_info = []
-    for word in root.iter('word'):
-        x, y = max(0, int(word.attrib['x'])), max(0, int(word.attrib['y']))
-        w, h = int(word.attrib['width']), int(word.attrib['height'])
-        bbox = [x, y, x + w, y, x + w, y + h, x, y + h]
-        chars = []
-        for character in word.iter('character'):
-            chars.append(character.attrib['char'])
-        word = ''.join(chars)
-        if len(word) == 0:
+
+    # 'textBBs' contains the printed texts of the table while 'fieldBBs'
+    #  contains the text filled by human.
+    for box_type in ['textBBs', 'fieldBBs']:
+        # NAF dataset only provides transcription GT for 'filedBBs', the
+        # 'textBBs' is only used for detection task.
+        if box_type == 'textBBs':
             continue
-        anno = dict(bbox=bbox, word=word)
-        anno_info.append(anno)
+        for anno in annotation[box_type]:
+            # Skip images containing detection annotations only
+            if 'transcriptions' not in annotation.keys():
+                continue
+            # Skip boxes without recognition GT
+            if anno['id'] not in annotation['transcriptions'].keys():
+                continue
+
+            word = annotation['transcriptions'][anno['id']]
+            # Skip blank boxes
+            if len(word) == 0:
+                continue
+
+            bbox = np.array(anno['poly_points']).reshape(1, 8)[0].tolist()
+
+            anno = dict(bbox=bbox, word=word)
+            anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def generate_ann(root_path, split, image_infos, preserve_vertical):
@@ -164,96 +175,98 @@
 
     Args:
         root_path (str): The root path of the dataset
         split (str): The split of dataset. Namely: training or test
         image_infos (list[dict]): A list of dicts of the img and
             annotation information
         preserve_vertical (bool): Whether to preserve vertical texts
-        format (str): Annotation format, should be either 'txt' or 'jsonl'
     """
 
     dst_image_root = osp.join(root_path, 'crops', split)
     ignore_image_root = osp.join(root_path, 'ignores', split)
     if split == 'training':
         dst_label_file = osp.join(root_path, 'train_label.json')
     elif split == 'val':
         dst_label_file = osp.join(root_path, 'val_label.json')
+    elif split == 'test':
+        dst_label_file = osp.join(root_path, 'test_label.json')
+    else:
+        raise NotImplementedError
     mmengine.mkdir_or_exist(dst_image_root)
     mmengine.mkdir_or_exist(ignore_image_root)
 
     img_info = []
     for image_info in image_infos:
         index = 1
         src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
         image = mmcv.imread(src_img_path)
         src_img_root = image_info['file_name'].split('.')[0]
 
         for anno in image_info['anno_info']:
             word = anno['word']
+            word = word.strip('\u202a')  # Remove unicode control character
+            word = word.replace('»',
+                                '').replace('«',
+                                            '')  # Remove strikethrough flag
             dst_img = crop_img(image, anno['bbox'], 0, 0)
             h, w, _ = dst_img.shape
 
             dst_img_name = f'{src_img_root}_{index}.png'
             index += 1
-            # Skip invalid annotations
-            if min(dst_img.shape) == 0:
+            # Skip invalid and illegible annotations
+            if min(dst_img.shape) == 0 or '§' in word or '¿' in word or len(
+                    word) == 0:
                 continue
-            # Filter out vertical texts
-            if not preserve_vertical and h / w > 2:
+            # Skip vertical texts
+            # (Do Not Filter For Val and Test Split)
+            if (not preserve_vertical and h / w > 2) and split == 'training':
                 dst_img_path = osp.join(ignore_image_root, dst_img_name)
                 mmcv.imwrite(dst_img, dst_img_path)
                 continue
 
             dst_img_path = osp.join(dst_image_root, dst_img_name)
             mmcv.imwrite(dst_img, dst_img_path)
 
             img_info.append({
                 'file_name': dst_img_name,
                 'anno_info': [{
                     'text': word
                 }]
             })
 
-    ensure_ascii = dict(ensure_ascii=False)
-    dump_ocr_data(img_info, dst_label_file, 'textrecog', **ensure_ascii)
+    dump_ocr_data(img_info, dst_label_file, 'textrecog')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of KAIST ')
-    parser.add_argument('root_path', help='Root dir path of KAIST')
-    parser.add_argument(
-        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
+        description='Generate training, val, and test set of NAF ')
+    parser.add_argument('root_path', help='Root dir path of NAF')
     parser.add_argument(
         '--preserve-vertical',
         help='Preserve samples containing vertical texts',
         action='store_true')
     parser.add_argument(
         '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    ratio = args.val_ratio
-
-    trn_files, val_files = collect_files(
-        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
-
-    # Train set
-    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
-    with mmengine.Timer(
-            print_tmpl='It takes {}s to convert KAIST Training annotation'):
-        generate_ann(root_path, 'training', trn_infos, args.preserve_vertical)
-
-    # Val set
-    if len(val_files) > 0:
-        val_infos = collect_annotations(val_files, nproc=args.nproc)
+    split_info = mmengine.load(
+        osp.join(root_path, 'annotations', 'train_valid_test_split.json'))
+    split_info['training'] = split_info.pop('train')
+    split_info['val'] = split_info.pop('valid')
+    for split in ['training', 'val', 'test']:
+        print(f'Processing {split} set...')
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert KAIST Val annotation'):
-            generate_ann(root_path, 'val', val_infos, args.preserve_vertical)
+                print_tmpl='It takes {}s to convert NAF annotation'):
+            files = collect_files(
+                osp.join(root_path, 'imgs'),
+                osp.join(root_path, 'annotations'), split_info[split])
+            image_infos = collect_annotations(files, nproc=args.nproc)
+            generate_ann(root_path, split, image_infos, args.preserve_vertical)
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/lmdb_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/lmdb_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/lsvt_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/lsvt_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/mtwi_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/mtwi_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/naf_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/rctw_converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
+import math
+import os
 import os.path as osp
 
 import mmcv
 import mmengine
-import numpy as np
 
 from mmocr.utils import crop_img, dump_ocr_data
 
 
-def collect_files(img_dir, gt_dir, split_info):
+def collect_files(img_dir, gt_dir, ratio):
     """Collect all images and their corresponding groundtruth files.
-
     Args:
         img_dir (str): The image directory
         gt_dir (str): The groundtruth directory
-        split_info (dict): The split information for train/val/test
+        ratio (float): Split ratio for val set
 
     Returns:
         files (list): The list of tuples (img_file, groundtruth_file)
     """
     assert isinstance(img_dir, str)
     assert img_dir
     assert isinstance(gt_dir, str)
     assert gt_dir
-    assert isinstance(split_info, dict)
-    assert split_info
+    assert isinstance(ratio, float)
+    assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
 
     ann_list, imgs_list = [], []
-    for group in split_info:
-        for img in split_info[group]:
-            image_path = osp.join(img_dir, img)
-            anno_path = osp.join(gt_dir, 'groups', group,
-                                 img.replace('jpg', 'json'))
-
-            # Filtering out the missing images
-            if not osp.exists(image_path) or not osp.exists(anno_path):
-                continue
-
-            imgs_list.append(image_path)
-            ann_list.append(anno_path)
+    for ann_file in os.listdir(gt_dir):
+        ann_list.append(osp.join(gt_dir, ann_file))
+        imgs_list.append(osp.join(img_dir, ann_file.replace('txt', 'jpg')))
+
+    all_files = list(zip(imgs_list, ann_list))
+    assert len(all_files), f'No images found in {img_dir}'
+    print(f'Loaded {len(all_files)} images from {img_dir}')
+
+    trn_files, val_files = [], []
+    if ratio > 0:
+        for i, file in enumerate(all_files):
+            if i % math.floor(1 / ratio):
+                trn_files.append(file)
+            else:
+                val_files.append(file)
+    else:
+        trn_files, val_files = all_files, []
 
-    files = list(zip(imgs_list, ann_list))
-    assert len(files), f'No images found in {img_dir}'
-    print(f'Loaded {len(files)} images from {img_dir}')
+    print(f'training #{len(trn_files)}, val #{len(val_files)}')
 
-    return files
+    return trn_files, val_files
 
 
 def collect_annotations(files, nproc=1):
     """Collect the annotation information.
-
     Args:
         files (list): The list of tuples (image_file, groundtruth_file)
         nproc (int): The number of process to collect annotations
 
     Returns:
         images (list): The list of image information dicts
     """
@@ -68,161 +70,119 @@
         images = mmengine.track_progress(load_img_info, files)
 
     return images
 
 
 def load_img_info(files):
     """Load the information of one image.
-
     Args:
         files (tuple): The tuple of (img_file, groundtruth_file)
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
     assert isinstance(files, tuple)
 
     img_file, gt_file = files
     assert osp.basename(gt_file).split('.')[0] == osp.basename(img_file).split(
         '.')[0]
-    # Read imgs while ignoring orientations
-    img = mmcv.imread(img_file, 'unchanged')
+    # read imgs while ignoring orientations
+    img = mmcv.imread(img_file)
 
     img_info = dict(
         file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
-    if osp.splitext(gt_file)[1] == '.json':
-        img_info = load_json_info(gt_file, img_info)
+    if osp.splitext(gt_file)[1] == '.txt':
+        img_info = load_txt_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
-def load_json_info(gt_file, img_info):
+def load_txt_info(gt_file, img_info):
     """Collect the annotation information.
 
-    Annotation Format
-    {
-        'filedBBs': [{
-            'poly_points': [[435,1406], [466,1406], [466,1439], [435,1439]],
-            "type": "fieldCheckBox",
-            "id": "f0",
-            "isBlank": 1, # 0:text,1:handwriting,2:print,3:blank,4:signature,
-        }], ...
-        "transcriptions":{
-            "f38": "CASE NUMBER",
-            "f29": "July 1, 1949",
-            "t20": "RANK",
-            "t19": "COMPANY",
-            ...
-        }
-    }
-
-    Some special characters are used in the transcription:
-    "«text»" indicates that "text" had a strikethrough
-    "¿" indicates the transcriber could not read a character
-    "§" indicates the whole line or word was illegible
-    "" (empty string) is if the field was blank
+    The annotation format is as the following:
+    x1, y1, x2, y2, x3, y3, x4, y4, difficult, text
+
+    390,902,1856,902,1856,1225,390,1225,0,"金氏眼镜"
+    1875,1170,2149,1170,2149,1245,1875,1245,0,"创于1989"
+    2054,1277,2190,1277,2190,1323,2054,1323,0,"城建店"
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
-    assert isinstance(gt_file, str)
-    assert isinstance(img_info, dict)
 
-    annotation = mmengine.load(gt_file)
     anno_info = []
+    with open(gt_file, encoding='utf-8-sig') as f:
+        lines = f.readlines()
+    for line in lines:
+        points = line.split(',')[0:8]
+        word = line.split(',')[9].rstrip('\n').strip('"')
+        difficult = 1 if line.split(',')[8] != '0' else 0
+        bbox = [int(pt) for pt in points]
 
-    # 'textBBs' contains the printed texts of the table while 'fieldBBs'
-    #  contains the text filled by human.
-    for box_type in ['textBBs', 'fieldBBs']:
-        # NAF dataset only provides transcription GT for 'filedBBs', the
-        # 'textBBs' is only used for detection task.
-        if box_type == 'textBBs':
+        if word == '###' or difficult == 1:
             continue
-        for anno in annotation[box_type]:
-            # Skip images containing detection annotations only
-            if 'transcriptions' not in annotation.keys():
-                continue
-            # Skip boxes without recognition GT
-            if anno['id'] not in annotation['transcriptions'].keys():
-                continue
-
-            word = annotation['transcriptions'][anno['id']]
-            # Skip blank boxes
-            if len(word) == 0:
-                continue
 
-            bbox = np.array(anno['poly_points']).reshape(1, 8)[0].tolist()
-
-            anno = dict(bbox=bbox, word=word)
-            anno_info.append(anno)
+        anno = dict(bbox=bbox, word=word)
+        anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def generate_ann(root_path, split, image_infos, preserve_vertical):
     """Generate cropped annotations and label txt file.
 
     Args:
         root_path (str): The root path of the dataset
-        split (str): The split of dataset. Namely: training or test
+        split (str): The split of dataset. Namely: training or val
         image_infos (list[dict]): A list of dicts of the img and
             annotation information
         preserve_vertical (bool): Whether to preserve vertical texts
     """
 
     dst_image_root = osp.join(root_path, 'crops', split)
     ignore_image_root = osp.join(root_path, 'ignores', split)
     if split == 'training':
         dst_label_file = osp.join(root_path, 'train_label.json')
     elif split == 'val':
         dst_label_file = osp.join(root_path, 'val_label.json')
-    elif split == 'test':
-        dst_label_file = osp.join(root_path, 'test_label.json')
-    else:
-        raise NotImplementedError
     mmengine.mkdir_or_exist(dst_image_root)
     mmengine.mkdir_or_exist(ignore_image_root)
 
     img_info = []
     for image_info in image_infos:
         index = 1
         src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
         image = mmcv.imread(src_img_path)
         src_img_root = image_info['file_name'].split('.')[0]
 
         for anno in image_info['anno_info']:
             word = anno['word']
-            word = word.strip('\u202a')  # Remove unicode control character
-            word = word.replace('»',
-                                '').replace('«',
-                                            '')  # Remove strikethrough flag
             dst_img = crop_img(image, anno['bbox'], 0, 0)
             h, w, _ = dst_img.shape
 
             dst_img_name = f'{src_img_root}_{index}.png'
             index += 1
-            # Skip invalid and illegible annotations
-            if min(dst_img.shape) == 0 or '§' in word or '¿' in word or len(
-                    word) == 0:
+            # Skip invalid annotations
+            if min(dst_img.shape) == 0:
                 continue
-            # Skip vertical texts
-            # (Do Not Filter For Val and Test Split)
-            if (not preserve_vertical and h / w > 2) and split == 'training':
+            # Filter out vertical texts
+            if not preserve_vertical and h / w > 2:
                 dst_img_path = osp.join(ignore_image_root, dst_img_name)
                 mmcv.imwrite(dst_img, dst_img_path)
                 continue
 
             dst_img_path = osp.join(dst_image_root, dst_img_name)
             mmcv.imwrite(dst_img, dst_img_path)
 
@@ -234,39 +194,45 @@
             })
 
     dump_ocr_data(img_info, dst_label_file, 'textrecog')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training, val, and test set of NAF ')
-    parser.add_argument('root_path', help='Root dir path of NAF')
+        description='Generate training and val set of RCTW.')
+    parser.add_argument('root_path', help='Root dir path of RCTW')
+    parser.add_argument(
+        '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
+    parser.add_argument(
+        '--nproc', default=1, type=int, help='Number of process')
     parser.add_argument(
         '--preserve-vertical',
         help='Preserve samples containing vertical texts',
         action='store_true')
-    parser.add_argument(
-        '--nproc', default=1, type=int, help='Number of process')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     root_path = args.root_path
-    split_info = mmengine.load(
-        osp.join(root_path, 'annotations', 'train_valid_test_split.json'))
-    split_info['training'] = split_info.pop('train')
-    split_info['val'] = split_info.pop('valid')
-    for split in ['training', 'val', 'test']:
-        print(f'Processing {split} set...')
+    ratio = args.val_ratio
+
+    trn_files, val_files = collect_files(
+        osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
+
+    # Train set
+    with mmengine.Timer(
+            print_tmpl='It takes {}s to convert RCTW Training annotation'):
+        trn_infos = collect_annotations(trn_files, nproc=args.nproc)
+        generate_ann(root_path, 'training', trn_infos, args.preserve_vertical)
+
+    # Val set
+    if len(val_files) > 0:
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert NAF annotation'):
-            files = collect_files(
-                osp.join(root_path, 'imgs'),
-                osp.join(root_path, 'annotations'), split_info[split])
-            image_infos = collect_annotations(files, nproc=args.nproc)
-            generate_ann(root_path, split, image_infos, args.preserve_vertical)
+                print_tmpl='It takes {}s to convert RCTW Val annotation'):
+            val_infos = collect_annotations(val_files, nproc=args.nproc)
+            generate_ann(root_path, 'val', val_infos, args.preserve_vertical)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/openvino_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/openvino_converter.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/dataset_converters/textrecog/rctw_converter.py` & `mmocr-1.0.1/mmocr/.mim/tools/dataset_converters/textrecog/rects_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     assert gt_dir
     assert isinstance(ratio, float)
     assert ratio < 1.0, 'val_ratio should be a float between 0.0 to 1.0'
 
     ann_list, imgs_list = [], []
     for ann_file in os.listdir(gt_dir):
         ann_list.append(osp.join(gt_dir, ann_file))
-        imgs_list.append(osp.join(img_dir, ann_file.replace('txt', 'jpg')))
+        imgs_list.append(osp.join(img_dir, ann_file.replace('json', 'jpg')))
 
     all_files = list(zip(imgs_list, ann_list))
     assert len(all_files), f'No images found in {img_dir}'
     print(f'Loaded {len(all_files)} images from {img_dir}')
 
     trn_files, val_files = [], []
     if ratio > 0:
@@ -90,77 +90,95 @@
 
     img_info = dict(
         file_name=osp.join(osp.basename(img_file)),
         height=img.shape[0],
         width=img.shape[1],
         segm_file=osp.join(osp.basename(gt_file)))
 
-    if osp.splitext(gt_file)[1] == '.txt':
-        img_info = load_txt_info(gt_file, img_info)
+    if osp.splitext(gt_file)[1] == '.json':
+        img_info = load_json_info(gt_file, img_info)
     else:
         raise NotImplementedError
 
     return img_info
 
 
-def load_txt_info(gt_file, img_info):
+def load_json_info(gt_file, img_info):
     """Collect the annotation information.
 
     The annotation format is as the following:
-    x1, y1, x2, y2, x3, y3, x4, y4, difficult, text
 
-    390,902,1856,902,1856,1225,390,1225,0,"金氏眼镜"
-    1875,1170,2149,1170,2149,1245,1875,1245,0,"创于1989"
-    2054,1277,2190,1277,2190,1323,2054,1323,0,"城建店"
+    {
+        "chars": [
+            {
+                "ignore": 0,
+                "transcription": "H",
+                "points": [25, 175, 112, 175, 112, 286, 25, 286]
+            },
+            {
+                "ignore": 0,
+                "transcription": "O",
+                "points": [102, 182, 210, 182, 210, 273, 102, 273]
+            }, ...
+        ]
+        "lines": [
+            {
+                "ignore": 0,
+                "transcription": "HOKI",
+                "points": [23, 173, 327, 180, 327, 290, 23, 283]
+            },
+            {
+                "ignore": 0,
+                "transcription": "TEA",
+                "points": [368, 180, 621, 180, 621, 294, 368, 294]
+            }, ...
+        ]
+    }
+
 
     Args:
         gt_file (str): The path to ground-truth
         img_info (dict): The dict of the img and annotation information
 
     Returns:
         img_info (dict): The dict of the img and annotation information
     """
 
+    annotation = mmengine.load(gt_file)
     anno_info = []
-    with open(gt_file, encoding='utf-8-sig') as f:
-        lines = f.readlines()
-    for line in lines:
-        points = line.split(',')[0:8]
-        word = line.split(',')[9].rstrip('\n').strip('"')
-        difficult = 1 if line.split(',')[8] != '0' else 0
-        bbox = [int(pt) for pt in points]
-
-        if word == '###' or difficult == 1:
+    for line in annotation['lines']:
+        if line['ignore'] == 1:
             continue
-
-        anno = dict(bbox=bbox, word=word)
+        segmentation = line['points']
+        word = line['transcription']
+        anno = dict(bbox=segmentation, word=word)
         anno_info.append(anno)
 
     img_info.update(anno_info=anno_info)
 
     return img_info
 
 
 def generate_ann(root_path, split, image_infos, preserve_vertical):
     """Generate cropped annotations and label txt file.
 
     Args:
         root_path (str): The root path of the dataset
-        split (str): The split of dataset. Namely: training or val
+        split (str): The split of dataset. Namely: training or test
         image_infos (list[dict]): A list of dicts of the img and
             annotation information
         preserve_vertical (bool): Whether to preserve vertical texts
     """
-
+    print('Cropping images...')
     dst_image_root = osp.join(root_path, 'crops', split)
     ignore_image_root = osp.join(root_path, 'ignores', split)
     if split == 'training':
-        dst_label_file = osp.join(root_path, f'train_label.{format}')
+        dst_label_file = osp.join(root_path, 'train_label.json')
     elif split == 'val':
-        dst_label_file = osp.join(root_path, f'val_label.{format}')
+        dst_label_file = osp.join(root_path, 'val_label.json')
     mmengine.mkdir_or_exist(dst_image_root)
     mmengine.mkdir_or_exist(ignore_image_root)
 
     img_info = []
     for image_info in image_infos:
         index = 1
         src_img_path = osp.join(root_path, 'imgs', image_info['file_name'])
@@ -173,16 +191,16 @@
             h, w, _ = dst_img.shape
 
             dst_img_name = f'{src_img_root}_{index}.png'
             index += 1
             # Skip invalid annotations
             if min(dst_img.shape) == 0:
                 continue
-            # Filter out vertical texts
-            if not preserve_vertical and h / w > 2:
+            # Skip vertical texts
+            if not preserve_vertical and h / w > 2 and split == 'training':
                 dst_img_path = osp.join(ignore_image_root, dst_img_name)
                 mmcv.imwrite(dst_img, dst_img_path)
                 continue
 
             dst_img_path = osp.join(dst_image_root, dst_img_name)
             mmcv.imwrite(dst_img, dst_img_path)
 
@@ -194,16 +212,16 @@
             })
 
     dump_ocr_data(img_info, dst_label_file, 'textrecog')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description='Generate training and val set of RCTW.')
-    parser.add_argument('root_path', help='Root dir path of RCTW')
+        description='Generate training and val set of ReCTS.')
+    parser.add_argument('root_path', help='Root dir path of ReCTS')
     parser.add_argument(
         '--val-ratio', help='Split ratio for val set', default=0.0, type=float)
     parser.add_argument(
         '--nproc', default=1, type=int, help='Number of process')
     parser.add_argument(
         '--preserve-vertical',
         help='Preserve samples containing vertical texts',
@@ -217,22 +235,22 @@
     root_path = args.root_path
     ratio = args.val_ratio
 
     trn_files, val_files = collect_files(
         osp.join(root_path, 'imgs'), osp.join(root_path, 'annotations'), ratio)
 
     # Train set
+    trn_infos = collect_annotations(trn_files, nproc=args.nproc)
     with mmengine.Timer(
-            print_tmpl='It takes {}s to convert RCTW Training annotation'):
-        trn_infos = collect_annotations(trn_files, nproc=args.nproc)
+            print_tmpl='It takes {}s to convert ReCTS Training annotation'):
         generate_ann(root_path, 'training', trn_infos, args.preserve_vertical)
 
     # Val set
     if len(val_files) > 0:
+        val_infos = collect_annotations(val_files, nproc=args.nproc)
         with mmengine.Timer(
-                print_tmpl='It takes {}s to convert RCTW Val annotation'):
-            val_infos = collect_annotations(val_files, nproc=args.nproc)
+                print_tmpl='It takes {}s to convert ReCTS Val annotation'):
             generate_ann(root_path, 'val', val_infos, args.preserve_vertical)
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/infer.py` & `mmocr-1.0.1/mmocr/.mim/tools/infer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/model_converters/publish_model.py` & `mmocr-1.0.1/mmocr/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/slurm_train.sh` & `mmocr-1.0.1/mmocr/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/test.py` & `mmocr-1.0.1/mmocr/.mim/tools/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,18 @@
     parser.add_argument(
         '--launcher',
         choices=['none', 'pytorch', 'slurm', 'mpi'],
         default='none',
         help='Job launcher')
     parser.add_argument(
         '--tta', action='store_true', help='Test time augmentation')
-    parser.add_argument('--local_rank', type=int, default=0)
+    # When using PyTorch version >= 2.0.0, the `torch.distributed.launch`
+    # will pass the `--local-rank` parameter to `tools/test.py` instead
+    # of `--local_rank`.
+    parser.add_argument('--local_rank', '--local-rank', type=int, default=0)
     args = parser.parse_args()
     if 'LOCAL_RANK' not in os.environ:
         os.environ['LOCAL_RANK'] = str(args.local_rank)
     return args
 
 
 def trigger_visualization_hook(cfg, args):
```

### Comparing `mmocr-1.0.0rc6/mmocr/.mim/tools/train.py` & `mmocr-1.0.1/mmocr/.mim/tools/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,18 @@
         'Note that the quotation marks are necessary and that no white space '
         'is allowed.')
     parser.add_argument(
         '--launcher',
         choices=['none', 'pytorch', 'slurm', 'mpi'],
         default='none',
         help='Job launcher')
-    parser.add_argument('--local_rank', type=int, default=0)
+    # When using PyTorch version >= 2.0.0, the `torch.distributed.launch`
+    # will pass the `--local-rank` parameter to `tools/train.py` instead
+    # of `--local_rank`.
+    parser.add_argument('--local_rank', '--local-rank', type=int, default=0)
     args = parser.parse_args()
     if 'LOCAL_RANK' not in os.environ:
         os.environ['LOCAL_RANK'] = str(args.local_rank)
 
     return args
```

### Comparing `mmocr-1.0.0rc6/mmocr/__init__.py` & `mmocr-1.0.1/mmocr/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 except ImportError:
     mmengine = None
     from mmcv import digit_version
 
 from .version import __version__, short_version
 
 mmcv_minimum_version = '2.0.0rc4'
-mmcv_maximum_version = '2.1.0'
+mmcv_maximum_version = '2.2.0'
 mmcv_version = digit_version(mmcv.__version__)
 if mmengine is not None:
-    mmengine_minimum_version = '0.6.0'
-    mmengine_maximum_version = '1.0.0'
+    mmengine_minimum_version = '0.7.1'
+    mmengine_maximum_version = '1.1.0'
     mmengine_version = digit_version(mmengine.__version__)
 
-if mmcv_version < digit_version('2.0.0rc0') or mmdet.__version__ < '3.0.0rc0':
+if not mmengine or mmcv_version < digit_version('2.0.0rc0') or digit_version(
+        mmdet.__version__) < digit_version('3.0.0rc0'):
     raise RuntimeError(
         'MMOCR 1.0 only runs with MMEngine, MMCV 2.0.0rc0+ and '
         'MMDetection 3.0.0rc0+, but got MMCV '
         f'{mmcv.__version__} and MMDetection '
         f'{mmdet.__version__}. For more information, please refer to '
         'https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html'
     )  # noqa
@@ -38,15 +39,15 @@
 assert (mmengine_version >= digit_version(mmengine_minimum_version)
         and mmengine_version < digit_version(mmengine_maximum_version)), \
     f'MMEngine=={mmengine.__version__} is used but incompatible. ' \
     f'Please install mmengine>={mmengine_minimum_version}, ' \
     f'<{mmengine_maximum_version}.'
 
 mmdet_minimum_version = '3.0.0rc5'
-mmdet_maximum_version = '3.1.0'
+mmdet_maximum_version = '3.2.0'
 mmdet_version = digit_version(mmdet.__version__)
 
 assert (mmdet_version >= digit_version(mmdet_minimum_version)
         and mmdet_version < digit_version(mmdet_maximum_version)), \
     f'MMDetection {mmdet.__version__} is incompatible ' \
     f'with MMOCR {__version__}. ' \
     f'Please use MMDetection >= {mmdet_minimum_version}, ' \
```

### Comparing `mmocr-1.0.0rc6/mmocr/apis/inferencers/base_mmocr_inferencer.py` & `mmocr-1.0.1/mmocr/apis/inferencers/base_mmocr_inferencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import mmcv
 import mmengine
 import numpy as np
 from mmengine.dataset import Compose
 from mmengine.infer.infer import BaseInferencer, ModelType
+from mmengine.model.utils import revert_sync_batchnorm
 from mmengine.registry import init_default_scope
 from mmengine.structures import InstanceData
 from rich.progress import track
 from torch import Tensor
 
 from mmocr.utils import ConfigType
 
@@ -59,14 +60,15 @@
                  scope: str = 'mmocr') -> None:
         # A global counter tracking the number of images given in the form
         # of ndarray, for naming the output images
         self.num_unnamed_imgs = 0
         init_default_scope(scope)
         super().__init__(
             model=model, weights=weights, device=device, scope=scope)
+        self.model = revert_sync_batchnorm(self.model)
 
     def preprocess(self, inputs: InputsType, batch_size: int = 1, **kwargs):
         """Process the inputs into a model-feedable format.
 
         Args:
             inputs (InputsType): Inputs given by user.
             batch_size (int): batch size. Defaults to 1.
```

### Comparing `mmocr-1.0.0rc6/mmocr/apis/inferencers/kie_inferencer.py` & `mmocr-1.0.1/mmocr/apis/inferencers/kie_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/apis/inferencers/mmocr_inferencer.py` & `mmocr-1.0.1/mmocr/apis/inferencers/mmocr_inferencer.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,15 +76,17 @@
                 self.mode = 'det_rec'
                 ts = str(datetime.timestamp(datetime.now()))
                 self.visualizer = VISUALIZERS.build(
                     dict(
                         type='TextSpottingLocalVisualizer',
                         name=f'inferencer{ts}',
                         font_families=self.textrec_inferencer.visualizer.
-                        font_families))
+                        font_families,
+                        font_properties=self.textrec_inferencer.visualizer.
+                        font_properties))
             else:
                 self.mode = 'rec'
         if kie is not None:
             if det is None or rec is None:
                 raise ValueError(
                     'kie_config is only applicable when det_config and '
                     'rec_config are both provided')
@@ -101,42 +103,62 @@
                 img_bytes = mmengine.fileio.get(item)
                 new_inputs.append(mmcv.imfrombytes(img_bytes))
             else:
                 raise NotImplementedError(f'The input type {type(item)} is not'
                                           'supported yet.')
         return new_inputs
 
-    def forward(self, inputs: InputsType, batch_size: int,
+    def forward(self,
+                inputs: InputsType,
+                batch_size: int = 1,
+                det_batch_size: Optional[int] = None,
+                rec_batch_size: Optional[int] = None,
+                kie_batch_size: Optional[int] = None,
                 **forward_kwargs) -> PredType:
         """Forward the inputs to the model.
 
         Args:
             inputs (InputsType): The inputs to be forwarded.
             batch_size (int): Batch size. Defaults to 1.
+            det_batch_size (Optional[int]): Batch size for text detection
+                model. Overwrite batch_size if it is not None.
+                Defaults to None.
+            rec_batch_size (Optional[int]): Batch size for text recognition
+                model. Overwrite batch_size if it is not None.
+                Defaults to None.
+            kie_batch_size (Optional[int]): Batch size for KIE model.
+                Overwrite batch_size if it is not None.
+                Defaults to None.
 
         Returns:
             Dict: The prediction results. Possibly with keys "det", "rec", and
             "kie"..
         """
         result = {}
         forward_kwargs['progress_bar'] = False
+        if det_batch_size is None:
+            det_batch_size = batch_size
+        if rec_batch_size is None:
+            rec_batch_size = batch_size
+        if kie_batch_size is None:
+            kie_batch_size = batch_size
         if self.mode == 'rec':
             # The extra list wrapper here is for the ease of postprocessing
             self.rec_inputs = inputs
             predictions = self.textrec_inferencer(
                 self.rec_inputs,
                 return_datasamples=True,
-                batch_size=batch_size,
+                batch_size=rec_batch_size,
                 **forward_kwargs)['predictions']
             result['rec'] = [[p] for p in predictions]
         elif self.mode.startswith('det'):  # 'det'/'det_rec'/'det_rec_kie'
             result['det'] = self.textdet_inferencer(
                 inputs,
                 return_datasamples=True,
-                batch_size=batch_size,
+                batch_size=det_batch_size,
                 **forward_kwargs)['predictions']
             if self.mode.startswith('det_rec'):  # 'det_rec'/'det_rec_kie'
                 result['rec'] = []
                 for img, det_data_sample in zip(
                         self._inputs2ndarrray(inputs), result['det']):
                     det_pred = det_data_sample.pred_instances
                     self.rec_inputs = []
@@ -145,15 +167,15 @@
                         # 4 points
                         quad = bbox2poly(poly2bbox(polygon)).tolist()
                         self.rec_inputs.append(crop_img(img, quad))
                     result['rec'].append(
                         self.textrec_inferencer(
                             self.rec_inputs,
                             return_datasamples=True,
-                            batch_size=batch_size,
+                            batch_size=rec_batch_size,
                             **forward_kwargs)['predictions'])
                 if self.mode == 'det_rec_kie':
                     self.kie_inputs = []
                     # TODO: when the det output is empty, kie will fail
                     # as no gt-instances can be provided. It's a known
                     # issue but cannot be solved elegantly since we support
                     # batch inference.
@@ -168,15 +190,15 @@
                                 dict(
                                     bbox=poly2bbox(polygon),
                                     text=rec_data_sample.pred_text.item))
                         self.kie_inputs.append(kie_input)
                     result['kie'] = self.kie_inferencer(
                         self.kie_inputs,
                         return_datasamples=True,
-                        batch_size=batch_size,
+                        batch_size=kie_batch_size,
                         **forward_kwargs)['predictions']
         return result
 
     def visualize(self, inputs: InputsType, preds: PredType,
                   **kwargs) -> Union[List[np.ndarray], None]:
         """Visualize predictions.
 
@@ -215,26 +237,38 @@
             return self.textdet_inferencer.visualize(inputs, preds['det'],
                                                      **kwargs)
 
     def __call__(
         self,
         inputs: InputsType,
         batch_size: int = 1,
+        det_batch_size: Optional[int] = None,
+        rec_batch_size: Optional[int] = None,
+        kie_batch_size: Optional[int] = None,
         out_dir: str = 'results/',
         return_vis: bool = False,
         save_vis: bool = False,
         save_pred: bool = False,
         **kwargs,
     ) -> dict:
         """Call the inferencer.
 
         Args:
             inputs (InputsType): Inputs for the inferencer. It can be a path
                 to image / image directory, or an array, or a list of these.
             batch_size (int): Batch size. Defaults to 1.
+            det_batch_size (Optional[int]): Batch size for text detection
+                model. Overwrite batch_size if it is not None.
+                Defaults to None.
+            rec_batch_size (Optional[int]): Batch size for text recognition
+                model. Overwrite batch_size if it is not None.
+                Defaults to None.
+            kie_batch_size (Optional[int]): Batch size for KIE model.
+                Overwrite batch_size if it is not None.
+                Defaults to None.
             out_dir (str): Output directory of results. Defaults to 'results/'.
             return_vis (bool): Whether to return the visualization result.
                 Defaults to False.
             save_vis (bool): Whether to save the visualization results to
                 "out_dir". Defaults to False.
             save_pred (bool): Whether to save the inference results to
                 "out_dir". Defaults to False.
@@ -265,20 +299,31 @@
         ) = self._dispatch_kwargs(
             save_vis=save_vis,
             save_pred=save_pred,
             return_vis=return_vis,
             **kwargs)
 
         ori_inputs = self._inputs_to_list(inputs)
+        if det_batch_size is None:
+            det_batch_size = batch_size
+        if rec_batch_size is None:
+            rec_batch_size = batch_size
+        if kie_batch_size is None:
+            kie_batch_size = batch_size
 
         chunked_inputs = super(BaseMMOCRInferencer,
                                self)._get_chunk_data(ori_inputs, batch_size)
         results = {'predictions': [], 'visualization': []}
         for ori_input in track(chunked_inputs, description='Inference'):
-            preds = self.forward(ori_input, batch_size, **forward_kwargs)
+            preds = self.forward(
+                ori_input,
+                det_batch_size=det_batch_size,
+                rec_batch_size=rec_batch_size,
+                kie_batch_size=kie_batch_size,
+                **forward_kwargs)
             visualization = self.visualize(
                 ori_input, preds, img_out_dir=img_out_dir, **visualize_kwargs)
             batch_res = self.postprocess(
                 preds,
                 visualization,
                 pred_out_dir=pred_out_dir,
                 **postprocess_kwargs)
@@ -351,15 +396,15 @@
             pred_key = 'det' if 'det' in self.mode else 'rec'
             for pred, pred_result in zip(preds[pred_key], pred_results):
                 img_path = (
                     pred.img_path if pred_key == 'det' else pred[0].img_path)
                 pred_name = osp.splitext(osp.basename(img_path))[0]
                 pred_name = f'{pred_name}.json'
                 pred_out_file = osp.join(pred_out_dir, pred_name)
-                mmengine.dump(pred_result, pred_out_file)
+                mmengine.dump(pred_result, pred_out_file, ensure_ascii=False)
 
         result_dict['predictions'] = pred_results
         if print_result:
             print(result_dict)
         result_dict['visualization'] = visualization
         return result_dict
```

### Comparing `mmocr-1.0.0rc6/mmocr/apis/inferencers/textdet_inferencer.py` & `mmocr-1.0.1/mmocr/apis/inferencers/textdet_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/apis/inferencers/textrec_inferencer.py` & `mmocr-1.0.1/mmocr/apis/inferencers/textrec_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/apis/inferencers/textspot_inferencer.py` & `mmocr-1.0.1/mmocr/apis/inferencers/textspot_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/__init__.py` & `mmocr-1.0.1/mmocr/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/dataset_wrapper.py` & `mmocr-1.0.1/mmocr/datasets/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/icdar_dataset.py` & `mmocr-1.0.1/mmocr/datasets/icdar_dataset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/ocr_dataset.py` & `mmocr-1.0.1/mmocr/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/base.py` & `mmocr-1.0.1/mmocr/datasets/preparers/config_generators/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/textdet_config_generator.py` & `mmocr-1.0.1/mmocr/datasets/preparers/config_generators/textdet_config_generator.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/textrecog_config_generator.py` & `mmocr-1.0.1/mmocr/datasets/preparers/config_generators/textrecog_config_generator.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/config_generators/textspotting_config_generator.py` & `mmocr-1.0.1/mmocr/datasets/preparers/config_generators/textspotting_config_generator.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/data_preparer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/data_preparer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/base.py` & `mmocr-1.0.1/mmocr/datasets/preparers/dumpers/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/json_dumper.py` & `mmocr-1.0.1/mmocr/datasets/preparers/dumpers/wild_receipt_openset_dumper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import os.path as osp
-from typing import Dict
-
-import mmengine
+from typing import List
 
 from mmocr.registry import DATA_DUMPERS
+from mmocr.utils import list_to_file
 from .base import BaseDumper
 
 
 @DATA_DUMPERS.register_module()
-class JsonDumper(BaseDumper):
-    """Dumper for json file."""
+class WildreceiptOpensetDumper(BaseDumper):
 
-    def dump(self, data: Dict) -> None:
-        """Dump data to json file.
+    def dump(self, data: List):
+        """Dump data to txt file.
 
         Args:
-            data (Dict): Data to be dumped.
+            data (List): Data to be dumped.
         """
 
-        filename = f'{self.task}_{self.split}.json'
+        filename = f'openset_{self.split}.txt'
         dst_file = osp.join(self.data_root, filename)
-        mmengine.dump(data, dst_file)
+        list_to_file(dst_file, data)
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/dumpers/lmdb_dumper.py` & `mmocr-1.0.1/mmocr/datasets/preparers/dumpers/lmdb_dumper.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/base.py` & `mmocr-1.0.1/mmocr/datasets/preparers/gatherers/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/mono_gatherer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/gatherers/mono_gatherer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/naf_gatherer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/gatherers/naf_gatherer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/gatherers/pair_gatherer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/gatherers/pair_gatherer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/obtainers/naive_data_obtainer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/obtainers/naive_data_obtainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,16 +84,26 @@
 
         if url is None and not osp.exists(dst_path):
             raise FileNotFoundError(
                 'Direct url is not available for this dataset.'
                 ' Please manually download the required files'
                 ' following the guides.')
 
-        print(f'Start to download {osp.basename(dst_path)}...')
-        print('If you stuck here for a long time, please check your network.')
+        if url.startswith('magnet'):
+            raise NotImplementedError('Please use any BitTorrent client to '
+                                      'download the following magnet link to '
+                                      f'{osp.abspath(dst_path)} and '
+                                      f'try again.\nLink: {url}')
+
+        print('Downloading...')
+        print(f'URL: {url}')
+        print(f'Destination: {osp.abspath(dst_path)}')
+        print('If you stuck here for a long time, please check your network, '
+              'or manually download the file to the destination path and '
+              'run the script again.')
         request.urlretrieve(url, dst_path, progress)
         print('')
 
     def extract(self,
                 src_path: str,
                 dst_path: str,
                 delete: bool = False) -> None:
@@ -172,18 +182,20 @@
         for src, dst in mapping:
             src = osp.join(self.data_root, src)
             dst = osp.join(self.data_root, dst)
 
             if '*' in src:
                 mkdir_or_exist(dst)
                 for f in glob.glob(src):
-                    if not osp.exists(osp.join(dst, osp.basename(f))):
+                    if not osp.exists(
+                            osp.join(dst, osp.relpath(f, self.data_root))):
                         shutil.move(f, dst)
 
             elif osp.exists(src) and not osp.exists(dst):
+                mkdir_or_exist(osp.dirname(dst))
                 shutil.move(src, dst)
 
     def clean(self) -> None:
         """Remove empty dirs."""
         for root, dirs, files in os.walk(self.data_root, topdown=False):
             if not files and not dirs:
                 os.rmdir(root)
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/base.py` & `mmocr-1.0.1/mmocr/datasets/preparers/packers/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/textdet_packer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/packers/textdet_packer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/textrecog_packer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/packers/textrecog_packer.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,19 +46,16 @@
             split (str): The split of the instance.
 
         Returns:
             Dict: The packed instance.
         """
 
         img_name, text = sample
-        # TODO: remove hard code
-        packed_instance = dict(
-            instances=[dict(text=text)],
-            img_path=osp.join('textrecog_imgs', self.split,
-                              osp.basename(img_name)))
+        img_name = osp.relpath(img_name, self.data_root)
+        packed_instance = dict(instances=[dict(text=text)], img_path=img_name)
 
         return packed_instance
 
     def add_meta(self, sample: List) -> Dict:
         """Add meta information to the sample.
 
         Args:
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/textspotting_packer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/packers/textspotting_packer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/packers/wildreceipt_packer.py` & `mmocr-1.0.1/mmocr/datasets/preparers/packers/wildreceipt_packer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/__init__.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .base import BaseParser
 from .coco_parser import COCOTextDetAnnParser
+from .ctw1500_parser import CTW1500AnnParser
 from .funsd_parser import FUNSDTextDetAnnParser
 from .icdar_txt_parser import (ICDARTxtTextDetAnnParser,
                                ICDARTxtTextRecogAnnParser)
+from .mjsynth_parser import MJSynthAnnParser
 from .naf_parser import NAFAnnParser
 from .sroie_parser import SROIETextDetAnnParser
 from .svt_parser import SVTTextDetAnnParser
+from .synthtext_parser import SynthTextAnnParser
 from .totaltext_parser import TotaltextTextDetAnnParser
 from .wildreceipt_parser import WildreceiptKIEAnnParser
 
 __all__ = [
     'BaseParser', 'ICDARTxtTextDetAnnParser', 'ICDARTxtTextRecogAnnParser',
     'TotaltextTextDetAnnParser', 'WildreceiptKIEAnnParser',
     'COCOTextDetAnnParser', 'SVTTextDetAnnParser', 'FUNSDTextDetAnnParser',
-    'SROIETextDetAnnParser', 'NAFAnnParser'
+    'SROIETextDetAnnParser', 'NAFAnnParser', 'CTW1500AnnParser',
+    'SynthTextAnnParser', 'MJSynthAnnParser'
 ]
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/base.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/coco_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/coco_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/funsd_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/funsd_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/icdar_txt_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/icdar_txt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,10 +118,10 @@
             text = anno['text'].strip()
             if self.remove_strs is not None:
                 for strs in self.remove_strs:
                     text = text.replace(strs, '')
             if text == self.ignore:
                 continue
             img_name = anno['img']
-            samples.append((osp.join(img_dir, osp.basename(img_name)), text))
+            samples.append((osp.join(img_dir, img_name), text))
 
         return samples
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/naf_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/naf_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/sroie_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/sroie_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/svt_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/svt_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/totaltext_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/totaltext_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/preparers/parsers/wildreceipt_parser.py` & `mmocr-1.0.1/mmocr/datasets/preparers/parsers/wildreceipt_parser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/recog_lmdb_dataset.py` & `mmocr-1.0.1/mmocr/datasets/recog_lmdb_dataset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/recog_text_dataset.py` & `mmocr-1.0.1/mmocr/datasets/recog_text_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from typing import Callable, List, Optional, Sequence, Union
 
 from mmengine.dataset import BaseDataset
 from mmengine.fileio import list_from_file
 
 from mmocr.registry import DATASETS, TASK_UTILS
 
-# TODO: replace all list_from_file from mmengine
-
 
 @DATASETS.register_module()
 class RecogTextDataset(BaseDataset):
     r"""RecogTextDataset for text recognition.
 
     The annotation format can be both in jsonl and txt. If the annotation file
     is in jsonl format, it should be a list of dicts. If the annotation file
@@ -29,17 +27,16 @@
     .. code-block:: none
 
         ``{"filename": "test_img1.jpg", "text": "OpenMMLab"}``
         ``{"filename": "test_img2.jpg", "text": "MMOCR"}``
 
     Args:
         ann_file (str): Annotation file path. Defaults to ''.
-        file_client_args (dict, optional): Arguments to instantiate a
-            FileClient. See :class:`mmengine.fileio.FileClient` for details.
-            Default: None.
+        backend_args (dict, optional): Arguments to instantiate the
+            prefix of uri corresponding backend. Defaults to None.
         parse_cfg (dict, optional): Config of parser for parsing annotations.
             Use ``LineJsonParser`` when the annotation file is in jsonl format
             with keys of ``filename`` and ``text``. The keys in parse_cfg
             should be consistent with the keys in jsonl annotations. The first
             key in parse_cfg should be the key of the path in jsonl
             annotations. The second key in parse_cfg should be the key of the
             text in jsonl Use ``LineStrParser`` when the annotation file is in
@@ -71,30 +68,30 @@
         max_refetch (int, optional): If ``RecogTextDataset.prepare_data`` get a
             None img. The maximum extra number of cycles to get a valid
             image. Defaults to 1000.
     """
 
     def __init__(self,
                  ann_file: str = '',
-                 file_client_args=None,
+                 backend_args=None,
                  parser_cfg: Optional[dict] = dict(
                      type='LineJsonParser', keys=['filename', 'text']),
                  metainfo: Optional[dict] = None,
                  data_root: Optional[str] = '',
                  data_prefix: dict = dict(img_path=''),
                  filter_cfg: Optional[dict] = None,
                  indices: Optional[Union[int, Sequence[int]]] = None,
                  serialize_data: bool = True,
                  pipeline: List[Union[dict, Callable]] = [],
                  test_mode: bool = False,
                  lazy_init: bool = False,
                  max_refetch: int = 1000) -> None:
 
         self.parser = TASK_UTILS.build(parser_cfg)
-        self.file_client_args = file_client_args
+        self.backend_args = backend_args
         super().__init__(
             ann_file=ann_file,
             metainfo=metainfo,
             data_root=data_root,
             data_prefix=data_prefix,
             filter_cfg=filter_cfg,
             indices=indices,
@@ -108,15 +105,15 @@
         """Load annotations from an annotation file named as ``self.ann_file``
 
         Returns:
             List[dict]: A list of annotation.
         """
         data_list = []
         raw_anno_infos = list_from_file(
-            self.ann_file, file_client_args=self.file_client_args)
+            self.ann_file, backend_args=self.backend_args)
         for raw_anno_info in raw_anno_infos:
             data_list.append(self.parse_data_info(raw_anno_info))
         return data_list
 
     def parse_data_info(self, raw_anno_info: str) -> dict:
         """Parse raw annotation to target format.
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/samplers/batch_aug.py` & `mmocr-1.0.1/mmocr/datasets/samplers/batch_aug.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/__init__.py` & `mmocr-1.0.1/mmocr/datasets/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/adapters.py` & `mmocr-1.0.1/mmocr/datasets/transforms/adapters.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/formatting.py` & `mmocr-1.0.1/mmocr/datasets/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/loading.py` & `mmocr-1.0.1/mmocr/datasets/transforms/loading.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 import warnings
 from typing import Optional, Union
 
 import mmcv
-import mmengine
+import mmengine.fileio as fileio
 import numpy as np
 from mmcv.transforms import BaseTransform
 from mmcv.transforms import LoadAnnotations as MMCV_LoadAnnotations
 from mmcv.transforms import LoadImageFromFile as MMCV_LoadImageFromFile
 
 from mmocr.registry import TRANSFORMS
 
@@ -35,50 +35,81 @@
             Defaults to 'color'.
         imdecode_backend (str): The image decoding backend type. The backend
             argument for :func:``mmcv.imfrombytes``.
             See :func:``mmcv.imfrombytes`` for details.
             Defaults to 'cv2'.
         file_client_args (dict): Arguments to instantiate a FileClient.
             See :class:`mmengine.fileio.FileClient` for details.
-            Defaults to ``dict(backend='disk')``.
+            Defaults to None. It will be deprecated in future. Please use
+            ``backend_args`` instead.
+            Deprecated in version 1.0.0rc6.
+        backend_args (dict, optional): Instantiates the corresponding file
+            backend. It may contain `backend` key to specify the file
+            backend. If it contains, the file backend corresponding to this
+            value will be used and initialized with the remaining values,
+            otherwise the corresponding file backend will be selected
+            based on the prefix of the file path. Defaults to None.
+            New in version 1.0.0rc6.
         ignore_empty (bool): Whether to allow loading empty image or file path
             not existent. Defaults to False.
         min_size (int): The minimum size of the image to be loaded. If the
             image is smaller than the minimum size, it will be regarded as a
             broken image. Defaults to 0.
     """
 
-    def __init__(self,
-                 to_float32: bool = False,
-                 color_type: str = 'color',
-                 imdecode_backend: str = 'cv2',
-                 file_client_args: dict = dict(backend='disk'),
-                 min_size: int = 0,
-                 ignore_empty: bool = False) -> None:
+    def __init__(
+        self,
+        to_float32: bool = False,
+        color_type: str = 'color',
+        imdecode_backend: str = 'cv2',
+        file_client_args: Optional[dict] = None,
+        min_size: int = 0,
+        ignore_empty: bool = False,
+        *,
+        backend_args: Optional[dict] = None,
+    ) -> None:
         self.ignore_empty = ignore_empty
         self.to_float32 = to_float32
         self.color_type = color_type
         self.imdecode_backend = imdecode_backend
-        self.file_client_args = file_client_args.copy()
-        self.file_client = mmengine.FileClient(**self.file_client_args)
         self.min_size = min_size
+        self.file_client_args = file_client_args
+        self.backend_args = backend_args
+        if file_client_args is not None:
+            warnings.warn(
+                '"file_client_args" will be deprecated in future. '
+                'Please use "backend_args" instead', DeprecationWarning)
+            if backend_args is not None:
+                raise ValueError(
+                    '"file_client_args" and "backend_args" cannot be set '
+                    'at the same time.')
+
+            self.file_client_args = file_client_args.copy()
+        if backend_args is not None:
+            self.backend_args = backend_args.copy()
 
     def transform(self, results: dict) -> Optional[dict]:
         """Functions to load image.
 
         Args:
             results (dict): Result dict from :obj:``mmcv.BaseDataset``.
 
         Returns:
             dict: The dict contains loaded image and meta information.
         """
 
         filename = results['img_path']
         try:
-            img_bytes = self.file_client.get(filename)
+            if getattr(self, 'file_client_args', None) is not None:
+                file_client = fileio.FileClient.infer_client(
+                    self.file_client_args, filename)
+                img_bytes = file_client.get(filename)
+            else:
+                img_bytes = fileio.get(
+                    filename, backend_args=self.backend_args)
             img = mmcv.imfrombytes(
                 img_bytes, flag=self.color_type, backend=self.imdecode_backend)
         except Exception as e:
             if self.ignore_empty:
                 warnings.warn(f'Failed to load {filename} due to {e}')
                 return None
             else:
@@ -99,16 +130,20 @@
 
     def __repr__(self):
         repr_str = (f'{self.__class__.__name__}('
                     f'ignore_empty={self.ignore_empty}, '
                     f'min_size={self.min_size}, '
                     f'to_float32={self.to_float32}, '
                     f"color_type='{self.color_type}', "
-                    f"imdecode_backend='{self.imdecode_backend}', "
-                    f'file_client_args={self.file_client_args})')
+                    f"imdecode_backend='{self.imdecode_backend}', ")
+
+        if self.file_client_args is not None:
+            repr_str += f'file_client_args={self.file_client_args})'
+        else:
+            repr_str += f'backend_args={self.backend_args})'
         return repr_str
 
 
 @TRANSFORMS.register_module()
 class LoadImageFromNDArray(LoadImageFromFile):
     """Load an image from ``results['img']``.
 
@@ -367,15 +402,19 @@
     def __repr__(self) -> str:
         repr_str = self.__class__.__name__
         repr_str += f'(with_bbox={self.with_bbox}, '
         repr_str += f'with_label={self.with_label}, '
         repr_str += f'with_polygon={self.with_polygon}, '
         repr_str += f'with_text={self.with_text}, '
         repr_str += f"imdecode_backend='{self.imdecode_backend}', "
-        repr_str += f'file_client_args={self.file_client_args})'
+
+        if self.file_client_args is not None:
+            repr_str += f'file_client_args={self.file_client_args})'
+        else:
+            repr_str += f'backend_args={self.backend_args})'
         return repr_str
 
 
 @TRANSFORMS.register_module()
 class LoadKIEAnnotations(MMCV_LoadAnnotations):
     """Load and process the ``instances`` annotation provided by dataset.
```

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/ocr_transforms.py` & `mmocr-1.0.1/mmocr/datasets/transforms/ocr_transforms.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/textdet_transforms.py` & `mmocr-1.0.1/mmocr/datasets/transforms/textdet_transforms.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/textrecog_transforms.py` & `mmocr-1.0.1/mmocr/datasets/transforms/textrecog_transforms.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/transforms/wrappers.py` & `mmocr-1.0.1/mmocr/datasets/transforms/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/datasets/wildreceipt_dataset.py` & `mmocr-1.0.1/mmocr/datasets/wildreceipt_dataset.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/engine/hooks/visualization_hook.py` & `mmocr-1.0.1/mmocr/engine/hooks/visualization_hook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import os.path as osp
-from typing import Sequence, Union
+from typing import Optional, Sequence, Union
 
 import mmcv
-import mmengine
+import mmengine.fileio as fileio
 from mmengine.hooks import Hook
 from mmengine.runner import Runner
 from mmengine.visualization import Visualizer
 
 from mmocr.registry import HOOKS
 from mmocr.structures import TextDetDataSample, TextRecogDataSample
 
@@ -22,39 +22,41 @@
         enable (bool): Whether to enable this hook. Defaults to False.
         interval (int): The interval of visualization. Defaults to 50.
         score_thr (float): The threshold to visualize the bboxes
             and masks. It's only useful for text detection. Defaults to 0.3.
         show (bool): Whether to display the drawn image. Defaults to False.
         wait_time (float): The interval of show in seconds. Defaults
             to 0.
-        file_client_args (dict): Arguments to instantiate a FileClient.
-            See :class:`mmengine.fileio.FileClient` for details.
-            Defaults to ``dict(backend='disk')``.
+        backend_args (dict, optional): Instantiates the corresponding file
+            backend. It may contain `backend` key to specify the file
+            backend. If it contains, the file backend corresponding to this
+            value will be used and initialized with the remaining values,
+            otherwise the corresponding file backend will be selected
+            based on the prefix of the file path. Defaults to None.
     """
 
     def __init__(
         self,
         enable: bool = False,
         interval: int = 50,
         score_thr: float = 0.3,
         show: bool = False,
         draw_pred: bool = False,
         draw_gt: bool = False,
         wait_time: float = 0.,
-        file_client_args: dict = dict(backend='disk')
+        backend_args: Optional[dict] = None,
     ) -> None:
         self._visualizer: Visualizer = Visualizer.get_current_instance()
         self.interval = interval
         self.score_thr = score_thr
         self.show = show
         self.draw_pred = draw_pred
         self.draw_gt = draw_gt
         self.wait_time = wait_time
-        self.file_client_args = file_client_args.copy()
-        self.file_client = None
+        self.backend_args = backend_args
         self.enable = enable
 
     # TODO after MultiDatasetWrapper, rewrites this function and try to merge
     # with after_val_iter and after_test_iter
     def after_val_iter(self, runner: Runner, batch_idx: int,
                        data_batch: Sequence[dict],
                        outputs: Sequence[Union[TextDetDataSample,
@@ -68,26 +70,24 @@
             outputs (Sequence[:obj:`TextDetDataSample` or
                 :obj:`TextRecogDataSample`]): Outputs from model.
         """
         # TODO: data_batch does not include annotation information
         if self.enable is False:
             return
 
-        if self.file_client is None:
-            self.file_client = mmengine.FileClient(**self.file_client_args)
-
         # There is no guarantee that the same batch of images
         # is visualized for each evaluation.
         total_curr_iter = runner.iter + batch_idx
 
         # Visualize only the first data
         if total_curr_iter % self.interval == 0:
             for output in outputs:
                 img_path = output.img_path
-                img_bytes = self.file_client.get(img_path)
+                img_bytes = fileio.get(
+                    img_path, backend_args=self.backend_args)
                 img = mmcv.imfrombytes(img_bytes, channel_order='rgb')
                 self._visualizer.add_datasample(
                     osp.splitext(osp.basename(img_path))[0],
                     img,
                     data_sample=output,
                     draw_gt=self.draw_gt,
                     draw_pred=self.draw_pred,
@@ -109,20 +109,17 @@
             outputs (Sequence[:obj:`TextDetDataSample` or
                 :obj:`TextRecogDataSample`]): Outputs from model.
         """
 
         if self.enable is False:
             return
 
-        if self.file_client is None:
-            self.file_client = mmengine.FileClient(**self.file_client_args)
-
         for output in outputs:
             img_path = output.img_path
-            img_bytes = self.file_client.get(img_path)
+            img_bytes = fileio.get(img_path, backend_args=self.backend_args)
             img = mmcv.imfrombytes(img_bytes, channel_order='rgb')
 
             self._visualizer.add_datasample(
                 osp.splitext(osp.basename(img_path))[0],
                 img,
                 data_sample=output,
                 show=self.show,
```

### Comparing `mmocr-1.0.0rc6/mmocr/evaluation/evaluator/multi_datasets_evaluator.py` & `mmocr-1.0.1/mmocr/evaluation/evaluator/multi_datasets_evaluator.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/evaluation/functional/hmean.py` & `mmocr-1.0.1/mmocr/evaluation/functional/hmean.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/evaluation/metrics/f_metric.py` & `mmocr-1.0.1/mmocr/evaluation/metrics/f_metric.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/evaluation/metrics/hmean_iou_metric.py` & `mmocr-1.0.1/mmocr/evaluation/metrics/hmean_iou_metric.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/evaluation/metrics/recog_metric.py` & `mmocr-1.0.1/mmocr/evaluation/metrics/recog_metric.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/backbones/clip_resnet.py` & `mmocr-1.0.1/mmocr/models/common/backbones/clip_resnet.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/backbones/unet.py` & `mmocr-1.0.1/mmocr/models/common/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/dictionary/dictionary.py` & `mmocr-1.0.1/mmocr/models/common/dictionary/dictionary.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/layers/transformer_layers.py` & `mmocr-1.0.1/mmocr/models/common/layers/transformer_layers.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/losses/__init__.py` & `mmocr-1.0.1/mmocr/models/common/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/losses/bce_loss.py` & `mmocr-1.0.1/mmocr/models/common/losses/bce_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/losses/dice_loss.py` & `mmocr-1.0.1/mmocr/models/common/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/losses/l1_loss.py` & `mmocr-1.0.1/mmocr/models/common/losses/l1_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/modules/transformer_module.py` & `mmocr-1.0.1/mmocr/models/common/modules/transformer_module.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/common/plugins/common.py` & `mmocr-1.0.1/mmocr/models/common/plugins/common.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/kie/extractors/sdmgr.py` & `mmocr-1.0.1/mmocr/models/kie/extractors/sdmgr.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/kie/heads/sdmgr_head.py` & `mmocr-1.0.1/mmocr/models/kie/heads/sdmgr_head.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/kie/module_losses/sdmgr_module_loss.py` & `mmocr-1.0.1/mmocr/models/kie/module_losses/sdmgr_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/kie/postprocessors/sdmgr_postprocessor.py` & `mmocr-1.0.1/mmocr/models/kie/postprocessors/sdmgr_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/data_preprocessors/data_preprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/data_preprocessors/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/detectors/base.py` & `mmocr-1.0.1/mmocr/models/textdet/detectors/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/detectors/mmdet_wrapper.py` & `mmocr-1.0.1/mmocr/models/textdet/detectors/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/detectors/single_stage_text_detector.py` & `mmocr-1.0.1/mmocr/models/textdet/detectors/single_stage_text_detector.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/base.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/db_head.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/db_head.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/drrg_head.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/drrg_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import cv2
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from lanms import merge_quadrangle_n9 as la_nms
+
+try:
+    from lanms import merge_quadrangle_n9 as la_nms
+except ImportError:
+    la_nms = None
 from mmcv.ops import RoIAlignRotated
 from mmengine.model import BaseModule
 from numpy import ndarray
 from torch import Tensor
 from torch.nn import init
 
 from mmocr.models.textdet.heads import BaseTextDetHead
@@ -834,14 +838,17 @@
             text_comps = self.propose_comps(score_map, top_height_map,
                                             bot_height_map, sin_map, cos_map,
                                             self.comp_score_thr,
                                             self.min_width, self.max_width,
                                             self.comp_shrink_ratio,
                                             self.comp_w_h_ratio)
 
+            if la_nms is None:
+                raise ImportError('lanms-neo is not installed, '
+                                  'please run "pip install lanms-neo==1.0.2".')
             text_comps = la_nms(text_comps, self.nms_thr)
             text_comp_mask = np.zeros(mask_sz)
             text_comp_boxes = text_comps[:, :8].reshape(
                 (-1, 4, 2)).astype(np.int32)
 
             cv2.drawContours(text_comp_mask, text_comp_boxes, -1, 1, -1)
             if (text_comp_mask * text_mask).sum() < text_comp_mask.sum() * 0.5:
```

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/fce_head.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/fce_head.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/pan_head.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/pan_head.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/pse_head.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/pse_head.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/heads/textsnake_head.py` & `mmocr-1.0.1/mmocr/models/textdet/heads/textsnake_head.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/__init__.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/base.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/db_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/db_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/drrg_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/drrg_module_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import Dict, List, Sequence, Tuple
 
 import cv2
 import numpy as np
 import torch
-from lanms import merge_quadrangle_n9 as la_nms
+
+try:
+    from lanms import merge_quadrangle_n9 as la_nms
+except ImportError:
+    la_nms = None
 from mmcv.image import imrescale
 from mmdet.models.utils import multi_apply
 from numpy import ndarray
 from numpy.linalg import norm
 from torch import Tensor
 
 from mmocr.registry import MODELS
@@ -443,14 +447,17 @@
         tr = top_mid_points[:, ::-1] + np.hstack([-r * sin, r * cos])
         br = bot_mid_points[:, ::-1] + np.hstack([-r * sin, r * cos])
         bl = bot_mid_points[:, ::-1] - np.hstack([-r * sin, r * cos])
         text_comps = np.hstack([tl, tr, br, bl]).astype(np.float32)
 
         score = np.ones((text_comps.shape[0], 1), dtype=np.float32)
         text_comps = np.hstack([text_comps, score])
+        if la_nms is None:
+            raise ImportError('lanms-neo is not installed, '
+                              'please run "pip install lanms-neo==1.0.2".')
         text_comps = la_nms(text_comps, self.text_comp_nms_thr)
 
         if text_comps.shape[0] >= 1:
             img_h, img_w = center_region_mask.shape
             text_comps[:, 0:8:2] = np.clip(text_comps[:, 0:8:2], 0, img_w - 1)
             text_comps[:, 1:8:2] = np.clip(text_comps[:, 1:8:2], 0, img_h - 1)
```

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/fce_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/fce_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/pan_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/pan_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/pse_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/pse_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/seg_based_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/seg_based_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/module_losses/textsnake_module_loss.py` & `mmocr-1.0.1/mmocr/models/textdet/module_losses/textsnake_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpem_ffm.py` & `mmocr-1.0.1/mmocr/models/textdet/necks/fpem_ffm.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpn_cat.py` & `mmocr-1.0.1/mmocr/models/textdet/necks/fpn_cat.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpn_unet.py` & `mmocr-1.0.1/mmocr/models/textdet/necks/fpn_unet.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/necks/fpnf.py` & `mmocr-1.0.1/mmocr/models/textdet/necks/fpnf.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/__init__.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/base.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/db_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/db_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/drrg_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/drrg_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/fce_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/fce_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/pan_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/pan_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/pse_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/pse_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textdet/postprocessors/textsnake_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textdet/postprocessors/textsnake_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/mini_vgg.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/mini_vgg.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/mobilenet_v2.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/nrtr_modality_transformer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/resnet.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/resnet31_ocr.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/resnet31_ocr.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/resnet_abi.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/resnet_abi.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/backbones/shallow_cnn.py` & `mmocr-1.0.1/mmocr/models/textrecog/backbones/shallow_cnn.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/data_preprocessors/data_preprocessor.py` & `mmocr-1.0.1/mmocr/models/textrecog/data_preprocessors/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/__init__.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/abi_fuser.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/abi_fuser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/abi_language_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/abi_language_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/abi_vision_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/abi_vision_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/aster_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/aster_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/base.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/crnn_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/crnn_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/master_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/master_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/nrtr_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/nrtr_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/position_attention_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/position_attention_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/robust_scanner_fuser.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/robust_scanner_fuser.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/sar_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/sar_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/sar_decoder_with_bs.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/sequence_attention_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/sequence_attention_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/decoders/svtr_decoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/decoders/svtr_decoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/__init__.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/abi_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/aster_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/aster_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/channel_reduction_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/channel_reduction_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/nrtr_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/nrtr_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/sar_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/sar_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/satrn_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/satrn_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/encoders/svtr_encoder.py` & `mmocr-1.0.1/mmocr/models/textrecog/encoders/svtr_encoder.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/__init__.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/conv_layer.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/conv_layer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/dot_product_attention_layer.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/dot_product_attention_layer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/lstm_layer.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/lstm_layer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/position_aware_layer.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/position_aware_layer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/robust_scanner_fusion_layer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/layers/satrn_layers.py` & `mmocr-1.0.1/mmocr/models/textrecog/layers/satrn_layers.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/abi_module_loss.py` & `mmocr-1.0.1/mmocr/models/textrecog/module_losses/abi_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/base.py` & `mmocr-1.0.1/mmocr/models/textrecog/module_losses/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/ce_module_loss.py` & `mmocr-1.0.1/mmocr/models/textrecog/module_losses/ce_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/module_losses/ctc_module_loss.py` & `mmocr-1.0.1/mmocr/models/textrecog/module_losses/ctc_module_loss.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/plugins/common.py` & `mmocr-1.0.1/mmocr/models/textrecog/plugins/common.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/attn_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textrecog/postprocessors/attn_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/base.py` & `mmocr-1.0.1/mmocr/models/textrecog/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/postprocessors/ctc_postprocessor.py` & `mmocr-1.0.1/mmocr/models/textrecog/postprocessors/ctc_postprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/preprocessors/tps_preprocessor.py` & `mmocr-1.0.1/mmocr/models/textrecog/preprocessors/tps_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/__init__.py` & `mmocr-1.0.1/mmocr/models/textrecog/recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/base.py` & `mmocr-1.0.1/mmocr/models/textrecog/recognizers/base.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer.py` & `mmocr-1.0.1/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer_tta.py` & `mmocr-1.0.1/mmocr/models/textrecog/recognizers/encoder_decoder_recognizer_tta.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     Examples:
         >>> tta_model = dict(
         >>>     type='EncoderDecoderRecognizerTTAModel')
         >>>
         >>> tta_pipeline = [
         >>>     dict(
         >>>         type='LoadImageFromFile',
-        >>>         color_type='grayscale',
-        >>>         file_client_args=file_client_args),
+        >>>         color_type='grayscale'),
         >>>     dict(
         >>>         type='TestTimeAug',
         >>>         transforms=[
         >>>             [
         >>>                 dict(
         >>>                     type='ConditionApply',
         >>>                     true_transforms=[
```

### Comparing `mmocr-1.0.0rc6/mmocr/registry.py` & `mmocr-1.0.1/mmocr/registry.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/structures/kie_data_sample.py` & `mmocr-1.0.1/mmocr/structures/kie_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/structures/textdet_data_sample.py` & `mmocr-1.0.1/mmocr/structures/textdet_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/structures/textrecog_data_sample.py` & `mmocr-1.0.1/mmocr/structures/textrecog_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/structures/textspotting_data_sample.py` & `mmocr-1.0.1/mmocr/structures/textspotting_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/testing/data.py` & `mmocr-1.0.1/mmocr/testing/data.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/__init__.py` & `mmocr-1.0.1/mmocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/bbox_utils.py` & `mmocr-1.0.1/mmocr/utils/bbox_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import functools
 from typing import List, Tuple
 
 import numpy as np
 from shapely.geometry import LineString, Point
 
-from mmocr.utils.check_argument import is_2dlist, is_type_list
+from mmocr.utils.check_argument import is_type_list
 from mmocr.utils.point_utils import point_distance, points_center
 from mmocr.utils.typing_utils import ArrayLike
 
 
 def rescale_bbox(bbox: np.ndarray,
                  scale_factor: Tuple[int, int],
                  mode: str = 'mul') -> np.ndarray:
@@ -175,22 +174,23 @@
                 rightmost_box_idx = j
 
         # split line into lines if the distance between two neighboring
         # sub-lines' is greater than max_x_dist
         lines = []
         line_idx = 0
         lines.append([line[0]])
+        rightmost = np.max(x_sorted_boxes[line[0]]['box'][::2])
         for k in range(1, len(line)):
             curr_box = x_sorted_boxes[line[k]]
-            prev_box = x_sorted_boxes[line[k - 1]]
-            dist = np.min(curr_box['box'][::2]) - np.max(prev_box['box'][::2])
+            dist = np.min(curr_box['box'][::2]) - rightmost
             if dist > max_x_dist:
                 line_idx += 1
                 lines.append([])
             lines[line_idx].append(line[k])
+            rightmost = max(rightmost, np.max(curr_box['box'][::2]))
 
         # Get merged boxes
         for box_group in lines:
             merged_box = {}
             merged_box['text'] = ' '.join(
                 [x_sorted_boxes[idx]['text'] for idx in box_group])
             x_min, y_min = float('inf'), float('inf')
@@ -244,55 +244,14 @@
         + np.outer(u ** 3, bezier[:, 3])
 
     # Convert points to polygon
     points = np.concatenate((points[:, :2], points[:, 2:]), axis=0)
     return points.tolist()
 
 
-def sort_points(points):
-    # TODO Add typehints & test & docstring
-    """Sort arbitory points in clockwise order. Reference:
-    https://stackoverflow.com/a/6989383.
-
-    Args:
-        points (list[ndarray] or ndarray or list[list]): A list of unsorted
-            boundary points.
-
-    Returns:
-        list[ndarray]: A list of points sorted in clockwise order.
-    """
-
-    assert is_type_list(points, np.ndarray) or isinstance(points, np.ndarray) \
-        or is_2dlist(points)
-
-    points = np.array(points)
-    center = np.mean(points, axis=0)
-
-    def cmp(a, b):
-        oa = a - center
-        ob = b - center
-
-        # Some corner cases
-        if oa[0] >= 0 and ob[0] < 0:
-            return 1
-        if oa[0] < 0 and ob[0] >= 0:
-            return -1
-
-        prod = np.cross(oa, ob)
-        if prod > 0:
-            return 1
-        if prod < 0:
-            return -1
-
-        # a, b are on the same line from the center
-        return 1 if (oa**2).sum() < (ob**2).sum() else -1
-
-    return sorted(points, key=functools.cmp_to_key(cmp))
-
-
 def sort_vertex(points_x, points_y):
     # TODO Add typehints & docstring & test
     """Sort box vertices in clockwise order from left-top first.
 
     Args:
         points_x (list[float]): x of four vertices.
         points_y (list[float]): y of four vertices.
```

### Comparing `mmocr-1.0.0rc6/mmocr/utils/bezier_utils.py` & `mmocr-1.0.1/mmocr/utils/bezier_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/check_argument.py` & `mmocr-1.0.1/mmocr/utils/check_argument.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/data_converter_utils.py` & `mmocr-1.0.1/mmocr/utils/data_converter_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/fileio.py` & `mmocr-1.0.1/mmocr/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/img_utils.py` & `mmocr-1.0.1/mmocr/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/mask_utils.py` & `mmocr-1.0.1/mmocr/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/parsers.py` & `mmocr-1.0.1/mmocr/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/point_utils.py` & `mmocr-1.0.1/mmocr/utils/point_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/polygon_utils.py` & `mmocr-1.0.1/mmocr/utils/polygon_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import functools
+import math
+import operator
+from functools import reduce
 from typing import List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pyclipper
 import shapely
 from mmengine.utils import is_list_of
 from shapely.geometry import MultiPolygon, Polygon
@@ -150,19 +152,17 @@
 
     Returns:
         np.array or None: Cropped polygon. If the polygon is not within the
             crop box, return None.
     """
     poly = poly_make_valid(poly2shapely(polygon))
     crop_poly = poly_make_valid(poly2shapely(bbox2poly(crop_box)))
-    poly_cropped = poly.intersection(crop_poly)
-    if poly_cropped.area == 0. or not isinstance(
+    area, poly_cropped = poly_intersection(poly, crop_poly, return_poly=True)
+    if area == 0 or area is None or not isinstance(
             poly_cropped, shapely.geometry.polygon.Polygon):
-        # If polygon is outside crop_box region or the intersection is not a
-        # polygon, return None.
         return None
     else:
         poly_cropped = poly_make_valid(poly_cropped)
         poly_cropped = np.array(poly_cropped.boundary.xy, dtype=np.float32)
         poly_cropped = poly_cropped.T
         # reverse poly_cropped to have clockwise order
         poly_cropped = poly_cropped[::-1, :].reshape(-1)
@@ -370,51 +370,40 @@
     target_poly = poly2shapely(target)
 
     return poly_iou(src_poly, target_poly, zero_division=zero_division)
 
 
 def sort_points(points):
     # TODO Add typehints & test & docstring
-    """Sort arbitory points in clockwise order. Reference:
-    https://stackoverflow.com/a/6989383.
+    """Sort arbitrary points in clockwise order in Cartesian coordinate, you
+    may need to reverse the output sequence if you are using OpenCV's image
+    coordinate.
+
+    Reference:
+    https://github.com/novioleo/Savior/blob/master/Utils/GeometryUtils.py.
+
+    Warning: This function can only sort convex polygons.
 
     Args:
         points (list[ndarray] or ndarray or list[list]): A list of unsorted
             boundary points.
 
     Returns:
         list[ndarray]: A list of points sorted in clockwise order.
     """
-
     assert is_list_of(points, np.ndarray) or isinstance(points, np.ndarray) \
         or is_2dlist(points)
-
-    points = np.array(points)
-    center = np.mean(points, axis=0)
-
-    def cmp(a, b):
-        oa = a - center
-        ob = b - center
-
-        # Some corner cases
-        if oa[0] >= 0 and ob[0] < 0:
-            return 1
-        if oa[0] < 0 and ob[0] >= 0:
-            return -1
-
-        prod = np.cross(oa, ob)
-        if prod > 0:
-            return 1
-        if prod < 0:
-            return -1
-
-        # a, b are on the same line from the center
-        return 1 if (oa**2).sum() < (ob**2).sum() else -1
-
-    return sorted(points, key=functools.cmp_to_key(cmp))
+    center_point = tuple(
+        map(operator.truediv,
+            reduce(lambda x, y: map(operator.add, x, y), points),
+            [len(points)] * 2))
+    return sorted(
+        points,
+        key=lambda coord: (180 + math.degrees(
+            math.atan2(*tuple(map(operator.sub, coord, center_point))))) % 360)
 
 
 def sort_vertex(points_x, points_y):
     # TODO Add typehints & test
     """Sort box vertices in clockwise order from left-top first.
 
     Args:
```

### Comparing `mmocr-1.0.0rc6/mmocr/utils/processing.py` & `mmocr-1.0.1/mmocr/utils/processing.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/setup_env.py` & `mmocr-1.0.1/mmocr/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/string_utils.py` & `mmocr-1.0.1/mmocr/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/transform_utils.py` & `mmocr-1.0.1/mmocr/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/utils/typing_utils.py` & `mmocr-1.0.1/mmocr/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/visualization/base_visualizer.py` & `mmocr-1.0.1/mmocr/visualization/base_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/visualization/kie_visualizer.py` & `mmocr-1.0.1/mmocr/visualization/kie_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
                 `matplotlib.colors` for full list of formats that are accepted.
                 Defaults to 'g'.
 
         Returns:
             np.ndarray: The image with edge labels drawn.
         """
         pairs = np.where(edge_labels > 0)
+        if torch.is_tensor(pairs):
+            pairs = pairs.cpu()
         key_bboxes = bboxes[pairs[0]]
         value_bboxes = bboxes[pairs[1]]
         x_data = np.stack([(key_bboxes[:, 2] + key_bboxes[:, 0]) / 2,
                            (value_bboxes[:, 0] + value_bboxes[:, 2]) / 2],
                           axis=-1)
         y_data = np.stack([(key_bboxes[:, 1] + key_bboxes[:, 3]) / 2,
                            (value_bboxes[:, 1] + value_bboxes[:, 3]) / 2],
```

### Comparing `mmocr-1.0.0rc6/mmocr/visualization/textdet_visualizer.py` & `mmocr-1.0.1/mmocr/visualization/textdet_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/visualization/textrecog_visualizer.py` & `mmocr-1.0.1/mmocr/visualization/textrecog_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr/visualization/textspotting_visualizer.py` & `mmocr-1.0.1/mmocr/visualization/textspotting_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/mmocr.egg-info/PKG-INFO` & `mmocr-1.0.1/mmocr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmocr
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: OpenMMLab Text Detection, OCR, and NLP Toolbox
 Home-page: https://github.com/open-mmlab/mmocr
 Maintainer: MMOCR Authors
 Maintainer-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmocr-logo.png" width="500px"/>
@@ -46,42 +46,44 @@
         <div align="center">
         
         English | [简体中文](README_zh-CN.md)
         
         </div>
         <div align="center">
           <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218352562-cdded397-b0f3-4ca1-b8dd-a60df8dca75b.png" width="3%" alt="" /></a>
+            <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
         ## Latest Updates
         
-        **The default branch has been switched to `1.x` from `main`, and we encourage
-        users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html) for more
-        details.**
-        
-        v1.0.0rc6 was released in 2023-03-07.
-        
-        1. Two new models, ABCNet v2 (inference only) and SPTS are added to `projects/` folder.
-        2. Announcing `Inferencer`, a unified inference interface in OpenMMLab for everyone's easy access and quick inference with all the pre-trained weights. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/inference.html)
-        3. Users can use test-time augmentation for text recognition tasks. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/train_test.html#test-time-augmentation)
-        4. Support [batch augmentation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf) through [`BatchAugSampler`](https://github.com/open-mmlab/mmocr/pull/1757), which is a technique used in SPTS.
-        5. Dataset Preparer has been refactored to allow more flexible configurations. Besides, users are now able to prepare text recognition datasets in LMDB formats. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/dataset_preparer.html#lmdb-format)
-        6. Some textspotting datasets have been revised to enhance the correctness and consistency with the common practice.
-        7. Potential spurious warnings from `shapely` have been eliminated.
+        **The default branch is now `main` and the code on the branch has been upgraded to v1.0.0. The old `main` branch (v0.6.3) code now exists on the `0.x` branch.** If you have been using the `main` branch and encounter upgrade issues, please read the [Migration Guide](https://mmocr.readthedocs.io/en/dev-1.x/migration/overview.html) and notes on [Branches](https://mmocr.readthedocs.io/en/dev-1.x/migration/branches.html) .
+        
+        v1.0.0 was released in 2023-04-06. Major updates from 1.0.0rc6 include:
+        
+        1. Support for SCUT-CTW1500, SynthText, and MJSynth datasets in Dataset Preparer
+        2. Updated FAQ and documentation
+        3. Deprecation of file_client_args in favor of backend_args
+        4. Added a new MMOCR tutorial notebook
         
+        To know more about the updates in MMOCR 1.0, please refer to [What's New in MMOCR 1.x](https://mmocr.readthedocs.io/en/dev-1.x/migration/news.html), or
         Read [Changelog](https://mmocr.readthedocs.io/en/dev-1.x/notes/changelog.html) for more details!
         
         ## Introduction
         
         MMOCR is an open-source toolbox based on PyTorch and mmdetection for text detection, text recognition, and the corresponding downstream tasks including key information extraction. It is part of the [OpenMMLab](https://openmmlab.com/) project.
         
         The main branch works with **PyTorch 1.6+**.
@@ -104,49 +106,27 @@
         
           The modular design of MMOCR enables users to define their own optimizers, data preprocessors, and model components such as backbones, necks and heads as well as losses. Please refer to [Overview](https://mmocr.readthedocs.io/en/dev-1.x/get_started/overview.html) for how to construct a customized model.
         
         - **Numerous Utilities**
         
           The toolbox provides a comprehensive set of utilities which can help users assess the performance of models. It includes visualizers which allow visualization of images, ground truths as well as predicted bounding boxes, and a validation tool for evaluating checkpoints during training.  It also includes data converters to demonstrate how to convert your own data to the annotation files which the toolbox supports.
         
-        ## What's New in MMOCR 1.0
-        
-        1. **New engines**. MMOCR 1.x is based on [MMEngine](https://github.com/open-mmlab/mmengine), which provides a general and powerful runner that allows more flexible customizations and significantly simplifies the entrypoints of high-level interfaces.
-        
-        2. **Unified interfaces**. As a part of the OpenMMLab 2.0 projects, MMOCR 1.x unifies and refactors the interfaces and internal logics of train, testing, datasets, models, evaluation, and visualization. All the OpenMMLab 2.0 projects share the same design in those interfaces and logics to allow the emergence of multi-task/modality algorithms.
-        
-        3. **Cross project calling**. Benefiting from the unified design, you can use the models implemented in other OpenMMLab projects, such as MMDet. We provide an example of how to use MMDetection's Mask R-CNN through `MMDetWrapper`. Check our documents for more details. More wrappers will be released in the future.
-        
-        4. **Stronger visualization**. We provide a series of useful tools which are mostly based on brand-new visualizers. As a result, it is more convenient for the users to explore the models and datasets now.
-        
-        5. **More documentation and tutorials**. We add a bunch of documentation and tutorials to help users get started more smoothly. Read it [here](https://mmocr.readthedocs.io/en/dev-1.x/).
-        
-        6. **One-stop Dataset Preparaion**. Multiple datasets are instantly ready with only one line of command, via our [Dataset Preparer](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/dataset_preparer.html).
-        
-        7. **Embracing more `projects/`**: We now introduce `projects/` folder, where some experimental features, frameworks and models can be placed, only needed to satisfy the minimum requirement on the code quality. Everyone is welcome to post their implementation of any great ideas in this folder! Learn more from our [example project](https://github.com/open-mmlab/mmocr/blob/dev-1.x/projects/example_project/).
-        
-        8. **More models**. MMOCR 1.0 supports more tasks and more state-of-the-art models!
-        
         ## Installation
         
         MMOCR depends on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-mmlab/mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection](https://github.com/open-mmlab/mmdetection).
         Below are quick steps for installation.
         Please refer to [Install Guide](https://mmocr.readthedocs.io/en/dev-1.x/get_started/install.html) for more detailed instruction.
         
         ```shell
         conda create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -y
         conda activate open-mmlab
         pip3 install openmim
-        mim install mmengine
-        mim install 'mmcv>=2.0.0rc1'
-        mim install 'mmdet>=3.0.0rc0'
         git clone https://github.com/open-mmlab/mmocr.git
         cd mmocr
-        git checkout 1.x
-        pip3 install -e .
+        mim install -e .
         ```
         
         ## Get Started
         
         Please see [Quick Run](https://mmocr.readthedocs.io/en/dev-1.x/get_started/quick_run.html) for the basic usage of MMOCR.
         
         ## [Model Zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html)
@@ -202,14 +182,18 @@
         - [x] [ABCNetV2](projects/ABCNet/README_V2.md) (TPAMI'2021)
         - [x] [SPTS](projects/SPTS/README.md) (ACM MM'2022)
         
         </details>
         
         Please refer to [model_zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more details.
         
+        ## Projects
+        
+        [Here](projects/README.md) are some implementations of SOTA models and solutions built on MMOCR, which are supported and maintained by community users. These projects demonstrate the best practices based on MMOCR for research and product development. We welcome and appreciate all the contributions to OpenMMLab ecosystem.
+        
         ## Contributing
         
         We appreciate all contributions to improve MMOCR. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guidelines.
         
         ## Acknowledgement
         
         MMOCR is an open-source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
@@ -228,15 +212,15 @@
         }
         ```
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE).
         
-        ## Projects in OpenMMLab
+        ## OpenMMLab Family
         
         - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
         - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
         - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
         - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmocr Version: 1.0.0rc6 Summary: OpenMMLab Text
+Metadata-Version: 2.1 Name: mmocr Version: 1.0.1 Summary: OpenMMLab Text
 Detection, OCR, and NLP Toolbox Home-page: https://github.com/open-mmlab/mmocr
 Maintainer: MMOCR Authors Maintainer-email: openmmlab@gmail.com License: Apache
 License 2.0 Description:
                           [resources/mmocr-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
@@ -22,35 +22,26 @@
       mmocr.readthedocs.io/en/dev-1.x/) | [ð ï¸Installation](https://
   mmocr.readthedocs.io/en/dev-1.x/get_started/install.html) | [ðModel Zoo]
   (https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) | [ðUpdate News]
 (https://mmocr.readthedocs.io/en/dev-1.x/notes/changelog.html) | [ð¤Reporting
         Issues](https://github.com/open-mmlab/mmocr/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-## Latest Updates **The default branch has been switched to `1.x` from `main`,
-and we encourage users to migrate to the latest version, though it comes with
-some cost. Please refer to [Migration Guide](https://mmocr.readthedocs.io/en/
-dev-1.x/migration/overview.html) for more details.** v1.0.0rc6 was released in
-2023-03-07. 1. Two new models, ABCNet v2 (inference only) and SPTS are added to
-`projects/` folder. 2. Announcing `Inferencer`, a unified inference interface
-in OpenMMLab for everyone's easy access and quick inference with all the pre-
-trained weights. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/
-inference.html) 3. Users can use test-time augmentation for text recognition
-tasks. [Docs](https://mmocr.readthedocs.io/en/dev-1.x/user_guides/
-train_test.html#test-time-augmentation) 4. Support [batch augmentation](https:/
-/openaccess.thecvf.com/content_CVPR_2020/papers/
-Hoffer_Augment_Your_Batch_Improving_Generalization_Through_Instance_Repetition_CVPR_2020_paper.pdf)
-through [`BatchAugSampler`](https://github.com/open-mmlab/mmocr/pull/1757),
-which is a technique used in SPTS. 5. Dataset Preparer has been refactored to
-allow more flexible configurations. Besides, users are now able to prepare text
-recognition datasets in LMDB formats. [Docs](https://mmocr.readthedocs.io/en/
-dev-1.x/user_guides/data_prepare/dataset_preparer.html#lmdb-format) 6. Some
-textspotting datasets have been revised to enhance the correctness and
-consistency with the common practice. 7. Potential spurious warnings from
-`shapely` have been eliminated. Read [Changelog](https://mmocr.readthedocs.io/
+## Latest Updates **The default branch is now `main` and the code on the branch
+has been upgraded to v1.0.0. The old `main` branch (v0.6.3) code now exists on
+the `0.x` branch.** If you have been using the `main` branch and encounter
+upgrade issues, please read the [Migration Guide](https://mmocr.readthedocs.io/
+en/dev-1.x/migration/overview.html) and notes on [Branches](https://
+mmocr.readthedocs.io/en/dev-1.x/migration/branches.html) . v1.0.0 was released
+in 2023-04-06. Major updates from 1.0.0rc6 include: 1. Support for SCUT-
+CTW1500, SynthText, and MJSynth datasets in Dataset Preparer 2. Updated FAQ and
+documentation 3. Deprecation of file_client_args in favor of backend_args 4.
+Added a new MMOCR tutorial notebook To know more about the updates in MMOCR
+1.0, please refer to [What's New in MMOCR 1.x](https://mmocr.readthedocs.io/en/
+dev-1.x/migration/news.html), or Read [Changelog](https://mmocr.readthedocs.io/
 en/dev-1.x/notes/changelog.html) for more details! ## Introduction MMOCR is an
 open-source toolbox based on PyTorch and mmdetection for text detection, text
 recognition, and the corresponding downstream tasks including key information
 extraction. It is part of the [OpenMMLab](https://openmmlab.com/) project. The
 main branch works with **PyTorch 1.6+**.
  [https://user-images.githubusercontent.com/24622904/187838618-1fdc61c0-2d46-
                           49f9-8502-976ffdf01f28.png]
@@ -64,126 +55,102 @@
 to [Overview](https://mmocr.readthedocs.io/en/dev-1.x/get_started/
 overview.html) for how to construct a customized model. - **Numerous
 Utilities** The toolbox provides a comprehensive set of utilities which can
 help users assess the performance of models. It includes visualizers which
 allow visualization of images, ground truths as well as predicted bounding
 boxes, and a validation tool for evaluating checkpoints during training. It
 also includes data converters to demonstrate how to convert your own data to
-the annotation files which the toolbox supports. ## What's New in MMOCR 1.0 1.
-**New engines**. MMOCR 1.x is based on [MMEngine](https://github.com/open-
-mmlab/mmengine), which provides a general and powerful runner that allows more
-flexible customizations and significantly simplifies the entrypoints of high-
-level interfaces. 2. **Unified interfaces**. As a part of the OpenMMLab 2.0
-projects, MMOCR 1.x unifies and refactors the interfaces and internal logics of
-train, testing, datasets, models, evaluation, and visualization. All the
-OpenMMLab 2.0 projects share the same design in those interfaces and logics to
-allow the emergence of multi-task/modality algorithms. 3. **Cross project
-calling**. Benefiting from the unified design, you can use the models
-implemented in other OpenMMLab projects, such as MMDet. We provide an example
-of how to use MMDetection's Mask R-CNN through `MMDetWrapper`. Check our
-documents for more details. More wrappers will be released in the future. 4.
-**Stronger visualization**. We provide a series of useful tools which are
-mostly based on brand-new visualizers. As a result, it is more convenient for
-the users to explore the models and datasets now. 5. **More documentation and
-tutorials**. We add a bunch of documentation and tutorials to help users get
-started more smoothly. Read it [here](https://mmocr.readthedocs.io/en/dev-1.x/
-). 6. **One-stop Dataset Preparaion**. Multiple datasets are instantly ready
-with only one line of command, via our [Dataset Preparer](https://
-mmocr.readthedocs.io/en/dev-1.x/user_guides/data_prepare/
-dataset_preparer.html). 7. **Embracing more `projects/`**: We now introduce
-`projects/` folder, where some experimental features, frameworks and models can
-be placed, only needed to satisfy the minimum requirement on the code quality.
-Everyone is welcome to post their implementation of any great ideas in this
-folder! Learn more from our [example project](https://github.com/open-mmlab/
-mmocr/blob/dev-1.x/projects/example_project/). 8. **More models**. MMOCR 1.0
-supports more tasks and more state-of-the-art models! ## Installation MMOCR
-depends on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-
-mmlab/mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection]
-(https://github.com/open-mmlab/mmdetection). Below are quick steps for
-installation. Please refer to [Install Guide](https://mmocr.readthedocs.io/en/
-dev-1.x/get_started/install.html) for more detailed instruction. ```shell conda
-create -n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -
-c pytorch -y conda activate open-mmlab pip3 install openmim mim install
-mmengine mim install 'mmcv>=2.0.0rc1' mim install 'mmdet>=3.0.0rc0' git clone
-https://github.com/open-mmlab/mmocr.git cd mmocr git checkout 1.x pip3 install
--e . ``` ## Get Started Please see [Quick Run](https://mmocr.readthedocs.io/en/
-dev-1.x/get_started/quick_run.html) for the basic usage of MMOCR. ## [Model
-Zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) Supported
-algorithms:  BackBone - [x] [oCLIP](configs/backbone/oclip/README.md)
-(ECCV'2022)   Text Detection - [x] [DBNet](configs/textdet/dbnet/README.md)
-(AAAI'2020) / [DBNet++](configs/textdet/dbnetpp/README.md) (TPAMI'2022) - [x]
-[Mask R-CNN](configs/textdet/maskrcnn/README.md) (ICCV'2017) - [x] [PANet]
-(configs/textdet/panet/README.md) (ICCV'2019) - [x] [PSENet](configs/textdet/
-psenet/README.md) (CVPR'2019) - [x] [TextSnake](configs/textdet/textsnake/
-README.md) (ECCV'2018) - [x] [DRRG](configs/textdet/drrg/README.md) (CVPR'2020)
-- [x] [FCENet](configs/textdet/fcenet/README.md) (CVPR'2021)   Text Recognition
-- [x] [ABINet](configs/textrecog/abinet/README.md) (CVPR'2021) - [x] [ASTER]
-(configs/textrecog/aster/README.md) (TPAMI'2018) - [x] [CRNN](configs/
-textrecog/crnn/README.md) (TPAMI'2016) - [x] [MASTER](configs/textrecog/master/
-README.md) (PR'2021) - [x] [NRTR](configs/textrecog/nrtr/README.md)
-(ICDAR'2019) - [x] [RobustScanner](configs/textrecog/robust_scanner/README.md)
-(ECCV'2020) - [x] [SAR](configs/textrecog/sar/README.md) (AAAI'2019) - [x]
-[SATRN](configs/textrecog/satrn/README.md) (CVPR'2020 Workshop on Text and
-Documents in the Deep Learning Era) - [x] [SVTR](configs/textrecog/svtr/
-README.md) (IJCAI'2022)   Key Information Extraction - [x] [SDMG-R](configs/
-kie/sdmgr/README.md) (ArXiv'2021)   Text Spotting - [x] [ABCNet](projects/
-ABCNet/README.md) (CVPR'2020) - [x] [ABCNetV2](projects/ABCNet/README_V2.md)
-(TPAMI'2021) - [x] [SPTS](projects/SPTS/README.md) (ACM MM'2022)  Please refer
-to [model_zoo](https://mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more
-details. ## Contributing We appreciate all contributions to improve MMOCR.
-Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
-guidelines. ## Acknowledgement MMOCR is an open-source project that is
-contributed by researchers and engineers from various colleges and companies.
-We appreciate all the contributors who implement their methods or add new
-features, as well as users who give valuable feedbacks. We hope the toolbox and
-benchmark could serve the growing research community by providing a flexible
-toolkit to reimplement existing methods and develop their own new OCR methods.
-## Citation If you find this project useful in your research, please consider
-cite: ```bibtex @article{mmocr2021, title={MMOCR: A Comprehensive Toolbox for
-Text Detection, Recognition and Understanding}, author={Kuang, Zhanghui and
-Sun, Hongbin and Li, Zhizhong and Yue, Xiaoyu and Lin, Tsui Hin and Chen,
-Jianyong and Wei, Huaqiang and Zhu, Yiqin and Gao, Tong and Zhang, Wenwei and
-Chen, Kai and Zhang, Wayne and Lin, Dahua}, journal= {arXiv preprint arXiv:
-2108.06543}, year={2021} } ``` ## License This project is released under the
-[Apache 2.0 license](LICENSE). ## Projects in OpenMMLab - [MMEngine](https://
-github.com/open-mmlab/mmengine): OpenMMLab foundational library for training
-deep learning models - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab
-foundational library for computer vision. - [MIM](https://github.com/open-
-mmlab/mim): MIM installs OpenMMLab packages. - [MMClassification](https://
-github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox
-and benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection):
-OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
-github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
-general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
-mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
-[MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab
-semantic segmentation toolbox and benchmark. - [MMOCR](https://github.com/open-
-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation
-toolbox and benchmark. - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d):
-OpenMMLab 3D human parametric model toolbox and benchmark. - [MMSelfSup](https:
-//github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox
-and benchmark. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab
-model compression toolbox and benchmark. - [MMFewShot](https://github.com/open-
-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark. -
-[MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-
-generation action understanding toolbox and benchmark. - [MMTracking](https://
-github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and
-benchmark. - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical
-flow toolbox and benchmark. - [MMEditing](https://github.com/open-mmlab/
-mmediting): OpenMMLab image and video editing toolbox. - [MMGeneration](https:/
-/github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative
-models toolbox. - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab
-model deployment framework. ## Welcome to the OpenMMLab community Scan the QR
-code below to follow the OpenMMLab team's [**Zhihu Official Account**](https://
-www.zhihu.com/people/openmmlab) and join the OpenMMLab team's [**QQ Group**]
-(https://jq.qq.com/?_wv=1027&k=aCvMxdr3), or join the official communication
-WeChat group by adding the WeChat, or join our [**Slack**](https://
-join.slack.com/t/mmocrworkspace/shared_invite/zt-1ifqhfla8-
-yKnLO_aKhVA2h71OrK8GZw)
+the annotation files which the toolbox supports. ## Installation MMOCR depends
+on [PyTorch](https://pytorch.org/), [MMEngine](https://github.com/open-mmlab/
+mmengine), [MMCV](https://github.com/open-mmlab/mmcv) and [MMDetection](https:/
+/github.com/open-mmlab/mmdetection). Below are quick steps for installation.
+Please refer to [Install Guide](https://mmocr.readthedocs.io/en/dev-1.x/
+get_started/install.html) for more detailed instruction. ```shell conda create
+-n open-mmlab python=3.8 pytorch=1.10 cudatoolkit=11.3 torchvision -c pytorch -
+y conda activate open-mmlab pip3 install openmim git clone https://github.com/
+open-mmlab/mmocr.git cd mmocr mim install -e . ``` ## Get Started Please see
+[Quick Run](https://mmocr.readthedocs.io/en/dev-1.x/get_started/quick_run.html)
+for the basic usage of MMOCR. ## [Model Zoo](https://mmocr.readthedocs.io/en/
+dev-1.x/modelzoo.html) Supported algorithms:  BackBone - [x] [oCLIP](configs/
+backbone/oclip/README.md) (ECCV'2022)   Text Detection - [x] [DBNet](configs/
+textdet/dbnet/README.md) (AAAI'2020) / [DBNet++](configs/textdet/dbnetpp/
+README.md) (TPAMI'2022) - [x] [Mask R-CNN](configs/textdet/maskrcnn/README.md)
+(ICCV'2017) - [x] [PANet](configs/textdet/panet/README.md) (ICCV'2019) - [x]
+[PSENet](configs/textdet/psenet/README.md) (CVPR'2019) - [x] [TextSnake]
+(configs/textdet/textsnake/README.md) (ECCV'2018) - [x] [DRRG](configs/textdet/
+drrg/README.md) (CVPR'2020) - [x] [FCENet](configs/textdet/fcenet/README.md)
+(CVPR'2021)   Text Recognition - [x] [ABINet](configs/textrecog/abinet/
+README.md) (CVPR'2021) - [x] [ASTER](configs/textrecog/aster/README.md)
+(TPAMI'2018) - [x] [CRNN](configs/textrecog/crnn/README.md) (TPAMI'2016) - [x]
+[MASTER](configs/textrecog/master/README.md) (PR'2021) - [x] [NRTR](configs/
+textrecog/nrtr/README.md) (ICDAR'2019) - [x] [RobustScanner](configs/textrecog/
+robust_scanner/README.md) (ECCV'2020) - [x] [SAR](configs/textrecog/sar/
+README.md) (AAAI'2019) - [x] [SATRN](configs/textrecog/satrn/README.md)
+(CVPR'2020 Workshop on Text and Documents in the Deep Learning Era) - [x]
+[SVTR](configs/textrecog/svtr/README.md) (IJCAI'2022)   Key Information
+Extraction - [x] [SDMG-R](configs/kie/sdmgr/README.md) (ArXiv'2021)   Text
+Spotting - [x] [ABCNet](projects/ABCNet/README.md) (CVPR'2020) - [x] [ABCNetV2]
+(projects/ABCNet/README_V2.md) (TPAMI'2021) - [x] [SPTS](projects/SPTS/
+README.md) (ACM MM'2022)  Please refer to [model_zoo](https://
+mmocr.readthedocs.io/en/dev-1.x/modelzoo.html) for more details. ## Projects
+[Here](projects/README.md) are some implementations of SOTA models and
+solutions built on MMOCR, which are supported and maintained by community
+users. These projects demonstrate the best practices based on MMOCR for
+research and product development. We welcome and appreciate all the
+contributions to OpenMMLab ecosystem. ## Contributing We appreciate all
+contributions to improve MMOCR. Please refer to [CONTRIBUTING.md](.github/
+CONTRIBUTING.md) for the contributing guidelines. ## Acknowledgement MMOCR is
+an open-source project that is contributed by researchers and engineers from
+various colleges and companies. We appreciate all the contributors who
+implement their methods or add new features, as well as users who give valuable
+feedbacks. We hope the toolbox and benchmark could serve the growing research
+community by providing a flexible toolkit to reimplement existing methods and
+develop their own new OCR methods. ## Citation If you find this project useful
+in your research, please consider cite: ```bibtex @article{mmocr2021, title=
+{MMOCR: A Comprehensive Toolbox for Text Detection, Recognition and
+Understanding}, author={Kuang, Zhanghui and Sun, Hongbin and Li, Zhizhong and
+Yue, Xiaoyu and Lin, Tsui Hin and Chen, Jianyong and Wei, Huaqiang and Zhu,
+Yiqin and Gao, Tong and Zhang, Wenwei and Chen, Kai and Zhang, Wayne and Lin,
+Dahua}, journal= {arXiv preprint arXiv:2108.06543}, year={2021} } ``` ##
+License This project is released under the [Apache 2.0 license](LICENSE). ##
+OpenMMLab Family - [MMEngine](https://github.com/open-mmlab/mmengine):
+OpenMMLab foundational library for training deep learning models - [MMCV]
+(https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for
+computer vision. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [MMClassification](https://github.com/open-mmlab/
+mmclassification): OpenMMLab image classification toolbox and benchmark. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMDetection3D](https://github.com/open-mmlab/
+mmdetection3d): OpenMMLab's next-generation platform for general 3D object
+detection. - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab
+rotated object detection toolbox and benchmark. - [MMSegmentation](https://
+github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox
+and benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text
+detection, recognition, and understanding toolbox. - [MMPose](https://
+github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human
+parametric model toolbox and benchmark. - [MMSelfSup](https://github.com/open-
+mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark. -
+[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
+toolbox and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
+OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
+github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
+understanding toolbox and benchmark. - [MMTracking](https://github.com/open-
+mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark. - [MMFlow]
+(https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and
+benchmark. - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab
+image and video editing toolbox. - [MMGeneration](https://github.com/open-
+mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. ## Welcome to the OpenMMLab community Scan the QR code below to
+follow the OpenMMLab team's [**Zhihu Official Account**](https://www.zhihu.com/
+people/openmmlab) and join the OpenMMLab team's [**QQ Group**](https://
+jq.qq.com/?_wv=1027&k=aCvMxdr3), or join the official communication WeChat
+group by adding the WeChat, or join our [**Slack**](https://join.slack.com/t/
+mmocrworkspace/shared_invite/zt-1ifqhfla8-yKnLO_aKhVA2h71OrK8GZw)
   [https://raw.githubusercontent.com/open-mmlab/mmcv/master/docs/en/_static/
  zhihu_qrcode.jpg] [https://raw.githubusercontent.com/open-mmlab/mmcv/master/
  docs/en/_static/qq_group_qrcode.jpg] [https://raw.githubusercontent.com/open-
              mmlab/mmcv/master/docs/en/_static/wechat_qrcode.jpg]
 We will provide you with the OpenMMLab community - ð¢ share the latest core
 technologies of AI frameworks - ð» Explaining PyTorch common module source
 Code - ð° News related to the release of OpenMMLab - ð Introduction of
```

### Comparing `mmocr-1.0.0rc6/mmocr.egg-info/SOURCES.txt` & `mmocr-1.0.1/mmocr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -143,82 +143,79 @@
 mmocr/.mim/configs/textrecog/satrn/satrn_shallow_5e_st_mj.py
 mmocr/.mim/configs/textrecog/svtr/_base_svtr-tiny.py
 mmocr/.mim/configs/textrecog/svtr/metafile.yml
 mmocr/.mim/configs/textrecog/svtr/svtr-base_20e_st_mj.py
 mmocr/.mim/configs/textrecog/svtr/svtr-large_20e_st_mj.py
 mmocr/.mim/configs/textrecog/svtr/svtr-small_20e_st_mj.py
 mmocr/.mim/configs/textrecog/svtr/svtr-tiny_20e_st_mj.py
+mmocr/.mim/dicts/chinese_english_digits.txt
+mmocr/.mim/dicts/english_digits_symbols.txt
+mmocr/.mim/dicts/english_digits_symbols_space.txt
+mmocr/.mim/dicts/korean_english_digits_symbols.txt
+mmocr/.mim/dicts/lower_english_digits.txt
+mmocr/.mim/dicts/lower_english_digits_space.txt
+mmocr/.mim/dicts/sdmgr_dict.txt
 mmocr/.mim/tools/dist_test.sh
 mmocr/.mim/tools/dist_train.sh
 mmocr/.mim/tools/infer.py
 mmocr/.mim/tools/slurm_test.sh
 mmocr/.mim/tools/slurm_train.sh
 mmocr/.mim/tools/test.py
 mmocr/.mim/tools/train.py
-mmocr/.mim/tools/analysis_tools/browse_dataset.py
 mmocr/.mim/tools/analysis_tools/get_flops.py
 mmocr/.mim/tools/analysis_tools/offline_eval.py
 mmocr/.mim/tools/analysis_tools/print_config.py
 mmocr/.mim/tools/dataset_converters/prepare_dataset.py
 mmocr/.mim/tools/dataset_converters/common/curvedsyntext_converter.py
 mmocr/.mim/tools/dataset_converters/common/extract_kaist.py
 mmocr/.mim/tools/dataset_converters/kie/closeset_to_openset.py
 mmocr/.mim/tools/dataset_converters/textdet/art_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/bid_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/coco_to_line_dict.py
 mmocr/.mim/tools/dataset_converters/textdet/cocotext_converter.py
-mmocr/.mim/tools/dataset_converters/textdet/ctw1500_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/data_migrator.py
 mmocr/.mim/tools/dataset_converters/textdet/detext_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/funsd_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/hiertext_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/ic11_converter.py
-mmocr/.mim/tools/dataset_converters/textdet/ic13_converter.py
-mmocr/.mim/tools/dataset_converters/textdet/icdar_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/ilst_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/imgur_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/kaist_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/lsvt_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/lv_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/mtwi_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/naf_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/rctw_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/rects_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/sroie_converter.py
-mmocr/.mim/tools/dataset_converters/textdet/synthtext_converter.py
-mmocr/.mim/tools/dataset_converters/textdet/textocr_converter.py
-mmocr/.mim/tools/dataset_converters/textdet/totaltext_converter.py
 mmocr/.mim/tools/dataset_converters/textdet/vintext_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/art_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/bid_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/cocotext_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/data_migrator.py
 mmocr/.mim/tools/dataset_converters/textrecog/detext_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/funsd_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/hiertext_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/ic11_converter.py
-mmocr/.mim/tools/dataset_converters/textrecog/ic13_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/ilst_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/imgur_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/kaist_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/lmdb_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/lsvt_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/lv_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/mtwi_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/naf_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/openvino_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/rctw_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/rects_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/sroie_converter.py
-mmocr/.mim/tools/dataset_converters/textrecog/svt_converter.py
-mmocr/.mim/tools/dataset_converters/textrecog/synthtext_converter.py
-mmocr/.mim/tools/dataset_converters/textrecog/textocr_converter.py
-mmocr/.mim/tools/dataset_converters/textrecog/totaltext_converter.py
 mmocr/.mim/tools/dataset_converters/textrecog/vintext_converter.py
 mmocr/.mim/tools/model_converters/publish_model.py
+mmocr/.mim/tools/visualizations/browse_dataset.py
+mmocr/.mim/tools/visualizations/vis_scheduler.py
 mmocr/apis/__init__.py
 mmocr/apis/inferencers/__init__.py
 mmocr/apis/inferencers/base_mmocr_inferencer.py
 mmocr/apis/inferencers/kie_inferencer.py
 mmocr/apis/inferencers/mmocr_inferencer.py
 mmocr/apis/inferencers/textdet_inferencer.py
 mmocr/apis/inferencers/textrec_inferencer.py
@@ -244,29 +241,33 @@
 mmocr/datasets/preparers/dumpers/wild_receipt_openset_dumper.py
 mmocr/datasets/preparers/gatherers/__init__.py
 mmocr/datasets/preparers/gatherers/base.py
 mmocr/datasets/preparers/gatherers/mono_gatherer.py
 mmocr/datasets/preparers/gatherers/naf_gatherer.py
 mmocr/datasets/preparers/gatherers/pair_gatherer.py
 mmocr/datasets/preparers/obtainers/__init__.py
+mmocr/datasets/preparers/obtainers/aws_s3_obtainer.py
 mmocr/datasets/preparers/obtainers/naive_data_obtainer.py
 mmocr/datasets/preparers/packers/__init__.py
 mmocr/datasets/preparers/packers/base.py
 mmocr/datasets/preparers/packers/textdet_packer.py
 mmocr/datasets/preparers/packers/textrecog_packer.py
 mmocr/datasets/preparers/packers/textspotting_packer.py
 mmocr/datasets/preparers/packers/wildreceipt_packer.py
 mmocr/datasets/preparers/parsers/__init__.py
 mmocr/datasets/preparers/parsers/base.py
 mmocr/datasets/preparers/parsers/coco_parser.py
+mmocr/datasets/preparers/parsers/ctw1500_parser.py
 mmocr/datasets/preparers/parsers/funsd_parser.py
 mmocr/datasets/preparers/parsers/icdar_txt_parser.py
+mmocr/datasets/preparers/parsers/mjsynth_parser.py
 mmocr/datasets/preparers/parsers/naf_parser.py
 mmocr/datasets/preparers/parsers/sroie_parser.py
 mmocr/datasets/preparers/parsers/svt_parser.py
+mmocr/datasets/preparers/parsers/synthtext_parser.py
 mmocr/datasets/preparers/parsers/totaltext_parser.py
 mmocr/datasets/preparers/parsers/wildreceipt_parser.py
 mmocr/datasets/samplers/__init__.py
 mmocr/datasets/samplers/batch_aug.py
 mmocr/datasets/transforms/__init__.py
 mmocr/datasets/transforms/adapters.py
 mmocr/datasets/transforms/formatting.py
```

### Comparing `mmocr-1.0.0rc6/mmocr.egg-info/requires.txt` & `mmocr-1.0.1/mmocr.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 imgaug
-lanms-neo==1.0.2
 lmdb
 matplotlib
 numpy
 opencv-python!=4.5.5.*,>=4.2.0.32
 pyclipper
 pycocotools
 rapidfuzz>=2.0.0
 scikit-image
 
 [all]
 numpy
 pyclipper
 torch>=1.1
+boto3
 imgaug
-lanms-neo==1.0.2
 lmdb
 matplotlib
 numpy
 opencv-python!=4.5.5.*,>=4.2.0.32
 pyclipper
 pycocotools
 rapidfuzz>=2.0.0
 scikit-image
 asynctest
 codecov
 flake8
 interrogate
 isort
 kwarray
+lanms-neo==1.0.2
 parameterized
 pytest
 pytest-cov
 pytest-runner
 ubelt
 xdoctest>=0.10.0
 yapf
 
 [build]
 numpy
 pyclipper
 torch>=1.1
 
 [mim]
-mmcv<2.1.0,>==2.0.0rc4
-mmdet<3.1.0,>=3.0.0rc5
-mmengine<1.0.0,>=0.6.0
+mmcv<2.2.0,>=2.0.0rc4
+mmdet<3.2.0,>=3.0.0rc5
+mmengine<1.1.0,>=0.7.0
 
 [optional]
+boto3
 
 [tests]
 asynctest
 codecov
 flake8
 interrogate
 isort
 kwarray
+lanms-neo==1.0.2
 parameterized
 pytest
 pytest-cov
 pytest-runner
 ubelt
 xdoctest>=0.10.0
 yapf
```

### Comparing `mmocr-1.0.0rc6/setup.cfg` & `mmocr-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmocr-1.0.0rc6/setup.py` & `mmocr-1.0.1/setup.py`

 * *Files identical despite different names*

