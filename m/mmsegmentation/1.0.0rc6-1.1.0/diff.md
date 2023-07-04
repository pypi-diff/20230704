# Comparing `tmp/mmsegmentation-1.0.0rc6.tar.gz` & `tmp/mmsegmentation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmsegmentation-1.0.0rc6.tar", last modified: Fri Mar  3 09:29:29 2023, max compression
+gzip compressed data, was "dist/mmsegmentation-1.1.0.tar", last modified: Tue Jul  4 03:20:55 2023, max compression
```

## Comparing `mmsegmentation-1.0.0rc6.tar` & `mmsegmentation-1.1.0.tar`

### file list

```diff
@@ -1,1151 +1,1197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/isaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/loveda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/potsdam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/refuge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/vaihingen.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/bisenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/erfnet_fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/setr_mla.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/setr_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/setr_pup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/stdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_convnext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_swin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_320k.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb8-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-amp-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/cgnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)    26875 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-769x769.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/
--rw-r--r--   0 runner    (1001) docker     (123)    30163 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-769x769.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnlnet.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dpt/dpt.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/emanet/
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/emanet/emanet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-769x769.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/encnet/encnet_r50s-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/erfnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/erfnet/erfnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/erfnet/erfnet_fcn_4xb4-160k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn.yml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastscnn/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastscnn/fastscnn.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-769x769.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/hrnet.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-80k_cityscapes-832x832.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mae/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mae/mae.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_r101-d32_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v2/mobilenet_v2.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet_v3.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_net.yml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/point_rend.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/pointrend_r101_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/pointrend_r101_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/fpn_poolformer_m36_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/fpn_poolformer_m48_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/fpn_poolformer_s24_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/fpn_poolformer_s36_8x4_512x512_40k_ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/poolformer.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/
--rw-r--r--   0 runner    (1001) docker     (123)    36141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d32_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50b-d32_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-769x769.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb2-80k_cityscapes512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb4-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-b_mask_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-s_fcn_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/sem_fpn/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/sem_fpn/sem_fpn.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/stdc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/stdc1_in1k-pre_4xb12-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/stdc2_4xb12-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/stdc2_in1k-pre_4xb12-80k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-base-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-large-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-b_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-l_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-b_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet_s5-d16_deeplabv3_4xb4-40k_chase-db1-128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r101_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r18_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r18_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r18_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r18_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r18_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r18_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/upernet/upernet_r50_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-s16-ln_mln_upernet_512x512_160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-s16_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-03 09:29:28.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/analyze_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/get_flops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/isaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/loveda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/potsdam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/refuge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/vaihingen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/voc_aug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/deployment/pytorch2torchscript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dist_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/print_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/publish_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/beit2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/mit2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/stdc2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/swin2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/twins2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/vit2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/vitjax2mmseg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/slurm_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/mmseg2torchserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/mmseg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/test_torchserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/.mim/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/apis/mmseg_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/basesegdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/coco_stuff.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/dark_zurich.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/decathlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/isaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/isprs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/lip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/loveda.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/night_driving.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/potsdam.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/refuge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/synapse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)    73873 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/engine/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/engine/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/evaluation/metrics/citys_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/evaluation/metrics/iou_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22825 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/bisenetv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/bisenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/erfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/icnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/mit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25701 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/stdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29703 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/swin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/timm_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)    23612 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/twins.py
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/data_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/dpt_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/isa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/knet_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/mask2former_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/maskformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/segformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/segmenter_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/setr_mla_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/setr_up_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/stdc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/featurepyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/ic_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/jpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/mla_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/segmentors/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/segmentors/seg_tta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/shape_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/models/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/structures/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/structures/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/structures/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/structures/sampler/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/structures/sampler/ohem_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/structures/seg_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/set_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/utils/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmseg/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/mmseg/visualization/local_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    65227 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7365 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_digit_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_bisenetv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_bisenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_erfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_icnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_mit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_stdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_swin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_timm_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)    30209 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_dpt_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_isa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_mask2former_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_maskformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_segformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_segmenter_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_setr_mla_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_setr_up_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_uper_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_heads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_feature2pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_ic_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_jpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_mla_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/test_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/test_seg_tta_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 09:29:29.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_utils/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_models/test_utils/test_shape_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-03 09:29:19.000000 mmsegmentation-1.0.0rc6/tests/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17883 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/isaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/levir_256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/loveda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v1_65.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/potsdam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/refuge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/vaihingen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/erfnet_fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_mla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_pup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/stdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_240k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_320k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb8-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-amp-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/ddrnet_23-slim_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/ddrnet_23_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44665 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-300k_mapillay_v1_65-1280x1280.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49026 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50s-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/erfnet_fcn_4xb4-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16642 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36768 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_r101-d32_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-80k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    24899 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-l_2xb6-120k_1024x1024-cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-m_2xb6-120k_1024x1024-cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-s_2xb6-120k_1024x1024-cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r101_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r101_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_m36_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_m48_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s24_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s36_8x4_512x512_40k_ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-80k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    55003 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d32_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50b-d32_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-769x769.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb2-80k_cityscapes512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb4-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-b_mask_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-s_fcn_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-b_1xb16-adamw-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-l_1xb16-adamw-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-s_1xb16-adamw-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-t_1xb16-adamw-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc1_in1k-pre_4xb12-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc2_4xb12-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc2_in1k-pre_4xb12-80k_cityscapes-512x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-large-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-b_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-l_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-b_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet_s5-d16_deeplabv3_4xb4-40k_chase-db1-128x128.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-80k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmseg/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/analyze_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/get_flops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/isaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/levircd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/loveda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/potsdam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/refuge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/vaihingen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/voc_aug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/deployment/pytorch2torchscript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dist_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/print_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/publish_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/beit2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/mit2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/stdc2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/swin2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/twins2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vit2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vitjax2mmseg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg2torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/test_torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/apis/mmseg_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/basesegdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/coco_stuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/dark_zurich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/decathlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/dsdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/isaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/isprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/levir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/lip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/loveda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/mapillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/night_driving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/potsdam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/refuge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/synapse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/engine/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/citys_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/iou_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22825 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/ddrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/erfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/icnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/pidnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25701 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/stdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29843 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/timm_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23612 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/data_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ddr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/dpt_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ham_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/isa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/knet_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/mask2former_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/maskformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/pid_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/segformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/segmenter_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_mla_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_up_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/stdc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/boundary_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/huasdorff_distance_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/ohem_cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/featurepyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/ic_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/jpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/mla_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14659 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/seg_tta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/basic_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/ppm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/shape_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/ohem_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/seg_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/set_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/visualization/local_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    67418 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/albu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7387 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_digit_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_erfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_icnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_pidnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_stdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_timm_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30209 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_dpt_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ham_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_isa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_mask2former_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_maskformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_pidnet_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_segformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_segmenter_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_mla_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_up_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_uper_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_feature2pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_ic_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_jpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_mla_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_seg_tta_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/test_shape_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_sampler.py
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/ade20k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/chase_db1.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/drive.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/hrf.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/isaid.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/isaid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/loveda.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/loveda.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_context.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/potsdam.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/potsdam.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/refuge.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/refuge.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/stare.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/synapse.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/synapse.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/datasets/vaihingen.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/vaihingen.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ann_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/bisenetv2.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/cgnet.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/danet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/erfnet_fcn.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/erfnet_fcn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fast_scnn.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fcn_hr18.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # model settings
 norm_cfg = dict(type='SyncBN', requires_grad=True)
 checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/poolformer/poolformer-s12_3rdparty_32xb128_in1k_20220414-f8d83051.pth'  # noqa
-# TODO: delete custom_imports after mmcls supports auto import
-# please install mmcls>=1.0
-# import mmcls.models to trigger register_module in mmcls
-custom_imports = dict(imports=['mmcls.models'], allow_failed_imports=False)
+# TODO: delete custom_imports after mmpretrain supports auto import
+# please install mmpretrain >= 1.0.0rc7
+# import mmpretrain.models to trigger register_module in mmpretrain
+custom_imports = dict(
+    imports=['mmpretrain.models'], allow_failed_imports=False)
 data_preprocessor = dict(
     type='SegDataPreProcessor',
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     bgr_to_rgb=True,
     pad_val=0,
     seg_pad_val=255)
 model = dict(
     type='EncoderDecoder',
     data_preprocessor=data_preprocessor,
     backbone=dict(
-        type='mmcls.PoolFormer',
+        type='mmpretrain.PoolFormer',
         arch='s12',
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file, prefix='backbone.'),
         in_patch_size=7,
         in_stride=4,
         in_pad=2,
         down_patch_size=3,
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/fpn_r50.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/pointrend_r50.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/setr_mla.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_mla.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/setr_naive.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_naive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/setr_pup.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_pup.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/stdc.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/stdc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_beit.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_beit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_convnext.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_convnext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 norm_cfg = dict(type='SyncBN', requires_grad=True)
-custom_imports = dict(imports='mmcls.models', allow_failed_imports=False)
+custom_imports = dict(imports='mmpretrain.models', allow_failed_imports=False)
 checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-base_3rdparty_32xb128-noema_in1k_20220301-2a0ee547.pth'  # noqa
 data_preprocessor = dict(
     type='SegDataPreProcessor',
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     bgr_to_rgb=True,
     pad_val=0,
     seg_pad_val=255)
 model = dict(
     type='EncoderDecoder',
     data_preprocessor=data_preprocessor,
     pretrained=None,
     backbone=dict(
-        type='mmcls.ConvNeXt',
+        type='mmpretrain.ConvNeXt',
         arch='base',
         out_indices=[0, 1, 2, 3],
         drop_path_rate=0.4,
         layer_scale_init_value=1.0,
         gap_before_final_norm=False,
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file,
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_mae.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_mae.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_r50.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_swin.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_swin.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_160k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_160k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_20k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_20k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_320k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_320k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_40k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_40k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/_base_/schedules/schedule_80k.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_80k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/cgnet.yml` & `mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/metafile.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 Collections:
 - Name: CGNet
+  License: Apache License 2.0
   Metadata:
     Training Data:
     - Cityscapes
   Paper:
-    URL: https://arxiv.org/abs/1811.08201
     Title: 'CGNet: A Light-weight Context Guided Network for Semantic Segmentation'
+    URL: https://arxiv.org/abs/1811.08201
   README: configs/cgnet/README.md
-  Code:
-    URL: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/cgnet.py#L187
-    Version: v0.17.0
-  Converted From:
-    Code: https://github.com/wutianyiRosun/CGNet
+  Frameworks:
+  - PyTorch
 Models:
 - Name: cgnet_fcn_4xb4-60k_cityscapes-680x680
   In Collection: CGNet
-  Metadata:
-    backbone: M3N21
-    crop size: (680,680)
-    lr schd: 60000
-    inference time (ms/im):
-    - value: 32.78
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (680,680)
-    Training Memory (GB): 7.5
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 65.63
       mIoU(ms+flip): 68.04
   Config: configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 16
+    Architecture:
+    - M3N21
+    - CGNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 7.5
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/cgnet/cgnet_680x680_60k_cityscapes/cgnet_680x680_60k_cityscapes_20201101_110253-4c0b2f2d.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/cgnet/cgnet_680x680_60k_cityscapes/cgnet_680x680_60k_cityscapes-20201101_110253.log.json
+  Paper:
+    Title: 'CGNet: A Light-weight Context Guided Network for Semantic Segmentation'
+    URL: https://arxiv.org/abs/1811.08201
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/cgnet.py#L187
+  Framework: PyTorch
 - Name: cgnet_fcn_4xb8-60k_cityscapes-512x1024
   In Collection: CGNet
-  Metadata:
-    backbone: M3N21
-    crop size: (512,1024)
-    lr schd: 60000
-    inference time (ms/im):
-    - value: 32.11
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 8.3
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 68.27
       mIoU(ms+flip): 70.33
   Config: configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 32
+    Architecture:
+    - M3N21
+    - CGNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 8.3
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/cgnet/cgnet_512x1024_60k_cityscapes/cgnet_512x1024_60k_cityscapes_20201101_110254-124ea03b.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/cgnet/cgnet_512x1024_60k_cityscapes/cgnet_512x1024_60k_cityscapes-20201101_110254.log.json
+  Paper:
+    Title: 'CGNet: A Light-weight Context Guided Network for Semantic Segmentation'
+    URL: https://arxiv.org/abs/1811.08201
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/cgnet.py#L187
+  Framework: PyTorch
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 crop_size = (640, 640)
 data_preprocessor = dict(size=crop_size)
 checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-base_3rdparty_in21k_20220301-262fd037.pth'  # noqa
 model = dict(
     data_preprocessor=data_preprocessor,
     backbone=dict(
-        type='mmcls.ConvNeXt',
+        type='mmpretrain.ConvNeXt',
         arch='base',
         out_indices=[0, 1, 2, 3],
         drop_path_rate=0.4,
         layer_scale_init_value=1.0,
         gap_before_final_norm=False,
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file,
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 _base_ = [
     '../_base_/models/upernet_convnext.py',
     '../_base_/datasets/ade20k_640x640.py', '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_160k.py'
 ]
 crop_size = (640, 640)
 data_preprocessor = dict(size=crop_size)
-checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-large_3rdparty_in21k_20220301-e6e0ea0a.pth'  # noqa
+checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-xlarge_3rdparty_in21k_20220301-08aa5ddc.pth'  # noqa
 model = dict(
     data_preprocessor=data_preprocessor,
     backbone=dict(
-        type='mmcls.ConvNeXt',
-        arch='large',
+        type='mmpretrain.ConvNeXt',
+        arch='xlarge',
         out_indices=[0, 1, 2, 3],
         drop_path_rate=0.4,
         layer_scale_init_value=1.0,
         gap_before_final_norm=False,
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file,
             prefix='backbone.')),
     decode_head=dict(
-        in_channels=[192, 384, 768, 1536],
+        in_channels=[256, 512, 1024, 2048],
         num_classes=150,
     ),
-    auxiliary_head=dict(in_channels=768, num_classes=150),
+    auxiliary_head=dict(in_channels=1024, num_classes=150),
     test_cfg=dict(mode='slide', crop_size=crop_size, stride=(426, 426)),
 )
 
 optim_wrapper = dict(
     _delete_=True,
     type='AmpOptimWrapper',
     optimizer=dict(
-        type='AdamW', lr=0.0001, betas=(0.9, 0.999), weight_decay=0.05),
+        type='AdamW', lr=0.00008, betas=(0.9, 0.999), weight_decay=0.05),
     paramwise_cfg={
         'decay_rate': 0.9,
         'decay_type': 'stage_wise',
         'num_layers': 12
     },
     constructor='LearningRateDecayOptimizerConstructor',
     loss_scale='dynamic')
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 _base_ = [
     '../_base_/models/upernet_convnext.py', '../_base_/datasets/ade20k.py',
     '../_base_/default_runtime.py', '../_base_/schedules/schedule_160k.py'
 ]
 crop_size = (512, 512)
 data_preprocessor = dict(size=crop_size)
-checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-small_3rdparty_32xb128-noema_in1k_20220301-303e75e3.pth'  # noqa
+checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-tiny_3rdparty_32xb128-noema_in1k_20220301-795e9634.pth'  # noqa
 model = dict(
     data_preprocessor=data_preprocessor,
     backbone=dict(
-        type='mmcls.ConvNeXt',
-        arch='small',
+        type='mmpretrain.ConvNeXt',
+        arch='tiny',
         out_indices=[0, 1, 2, 3],
-        drop_path_rate=0.3,
+        drop_path_rate=0.4,
         layer_scale_init_value=1.0,
         gap_before_final_norm=False,
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file,
             prefix='backbone.')),
     decode_head=dict(
         in_channels=[96, 192, 384, 768],
@@ -29,15 +29,15 @@
     _delete_=True,
     type='AmpOptimWrapper',
     optimizer=dict(
         type='AdamW', lr=0.0001, betas=(0.9, 0.999), weight_decay=0.05),
     paramwise_cfg={
         'decay_rate': 0.9,
         'decay_type': 'stage_wise',
-        'num_layers': 12
+        'num_layers': 6
     },
     constructor='LearningRateDecayOptimizerConstructor',
     loss_scale='dynamic')
 
 param_scheduler = [
     dict(
         type='LinearLR', start_factor=1e-6, by_epoch=False, begin=0, end=1500),
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 _base_ = [
     '../_base_/models/upernet_convnext.py', '../_base_/datasets/ade20k.py',
     '../_base_/default_runtime.py', '../_base_/schedules/schedule_160k.py'
 ]
 crop_size = (512, 512)
 data_preprocessor = dict(size=crop_size)
-checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-tiny_3rdparty_32xb128-noema_in1k_20220301-795e9634.pth'  # noqa
+checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-small_3rdparty_32xb128-noema_in1k_20220301-303e75e3.pth'  # noqa
 model = dict(
     data_preprocessor=data_preprocessor,
     backbone=dict(
-        type='mmcls.ConvNeXt',
-        arch='tiny',
+        type='mmpretrain.ConvNeXt',
+        arch='small',
         out_indices=[0, 1, 2, 3],
-        drop_path_rate=0.4,
+        drop_path_rate=0.3,
         layer_scale_init_value=1.0,
         gap_before_final_norm=False,
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file,
             prefix='backbone.')),
     decode_head=dict(
         in_channels=[96, 192, 384, 768],
@@ -29,15 +29,15 @@
     _delete_=True,
     type='AmpOptimWrapper',
     optimizer=dict(
         type='AdamW', lr=0.0001, betas=(0.9, 0.999), weight_decay=0.05),
     paramwise_cfg={
         'decay_rate': 0.9,
         'decay_type': 'stage_wise',
-        'num_layers': 6
+        'num_layers': 12
     },
     constructor='LearningRateDecayOptimizerConstructor',
     loss_scale='dynamic')
 
 param_scheduler = [
     dict(
         type='LinearLR', start_factor=1e-6, by_epoch=False, begin=0, end=1500),
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 _base_ = [
     '../_base_/models/upernet_convnext.py',
     '../_base_/datasets/ade20k_640x640.py', '../_base_/default_runtime.py',
     '../_base_/schedules/schedule_160k.py'
 ]
 crop_size = (640, 640)
 data_preprocessor = dict(size=crop_size)
-checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-xlarge_3rdparty_in21k_20220301-08aa5ddc.pth'  # noqa
+checkpoint_file = 'https://download.openmmlab.com/mmclassification/v0/convnext/downstream/convnext-large_3rdparty_in21k_20220301-e6e0ea0a.pth'  # noqa
 model = dict(
     data_preprocessor=data_preprocessor,
     backbone=dict(
-        type='mmcls.ConvNeXt',
-        arch='xlarge',
+        type='mmpretrain.ConvNeXt',
+        arch='large',
         out_indices=[0, 1, 2, 3],
         drop_path_rate=0.4,
         layer_scale_init_value=1.0,
         gap_before_final_norm=False,
         init_cfg=dict(
             type='Pretrained', checkpoint=checkpoint_file,
             prefix='backbone.')),
     decode_head=dict(
-        in_channels=[256, 512, 1024, 2048],
+        in_channels=[192, 384, 768, 1536],
         num_classes=150,
     ),
-    auxiliary_head=dict(in_channels=1024, num_classes=150),
+    auxiliary_head=dict(in_channels=768, num_classes=150),
     test_cfg=dict(mode='slide', crop_size=crop_size, stride=(426, 426)),
 )
 
 optim_wrapper = dict(
     _delete_=True,
     type='AmpOptimWrapper',
     optimizer=dict(
-        type='AdamW', lr=0.00008, betas=(0.9, 0.999), weight_decay=0.05),
+        type='AdamW', lr=0.0001, betas=(0.9, 0.999), weight_decay=0.05),
     paramwise_cfg={
         'decay_rate': 0.9,
         'decay_type': 'stage_wise',
         'num_layers': 12
     },
     constructor='LearningRateDecayOptimizerConstructor',
     loss_scale='dynamic')
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dmnet/dmnet.yml` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/metafile.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,232 +1,186 @@
-Collections:
-- Name: DMNet
-  Metadata:
-    Training Data:
-    - Cityscapes
-    - ADE20K
-  Paper:
-    URL: https://openaccess.thecvf.com/content_ICCV_2019/papers/He_Dynamic_Multi-Scale_Filters_for_Semantic_Segmentation_ICCV_2019_paper.pdf
-    Title: Dynamic Multi-scale Filters for Semantic Segmentation
-  README: configs/dmnet/README.md
-  Code:
-    URL: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/dm_head.py#L93
-    Version: v0.17.0
-  Converted From:
-    Code: https://github.com/Junjun2016/DMNet
 Models:
-- Name: dmnet_r50-d8_4xb2-40k_cityscapes-512x1024
-  In Collection: DMNet
-  Metadata:
-    backbone: R-50-D8
-    crop size: (512,1024)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 273.22
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 7.0
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 77.78
-      mIoU(ms+flip): 79.14
-  Config: configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r50-d8_512x1024_40k_cityscapes/dmnet_r50-d8_512x1024_40k_cityscapes_20201215_042326-615373cf.pth
-- Name: dmnet_r101-d8_4xb2-40k_cityscapes-512x1024
-  In Collection: DMNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,1024)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 393.7
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 10.6
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 78.37
-      mIoU(ms+flip): 79.72
-  Config: configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r101-d8_512x1024_40k_cityscapes/dmnet_r101-d8_512x1024_40k_cityscapes_20201215_043100-8291e976.pth
-- Name: dmnet_r50-d8_4xb2-40k_cityscapes-769x769
-  In Collection: DMNet
-  Metadata:
-    backbone: R-50-D8
-    crop size: (769,769)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 636.94
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (769,769)
-    Training Memory (GB): 7.9
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 78.49
-      mIoU(ms+flip): 80.27
-  Config: configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-769x769.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r50-d8_769x769_40k_cityscapes/dmnet_r50-d8_769x769_40k_cityscapes_20201215_093706-e7f0e23e.pth
-- Name: dmnet_r101-d8_4xb2-40k_cityscapes-769x769
-  In Collection: DMNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (769,769)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 990.1
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (769,769)
-    Training Memory (GB): 12.0
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 77.62
-      mIoU(ms+flip): 78.94
-  Config: configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-769x769.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r101-d8_769x769_40k_cityscapes/dmnet_r101-d8_769x769_40k_cityscapes_20201215_081348-a74261f6.pth
-- Name: dmnet_r50-d8_4xb2-80k_cityscapes-512x1024
-  In Collection: DMNet
-  Metadata:
-    backbone: R-50-D8
-    crop size: (512,1024)
-    lr schd: 80000
+- Name: mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024
+  In Collection: FCN
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
-      mIoU: 79.07
-      mIoU(ms+flip): 80.22
-  Config: configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r50-d8_512x1024_80k_cityscapes/dmnet_r50-d8_512x1024_80k_cityscapes_20201215_053728-3c8893b9.pth
-- Name: dmnet_r101-d8_4xb2-80k_cityscapes-512x1024
-  In Collection: DMNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,1024)
-    lr schd: 80000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 79.64
-      mIoU(ms+flip): 80.67
-  Config: configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r101-d8_512x1024_80k_cityscapes/dmnet_r101-d8_512x1024_80k_cityscapes_20201215_031718-fa081cb8.pth
-- Name: dmnet_r50-d8_4xb2-80k_cityscapes-769x769
-  In Collection: DMNet
-  Metadata:
-    backbone: R-50-D8
-    crop size: (769,769)
-    lr schd: 80000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 79.22
-      mIoU(ms+flip): 80.55
-  Config: configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-769x769.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r50-d8_769x769_80k_cityscapes/dmnet_r50-d8_769x769_80k_cityscapes_20201215_034006-6060840e.pth
-- Name: dmnet_r101-d8_4xb2-80k_cityscapes-769x769
-  In Collection: DMNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (769,769)
-    lr schd: 80000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 79.19
-      mIoU(ms+flip): 80.65
-  Config: configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-769x769.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r101-d8_769x769_80k_cityscapes/dmnet_r101-d8_769x769_80k_cityscapes_20201215_082810-7f0de59a.pth
-- Name: dmnet_r50-d8_4xb4-80k_ade20k-512x512
-  In Collection: DMNet
-  Metadata:
-    backbone: R-50-D8
-    crop size: (512,512)
-    lr schd: 80000
-    inference time (ms/im):
-    - value: 47.73
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 9.4
+      mIoU: 71.19
+      mIoU(ms+flip): 73.34
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - M-V2-D8
+    - FCN
+    Training Resources: 4x A100 GPUS
+    Memory (GB): 3.4
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024-20230224_185436-13fef4ea.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024_20230224_185436.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024
+  In Collection: PSPNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 70.23
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - M-V2-D8
+    - PSPNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 3.6
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/pspnet_m-v2-d8_512x1024_80k_cityscapes/pspnet_m-v2-d8_512x1024_80k_cityscapes_20200825_124817-19e81d51.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/pspnet_m-v2-d8_512x1024_80k_cityscapes/pspnet_m-v2-d8_512x1024_80k_cityscapes-20200825_124817.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024
+  In Collection: DeepLabV3
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 73.84
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - M-V2-D8
+    - DeepLabV3
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 3.9
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3_m-v2-d8_512x1024_80k_cityscapes/deeplabv3_m-v2-d8_512x1024_80k_cityscapes_20200825_124836-bef03590.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3_m-v2-d8_512x1024_80k_cityscapes/deeplabv3_m-v2-d8_512x1024_80k_cityscapes-20200825_124836.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024
+  In Collection: DeepLabV3+
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 75.2
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - M-V2-D8
+    - DeepLabV3+
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 5.1
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3plus_m-v2-d8_512x1024_80k_cityscapes/deeplabv3plus_m-v2-d8_512x1024_80k_cityscapes_20200825_124836-d256dd4b.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3plus_m-v2-d8_512x1024_80k_cityscapes/deeplabv3plus_m-v2-d8_512x1024_80k_cityscapes-20200825_124836.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512
+  In Collection: FCN
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 42.37
-      mIoU(ms+flip): 43.62
-  Config: configs/dmnet/dmnet_r50-d8_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r50-d8_512x512_80k_ade20k/dmnet_r50-d8_512x512_80k_ade20k_20201215_144744-f89092a6.pth
-- Name: dmnet_r101-d8_4xb4-80k_ade20k-512x512
-  In Collection: DMNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,512)
-    lr schd: 80000
-    inference time (ms/im):
-    - value: 72.05
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 13.0
+      mIoU: 19.71
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - M-V2-D8
+    - FCN
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 6.5
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/fcn_m-v2-d8_512x512_160k_ade20k/fcn_m-v2-d8_512x512_160k_ade20k_20200825_214953-c40e1095.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/fcn_m-v2-d8_512x512_160k_ade20k/fcn_m-v2-d8_512x512_160k_ade20k-20200825_214953.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512
+  In Collection: PSPNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 45.34
-      mIoU(ms+flip): 46.13
-  Config: configs/dmnet/dmnet_r101-d8_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r101-d8_512x512_80k_ade20k/dmnet_r101-d8_512x512_80k_ade20k_20201215_104812-bfa45311.pth
-- Name: dmnet_r50-d8_4xb4-160k_ade20k-512x512
-  In Collection: DMNet
-  Metadata:
-    backbone: R-50-D8
-    crop size: (512,512)
-    lr schd: 160000
+      mIoU: 29.68
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - M-V2-D8
+    - PSPNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 6.5
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/pspnet_m-v2-d8_512x512_160k_ade20k/pspnet_m-v2-d8_512x512_160k_ade20k_20200825_214953-f5942f7a.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/pspnet_m-v2-d8_512x512_160k_ade20k/pspnet_m-v2-d8_512x512_160k_ade20k-20200825_214953.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512
+  In Collection: DeepLabV3
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 43.15
-      mIoU(ms+flip): 44.17
-  Config: configs/dmnet/dmnet_r50-d8_4xb4-160k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r50-d8_512x512_160k_ade20k/dmnet_r50-d8_512x512_160k_ade20k_20201215_115313-025ab3f9.pth
-- Name: dmnet_r101-d8_4xb4-160k_ade20k-512x512
-  In Collection: DMNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,512)
-    lr schd: 160000
+      mIoU: 34.08
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - M-V2-D8
+    - DeepLabV3
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 6.8
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3_m-v2-d8_512x512_160k_ade20k/deeplabv3_m-v2-d8_512x512_160k_ade20k_20200825_223255-63986343.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3_m-v2-d8_512x512_160k_ade20k/deeplabv3_m-v2-d8_512x512_160k_ade20k-20200825_223255.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
+- Name: mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512
+  In Collection: DeepLabV3+
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 45.42
-      mIoU(ms+flip): 46.76
-  Config: configs/dmnet/dmnet_r101-d8_4xb4-160k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/dmnet/dmnet_r101-d8_512x512_160k_ade20k/dmnet_r101-d8_512x512_160k_ade20k_20201215_111145-a0bc02ef.pth
+      mIoU: 34.02
+  Config: configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - M-V2-D8
+    - DeepLabV3+
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 8.2
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3plus_m-v2-d8_512x512_160k_ade20k/deeplabv3plus_m-v2-d8_512x512_160k_ade20k_20200825_223255-465a01d4.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v2/deeplabv3plus_m-v2-d8_512x512_160k_ade20k/deeplabv3plus_m-v2-d8_512x512_160k_ade20k-20200825_223255.log.json
+  Paper:
+    Title: 'MobileNetV2: Inverted Residuals and Linear Bottlenecks'
+    URL: https://arxiv.org/abs/1801.04381
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v2.py#L14
+  Framework: PyTorch
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/erfnet/erfnet.yml` & `mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/metafile.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Collections:
 - Name: ERFNet
+  License: Apache License 2.0
   Metadata:
     Training Data:
     - Cityscapes
   Paper:
-    URL: http://www.robesafe.uah.es/personal/eduardo.romera/pdfs/Romera17tits.pdf
     Title: 'ERFNet: Efficient Residual Factorized ConvNet for Real-time Semantic Segmentation'
+    URL: http://www.robesafe.uah.es/personal/eduardo.romera/pdfs/Romera17tits.pdf
   README: configs/erfnet/README.md
-  Code:
-    URL: https://github.com/open-mmlab/mmsegmentation/blob/v0.20.0/mmseg/models/backbones/erfnet.py#L321
-    Version: v0.20.0
-  Converted From:
-    Code: https://github.com/Eromera/erfnet_pytorch
+  Frameworks:
+  - PyTorch
 Models:
 - Name: erfnet_fcn_4xb4-160k_cityscapes-512x1024
   In Collection: ERFNet
-  Metadata:
-    backbone: ERFNet
-    crop size: (512,1024)
-    lr schd: 160000
-    inference time (ms/im):
-    - value: 65.53
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 6.04
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 72.5
       mIoU(ms+flip): 74.75
   Config: configs/erfnet/erfnet_fcn_4xb4-160k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 16
+    Architecture:
+    - ERFNet
+    - ERFNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 6.04
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/erfnet/erfnet_fcn_4x4_512x1024_160k_cityscapes/erfnet_fcn_4x4_512x1024_160k_cityscapes_20220704_162145-dc90157a.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/erfnet/erfnet_fcn_4x4_512x1024_160k_cityscapes/erfnet_fcn_4x4_512x1024_160k_cityscapes_20220704_162145.log.json
+  Paper:
+    Title: 'ERFNet: Efficient Residual Factorized ConvNet for Real-time Semantic Segmentation'
+    URL: http://www.robesafe.uah.es/personal/eduardo.romera/pdfs/Romera17tits.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.20.0/mmseg/models/backbones/erfnet.py#L321
+  Framework: PyTorch
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/mobilenet_v3/mobilenet_v3.yml` & `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/metafile.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,109 @@
 Collections:
 - Name: LRASPP
+  License: Apache License 2.0
   Metadata:
     Training Data:
     - Cityscapes
   Paper:
-    URL: https://arxiv.org/abs/1905.02244
     Title: Searching for MobileNetV3
+    URL: https://arxiv.org/abs/1905.02244
   README: configs/mobilenet_v3/README.md
-  Code:
-    URL: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v3.py#L15
-    Version: v0.17.0
-  Converted From:
-    Code: https://github.com/tensorflow/models/tree/master/research/deeplab
+  Frameworks:
+  - PyTorch
 Models:
 - Name: mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024
   In Collection: LRASPP
-  Metadata:
-    backbone: M-V3-D8
-    crop size: (512,1024)
-    lr schd: 320000
-    inference time (ms/im):
-    - value: 65.7
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 8.9
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 69.54
       mIoU(ms+flip): 70.89
   Config: configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 16
+    Architecture:
+    - M-V3-D8
+    - LRASPP
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 8.9
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3-d8_512x1024_320k_cityscapes/lraspp_m-v3-d8_512x1024_320k_cityscapes_20201224_220337-cfe8fb07.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3-d8_512x1024_320k_cityscapes/lraspp_m-v3-d8_512x1024_320k_cityscapes-20201224_220337.log.json
+  Paper:
+    Title: Searching for MobileNetV3
+    URL: https://arxiv.org/abs/1905.02244
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v3.py#L15
+  Framework: PyTorch
 - Name: mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024
   In Collection: LRASPP
-  Metadata:
-    backbone: M-V3-D8 (scratch)
-    crop size: (512,1024)
-    lr schd: 320000
-    inference time (ms/im):
-    - value: 67.7
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 8.9
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 67.87
       mIoU(ms+flip): 69.78
   Config: configs/mobilenet_v3/mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 16
+    Architecture:
+    - M-V3-D8
+    - LRASPP
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 8.9
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3-d8_scratch_512x1024_320k_cityscapes/lraspp_m-v3-d8_scratch_512x1024_320k_cityscapes_20201224_220337-9f29cd72.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3-d8_scratch_512x1024_320k_cityscapes/lraspp_m-v3-d8_scratch_512x1024_320k_cityscapes-20201224_220337.log.json
+  Paper:
+    Title: Searching for MobileNetV3
+    URL: https://arxiv.org/abs/1905.02244
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v3.py#L15
+  Framework: PyTorch
 - Name: mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024
   In Collection: LRASPP
-  Metadata:
-    backbone: M-V3s-D8
-    crop size: (512,1024)
-    lr schd: 320000
-    inference time (ms/im):
-    - value: 42.3
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 5.3
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 64.11
       mIoU(ms+flip): 66.42
   Config: configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 16
+    Architecture:
+    - M-V3s-D8
+    - LRASPP
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 5.3
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3s-d8_512x1024_320k_cityscapes/lraspp_m-v3s-d8_512x1024_320k_cityscapes_20201224_223935-61565b34.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3s-d8_512x1024_320k_cityscapes/lraspp_m-v3s-d8_512x1024_320k_cityscapes-20201224_223935.log.json
+  Paper:
+    Title: Searching for MobileNetV3
+    URL: https://arxiv.org/abs/1905.02244
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v3.py#L15
+  Framework: PyTorch
 - Name: mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024
   In Collection: LRASPP
-  Metadata:
-    backbone: M-V3s-D8 (scratch)
-    crop size: (512,1024)
-    lr schd: 320000
-    inference time (ms/im):
-    - value: 40.82
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 5.3
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
       mIoU: 62.74
       mIoU(ms+flip): 65.01
   Config: configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 16
+    Architecture:
+    - M-V3s-D8
+    - LRASPP
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 5.3
   Weights: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3s-d8_scratch_512x1024_320k_cityscapes/lraspp_m-v3s-d8_scratch_512x1024_320k_cityscapes_20201224_223935-03daeabb.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/mobilenet_v3/lraspp_m-v3s-d8_scratch_512x1024_320k_cityscapes/lraspp_m-v3s-d8_scratch_512x1024_320k_cityscapes-20201224_223935.log.json
+  Paper:
+    Title: Searching for MobileNetV3
+    URL: https://arxiv.org/abs/1905.02244
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/backbones/mobilenet_v3.py#L15
+  Framework: PyTorch
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet.yml` & `mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/metafile.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,438 +1,391 @@
 Collections:
-- Name: OCRNet
+- Name: UPerNet
+  License: Apache License 2.0
   Metadata:
     Training Data:
     - Cityscapes
     - ADE20K
     - Pascal VOC 2012 + Aug
   Paper:
-    URL: https://arxiv.org/abs/1909.11065
-    Title: Object-Contextual Representations for Semantic Segmentation
-  README: configs/ocrnet/README.md
-  Code:
-    URL: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/ocr_head.py#L86
-    Version: v0.17.0
-  Converted From:
-    Code: https://github.com/openseg-group/OCNet.pytorch
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  README: configs/upernet/README.md
+  Frameworks:
+  - PyTorch
 Models:
-- Name: ocrnet_hr18s_4xb2-40k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,1024)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 95.69
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 3.5
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 76.61
-      mIoU(ms+flip): 78.01
-  Config: configs/ocrnet/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024_20230227_145026-6c052a14.pth
-- Name: ocrnet_hr18_4xb2-40k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,1024)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 133.33
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 4.7
+- Name: upernet_r50_4xb2-40k_cityscapes-512x1024
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
-      mIoU: 77.72
-      mIoU(ms+flip): 79.49
-  Config: configs/ocrnet/ocrnet_hr18_4xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x1024_40k_cityscapes/ocrnet_hr18_512x1024_40k_cityscapes_20200601_033320-401c5bdd.pth
-- Name: ocrnet_hr48_4xb2-40k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,1024)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 236.97
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 8.0
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 80.58
-      mIoU(ms+flip): 81.79
-  Config: configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x1024_40k_cityscapes/ocrnet_hr48_512x1024_40k_cityscapes_20200601_033336-55b32491.pth
-- Name: ocrnet_hr18s_4xb2-80k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,1024)
-    lr schd: 80000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 77.16
-      mIoU(ms+flip): 78.66
-  Config: configs/ocrnet/ocrnet_hr18s_4xb2-80k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_512x1024_80k_cityscapes/ocrnet_hr18s_512x1024_80k_cityscapes_20200601_222735-55979e63.pth
-- Name: ocrnet_hr18_4xb2-80k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,1024)
-    lr schd: 80000
+      mIoU: 77.1
+      mIoU(ms+flip): 78.37
+  Config: configs/upernet/upernet_r50_4xb2-40k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 6.4
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_40k_cityscapes/upernet_r50_512x1024_40k_cityscapes_20200605_094827-aa54cb54.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_40k_cityscapes/upernet_r50_512x1024_40k_cityscapes_20200605_094827.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb2-40k_cityscapes-512x1024
+  In Collection: UPerNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 78.69
+      mIoU(ms+flip): 80.11
+  Config: configs/upernet/upernet_r101_4xb2-40k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 7.4
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_40k_cityscapes/upernet_r101_512x1024_40k_cityscapes_20200605_094933-ebce3b10.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_40k_cityscapes/upernet_r101_512x1024_40k_cityscapes_20200605_094933.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb2-40k_cityscapes-769x769
+  In Collection: UPerNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 77.98
+      mIoU(ms+flip): 79.7
+  Config: configs/upernet/upernet_r50_4xb2-40k_cityscapes-769x769.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 7.2
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_40k_cityscapes/upernet_r50_769x769_40k_cityscapes_20200530_033048-92d21539.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_40k_cityscapes/upernet_r50_769x769_40k_cityscapes_20200530_033048.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb2-40k_cityscapes-769x769
+  In Collection: UPerNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 79.03
+      mIoU(ms+flip): 80.77
+  Config: configs/upernet/upernet_r101_4xb2-40k_cityscapes-769x769.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 8.4
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_40k_cityscapes/upernet_r101_769x769_40k_cityscapes_20200530_040819-83c95d01.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_40k_cityscapes/upernet_r101_769x769_40k_cityscapes_20200530_040819.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb2-80k_cityscapes-512x1024
+  In Collection: UPerNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 78.19
+      mIoU(ms+flip): 79.19
+  Config: configs/upernet/upernet_r50_4xb2-80k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_80k_cityscapes/upernet_r50_512x1024_80k_cityscapes_20200607_052207-848beca8.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x1024_80k_cityscapes/upernet_r50_512x1024_80k_cityscapes_20200607_052207.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb2-80k_cityscapes-512x1024
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Cityscapes
     Metrics:
-      mIoU: 78.57
+      mIoU: 79.4
       mIoU(ms+flip): 80.46
-  Config: configs/ocrnet/ocrnet_hr18_4xb2-80k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x1024_80k_cityscapes/ocrnet_hr18_512x1024_80k_cityscapes_20200614_230521-c2e1dd4a.pth
-- Name: ocrnet_hr48_4xb2-80k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,1024)
-    lr schd: 80000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 80.7
-      mIoU(ms+flip): 81.87
-  Config: configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x1024_80k_cityscapes/ocrnet_hr48_512x1024_80k_cityscapes_20200601_222752-9076bcdf.pth
-- Name: ocrnet_hr18s_4xb2-160k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,1024)
-    lr schd: 160000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 78.45
-      mIoU(ms+flip): 79.97
-  Config: configs/ocrnet/ocrnet_hr18s_4xb2-160k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_512x1024_160k_cityscapes/ocrnet_hr18s_512x1024_160k_cityscapes_20200602_191005-f4a7af28.pth
-- Name: ocrnet_hr18_4xb2-160k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,1024)
-    lr schd: 160000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 79.47
-      mIoU(ms+flip): 80.91
-  Config: configs/ocrnet/ocrnet_hr18_4xb2-160k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x1024_160k_cityscapes/ocrnet_hr18_512x1024_160k_cityscapes_20200602_191001-b9172d0c.pth
-- Name: ocrnet_hr48_4xb2-160k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,1024)
-    lr schd: 160000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 81.35
-      mIoU(ms+flip): 82.7
-  Config: configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x1024_160k_cityscapes/ocrnet_hr48_512x1024_160k_cityscapes_20200602_191037-dfbf1b0c.pth
-- Name: ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,1024)
-    lr schd: 40000
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 80.09
-  Config: configs/ocrnet/ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_r101-d8_512x1024_40k_b8_cityscapes/ocrnet_r101-d8_512x1024_40k_b8_cityscapes_20200717_110721-02ac0f13.pth
-- Name: ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,1024)
-    lr schd: 40000
-    inference time (ms/im):
-    - value: 331.13
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 8.8
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 80.3
-  Config: configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_r101-d8_512x1024_40k_b16_cityscapes/ocrnet_r101-d8_512x1024_40k_b16_cityscapes_20200723_193726-db500f80.pth
-- Name: ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024
-  In Collection: OCRNet
-  Metadata:
-    backbone: R-101-D8
-    crop size: (512,1024)
-    lr schd: 80000
-    inference time (ms/im):
-    - value: 331.13
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,1024)
-    Training Memory (GB): 8.8
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Cityscapes
-    Metrics:
-      mIoU: 80.81
-  Config: configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_r101-d8_512x1024_80k_b16_cityscapes/ocrnet_r101-d8_512x1024_80k_b16_cityscapes_20200723_192421-78688424.pth
-- Name: ocrnet_hr18s_4xb4-80k_ade20k-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,512)
-    lr schd: 80000
-    inference time (ms/im):
-    - value: 34.51
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 6.7
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: ADE20K
-    Metrics:
-      mIoU: 35.06
-      mIoU(ms+flip): 35.8
-  Config: configs/ocrnet/ocrnet_hr18s_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_512x512_80k_ade20k/ocrnet_hr18s_512x512_80k_ade20k_20200615_055600-e80b62af.pth
-- Name: ocrnet_hr18_4xb4-80k_ade20k-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,512)
-    lr schd: 80000
-    inference time (ms/im):
-    - value: 52.83
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 7.9
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: ADE20K
-    Metrics:
-      mIoU: 37.79
-      mIoU(ms+flip): 39.16
-  Config: configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x512_80k_ade20k/ocrnet_hr18_512x512_80k_ade20k_20200615_053157-d173d83b.pth
-- Name: ocrnet_hr48_4xb4-80k_ade20k-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,512)
-    lr schd: 80000
-    inference time (ms/im):
-    - value: 58.86
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 11.2
+  Config: configs/upernet/upernet_r101_4xb2-80k_cityscapes-512x1024.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_80k_cityscapes/upernet_r101_512x1024_80k_cityscapes_20200607_002403-f05f2345.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x1024_80k_cityscapes/upernet_r101_512x1024_80k_cityscapes_20200607_002403.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb2-80k_cityscapes-769x769
+  In Collection: UPerNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 79.39
+      mIoU(ms+flip): 80.92
+  Config: configs/upernet/upernet_r50_4xb2-80k_cityscapes-769x769.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_80k_cityscapes/upernet_r50_769x769_80k_cityscapes_20200607_005107-82ae7d15.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_769x769_80k_cityscapes/upernet_r50_769x769_80k_cityscapes_20200607_005107.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb2-80k_cityscapes-769x769
+  In Collection: UPerNet
+  Results:
+    Task: Semantic Segmentation
+    Dataset: Cityscapes
+    Metrics:
+      mIoU: 80.1
+      mIoU(ms+flip): 81.49
+  Config: configs/upernet/upernet_r101_4xb2-80k_cityscapes-769x769.py
+  Metadata:
+    Training Data: Cityscapes
+    Batch Size: 8
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_80k_cityscapes/upernet_r101_769x769_80k_cityscapes_20200607_001014-082fc334.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_769x769_80k_cityscapes/upernet_r101_769x769_80k_cityscapes_20200607_001014.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb4-80k_ade20k-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 43.0
-      mIoU(ms+flip): 44.3
-  Config: configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x512_80k_ade20k/ocrnet_hr48_512x512_80k_ade20k_20200615_021518-d168c2d1.pth
-- Name: ocrnet_hr18s_4xb4-80k_ade20k-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,512)
-    lr schd: 160000
+      mIoU: 40.7
+      mIoU(ms+flip): 41.81
+  Config: configs/upernet/upernet_r50_4xb4-80k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 8.1
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_80k_ade20k/upernet_r50_512x512_80k_ade20k_20200614_144127-ecc8377b.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_80k_ade20k/upernet_r50_512x512_80k_ade20k_20200614_144127.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb4-80k_ade20k-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 37.19
-      mIoU(ms+flip): 38.4
-  Config: configs/ocrnet/ocrnet_hr18s_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_512x512_160k_ade20k/ocrnet_hr18s_512x512_160k_ade20k_20200615_184505-8e913058.pth
-- Name: ocrnet_hr18_4xb4-80k_ade20k-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,512)
-    lr schd: 160000
+      mIoU: 42.91
+      mIoU(ms+flip): 43.96
+  Config: configs/upernet/upernet_r101_4xb4-80k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 9.1
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_80k_ade20k/upernet_r101_512x512_80k_ade20k_20200614_185117-32e4db94.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_80k_ade20k/upernet_r101_512x512_80k_ade20k_20200614_185117.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb4-160k_ade20k-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 39.32
-      mIoU(ms+flip): 40.8
-  Config: configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x512_160k_ade20k/ocrnet_hr18_512x512_160k_ade20k_20200615_200940-d8fcd9d1.pth
-- Name: ocrnet_hr48_4xb4-160k_ade20k-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,512)
-    lr schd: 160000
+      mIoU: 42.05
+      mIoU(ms+flip): 42.78
+  Config: configs/upernet/upernet_r50_4xb4-160k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_160k_ade20k/upernet_r50_512x512_160k_ade20k_20200615_184328-8534de8d.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_160k_ade20k/upernet_r50_512x512_160k_ade20k_20200615_184328.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb4-160k_ade20k-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: ADE20K
     Metrics:
-      mIoU: 43.25
-      mIoU(ms+flip): 44.88
-  Config: configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x512_160k_ade20k/ocrnet_hr48_512x512_160k_ade20k_20200615_184705-a073726d.pth
-- Name: ocrnet_hr18s_4xb4-20k_voc12aug-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,512)
-    lr schd: 20000
-    inference time (ms/im):
-    - value: 31.7
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 3.5
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Pascal VOC 2012 + Aug
-    Metrics:
-      mIoU: 71.7
-      mIoU(ms+flip): 73.84
-  Config: configs/ocrnet/ocrnet_hr18s_4xb4-20k_voc12aug-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_512x512_20k_voc12aug/ocrnet_hr18s_512x512_20k_voc12aug_20200617_233913-02b04fcb.pth
-- Name: ocrnet_hr18_4xb4-20k_voc12aug-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,512)
-    lr schd: 20000
-    inference time (ms/im):
-    - value: 50.23
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 4.7
-  Results:
-  - Task: Semantic Segmentation
-    Dataset: Pascal VOC 2012 + Aug
-    Metrics:
-      mIoU: 74.75
-      mIoU(ms+flip): 77.11
-  Config: configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x512_20k_voc12aug/ocrnet_hr18_512x512_20k_voc12aug_20200617_233932-8954cbb7.pth
-- Name: ocrnet_hr48_4xb4-20k_voc12aug-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,512)
-    lr schd: 20000
-    inference time (ms/im):
-    - value: 56.09
-      hardware: V100
-      backend: PyTorch
-      batch size: 1
-      mode: FP32
-      resolution: (512,512)
-    Training Memory (GB): 8.1
+      mIoU: 43.82
+      mIoU(ms+flip): 44.85
+  Config: configs/upernet/upernet_r101_4xb4-160k_ade20k-512x512.py
+  Metadata:
+    Training Data: ADE20K
+    Batch Size: 16
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_160k_ade20k/upernet_r101_512x512_160k_ade20k_20200615_161951-91b32684.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_160k_ade20k/upernet_r101_512x512_160k_ade20k_20200615_161951.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb4-20k_voc12aug-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Pascal VOC 2012 + Aug
     Metrics:
-      mIoU: 77.72
-      mIoU(ms+flip): 79.87
-  Config: configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x512_20k_voc12aug/ocrnet_hr48_512x512_20k_voc12aug_20200617_233932-9e82080a.pth
-- Name: ocrnet_hr18s_4xb4-40k_voc12aug-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18-Small
-    crop size: (512,512)
-    lr schd: 40000
+      mIoU: 74.82
+      mIoU(ms+flip): 76.35
+  Config: configs/upernet/upernet_r50_4xb4-20k_voc12aug-512x512.py
+  Metadata:
+    Training Data: Pascal VOC 2012 + Aug
+    Batch Size: 16
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 6.4
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_20k_voc12aug/upernet_r50_512x512_20k_voc12aug_20200617_165330-5b5890a7.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_20k_voc12aug/upernet_r50_512x512_20k_voc12aug_20200617_165330.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb4-20k_voc12aug-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Pascal VOC 2012 + Aug
     Metrics:
-      mIoU: 72.76
-      mIoU(ms+flip): 74.6
-  Config: configs/ocrnet/ocrnet_hr18s_4xb4-40k_voc12aug-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18s_512x512_40k_voc12aug/ocrnet_hr18s_512x512_40k_voc12aug_20200614_002025-42b587ac.pth
-- Name: ocrnet_hr18_4xb4-40k_voc12aug-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W18
-    crop size: (512,512)
-    lr schd: 40000
+      mIoU: 77.1
+      mIoU(ms+flip): 78.29
+  Config: configs/upernet/upernet_r101_4xb4-20k_voc12aug-512x512.py
+  Metadata:
+    Training Data: Pascal VOC 2012 + Aug
+    Batch Size: 16
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+    Memory (GB): 7.5
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_20k_voc12aug/upernet_r101_512x512_20k_voc12aug_20200617_165629-f14e7f27.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_20k_voc12aug/upernet_r101_512x512_20k_voc12aug_20200617_165629.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r50_4xb4-40k_voc12aug-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Pascal VOC 2012 + Aug
     Metrics:
-      mIoU: 74.98
-      mIoU(ms+flip): 77.4
-  Config: configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr18_512x512_40k_voc12aug/ocrnet_hr18_512x512_40k_voc12aug_20200614_015958-714302be.pth
-- Name: ocrnet_hr48_4xb4-40k_voc12aug-512x512
-  In Collection: OCRNet
-  Metadata:
-    backbone: HRNetV2p-W48
-    crop size: (512,512)
-    lr schd: 40000
+      mIoU: 75.92
+      mIoU(ms+flip): 77.44
+  Config: configs/upernet/upernet_r50_4xb4-40k_voc12aug-512x512.py
+  Metadata:
+    Training Data: Pascal VOC 2012 + Aug
+    Batch Size: 16
+    Architecture:
+    - R-50
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_40k_voc12aug/upernet_r50_512x512_40k_voc12aug_20200613_162257-ca9bcc6b.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r50_512x512_40k_voc12aug/upernet_r50_512x512_40k_voc12aug_20200613_162257.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
+- Name: upernet_r101_4xb4-40k_voc12aug-512x512
+  In Collection: UPerNet
   Results:
-  - Task: Semantic Segmentation
+    Task: Semantic Segmentation
     Dataset: Pascal VOC 2012 + Aug
     Metrics:
-      mIoU: 77.14
-      mIoU(ms+flip): 79.71
-  Config: configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py
-  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/ocrnet/ocrnet_hr48_512x512_40k_voc12aug/ocrnet_hr48_512x512_40k_voc12aug_20200614_015958-255bc5ce.pth
+      mIoU: 77.43
+      mIoU(ms+flip): 78.56
+  Config: configs/upernet/upernet_r101_4xb4-40k_voc12aug-512x512.py
+  Metadata:
+    Training Data: Pascal VOC 2012 + Aug
+    Batch Size: 16
+    Architecture:
+    - R-101
+    - UPerNet
+    Training Resources: 4x V100 GPUS
+  Weights: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_40k_voc12aug/upernet_r101_512x512_40k_voc12aug_20200613_163549-e26476ac.pth
+  Training log: https://download.openmmlab.com/mmsegmentation/v0.5/upernet/upernet_r101_512x512_40k_voc12aug/upernet_r101_512x512_40k_voc12aug_20200613_163549.log.json
+  Paper:
+    Title: Unified Perceptual Parsing for Scene Understanding
+    URL: https://arxiv.org/pdf/1807.10221.pdf
+  Code: https://github.com/open-mmlab/mmsegmentation/blob/v0.17.0/mmseg/models/decode_heads/uper_head.py#L13
+  Framework: PyTorch
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 _base_ = [
-    '../_base_/models/segformer_mit-b0.py',
-    '../_base_/datasets/cityscapes_1024x1024.py',
+    '../_base_/models/segformer_mit-b0.py', '../_base_/datasets/ade20k.py',
     '../_base_/default_runtime.py', '../_base_/schedules/schedule_160k.py'
 ]
-crop_size = (1024, 1024)
+crop_size = (512, 512)
 data_preprocessor = dict(size=crop_size)
+checkpoint = 'https://download.openmmlab.com/mmsegmentation/v0.5/pretrain/segformer/mit_b0_20220624-7e0fe6dd.pth'  # noqa
 model = dict(
     data_preprocessor=data_preprocessor,
-    backbone=dict(
-        init_cfg=dict(type='Pretrained', checkpoint='pretrain/mit_b0.pth')),
-    test_cfg=dict(mode='slide', crop_size=(1024, 1024), stride=(768, 768)))
+    backbone=dict(init_cfg=dict(type='Pretrained', checkpoint=checkpoint)),
+    decode_head=dict(num_classes=150))
 
 optim_wrapper = dict(
     _delete_=True,
     type='OptimWrapper',
     optimizer=dict(
         type='AdamW', lr=0.00006, betas=(0.9, 0.999), weight_decay=0.01),
     paramwise_cfg=dict(
@@ -31,11 +30,10 @@
         eta_min=0.0,
         power=1.0,
         begin=1500,
         end=160000,
         by_epoch=False,
     )
 ]
-
-train_dataloader = dict(batch_size=1, num_workers=4)
+train_dataloader = dict(batch_size=2, num_workers=2)
 val_dataloader = dict(batch_size=1, num_workers=4)
 test_dataloader = val_dataloader
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 _base_ = [
-    '../_base_/models/segformer_mit-b0.py', '../_base_/datasets/ade20k.py',
-    '../_base_/default_runtime.py', '../_base_/schedules/schedule_160k.py'
+    '../_base_/models/upernet_vit-b16_ln_mln.py',
+    '../_base_/datasets/ade20k.py', '../_base_/default_runtime.py',
+    '../_base_/schedules/schedule_160k.py'
 ]
 crop_size = (512, 512)
 data_preprocessor = dict(size=crop_size)
 model = dict(
     data_preprocessor=data_preprocessor,
-    pretrained='pretrain/mit_b0.pth',
-    decode_head=dict(num_classes=150))
+    pretrained='pretrain/vit_base_patch16_224.pth',
+    backbone=dict(drop_path_rate=0.1, final_norm=True),
+    decode_head=dict(num_classes=150),
+    auxiliary_head=dict(num_classes=150))
 
+# AdamW optimizer, no weight decay for position embedding & layer norm
+# in backbone
 optim_wrapper = dict(
     _delete_=True,
     type='OptimWrapper',
     optimizer=dict(
         type='AdamW', lr=0.00006, betas=(0.9, 0.999), weight_decay=0.01),
     paramwise_cfg=dict(
         custom_keys={
-            'pos_block': dict(decay_mult=0.),
-            'norm': dict(decay_mult=0.),
-            'head': dict(lr_mult=10.)
+            'pos_embed': dict(decay_mult=0.),
+            'cls_token': dict(decay_mult=0.),
+            'norm': dict(decay_mult=0.)
         }))
 
 param_scheduler = [
     dict(
         type='LinearLR', start_factor=1e-6, by_epoch=False, begin=0, end=1500),
     dict(
         type='PolyLR',
         eta_min=0.0,
         power=1.0,
         begin=1500,
         end=160000,
         by_epoch=False,
     )
 ]
-train_dataloader = dict(batch_size=2, num_workers=2)
-val_dataloader = dict(batch_size=1, num_workers=4)
+
+# By default, models are trained on 8 GPUs with 2 images per GPU
+train_dataloader = dict(batch_size=2)
+val_dataloader = dict(batch_size=1)
 test_dataloader = val_dataloader
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 _base_ = ['./segformer_mit-b0_8xb2-160k_ade20k-512x512.py']
 
+checkpoint = 'https://download.openmmlab.com/mmsegmentation/v0.5/pretrain/segformer/mit_b5_20220624-658746d9.pth'  # noqa
+
 # dataset settings
 crop_size = (640, 640)
 data_preprocessor = dict(size=crop_size)
 train_pipeline = [
     dict(type='LoadImageFromFile'),
     dict(type='LoadAnnotations', reduce_zero_label=True),
     dict(
@@ -27,11 +29,13 @@
 train_dataloader = dict(dataset=dict(pipeline=train_pipeline))
 val_dataloader = dict(batch_size=1, dataset=dict(pipeline=test_pipeline))
 test_dataloader = val_dataloader
 
 # model settings
 model = dict(
     data_preprocessor=data_preprocessor,
-    pretrained='pretrain/mit_b5.pth',
     backbone=dict(
-        embed_dims=64, num_heads=[1, 2, 5, 8], num_layers=[3, 6, 40, 3]),
+        init_cfg=dict(type='Pretrained', checkpoint=checkpoint),
+        embed_dims=64,
+        num_heads=[1, 2, 5, 8],
+        num_layers=[3, 6, 40, 3]),
     decode_head=dict(in_channels=[64, 128, 320, 512]))
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 _base_ = [
     '../_base_/models/upernet_vit-b16_ln_mln.py',
     '../_base_/datasets/ade20k.py', '../_base_/default_runtime.py',
-    '../_base_/schedules/schedule_160k.py'
+    '../_base_/schedules/schedule_80k.py'
 ]
 crop_size = (512, 512)
 data_preprocessor = dict(size=crop_size)
 model = dict(
     data_preprocessor=data_preprocessor,
     pretrained='pretrain/vit_base_patch16_224.pth',
-    backbone=dict(drop_path_rate=0.1, final_norm=True),
     decode_head=dict(num_classes=150),
     auxiliary_head=dict(num_classes=150))
 
 # AdamW optimizer, no weight decay for position embedding & layer norm
 # in backbone
 optim_wrapper = dict(
     _delete_=True,
@@ -30,15 +29,15 @@
     dict(
         type='LinearLR', start_factor=1e-6, by_epoch=False, begin=0, end=1500),
     dict(
         type='PolyLR',
         eta_min=0.0,
         power=1.0,
         begin=1500,
-        end=160000,
+        end=80000,
         by_epoch=False,
     )
 ]
 
 # By default, models are trained on 8 GPUs with 2 images per GPU
 train_dataloader = dict(batch_size=2)
 val_dataloader = dict(batch_size=1)
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py` & `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 _base_ = [
-    '../_base_/models/upernet_vit-b16_ln_mln.py',
-    '../_base_/datasets/ade20k.py', '../_base_/default_runtime.py',
-    '../_base_/schedules/schedule_80k.py'
+    '../_base_/models/upernet_swin.py', '../_base_/datasets/levir_256x256.py',
+    '../_base_/default_runtime.py', '../_base_/schedules/schedule_20k.py'
 ]
-crop_size = (512, 512)
-data_preprocessor = dict(size=crop_size)
+crop_size = (256, 256)
+norm_cfg = dict(type='BN', requires_grad=True)
+data_preprocessor = dict(
+    size=crop_size,
+    type='SegDataPreProcessor',
+    mean=[123.675, 116.28, 103.53, 123.675, 116.28, 103.53],
+    std=[58.395, 57.12, 57.375, 58.395, 57.12, 57.375])
+
 model = dict(
     data_preprocessor=data_preprocessor,
-    pretrained='pretrain/vit_base_patch16_224.pth',
-    decode_head=dict(num_classes=150),
-    auxiliary_head=dict(num_classes=150))
+    backbone=dict(
+        in_channels=6,
+        embed_dims=96,
+        depths=[2, 2, 6, 2],
+        num_heads=[3, 6, 12, 24],
+        window_size=7,
+        use_abs_pos_embed=False,
+        drop_path_rate=0.3,
+        patch_norm=True),
+    decode_head=dict(in_channels=[96, 192, 384, 768], num_classes=2),
+    auxiliary_head=dict(in_channels=384, num_classes=2))
 
 # AdamW optimizer, no weight decay for position embedding & layer norm
 # in backbone
 optim_wrapper = dict(
     _delete_=True,
     type='OptimWrapper',
     optimizer=dict(
         type='AdamW', lr=0.00006, betas=(0.9, 0.999), weight_decay=0.01),
     paramwise_cfg=dict(
         custom_keys={
-            'pos_embed': dict(decay_mult=0.),
-            'cls_token': dict(decay_mult=0.),
+            'absolute_pos_embed': dict(decay_mult=0.),
+            'relative_position_bias_table': dict(decay_mult=0.),
             'norm': dict(decay_mult=0.)
         }))
 
 param_scheduler = [
     dict(
         type='LinearLR', start_factor=1e-6, by_epoch=False, begin=0, end=1500),
     dict(
         type='PolyLR',
         eta_min=0.0,
         power=1.0,
         begin=1500,
-        end=80000,
+        end=20000,
         by_epoch=False,
     )
 ]
 
-# By default, models are trained on 8 GPUs with 2 images per GPU
-train_dataloader = dict(batch_size=2)
+train_dataloader = dict(batch_size=4)
 val_dataloader = dict(batch_size=1)
 test_dataloader = val_dataloader
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/analyze_logs.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/benchmark.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/browse_dataset.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/analysis_tools/confusion_matrix.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/chase_db1.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/chase_db1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/cityscapes.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/drive.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/drive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/hrf.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/hrf.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/isaid.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/isaid.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             img_patch = img[y_str:y_end, x_str:x_end, :]
             img_patch = Image.fromarray(img_patch.astype(np.uint8))
             image = osp.basename(src_path).split('.')[0] + '_' + str(
                 y_str) + '_' + str(y_end) + '_' + str(x_str) + '_' + str(
                     x_end) + '.png'
             # print(image)
             save_path_image = osp.join(out_dir, 'img_dir', mode, str(image))
-            img_patch.save(save_path_image)
+            img_patch.save(save_path_image, format='BMP')
 
 
 def slide_crop_label(src_path, out_dir, mode, patch_H, patch_W, overlap):
     label = mmcv.imread(src_path, channel_order='rgb')
     label = iSAID_convert_from_color(label)
     img_H, img_W = label.shape
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/loveda.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/loveda.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/pascal_context.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/pascal_context.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/potsdam.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/potsdam.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/refuge.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/refuge.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/stare.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/stare.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/synapse.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/synapse.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/vaihingen.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/vaihingen.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/dataset_converters/voc_aug.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/voc_aug.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/deployment/pytorch2torchscript.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/deployment/pytorch2torchscript.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/browse_dataset.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/misc/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/print_config.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/misc/publish_model.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/misc/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/beit2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/beit2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/mit2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/mit2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/stdc2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/stdc2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/swin2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/swin2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/twins2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/twins2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/vit2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vit2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/model_converters/vitjax2mmseg.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vitjax2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/slurm_test.sh` & `mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/slurm_train.sh` & `mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/test.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     parser.add_argument('config', help='train config file path')
     parser.add_argument('checkpoint', help='checkpoint file')
     parser.add_argument(
         '--work-dir',
         help=('if specified, the evaluation metric results will be dumped'
               'into the directory as json'))
     parser.add_argument(
+        '--out',
+        type=str,
+        help='The directory to save output prediction for offline evaluation')
+    parser.add_argument(
         '--show', action='store_true', help='show prediction results')
     parser.add_argument(
         '--show-dir',
         help='directory where painted images will be saved. '
         'If specified, it will be automatically saved '
         'to the work_dir/timestamp/show_dir')
     parser.add_argument(
@@ -39,15 +43,18 @@
     parser.add_argument(
         '--launcher',
         choices=['none', 'pytorch', 'slurm', 'mpi'],
         default='none',
         help='job launcher')
     parser.add_argument(
         '--tta', action='store_true', help='Test time augmentation')
-    parser.add_argument('--local_rank', type=int, default=0)
+    # When using PyTorch version >= 2.0.0, the `torch.distributed.launch`
+    # will pass the `--local-rank` parameter to `tools/train.py` instead
+    # of `--local_rank`.
+    parser.add_argument('--local_rank', '--local-rank', type=int, default=0)
     args = parser.parse_args()
     if 'LOCAL_RANK' not in os.environ:
         os.environ['LOCAL_RANK'] = str(args.local_rank)
 
     return args
 
 
@@ -57,16 +64,16 @@
         visualization_hook = default_hooks['visualization']
         # Turn on visualization
         visualization_hook['draw'] = True
         if args.show:
             visualization_hook['show'] = True
             visualization_hook['wait_time'] = args.wait_time
         if args.show_dir:
-            visulizer = cfg.visualizer
-            visulizer['save_dir'] = args.show_dir
+            visualizer = cfg.visualizer
+            visualizer['save_dir'] = args.show_dir
     else:
         raise RuntimeError(
             'VisualizationHook must be included in default_hooks.'
             'refer to usage '
             '"visualization=dict(type=\'VisualizationHook\')"')
 
     return cfg
@@ -96,14 +103,19 @@
         cfg = trigger_visualization_hook(cfg, args)
 
     if args.tta:
         cfg.test_dataloader.dataset.pipeline = cfg.tta_pipeline
         cfg.tta_model.module = cfg.model
         cfg.model = cfg.tta_model
 
+    # add output_dir in metric
+    if args.out is not None:
+        cfg.test_evaluator['output_dir'] = args.out
+        cfg.test_evaluator['keep_results'] = True
+
     # build the runner from config
     runner = Runner.from_cfg(cfg)
 
     # start testing
     runner.test()
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/mmseg2torchserve.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg2torchserve.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/mmseg_handler.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg_handler.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/torchserve/test_torchserve.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/test_torchserve.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/.mim/tools/train.py` & `mmsegmentation-1.1.0/mmseg/.mim/tools/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,18 @@
         'Note that the quotation marks are necessary and that no white space '
         'is allowed.')
     parser.add_argument(
         '--launcher',
         choices=['none', 'pytorch', 'slurm', 'mpi'],
         default='none',
         help='job launcher')
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

### Comparing `mmsegmentation-1.0.0rc6/mmseg/__init__.py` & `mmsegmentation-1.1.0/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/apis/inference.py` & `mmsegmentation-1.1.0/mmseg/apis/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
     Returns:
         np.ndarray: the drawn image which channel is RGB.
     """
     if hasattr(model, 'module'):
         model = model.module
     if isinstance(img, str):
-        image = mmcv.imread(img)
+        image = mmcv.imread(img, channel_order='rgb')
     else:
         image = img
     if save_dir is not None:
         mkdir_or_exist(save_dir)
     # init visualizer
     visualizer = SegLocalVisualizer(
         vis_backends=[dict(type='LocalVisBackend')],
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/apis/mmseg_inferencer.py` & `mmsegmentation-1.1.0/mmseg/apis/mmseg_inferencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class MMSegInferencer(BaseInferencer):
     """Semantic segmentation inferencer, provides inference and visualization
     interfaces. Note: MMEngine >= 0.5.0 is required.
 
     Args:
         model (str, optional): Path to the config file or the model name
-            defined in metafile. Take the `mmseg metafile <https://github.com/open-mmlab/mmsegmentation/blob/dev-1.x/configs/fcn/fcn.yml>`_
+            defined in metafile. Take the `mmseg metafile <https://github.com/open-mmlab/mmsegmentation/blob/main/configs/fcn/metafile.yaml>`_
             as an example the `model` could be
             "fcn_r50-d8_4xb2-40k_cityscapes-512x1024", and the weights of model
             will be download automatically. If use config file, like
             "configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-512x1024.py", the
             `weights` should be defined.
         weights (str, optional): Path to the checkpoint. If it is not specified
             and model is a model name of metafile, the weights will be loaded
@@ -44,15 +44,15 @@
             indices, `classes` is a list which includes items responding to the
             label indices. If classes is not defined, visualizer will take
             `cityscapes` classes by default. Defaults to None.
         palette (list, optional): Input palette for result rendering, which is
             a list of color palette responding to the classes. If palette is
             not defined, visualizer will take `cityscapes` palette by default.
             Defaults to None.
-        dataset_name (str, optional): `Dataset name or alias <https://github.com/open-mmlab/mmsegmentation/blob/dev-1.x/mmseg/utils/class_names.py#L302-L317>`_
+        dataset_name (str, optional): `Dataset name or alias <https://github.com/open-mmlab/mmsegmentation/blob/main/mmseg/utils/class_names.py#L302-L317>`_
             visulizer will use the meta information of the dataset i.e. classes
             and palette, but the `classes` and `palette` have higher priority.
             Defaults to None.
         device (str, optional): Device to run inference. If None, the available
             device will be automatically used. Defaults to None.
         scope (str, optional): The scope of the model. Defaults to 'mmseg'.
     """ # noqa
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/__init__.py` & `mmsegmentation-1.1.0/mmseg/datasets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 # yapf: disable
 from .ade import ADE20KDataset
-from .basesegdataset import BaseSegDataset
+from .basesegdataset import BaseCDDataset, BaseSegDataset
 from .chase_db1 import ChaseDB1Dataset
 from .cityscapes import CityscapesDataset
 from .coco_stuff import COCOStuffDataset
 from .dark_zurich import DarkZurichDataset
 from .dataset_wrappers import MultiImageMixDataset
 from .decathlon import DecathlonDataset
 from .drive import DRIVEDataset
+from .dsdl import DSDLSegDataset
 from .hrf import HRFDataset
 from .isaid import iSAIDDataset
 from .isprs import ISPRSDataset
+from .levir import LEVIRCDDataset
 from .lip import LIPDataset
 from .loveda import LoveDADataset
+from .mapillary import MapillaryDataset_v1, MapillaryDataset_v2
 from .night_driving import NightDrivingDataset
 from .pascal_context import PascalContextDataset, PascalContextDataset59
 from .potsdam import PotsdamDataset
 from .refuge import REFUGEDataset
 from .stare import STAREDataset
 from .synapse import SynapseDataset
 # yapf: disable
-from .transforms import (CLAHE, AdjustGamma, BioMedical3DPad,
+from .transforms import (CLAHE, AdjustGamma, Albu, BioMedical3DPad,
                          BioMedical3DRandomCrop, BioMedical3DRandomFlip,
                          BioMedicalGaussianBlur, BioMedicalGaussianNoise,
-                         BioMedicalRandomGamma, GenerateEdge, LoadAnnotations,
-                         LoadBiomedicalAnnotation, LoadBiomedicalData,
-                         LoadBiomedicalImageFromFile, LoadImageFromNDArray,
-                         PackSegInputs, PhotoMetricDistortion, RandomCrop,
-                         RandomCutOut, RandomMosaic, RandomRotate,
-                         RandomRotFlip, Rerange, ResizeShortestEdge,
-                         ResizeToMultiple, RGB2Gray, SegRescale)
+                         BioMedicalRandomGamma, ConcatCDInput, GenerateEdge,
+                         LoadAnnotations, LoadBiomedicalAnnotation,
+                         LoadBiomedicalData, LoadBiomedicalImageFromFile,
+                         LoadImageFromNDArray, LoadMultipleRSImageFromFile,
+                         LoadSingleRSImageFromFile, PackSegInputs,
+                         PhotoMetricDistortion, RandomCrop, RandomCutOut,
+                         RandomMosaic, RandomRotate, RandomRotFlip, Rerange,
+                         ResizeShortestEdge, ResizeToMultiple, RGB2Gray,
+                         SegRescale)
 from .voc import PascalVOCDataset
 
 # yapf: enable
 __all__ = [
     'BaseSegDataset', 'BioMedical3DRandomCrop', 'BioMedical3DRandomFlip',
     'CityscapesDataset', 'PascalVOCDataset', 'ADE20KDataset',
     'PascalContextDataset', 'PascalContextDataset59', 'ChaseDB1Dataset',
@@ -45,9 +50,12 @@
     'RandomRotate', 'AdjustGamma', 'CLAHE', 'Rerange', 'RGB2Gray',
     'RandomCutOut', 'RandomMosaic', 'PackSegInputs', 'ResizeToMultiple',
     'LoadImageFromNDArray', 'LoadBiomedicalImageFromFile',
     'LoadBiomedicalAnnotation', 'LoadBiomedicalData', 'GenerateEdge',
     'DecathlonDataset', 'LIPDataset', 'ResizeShortestEdge',
     'BioMedicalGaussianNoise', 'BioMedicalGaussianBlur',
     'BioMedicalRandomGamma', 'BioMedical3DPad', 'RandomRotFlip',
-    'SynapseDataset', 'REFUGEDataset'
+    'SynapseDataset', 'REFUGEDataset', 'MapillaryDataset_v1',
+    'MapillaryDataset_v2', 'Albu', 'LEVIRCDDataset',
+    'LoadMultipleRSImageFromFile', 'LoadSingleRSImageFromFile',
+    'ConcatCDInput', 'BaseCDDataset', 'DSDLSegDataset'
 ]
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/ade.py` & `mmsegmentation-1.1.0/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/chase_db1.py` & `mmsegmentation-1.1.0/mmseg/datasets/stare.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import mmengine.fileio as fileio
 
 from mmseg.registry import DATASETS
 from .basesegdataset import BaseSegDataset
 
 
 @DATASETS.register_module()
-class ChaseDB1Dataset(BaseSegDataset):
-    """Chase_db1 dataset.
+class STAREDataset(BaseSegDataset):
+    """STARE dataset.
 
-    In segmentation map annotation for Chase_db1, 0 stands for background,
-    which is included in 2 categories. ``reduce_zero_label`` is fixed to False.
-    The ``img_suffix`` is fixed to '.png' and ``seg_map_suffix`` is fixed to
-    '_1stHO.png'.
+    In segmentation map annotation for STARE, 0 stands for background, which is
+    included in 2 categories. ``reduce_zero_label`` is fixed to False. The
+    ``img_suffix`` is fixed to '.png' and ``seg_map_suffix`` is fixed to
+    '.ah.png'.
     """
     METAINFO = dict(
         classes=('background', 'vessel'),
         palette=[[120, 120, 120], [6, 230, 230]])
 
     def __init__(self,
                  img_suffix='.png',
-                 seg_map_suffix='_1stHO.png',
+                 seg_map_suffix='.ah.png',
                  reduce_zero_label=False,
                  **kwargs) -> None:
         super().__init__(
             img_suffix=img_suffix,
             seg_map_suffix=seg_map_suffix,
             reduce_zero_label=reduce_zero_label,
             **kwargs)
-        assert self.file_client.exists(self.data_prefix['img_path'])
+        assert fileio.exists(
+            self.data_prefix['img_path'], backend_args=self.backend_args)
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/cityscapes.py` & `mmsegmentation-1.1.0/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/coco_stuff.py` & `mmsegmentation-1.1.0/mmseg/datasets/coco_stuff.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/dataset_wrappers.py` & `mmsegmentation-1.1.0/mmseg/datasets/dataset_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,19 +102,19 @@
         for (transform, transform_type) in zip(self.pipeline,
                                                self.pipeline_types):
             if self._skip_type_keys is not None and \
                     transform_type in self._skip_type_keys:
                 continue
 
             if hasattr(transform, 'get_indices'):
-                indexes = transform.get_indices(self.dataset)
-                if not isinstance(indexes, collections.abc.Sequence):
-                    indexes = [indexes]
+                indices = transform.get_indices(self.dataset)
+                if not isinstance(indices, collections.abc.Sequence):
+                    indices = [indices]
                 mix_results = [
-                    copy.deepcopy(self.dataset[index]) for index in indexes
+                    copy.deepcopy(self.dataset[index]) for index in indices
                 ]
                 results['mix_results'] = mix_results
 
             results = transform(results)
 
             if 'mix_results' in results:
                 results.pop('mix_results')
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/decathlon.py` & `mmsegmentation-1.1.0/mmseg/datasets/decathlon.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/drive.py` & `mmsegmentation-1.1.0/mmseg/datasets/chase_db1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import mmengine.fileio as fileio
 
 from mmseg.registry import DATASETS
 from .basesegdataset import BaseSegDataset
 
 
 @DATASETS.register_module()
-class DRIVEDataset(BaseSegDataset):
-    """DRIVE dataset.
+class ChaseDB1Dataset(BaseSegDataset):
+    """Chase_db1 dataset.
 
-    In segmentation map annotation for DRIVE, 0 stands for background, which is
-    included in 2 categories. ``reduce_zero_label`` is fixed to False. The
-    ``img_suffix`` is fixed to '.png' and ``seg_map_suffix`` is fixed to
-    '_manual1.png'.
+    In segmentation map annotation for Chase_db1, 0 stands for background,
+    which is included in 2 categories. ``reduce_zero_label`` is fixed to False.
+    The ``img_suffix`` is fixed to '.png' and ``seg_map_suffix`` is fixed to
+    '_1stHO.png'.
     """
     METAINFO = dict(
         classes=('background', 'vessel'),
         palette=[[120, 120, 120], [6, 230, 230]])
 
     def __init__(self,
                  img_suffix='.png',
-                 seg_map_suffix='_manual1.png',
+                 seg_map_suffix='_1stHO.png',
                  reduce_zero_label=False,
                  **kwargs) -> None:
         super().__init__(
             img_suffix=img_suffix,
             seg_map_suffix=seg_map_suffix,
             reduce_zero_label=reduce_zero_label,
             **kwargs)
-        assert self.file_client.exists(self.data_prefix['img_path'])
+        assert fileio.exists(
+            self.data_prefix['img_path'], backend_args=self.backend_args)
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/hrf.py` & `mmsegmentation-1.1.0/mmseg/datasets/drive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import mmengine.fileio as fileio
 
 from mmseg.registry import DATASETS
 from .basesegdataset import BaseSegDataset
 
 
 @DATASETS.register_module()
-class HRFDataset(BaseSegDataset):
-    """HRF dataset.
+class DRIVEDataset(BaseSegDataset):
+    """DRIVE dataset.
 
-    In segmentation map annotation for HRF, 0 stands for background, which is
+    In segmentation map annotation for DRIVE, 0 stands for background, which is
     included in 2 categories. ``reduce_zero_label`` is fixed to False. The
     ``img_suffix`` is fixed to '.png' and ``seg_map_suffix`` is fixed to
-    '.png'.
+    '_manual1.png'.
     """
     METAINFO = dict(
         classes=('background', 'vessel'),
         palette=[[120, 120, 120], [6, 230, 230]])
 
     def __init__(self,
                  img_suffix='.png',
-                 seg_map_suffix='.png',
+                 seg_map_suffix='_manual1.png',
                  reduce_zero_label=False,
                  **kwargs) -> None:
         super().__init__(
             img_suffix=img_suffix,
             seg_map_suffix=seg_map_suffix,
             reduce_zero_label=reduce_zero_label,
             **kwargs)
-        assert self.file_client.exists(self.data_prefix['img_path'])
+        assert fileio.exists(
+            self.data_prefix['img_path'], backend_args=self.backend_args)
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/isaid.py` & `mmsegmentation-1.1.0/mmseg/datasets/isaid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/isprs.py` & `mmsegmentation-1.1.0/mmseg/datasets/isprs.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/lip.py` & `mmsegmentation-1.1.0/mmseg/datasets/lip.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/loveda.py` & `mmsegmentation-1.1.0/mmseg/datasets/loveda.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/night_driving.py` & `mmsegmentation-1.1.0/mmseg/datasets/night_driving.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/pascal_context.py` & `mmsegmentation-1.1.0/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/potsdam.py` & `mmsegmentation-1.1.0/mmseg/datasets/potsdam.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/refuge.py` & `mmsegmentation-1.1.0/mmseg/datasets/refuge.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/synapse.py` & `mmsegmentation-1.1.0/mmseg/datasets/synapse.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/__init__.py` & `mmsegmentation-1.1.0/mmseg/datasets/transforms/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .formatting import PackSegInputs
 from .loading import (LoadAnnotations, LoadBiomedicalAnnotation,
                       LoadBiomedicalData, LoadBiomedicalImageFromFile,
-                      LoadImageFromNDArray)
+                      LoadImageFromNDArray, LoadMultipleRSImageFromFile,
+                      LoadSingleRSImageFromFile)
 # yapf: disable
-from .transforms import (CLAHE, AdjustGamma, BioMedical3DPad,
+from .transforms import (CLAHE, AdjustGamma, Albu, BioMedical3DPad,
                          BioMedical3DRandomCrop, BioMedical3DRandomFlip,
                          BioMedicalGaussianBlur, BioMedicalGaussianNoise,
-                         BioMedicalRandomGamma, GenerateEdge,
+                         BioMedicalRandomGamma, ConcatCDInput, GenerateEdge,
                          PhotoMetricDistortion, RandomCrop, RandomCutOut,
                          RandomMosaic, RandomRotate, RandomRotFlip, Rerange,
                          ResizeShortestEdge, ResizeToMultiple, RGB2Gray,
                          SegRescale)
 
 # yapf: enable
 __all__ = [
     'LoadAnnotations', 'RandomCrop', 'BioMedical3DRandomCrop', 'SegRescale',
     'PhotoMetricDistortion', 'RandomRotate', 'AdjustGamma', 'CLAHE', 'Rerange',
     'RGB2Gray', 'RandomCutOut', 'RandomMosaic', 'PackSegInputs',
     'ResizeToMultiple', 'LoadImageFromNDArray', 'LoadBiomedicalImageFromFile',
     'LoadBiomedicalAnnotation', 'LoadBiomedicalData', 'GenerateEdge',
     'ResizeShortestEdge', 'BioMedicalGaussianNoise', 'BioMedicalGaussianBlur',
     'BioMedical3DRandomFlip', 'BioMedicalRandomGamma', 'BioMedical3DPad',
-    'RandomRotFlip'
+    'RandomRotFlip', 'Albu', 'LoadSingleRSImageFromFile', 'ConcatCDInput',
+    'LoadMultipleRSImageFromFile'
 ]
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/formatting.py` & `mmsegmentation-1.1.0/mmseg/datasets/transforms/formatting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import warnings
+
 import numpy as np
 from mmcv.transforms import to_tensor
 from mmcv.transforms.base import BaseTransform
 from mmengine.structures import PixelData
 
 from mmseg.registry import TRANSFORMS
 from mmseg.structures import SegDataSample
@@ -38,15 +40,15 @@
             'img_shape', 'pad_shape', 'scale_factor', 'flip',
             'flip_direction')``
     """
 
     def __init__(self,
                  meta_keys=('img_path', 'seg_map_path', 'ori_shape',
                             'img_shape', 'pad_shape', 'scale_factor', 'flip',
-                            'flip_direction')):
+                            'flip_direction', 'reduce_zero_label')):
         self.meta_keys = meta_keys
 
     def transform(self, results: dict) -> dict:
         """Method to pack the input data.
 
         Args:
             results (dict): Result dict from the data pipeline.
@@ -68,17 +70,24 @@
             else:
                 img = img.transpose(2, 0, 1)
                 img = to_tensor(img).contiguous()
             packed_results['inputs'] = img
 
         data_sample = SegDataSample()
         if 'gt_seg_map' in results:
-            gt_sem_seg_data = dict(
-                data=to_tensor(results['gt_seg_map'][None,
-                                                     ...].astype(np.int64)))
+            if len(results['gt_seg_map'].shape) == 2:
+                data = to_tensor(results['gt_seg_map'][None,
+                                                       ...].astype(np.int64))
+            else:
+                warnings.warn('Please pay attention your ground truth '
+                              'segmentation map, usually the segmentation '
+                              'map is 2D, but got '
+                              f'{results["gt_seg_map"].shape}')
+                data = to_tensor(results['gt_seg_map'].astype(np.int64))
+            gt_sem_seg_data = dict(data=data)
             data_sample.gt_sem_seg = PixelData(**gt_sem_seg_data)
 
         if 'gt_edge_map' in results:
             gt_edge_data = dict(
                 data=to_tensor(results['gt_edge_map'][None,
                                                       ...].astype(np.int64)))
             data_sample.set_data(dict(gt_edge_map=PixelData(**gt_edge_data)))
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/loading.py` & `mmsegmentation-1.1.0/mmseg/datasets/transforms/loading.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from mmcv.transforms import BaseTransform
 from mmcv.transforms import LoadAnnotations as MMCV_LoadAnnotations
 from mmcv.transforms import LoadImageFromFile
 
 from mmseg.registry import TRANSFORMS
 from mmseg.utils import datafrombytes
 
+try:
+    from osgeo import gdal
+except ImportError:
+    gdal = None
+
 
 @TRANSFORMS.register_module()
 class LoadAnnotations(MMCV_LoadAnnotations):
     """Load annotations for semantic segmentation provided by dataset.
 
     The annotation format is as the following:
 
@@ -489,7 +494,134 @@
             inputs = single_input
         else:
             raise NotImplementedError
 
         if 'img' in inputs:
             return self.from_ndarray(inputs)
         return self.from_file(inputs)
+
+
+@TRANSFORMS.register_module()
+class LoadSingleRSImageFromFile(BaseTransform):
+    """Load a Remote Sensing mage from file.
+
+    Required Keys:
+
+    - img_path
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - ori_shape
+
+    Args:
+        to_float32 (bool): Whether to convert the loaded image to a float32
+            numpy array. If set to False, the loaded image is a float64 array.
+            Defaults to True.
+    """
+
+    def __init__(self, to_float32: bool = True):
+        self.to_float32 = to_float32
+
+        if gdal is None:
+            raise RuntimeError('gdal is not installed')
+
+    def transform(self, results: Dict) -> Dict:
+        """Functions to load image.
+
+        Args:
+            results (dict): Result dict from :obj:``mmcv.BaseDataset``.
+
+        Returns:
+            dict: The dict contains loaded image and meta information.
+        """
+
+        filename = results['img_path']
+        ds = gdal.Open(filename)
+        if ds is None:
+            raise Exception(f'Unable to open file: {filename}')
+        img = np.einsum('ijk->jki', ds.ReadAsArray())
+
+        if self.to_float32:
+            img = img.astype(np.float32)
+
+        results['img'] = img
+        results['img_shape'] = img.shape[:2]
+        results['ori_shape'] = img.shape[:2]
+        return results
+
+    def __repr__(self):
+        repr_str = (f'{self.__class__.__name__}('
+                    f'to_float32={self.to_float32})')
+        return repr_str
+
+
+@TRANSFORMS.register_module()
+class LoadMultipleRSImageFromFile(BaseTransform):
+    """Load two Remote Sensing mage from file.
+
+    Required Keys:
+
+    - img_path
+    - img_path2
+
+    Modified Keys:
+
+    - img
+    - img2
+    - img_shape
+    - ori_shape
+
+    Args:
+        to_float32 (bool): Whether to convert the loaded image to a float32
+            numpy array. If set to False, the loaded image is a float64 array.
+            Defaults to True.
+    """
+
+    def __init__(self, to_float32: bool = True):
+        if gdal is None:
+            raise RuntimeError('gdal is not installed')
+        self.to_float32 = to_float32
+
+    def transform(self, results: Dict) -> Dict:
+        """Functions to load image.
+
+        Args:
+            results (dict): Result dict from :obj:``mmcv.BaseDataset``.
+
+        Returns:
+            dict: The dict contains loaded image and meta information.
+        """
+
+        filename = results['img_path']
+        filename2 = results['img_path2']
+
+        ds = gdal.Open(filename)
+        ds2 = gdal.Open(filename2)
+
+        if ds is None:
+            raise Exception(f'Unable to open file: {filename}')
+        if ds2 is None:
+            raise Exception(f'Unable to open file: {filename2}')
+
+        img = np.einsum('ijk->jki', ds.ReadAsArray())
+        img2 = np.einsum('ijk->jki', ds2.ReadAsArray())
+
+        if self.to_float32:
+            img = img.astype(np.float32)
+            img2 = img2.astype(np.float32)
+
+        if img.shape != img2.shape:
+            raise Exception(f'Image shapes do not match:'
+                            f' {img.shape} vs {img2.shape}')
+
+        results['img'] = img
+        results['img2'] = img2
+        results['img_shape'] = img.shape[:2]
+        results['ori_shape'] = img.shape[:2]
+        return results
+
+    def __repr__(self):
+        repr_str = (f'{self.__class__.__name__}('
+                    f'to_float32={self.to_float32})')
+        return repr_str
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/transforms/transforms.py` & `mmsegmentation-1.1.0/mmseg/datasets/transforms/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
+import inspect
 import warnings
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import cv2
 import mmcv
+import mmengine
 import numpy as np
 from mmcv.transforms.base import BaseTransform
 from mmcv.transforms.utils import cache_randomness
 from mmengine.utils import is_tuple_of
 from numpy import random
 from scipy.ndimage import gaussian_filter
 
 from mmseg.datasets.dataset_wrappers import MultiImageMixDataset
 from mmseg.registry import TRANSFORMS
 
+try:
+    import albumentations
+    from albumentations import Compose
+    ALBU_INSTALLED = True
+except ImportError:
+    albumentations = None
+    Compose = None
+    ALBU_INSTALLED = False
+
 
 @TRANSFORMS.register_module()
 class ResizeToMultiple(BaseTransform):
     """Resize images & seg to multiple of divisor.
 
     Required Keys:
 
@@ -182,15 +193,15 @@
                 np.array(results['img'][:, :, i], dtype=np.uint8),
                 self.clip_limit, self.tile_grid_size)
 
         return results
 
     def __repr__(self):
         repr_str = self.__class__.__name__
-        repr_str += f'(clip_limit={self.clip_limit}, '\
+        repr_str += f'(clip_limit={self.clip_limit}, ' \
                     f'tile_grid_size={self.tile_grid_size})'
         return repr_str
 
 
 @TRANSFORMS.register_module()
 class RandomCrop(BaseTransform):
     """Random crop the image & seg.
@@ -1025,25 +1036,25 @@
         mosaic = self.do_mosaic()
         if mosaic:
             results = self._mosaic_transform_img(results)
             results = self._mosaic_transform_seg(results)
         return results
 
     def get_indices(self, dataset: MultiImageMixDataset) -> list:
-        """Call function to collect indexes.
+        """Call function to collect indices.
 
         Args:
             dataset (:obj:`MultiImageMixDataset`): The dataset.
 
         Returns:
-            list: indexes.
+            list: indices.
         """
 
-        indexes = [random.randint(0, len(dataset)) for _ in range(3)]
-        return indexes
+        indices = [random.randint(0, len(dataset)) for _ in range(3)]
+        return indices
 
     @cache_randomness
     def generate_mosaic_center(self):
         # mosaic center x, y
         center_x = int(
             random.uniform(*self.center_ratio_range) * self.img_scale[1])
         center_y = int(
@@ -1058,16 +1069,17 @@
 
         Returns:
             dict: Updated result dict.
         """
 
         assert 'mix_results' in results
         if len(results['img'].shape) == 3:
+            c = results['img'].shape[2]
             mosaic_img = np.full(
-                (int(self.img_scale[0] * 2), int(self.img_scale[1] * 2), 3),
+                (int(self.img_scale[0] * 2), int(self.img_scale[1] * 2), c),
                 self.pad_val,
                 dtype=results['img'].dtype)
         else:
             mosaic_img = np.full(
                 (int(self.img_scale[0] * 2), int(self.img_scale[1] * 2)),
                 self.pad_val,
                 dtype=results['img'].dtype)
@@ -1146,16 +1158,16 @@
                 # compute the combine parameters
                 paste_coord, crop_coord = self._mosaic_combine(
                     loc, center_position, gt_seg_i.shape[:2][::-1])
                 x1_p, y1_p, x2_p, y2_p = paste_coord
                 x1_c, y1_c, x2_c, y2_c = crop_coord
 
                 # crop and paste image
-                mosaic_seg[y1_p:y2_p, x1_p:x2_p] = gt_seg_i[y1_c:y2_c,
-                                                            x1_c:x2_c]
+                mosaic_seg[y1_p:y2_p, x1_p:x2_p] = \
+                    gt_seg_i[y1_c:y2_c, x1_c:x2_c]
 
             results[key] = mosaic_seg
 
         return results
 
     def _mosaic_combine(self, loc: str, center_position_xy: Sequence[float],
                         img_shape_wh: Sequence[int]) -> tuple:
@@ -1755,17 +1767,17 @@
         return results
 
     def __repr__(self):
         repr_str = self.__class__.__name__
         repr_str += f'(prob={self.prob}, '
         repr_str += f'prob_per_channel={self.prob_per_channel}, '
         repr_str += f'sigma_range={self.sigma_range}, '
-        repr_str += 'different_sigma_per_channel='\
+        repr_str += 'different_sigma_per_channel=' \
                     f'{self.different_sigma_per_channel}, '
-        repr_str += 'different_sigma_per_axis='\
+        repr_str += 'different_sigma_per_axis=' \
                     f'{self.different_sigma_per_axis})'
         return repr_str
 
 
 @TRANSFORMS.register_module()
 class BioMedicalRandomGamma(BaseTransform):
     """Using random gamma correction to process the biomedical image.
@@ -2130,7 +2142,182 @@
         return results
 
     def __repr__(self):
         repr_str = self.__class__.__name__
         repr_str += f'(prob={self.prob}, axes={self.axes}, ' \
                     f'swap_label_pairs={self.swap_label_pairs})'
         return repr_str
+
+
+@TRANSFORMS.register_module()
+class Albu(BaseTransform):
+    """Albumentation augmentation. Adds custom transformations from
+    Albumentations library. Please, visit
+    `https://albumentations.readthedocs.io` to get more information. An example
+    of ``transforms`` is as followed:
+
+    .. code-block::
+        [
+            dict(
+                type='ShiftScaleRotate',
+                shift_limit=0.0625,
+                scale_limit=0.0,
+                rotate_limit=0,
+                interpolation=1,
+                p=0.5),
+            dict(
+                type='RandomBrightnessContrast',
+                brightness_limit=[0.1, 0.3],
+                contrast_limit=[0.1, 0.3],
+                p=0.2),
+            dict(type='ChannelShuffle', p=0.1),
+            dict(
+                type='OneOf',
+                transforms=[
+                    dict(type='Blur', blur_limit=3, p=1.0),
+                    dict(type='MedianBlur', blur_limit=3, p=1.0)
+                ],
+                p=0.1),
+        ]
+    Args:
+        transforms (list[dict]): A list of albu transformations
+        keymap (dict): Contains {'input key':'albumentation-style key'}
+        update_pad_shape (bool): Whether to update padding shape according to \
+            the output shape of the last transform
+    """
+
+    def __init__(self,
+                 transforms: List[dict],
+                 keymap: Optional[dict] = None,
+                 update_pad_shape: bool = False):
+        if not ALBU_INSTALLED:
+            raise ImportError(
+                'albumentations is not installed, '
+                'we suggest install albumentation by '
+                '"pip install albumentations>=0.3.2 --no-binary qudida,albumentations"'  # noqa
+            )
+
+        # Args will be modified later, copying it will be safer
+        transforms = copy.deepcopy(transforms)
+
+        self.transforms = transforms
+        self.keymap = keymap
+        self.update_pad_shape = update_pad_shape
+
+        self.aug = Compose([self.albu_builder(t) for t in self.transforms])
+
+        if not keymap:
+            self.keymap_to_albu = {
+                'img': 'image',
+                'gt_masks': 'masks',
+            }
+        else:
+            self.keymap_to_albu = copy.deepcopy(keymap)
+        self.keymap_back = {v: k for k, v in self.keymap_to_albu.items()}
+
+    def albu_builder(self, cfg: dict) -> object:
+        """Build a callable object from a dict containing albu arguments.
+
+        Args:
+            cfg (dict): Config dict. It should at least contain the key "type".
+
+        Returns:
+            Callable: A callable object.
+        """
+
+        assert isinstance(cfg, dict) and 'type' in cfg
+        args = cfg.copy()
+
+        obj_type = args.pop('type')
+        if mmengine.is_str(obj_type):
+            if not ALBU_INSTALLED:
+                raise ImportError(
+                    'albumentations is not installed, '
+                    'we suggest install albumentation by '
+                    '"pip install albumentations>=0.3.2 --no-binary qudida,albumentations"'  # noqa
+                )
+            obj_cls = getattr(albumentations, obj_type)
+        elif inspect.isclass(obj_type):
+            obj_cls = obj_type
+        else:
+            raise TypeError(
+                f'type must be a valid type or str, but got {type(obj_type)}')
+
+        if 'transforms' in args:
+            args['transforms'] = [
+                self.albu_builder(t) for t in args['transforms']
+            ]
+
+        return obj_cls(**args)
+
+    @staticmethod
+    def mapper(d: dict, keymap: dict):
+        """Dictionary mapper.
+
+        Renames keys according to keymap provided.
+        Args:
+            d (dict): old dict
+            keymap (dict): {'old_key':'new_key'}
+        Returns:
+            dict: new dict.
+        """
+
+        updated_dict = {}
+        for k, _ in zip(d.keys(), d.values()):
+            new_k = keymap.get(k, k)
+            updated_dict[new_k] = d[k]
+        return updated_dict
+
+    def transform(self, results):
+        # dict to albumentations format
+        results = self.mapper(results, self.keymap_to_albu)
+
+        # Convert to RGB since Albumentations works with RGB images
+        results['image'] = cv2.cvtColor(results['image'], cv2.COLOR_BGR2RGB)
+
+        results = self.aug(**results)
+
+        # Convert back to BGR
+        results['image'] = cv2.cvtColor(results['image'], cv2.COLOR_RGB2BGR)
+
+        # back to the original format
+        results = self.mapper(results, self.keymap_back)
+
+        # update final shape
+        if self.update_pad_shape:
+            results['pad_shape'] = results['img'].shape
+
+        return results
+
+    def __repr__(self):
+        repr_str = self.__class__.__name__ + f'(transforms={self.transforms})'
+        return repr_str
+
+
+@TRANSFORMS.register_module()
+class ConcatCDInput(BaseTransform):
+    """Concat images for change detection.
+
+    Required Keys:
+
+    - img
+    - img2
+
+    Args:
+        input_keys (tuple):  Input image keys for change detection.
+            Default: ('img', 'img2').
+    """
+
+    def __init__(self, input_keys=('img', 'img2')):
+        self.input_keys = input_keys
+
+    def transform(self, results: dict) -> dict:
+        img = []
+        for input_key in self.input_keys:
+            img.append(results.pop(input_key))
+        results['img'] = np.concatenate(img, axis=2)
+        return results
+
+    def __repr__(self):
+        repr_str = self.__class__.__name__
+        repr_str += f'(input_keys={self.input_keys}, '
+        return repr_str
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/datasets/voc.py` & `mmsegmentation-1.1.0/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/engine/hooks/visualization_hook.py` & `mmsegmentation-1.1.0/mmseg/engine/hooks/visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py` & `mmsegmentation-1.1.0/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/evaluation/metrics/citys_metric.py` & `mmsegmentation-1.1.0/mmseg/evaluation/metrics/citys_metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import os.path as osp
-from typing import Dict, List, Optional, Sequence
+import shutil
+from collections import OrderedDict
+from typing import Dict, Optional, Sequence
+
+try:
+
+    import cityscapesscripts.evaluation.evalPixelLevelSemanticLabeling as CSEval  # noqa
+    import cityscapesscripts.helpers.labels as CSLabels
+except ImportError:
+    CSLabels = None
+    CSEval = None
 
 import numpy as np
+from mmengine.dist import is_main_process, master_only
 from mmengine.evaluator import BaseMetric
 from mmengine.logging import MMLogger, print_log
-from mmengine.utils import mkdir_or_exist, scandir
+from mmengine.utils import mkdir_or_exist
 from PIL import Image
 
 from mmseg.registry import METRICS
 
 
 @METRICS.register_module()
-class CitysMetric(BaseMetric):
+class CityscapesMetric(BaseMetric):
     """Cityscapes evaluation metric.
 
     Args:
+        output_dir (str): The directory for output prediction
         ignore_index (int): Index that will be ignored in evaluation.
             Default: 255.
-        citys_metrics (list[str] | str): Metrics to be evaluated,
-            Default: ['cityscapes'].
-        to_label_id (bool): whether convert output to label_id for
-            submission. Default: True.
-        suffix (str): The filename prefix of the png files.
-            If the prefix is "somepath/xxx", the png files will be
-            named "somepath/xxx.png". Default: '.format_cityscapes'.
+        format_only (bool): Only format result for results commit without
+            perform evaluation. It is useful when you want to format the result
+            to a specific format and submit it to the test server.
+            Defaults to False.
+        keep_results (bool): Whether to keep the results. When ``format_only``
+            is True, ``keep_results`` must be True. Defaults to False.
         collect_device (str): Device name used for collecting results from
             different ranks during distributed training. Must be 'cpu' or
             'gpu'. Defaults to 'cpu'.
         prefix (str, optional): The prefix that will be added in the metric
             names to disambiguate homonymous metrics of different evaluators.
             If prefix is not provided in the argument, self.default_prefix
             will be used instead. Defaults to None.
     """
 
     def __init__(self,
+                 output_dir: str,
                  ignore_index: int = 255,
-                 citys_metrics: List[str] = ['cityscapes'],
-                 to_label_id: bool = True,
-                 suffix: str = '.format_cityscapes',
+                 format_only: bool = False,
+                 keep_results: bool = False,
                  collect_device: str = 'cpu',
-                 prefix: Optional[str] = None) -> None:
+                 prefix: Optional[str] = None,
+                 **kwargs) -> None:
         super().__init__(collect_device=collect_device, prefix=prefix)
-
+        if CSEval is None:
+            raise ImportError('Please run "pip install cityscapesscripts" to '
+                              'install cityscapesscripts first.')
+        self.output_dir = output_dir
         self.ignore_index = ignore_index
-        self.metrics = citys_metrics
-        assert self.metrics[0] == 'cityscapes'
-        self.to_label_id = to_label_id
-        self.suffix = suffix
+
+        self.format_only = format_only
+        if format_only:
+            assert keep_results, (
+                'When format_only is True, the results must be keep, please '
+                f'set keep_results as True, but got {keep_results}')
+        self.keep_results = keep_results
+        self.prefix = prefix
+        if is_main_process():
+            mkdir_or_exist(self.output_dir)
+
+    @master_only
+    def __del__(self) -> None:
+        """Clean up."""
+        if not self.keep_results:
+            shutil.rmtree(self.output_dir)
 
     def process(self, data_batch: dict, data_samples: Sequence[dict]) -> None:
         """Process one batch of data and data_samples.
 
         The processed results should be stored in ``self.results``, which will
         be used to computed the metrics when all batches have been processed.
 
         Args:
             data_batch (dict): A batch of data from the dataloader.
             data_samples (Sequence[dict]): A batch of outputs from the model.
         """
-        mkdir_or_exist(self.suffix)
+        mkdir_or_exist(self.output_dir)
 
         for data_sample in data_samples:
             pred_label = data_sample['pred_sem_seg']['data'][0].cpu().numpy()
-            # results2img
-            if self.to_label_id:
-                pred_label = self._convert_to_label_id(pred_label)
+            # when evaluating with official cityscapesscripts,
+            # labelIds should be used
+            pred_label = self._convert_to_label_id(pred_label)
             basename = osp.splitext(osp.basename(data_sample['img_path']))[0]
-            png_filename = osp.join(self.suffix, f'{basename}.png')
+            png_filename = osp.abspath(
+                osp.join(self.output_dir, f'{basename}.png'))
             output = Image.fromarray(pred_label.astype(np.uint8)).convert('P')
-            import cityscapesscripts.helpers.labels as CSLabels
-            palette = np.zeros((len(CSLabels.id2label), 3), dtype=np.uint8)
-            for label_id, label in CSLabels.id2label.items():
-                palette[label_id] = label.color
-            output.putpalette(palette)
             output.save(png_filename)
-
-        ann_dir = osp.join(data_samples[0]['seg_map_path'].split('val')[0],
-                           'val')
-        self.results.append(ann_dir)
+            if self.format_only:
+                # format_only always for test dataset without ground truth
+                gt_filename = ''
+            else:
+                # when evaluating with official cityscapesscripts,
+                # **_gtFine_labelIds.png is used
+                gt_filename = data_sample['seg_map_path'].replace(
+                    'labelTrainIds.png', 'labelIds.png')
+            self.results.append((png_filename, gt_filename))
 
     def compute_metrics(self, results: list) -> Dict[str, float]:
         """Compute the metrics from processed results.
 
         Args:
             results (list): Testing results of the dataset.
 
         Returns:
             dict[str: float]: Cityscapes evaluation results.
         """
         logger: MMLogger = MMLogger.get_current_instance()
-        try:
-            import cityscapesscripts.evaluation.evalPixelLevelSemanticLabeling as CSEval  # noqa
-        except ImportError:
-            raise ImportError('Please run "pip install cityscapesscripts" to '
-                              'install cityscapesscripts first.')
-        msg = 'Evaluating in Cityscapes style'
+        if self.format_only:
+            logger.info(f'results are saved to {osp.dirname(self.output_dir)}')
+            return OrderedDict()
 
+        msg = 'Evaluating in Cityscapes style'
         if logger is None:
             msg = '\n' + msg
         print_log(msg, logger=logger)
 
-        result_dir = self.suffix
-
         eval_results = dict()
-        print_log(f'Evaluating results under {result_dir} ...', logger=logger)
+        print_log(
+            f'Evaluating results under {self.output_dir} ...', logger=logger)
 
         CSEval.args.evalInstLevelScore = True
-        CSEval.args.predictionPath = osp.abspath(result_dir)
+        CSEval.args.predictionPath = osp.abspath(self.output_dir)
         CSEval.args.evalPixelAccuracy = True
         CSEval.args.JSONOutput = False
 
-        seg_map_list = []
-        pred_list = []
-        ann_dir = results[0]
-        # when evaluating with official cityscapesscripts,
-        # **_gtFine_labelIds.png is used
-        for seg_map in scandir(ann_dir, 'gtFine_labelIds.png', recursive=True):
-            seg_map_list.append(osp.join(ann_dir, seg_map))
-            pred_list.append(CSEval.getPrediction(CSEval.args, seg_map))
+        pred_list, gt_list = zip(*results)
         metric = dict()
         eval_results.update(
-            CSEval.evaluateImgLists(pred_list, seg_map_list, CSEval.args))
+            CSEval.evaluateImgLists(pred_list, gt_list, CSEval.args))
         metric['averageScoreCategories'] = eval_results[
             'averageScoreCategories']
         metric['averageScoreInstCategories'] = eval_results[
             'averageScoreInstCategories']
         return metric
 
     @staticmethod
     def _convert_to_label_id(result):
         """Convert trainId to id for cityscapes."""
         if isinstance(result, str):
             result = np.load(result)
-        import cityscapesscripts.helpers.labels as CSLabels
         result_copy = result.copy()
         for trainId, label in CSLabels.trainId2label.items():
             result_copy[result == trainId] = label.id
 
         return result_copy
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/evaluation/metrics/iou_metric.py` & `mmsegmentation-1.1.0/mmseg/evaluation/metrics/iou_metric.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import os.path as osp
 from collections import OrderedDict
 from typing import Dict, List, Optional, Sequence
 
 import numpy as np
 import torch
+from mmengine.dist import is_main_process
 from mmengine.evaluator import BaseMetric
 from mmengine.logging import MMLogger, print_log
+from mmengine.utils import mkdir_or_exist
+from PIL import Image
 from prettytable import PrettyTable
 
 from mmseg.registry import METRICS
 
 
 @METRICS.register_module()
 class IoUMetric(BaseMetric):
@@ -23,66 +27,98 @@
         nan_to_num (int, optional): If specified, NaN values will be replaced
             by the numbers defined by the user. Default: None.
         beta (int): Determines the weight of recall in the combined score.
             Default: 1.
         collect_device (str): Device name used for collecting results from
             different ranks during distributed training. Must be 'cpu' or
             'gpu'. Defaults to 'cpu'.
+        output_dir (str): The directory for output prediction. Defaults to
+            None.
+        format_only (bool): Only format result for results commit without
+            perform evaluation. It is useful when you want to save the result
+            to a specific format and submit it to the test server.
+            Defaults to False.
         prefix (str, optional): The prefix that will be added in the metric
             names to disambiguate homonymous metrics of different evaluators.
             If prefix is not provided in the argument, self.default_prefix
             will be used instead. Defaults to None.
     """
 
     def __init__(self,
                  ignore_index: int = 255,
                  iou_metrics: List[str] = ['mIoU'],
                  nan_to_num: Optional[int] = None,
                  beta: int = 1,
                  collect_device: str = 'cpu',
-                 prefix: Optional[str] = None) -> None:
+                 output_dir: Optional[str] = None,
+                 format_only: bool = False,
+                 prefix: Optional[str] = None,
+                 **kwargs) -> None:
         super().__init__(collect_device=collect_device, prefix=prefix)
 
         self.ignore_index = ignore_index
         self.metrics = iou_metrics
         self.nan_to_num = nan_to_num
         self.beta = beta
+        self.output_dir = output_dir
+        if self.output_dir and is_main_process():
+            mkdir_or_exist(self.output_dir)
+        self.format_only = format_only
 
     def process(self, data_batch: dict, data_samples: Sequence[dict]) -> None:
         """Process one batch of data and data_samples.
 
         The processed results should be stored in ``self.results``, which will
         be used to compute the metrics when all batches have been processed.
 
         Args:
             data_batch (dict): A batch of data from the dataloader.
             data_samples (Sequence[dict]): A batch of outputs from the model.
         """
         num_classes = len(self.dataset_meta['classes'])
         for data_sample in data_samples:
             pred_label = data_sample['pred_sem_seg']['data'].squeeze()
-            label = data_sample['gt_sem_seg']['data'].squeeze().to(pred_label)
-            self.results.append(
-                self.intersect_and_union(pred_label, label, num_classes,
-                                         self.ignore_index))
+            # format_only always for test dataset without ground truth
+            if not self.format_only:
+                label = data_sample['gt_sem_seg']['data'].squeeze().to(
+                    pred_label)
+                self.results.append(
+                    self.intersect_and_union(pred_label, label, num_classes,
+                                             self.ignore_index))
+            # format_result
+            if self.output_dir is not None:
+                basename = osp.splitext(osp.basename(
+                    data_sample['img_path']))[0]
+                png_filename = osp.abspath(
+                    osp.join(self.output_dir, f'{basename}.png'))
+                output_mask = pred_label.cpu().numpy()
+                # The index range of official ADE20k dataset is from 0 to 150.
+                # But the index range of output is from 0 to 149.
+                # That is because we set reduce_zero_label=True.
+                if data_sample.get('reduce_zero_label', False):
+                    output_mask = output_mask + 1
+                output = Image.fromarray(output_mask.astype(np.uint8))
+                output.save(png_filename)
 
     def compute_metrics(self, results: list) -> Dict[str, float]:
         """Compute the metrics from processed results.
 
         Args:
             results (list): The processed results of each batch.
 
         Returns:
             Dict[str, float]: The computed metrics. The keys are the names of
                 the metrics, and the values are corresponding results. The key
                 mainly includes aAcc, mIoU, mAcc, mDice, mFscore, mPrecision,
                 mRecall.
         """
         logger: MMLogger = MMLogger.get_current_instance()
-
+        if self.format_only:
+            logger.info(f'results are saved to {osp.dirname(self.output_dir)}')
+            return OrderedDict()
         # convert list of tuples to tuple of lists, e.g.
         # [(A_1, B_1, C_1, D_1), ...,  (A_n, B_n, C_n, D_n)] to
         # ([A_1, ..., A_n], ..., [D_1, ..., D_n])
         results = tuple(zip(*results))
         assert len(results) == 4
 
         total_area_intersect = sum(results[0])
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/__init__.py` & `mmsegmentation-1.1.0/mmseg/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/__init__.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .beit import BEiT
 from .bisenetv1 import BiSeNetV1
 from .bisenetv2 import BiSeNetV2
 from .cgnet import CGNet
+from .ddrnet import DDRNet
 from .erfnet import ERFNet
 from .fast_scnn import FastSCNN
 from .hrnet import HRNet
 from .icnet import ICNet
 from .mae import MAE
 from .mit import MixVisionTransformer
 from .mobilenet_v2 import MobileNetV2
 from .mobilenet_v3 import MobileNetV3
+from .mscan import MSCAN
+from .pidnet import PIDNet
 from .resnest import ResNeSt
 from .resnet import ResNet, ResNetV1c, ResNetV1d
 from .resnext import ResNeXt
 from .stdc import STDCContextPathNet, STDCNet
 from .swin import SwinTransformer
 from .timm_backbone import TIMMBackbone
 from .twins import PCPVT, SVT
@@ -22,9 +25,10 @@
 from .vit import VisionTransformer
 
 __all__ = [
     'ResNet', 'ResNetV1c', 'ResNetV1d', 'ResNeXt', 'HRNet', 'FastSCNN',
     'ResNeSt', 'MobileNetV2', 'UNet', 'CGNet', 'MobileNetV3',
     'VisionTransformer', 'SwinTransformer', 'MixVisionTransformer',
     'BiSeNetV1', 'BiSeNetV2', 'ICNet', 'TIMMBackbone', 'ERFNet', 'PCPVT',
-    'SVT', 'STDCNet', 'STDCContextPathNet', 'BEiT', 'MAE'
+    'SVT', 'STDCNet', 'STDCContextPathNet', 'BEiT', 'MAE', 'PIDNet', 'MSCAN',
+    'DDRNet'
 ]
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/beit.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/bisenetv1.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/bisenetv2.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/cgnet.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/erfnet.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/erfnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/fast_scnn.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/hrnet.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/icnet.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/icnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/mae.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/mae.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/mit.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/mit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/mobilenet_v2.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/mobilenet_v3.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/resnest.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/resnet.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/resnext.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/stdc.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/stdc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/swin.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/swin.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,28 +712,30 @@
             # interpolate position bias table if needed
             relative_position_bias_table_keys = [
                 k for k in state_dict.keys()
                 if 'relative_position_bias_table' in k
             ]
             for table_key in relative_position_bias_table_keys:
                 table_pretrained = state_dict[table_key]
-                table_current = self.state_dict()[table_key]
-                L1, nH1 = table_pretrained.size()
-                L2, nH2 = table_current.size()
-                if nH1 != nH2:
-                    print_log(f'Error in loading {table_key}, pass')
-                elif L1 != L2:
-                    S1 = int(L1**0.5)
-                    S2 = int(L2**0.5)
-                    table_pretrained_resized = F.interpolate(
-                        table_pretrained.permute(1, 0).reshape(1, nH1, S1, S1),
-                        size=(S2, S2),
-                        mode='bicubic')
-                    state_dict[table_key] = table_pretrained_resized.view(
-                        nH2, L2).permute(1, 0).contiguous()
+                if table_key in self.state_dict():
+                    table_current = self.state_dict()[table_key]
+                    L1, nH1 = table_pretrained.size()
+                    L2, nH2 = table_current.size()
+                    if nH1 != nH2:
+                        print_log(f'Error in loading {table_key}, pass')
+                    elif L1 != L2:
+                        S1 = int(L1**0.5)
+                        S2 = int(L2**0.5)
+                        table_pretrained_resized = F.interpolate(
+                            table_pretrained.permute(1, 0).reshape(
+                                1, nH1, S1, S1),
+                            size=(S2, S2),
+                            mode='bicubic')
+                        state_dict[table_key] = table_pretrained_resized.view(
+                            nH2, L2).permute(1, 0).contiguous()
 
             # load state_dict
             self.load_state_dict(state_dict, strict=False)
 
     def forward(self, x):
         x, hw_shape = self.patch_embed(x)
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/timm_backbone.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/twins.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/twins.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/unet.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/backbones/vit.py` & `mmsegmentation-1.1.0/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/builder.py` & `mmsegmentation-1.1.0/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/data_preprocessor.py` & `mmsegmentation-1.1.0/mmseg/models/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/__init__.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .ann_head import ANNHead
 from .apc_head import APCHead
 from .aspp_head import ASPPHead
 from .cc_head import CCHead
 from .da_head import DAHead
+from .ddr_head import DDRHead
 from .dm_head import DMHead
 from .dnl_head import DNLHead
 from .dpt_head import DPTHead
 from .ema_head import EMAHead
 from .enc_head import EncHead
 from .fcn_head import FCNHead
 from .fpn_head import FPNHead
 from .gc_head import GCHead
+from .ham_head import LightHamHead
 from .isa_head import ISAHead
 from .knet_head import IterativeDecodeHead, KernelUpdateHead, KernelUpdator
 from .lraspp_head import LRASPPHead
 from .mask2former_head import Mask2FormerHead
 from .maskformer_head import MaskFormerHead
 from .nl_head import NLHead
 from .ocr_head import OCRHead
+from .pid_head import PIDHead
 from .point_head import PointHead
 from .psa_head import PSAHead
 from .psp_head import PSPHead
 from .segformer_head import SegformerHead
 from .segmenter_mask_head import SegmenterMaskTransformerHead
 from .sep_aspp_head import DepthwiseSeparableASPPHead
 from .sep_fcn_head import DepthwiseSeparableFCNHead
@@ -34,9 +37,10 @@
 __all__ = [
     'FCNHead', 'PSPHead', 'ASPPHead', 'PSAHead', 'NLHead', 'GCHead', 'CCHead',
     'UPerHead', 'DepthwiseSeparableASPPHead', 'ANNHead', 'DAHead', 'OCRHead',
     'EncHead', 'DepthwiseSeparableFCNHead', 'FPNHead', 'EMAHead', 'DNLHead',
     'PointHead', 'APCHead', 'DMHead', 'LRASPPHead', 'SETRUPHead',
     'SETRMLAHead', 'DPTHead', 'SETRMLAHead', 'SegmenterMaskTransformerHead',
     'SegformerHead', 'ISAHead', 'STDCHead', 'IterativeDecodeHead',
-    'KernelUpdateHead', 'KernelUpdator', 'MaskFormerHead', 'Mask2FormerHead'
+    'KernelUpdateHead', 'KernelUpdator', 'MaskFormerHead', 'Mask2FormerHead',
+    'LightHamHead', 'PIDHead', 'DDRHead'
 ]
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/ann_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/apc_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/aspp_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/cascade_decode_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/cc_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/da_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/decode_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/decode_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     predict(): forward() -> predict_by_feat()
 
     Args:
         in_channels (int|Sequence[int]): Input channels.
         channels (int): Channels after modules, before conv_seg.
         num_classes (int): Number of classes.
-        out_channels (int): Output channels of conv_seg.
+        out_channels (int): Output channels of conv_seg. Default: None.
         threshold (float): Threshold for binary segmentation in the case of
             `num_classes==1`. Default: None.
         dropout_ratio (float): Ratio of dropout layer. Default: 0.1.
         conv_cfg (dict|None): Config of conv layers. Default: None.
         norm_cfg (dict|None): Config of norm layers. Default: None.
         act_cfg (dict): Config of activation layers.
             Default: dict(type='ReLU')
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/dm_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/dnl_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/dpt_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/dpt_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/ema_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/enc_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/fcn_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/fpn_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/gc_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/isa_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/isa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/knet_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/knet_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/lraspp_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/mask2former_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/mask2former_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/maskformer_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/maskformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/nl_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/ocr_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/point_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/psa_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/psp_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/segformer_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/segformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/segmenter_mask_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/segmenter_mask_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/sep_aspp_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/sep_fcn_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/setr_mla_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_mla_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/setr_up_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_up_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/stdc_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/stdc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/decode_heads/uper_head.py` & `mmsegmentation-1.1.0/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/__init__.py` & `mmsegmentation-1.1.0/mmseg/models/losses/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .accuracy import Accuracy, accuracy
+from .boundary_loss import BoundaryLoss
 from .cross_entropy_loss import (CrossEntropyLoss, binary_cross_entropy,
                                  cross_entropy, mask_cross_entropy)
 from .dice_loss import DiceLoss
 from .focal_loss import FocalLoss
+from .huasdorff_distance_loss import HuasdorffDisstanceLoss
 from .lovasz_loss import LovaszLoss
+from .ohem_cross_entropy_loss import OhemCrossEntropy
 from .tversky_loss import TverskyLoss
 from .utils import reduce_loss, weight_reduce_loss, weighted_loss
 
 __all__ = [
     'accuracy', 'Accuracy', 'cross_entropy', 'binary_cross_entropy',
     'mask_cross_entropy', 'CrossEntropyLoss', 'reduce_loss',
     'weight_reduce_loss', 'weighted_loss', 'LovaszLoss', 'DiceLoss',
-    'FocalLoss', 'TverskyLoss'
+    'FocalLoss', 'TverskyLoss', 'OhemCrossEntropy', 'BoundaryLoss',
+    'HuasdorffDisstanceLoss'
 ]
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/accuracy.py` & `mmsegmentation-1.1.0/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/cross_entropy_loss.py` & `mmsegmentation-1.1.0/mmseg/models/losses/cross_entropy_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         # [N, 1, H, W] and that of label is [N, H, W].
         # As the ignore_index often set as 255, so the
         # binary class label check should mask out
         # ignore_index
         assert label[label != ignore_index].max() <= 1, \
             'For pred with shape [N, 1, H, W], its label must have at ' \
             'most 2 classes'
-        pred = pred.squeeze()
+        pred = pred.squeeze(1)
     if pred.dim() != label.dim():
         assert (pred.dim() == 2 and label.dim() == 1) or (
                 pred.dim() == 4 and label.dim() == 3), \
             'Only pred shape [N, C], label shape [N] or pred shape [N, C, ' \
             'H, W], label shape [N, H, W] are supported'
         # `weight` returned from `_expand_onehot_labels`
         # has been treated for valid (non-ignore) pixels
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/dice_loss.py` & `mmsegmentation-1.1.0/mmseg/models/losses/tversky_loss.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,127 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-"""Modified from https://github.com/LikeLy-Journey/SegmenTron/blob/master/
-segmentron/solver/loss.py (Apache-2.0 License)"""
+"""Modified from
+https://github.com/JunMa11/SegLoss/blob/master/losses_pytorch/dice_loss.py#L333
+(Apache-2.0 License)"""
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from mmseg.registry import MODELS
+from ..builder import LOSSES
 from .utils import get_class_weight, weighted_loss
 
 
 @weighted_loss
-def dice_loss(pred,
-              target,
-              valid_mask,
-              smooth=1,
-              exponent=2,
-              class_weight=None,
-              ignore_index=255):
+def tversky_loss(pred,
+                 target,
+                 valid_mask,
+                 alpha=0.3,
+                 beta=0.7,
+                 smooth=1,
+                 class_weight=None,
+                 ignore_index=255):
     assert pred.shape[0] == target.shape[0]
     total_loss = 0
     num_classes = pred.shape[1]
     for i in range(num_classes):
         if i != ignore_index:
-            dice_loss = binary_dice_loss(
+            tversky_loss = binary_tversky_loss(
                 pred[:, i],
                 target[..., i],
                 valid_mask=valid_mask,
-                smooth=smooth,
-                exponent=exponent)
+                alpha=alpha,
+                beta=beta,
+                smooth=smooth)
             if class_weight is not None:
-                dice_loss *= class_weight[i]
-            total_loss += dice_loss
+                tversky_loss *= class_weight[i]
+            total_loss += tversky_loss
     return total_loss / num_classes
 
 
 @weighted_loss
-def binary_dice_loss(pred, target, valid_mask, smooth=1, exponent=2, **kwards):
+def binary_tversky_loss(pred,
+                        target,
+                        valid_mask,
+                        alpha=0.3,
+                        beta=0.7,
+                        smooth=1):
     assert pred.shape[0] == target.shape[0]
     pred = pred.reshape(pred.shape[0], -1)
     target = target.reshape(target.shape[0], -1)
     valid_mask = valid_mask.reshape(valid_mask.shape[0], -1)
 
-    num = torch.sum(torch.mul(pred, target) * valid_mask, dim=1) * 2 + smooth
-    den = torch.sum(pred.pow(exponent) + target.pow(exponent), dim=1) + smooth
-
-    return 1 - num / den
+    TP = torch.sum(torch.mul(pred, target) * valid_mask, dim=1)
+    FP = torch.sum(torch.mul(pred, 1 - target) * valid_mask, dim=1)
+    FN = torch.sum(torch.mul(1 - pred, target) * valid_mask, dim=1)
+    tversky = (TP + smooth) / (TP + alpha * FP + beta * FN + smooth)
 
+    return 1 - tversky
 
-@MODELS.register_module()
-class DiceLoss(nn.Module):
-    """DiceLoss.
 
-    This loss is proposed in `V-Net: Fully Convolutional Neural Networks for
-    Volumetric Medical Image Segmentation <https://arxiv.org/abs/1606.04797>`_.
+@LOSSES.register_module()
+class TverskyLoss(nn.Module):
+    """TverskyLoss. This loss is proposed in `Tversky loss function for image
+    segmentation using 3D fully convolutional deep networks.
 
+    <https://arxiv.org/abs/1706.05721>`_.
     Args:
         smooth (float): A float number to smooth loss, and avoid NaN error.
-            Default: 1
-        exponent (float): An float number to calculate denominator
-            value: \\sum{x^exponent} + \\sum{y^exponent}. Default: 2.
-        reduction (str, optional): The method used to reduce the loss. Options
-            are "none", "mean" and "sum". This parameter only works when
-            per_image is True. Default: 'mean'.
+            Default: 1.
         class_weight (list[float] | str, optional): Weight of each class. If in
             str format, read them from a file. Defaults to None.
         loss_weight (float, optional): Weight of the loss. Default to 1.0.
         ignore_index (int | None): The label index to be ignored. Default: 255.
+        alpha(float, in [0, 1]):
+            The coefficient of false positives. Default: 0.3.
+        beta (float, in [0, 1]):
+            The coefficient of false negatives. Default: 0.7.
+            Note: alpha + beta = 1.
         loss_name (str, optional): Name of the loss item. If you want this loss
             item to be included into the backward graph, `loss_` must be the
-            prefix of the name. Defaults to 'loss_dice'.
+            prefix of the name. Defaults to 'loss_tversky'.
     """
 
     def __init__(self,
                  smooth=1,
-                 exponent=2,
-                 reduction='mean',
                  class_weight=None,
                  loss_weight=1.0,
                  ignore_index=255,
-                 loss_name='loss_dice',
-                 **kwards):
+                 alpha=0.3,
+                 beta=0.7,
+                 loss_name='loss_tversky'):
         super().__init__()
         self.smooth = smooth
-        self.exponent = exponent
-        self.reduction = reduction
         self.class_weight = get_class_weight(class_weight)
         self.loss_weight = loss_weight
         self.ignore_index = ignore_index
+        assert (alpha + beta == 1.0), 'Sum of alpha and beta but be 1.0!'
+        self.alpha = alpha
+        self.beta = beta
         self._loss_name = loss_name
 
-    def forward(self,
-                pred,
-                target,
-                avg_factor=None,
-                reduction_override=None,
-                **kwards):
-        assert reduction_override in (None, 'none', 'mean', 'sum')
-        reduction = (
-            reduction_override if reduction_override else self.reduction)
+    def forward(self, pred, target, **kwargs):
         if self.class_weight is not None:
             class_weight = pred.new_tensor(self.class_weight)
         else:
             class_weight = None
 
         pred = F.softmax(pred, dim=1)
         num_classes = pred.shape[1]
         one_hot_target = F.one_hot(
             torch.clamp(target.long(), 0, num_classes - 1),
             num_classes=num_classes)
         valid_mask = (target != self.ignore_index).long()
 
-        loss = self.loss_weight * dice_loss(
+        loss = self.loss_weight * tversky_loss(
             pred,
             one_hot_target,
             valid_mask=valid_mask,
-            reduction=reduction,
-            avg_factor=avg_factor,
+            alpha=self.alpha,
+            beta=self.beta,
             smooth=self.smooth,
-            exponent=self.exponent,
             class_weight=class_weight,
             ignore_index=self.ignore_index)
         return loss
 
     @property
     def loss_name(self):
         """Loss Name.
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/focal_loss.py` & `mmsegmentation-1.1.0/mmseg/models/losses/focal_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -267,24 +267,34 @@
 
         reduction = (
             reduction_override if reduction_override else self.reduction)
         if self.use_sigmoid:
             num_classes = pred.size(1)
             if torch.cuda.is_available() and pred.is_cuda:
                 if target.dim() == 1:
-                    one_hot_target = F.one_hot(target, num_classes=num_classes)
+                    one_hot_target = F.one_hot(
+                        target, num_classes=num_classes + 1)
+                    if num_classes == 1:
+                        one_hot_target = one_hot_target[:, 1]
+                        target = 1 - target
+                    else:
+                        one_hot_target = one_hot_target[:, :num_classes]
                 else:
                     one_hot_target = target
                     target = target.argmax(dim=1)
                     valid_mask = (target != ignore_index).view(-1, 1)
                 calculate_loss_func = sigmoid_focal_loss
             else:
                 one_hot_target = None
                 if target.dim() == 1:
-                    target = F.one_hot(target, num_classes=num_classes)
+                    target = F.one_hot(target, num_classes=num_classes + 1)
+                    if num_classes == 1:
+                        target = target[:, 1]
+                    else:
+                        target = target[:, num_classes]
                 else:
                     valid_mask = (target.argmax(dim=1) != ignore_index).view(
                         -1, 1)
                 calculate_loss_func = py_sigmoid_focal_loss
 
             loss_cls = self.loss_weight * calculate_loss_func(
                 pred,
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/lovasz_loss.py` & `mmsegmentation-1.1.0/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/losses/utils.py` & `mmsegmentation-1.1.0/mmseg/models/losses/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         else:
             # pkl, json or yaml
             class_weight = load(class_weight)
 
     return class_weight
 
 
-def reduce_loss(loss, reduction):
+def reduce_loss(loss, reduction) -> torch.Tensor:
     """Reduce loss as specified.
 
     Args:
         loss (Tensor): Elementwise loss tensor.
         reduction (str): Options are "none", "mean" and "sum".
 
     Return:
@@ -41,15 +41,18 @@
         return loss
     elif reduction_enum == 1:
         return loss.mean()
     elif reduction_enum == 2:
         return loss.sum()
 
 
-def weight_reduce_loss(loss, weight=None, reduction='mean', avg_factor=None):
+def weight_reduce_loss(loss,
+                       weight=None,
+                       reduction='mean',
+                       avg_factor=None) -> torch.Tensor:
     """Apply element-wise weight and reduce loss.
 
     Args:
         loss (Tensor): Element-wise loss.
         weight (Tensor): Element-wise weights.
         reduction (str): Same as built-in losses of PyTorch.
         avg_factor (float): Average factor when computing the mean of losses.
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/necks/featurepyramid.py` & `mmsegmentation-1.1.0/mmseg/models/necks/featurepyramid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/necks/fpn.py` & `mmsegmentation-1.1.0/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/necks/ic_neck.py` & `mmsegmentation-1.1.0/mmseg/models/necks/ic_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/necks/jpu.py` & `mmsegmentation-1.1.0/mmseg/models/necks/jpu.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/necks/mla_neck.py` & `mmsegmentation-1.1.0/mmseg/models/necks/mla_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/necks/multilevel_neck.py` & `mmsegmentation-1.1.0/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/segmentors/base.py` & `mmsegmentation-1.1.0/mmseg/models/segmentors/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -183,14 +183,15 @@
                     warning=False).squeeze(0)
             else:
                 i_seg_logits = seg_logits[i]
 
             if C > 1:
                 i_seg_pred = i_seg_logits.argmax(dim=0, keepdim=True)
             else:
+                i_seg_logits = i_seg_logits.sigmoid()
                 i_seg_pred = (i_seg_logits >
                               self.decode_head.threshold).to(i_seg_logits)
             data_samples[i].set_data({
                 'seg_logits':
                 PixelData(**{'data': i_seg_logits}),
                 'pred_sem_seg':
                 PixelData(**{'data': i_seg_pred})
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/segmentors/cascade_encoder_decoder.py` & `mmsegmentation-1.1.0/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/segmentors/encoder_decoder.py` & `mmsegmentation-1.1.0/mmseg/models/segmentors/encoder_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
      loss(): extract_feat() -> _decode_head_forward_train() -> _auxiliary_head_forward_train (optional)
      _decode_head_forward_train(): decode_head.loss()
      _auxiliary_head_forward_train(): auxiliary_head.loss (optional)
 
     2. The ``predict`` method is used to predict segmentation results,
     which includes two steps: (1) Run inference function to obtain the list of
     seg_logits (2) Call post-processing function to obtain list of
-    ``SegDataSampel`` including ``pred_sem_seg`` and ``seg_logits``.
+    ``SegDataSample`` including ``pred_sem_seg`` and ``seg_logits``.
 
     .. code:: text
 
      predict(): inference() -> postprocess_result()
      infercen(): whole_inference()/slide_inference()
      whole_inference()/slide_inference(): encoder_decoder()
      encoder_decoder(): extract_feat() -> decode_head.predict()
@@ -256,18 +256,18 @@
             Tensor: The segmentation results, seg_logits from model of each
                 input image.
         """
 
         h_stride, w_stride = self.test_cfg.stride
         h_crop, w_crop = self.test_cfg.crop_size
         batch_size, _, h_img, w_img = inputs.size()
-        num_classes = self.num_classes
+        out_channels = self.out_channels
         h_grids = max(h_img - h_crop + h_stride - 1, 0) // h_stride + 1
         w_grids = max(w_img - w_crop + w_stride - 1, 0) // w_stride + 1
-        preds = inputs.new_zeros((batch_size, num_classes, h_img, w_img))
+        preds = inputs.new_zeros((batch_size, out_channels, h_img, w_img))
         count_mat = inputs.new_zeros((batch_size, 1, h_img, w_img))
         for h_idx in range(h_grids):
             for w_idx in range(w_grids):
                 y1 = h_idx * h_stride
                 x1 = w_idx * w_stride
                 y2 = min(y1 + h_crop, h_img)
                 x2 = min(x1 + w_crop, w_img)
@@ -322,16 +322,17 @@
                 For details on the values of these keys see
                 `mmseg/datasets/pipelines/formatting.py:PackSegInputs`.
 
         Returns:
             Tensor: The segmentation results, seg_logits from model of each
                 input image.
         """
-
-        assert self.test_cfg.mode in ['slide', 'whole']
+        assert self.test_cfg.get('mode', 'whole') in ['slide', 'whole'], \
+            f'Only "slide" or "whole" test mode are supported, but got ' \
+            f'{self.test_cfg["mode"]}.'
         ori_shape = batch_img_metas[0]['ori_shape']
         assert all(_['ori_shape'] == ori_shape for _ in batch_img_metas)
         if self.test_cfg.mode == 'slide':
             seg_logit = self.slide_inference(inputs, batch_img_metas)
         else:
             seg_logit = self.whole_inference(inputs, batch_img_metas)
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/segmentors/seg_tta.py` & `mmsegmentation-1.1.0/mmseg/models/segmentors/seg_tta.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,9 +40,10 @@
             else:
                 seg_pred = logits.argmax(dim=0)
             data_sample = SegDataSample(
                 **{
                     'pred_sem_seg': PixelData(data=seg_pred),
                     'gt_sem_seg': data_samples[0].gt_sem_seg
                 })
+            data_sample.set_metainfo({'img_path': data_samples[0].img_path})
             predictions.append(data_sample)
         return predictions
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/__init__.py` & `mmsegmentation-1.1.0/mmseg/models/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from .basic_block import BasicBlock, Bottleneck
 from .embed import PatchEmbed
 from .encoding import Encoding
 from .inverted_residual import InvertedResidual, InvertedResidualV3
 from .make_divisible import make_divisible
+from .ppm import DAPPM, PAPPM
 from .res_layer import ResLayer
 from .se_layer import SELayer
 from .self_attention_block import SelfAttentionBlock
 from .shape_convert import (nchw2nlc2nchw, nchw_to_nlc, nlc2nchw2nlc,
                             nlc_to_nchw)
 from .up_conv_block import UpConvBlock
 from .wrappers import Upsample, resize
 
 __all__ = [
     'ResLayer', 'SelfAttentionBlock', 'make_divisible', 'InvertedResidual',
     'UpConvBlock', 'InvertedResidualV3', 'SELayer', 'PatchEmbed',
     'nchw_to_nlc', 'nlc_to_nchw', 'nchw2nlc2nchw', 'nlc2nchw2nlc', 'Encoding',
-    'Upsample', 'resize'
+    'Upsample', 'resize', 'DAPPM', 'PAPPM', 'BasicBlock', 'Bottleneck'
 ]
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/embed.py` & `mmsegmentation-1.1.0/mmseg/models/utils/embed.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/encoding.py` & `mmsegmentation-1.1.0/mmseg/models/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/inverted_residual.py` & `mmsegmentation-1.1.0/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/make_divisible.py` & `mmsegmentation-1.1.0/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/res_layer.py` & `mmsegmentation-1.1.0/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/se_layer.py` & `mmsegmentation-1.1.0/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/self_attention_block.py` & `mmsegmentation-1.1.0/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/shape_convert.py` & `mmsegmentation-1.1.0/mmseg/models/utils/shape_convert.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/up_conv_block.py` & `mmsegmentation-1.1.0/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/models/utils/wrappers.py` & `mmsegmentation-1.1.0/mmseg/models/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/registry/__init__.py` & `mmsegmentation-1.1.0/mmseg/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/registry/registry.py` & `mmsegmentation-1.1.0/mmseg/registry/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-"""MMSegmentation provides 17 registry nodes to support using modules across
+"""MMSegmentation provides 21 registry nodes to support using modules across
 projects. Each node is a child of the root registry in MMEngine.
 
 More details can be found at
-https://mmengine.readthedocs.io/en/latest/tutorials/registry.html.
+https://mmengine.readthedocs.io/en/latest/advanced_tutorials/registry.html.
 """
 
 from mmengine.registry import DATA_SAMPLERS as MMENGINE_DATA_SAMPLERS
 from mmengine.registry import DATASETS as MMENGINE_DATASETS
 from mmengine.registry import EVALUATOR as MMENGINE_EVALUATOR
 from mmengine.registry import HOOKS as MMENGINE_HOOKS
 from mmengine.registry import INFERENCERS as MMENGINE_INFERENCERS
@@ -42,18 +42,15 @@
 # manage all kinds of hooks like `CheckpointHook`
 HOOKS = Registry(
     'hook', parent=MMENGINE_HOOKS, locations=['mmseg.engine.hooks'])
 
 # manage data-related modules
 DATASETS = Registry(
     'dataset', parent=MMENGINE_DATASETS, locations=['mmseg.datasets'])
-DATA_SAMPLERS = Registry(
-    'data sampler',
-    parent=MMENGINE_DATA_SAMPLERS,
-    locations=['mmseg.datasets.samplers'])
+DATA_SAMPLERS = Registry('data sampler', parent=MMENGINE_DATA_SAMPLERS)
 TRANSFORMS = Registry(
     'transform',
     parent=MMENGINE_TRANSFORMS,
     locations=['mmseg.datasets.transforms'])
 
 # mangage all kinds of modules inheriting `nn.Module`
 MODELS = Registry('model', parent=MMENGINE_MODELS, locations=['mmseg.models'])
@@ -81,17 +78,15 @@
 # manage constructors that customize the optimization hyperparameters.
 OPTIM_WRAPPER_CONSTRUCTORS = Registry(
     'optimizer wrapper constructor',
     parent=MMENGINE_OPTIM_WRAPPER_CONSTRUCTORS,
     locations=['mmseg.engine.optimizers'])
 # mangage all kinds of parameter schedulers like `MultiStepLR`
 PARAM_SCHEDULERS = Registry(
-    'parameter scheduler',
-    parent=MMENGINE_PARAM_SCHEDULERS,
-    locations=['mmseg.engine.schedulers'])
+    'parameter scheduler', parent=MMENGINE_PARAM_SCHEDULERS)
 
 # manage all kinds of metrics
 METRICS = Registry(
     'metric', parent=MMENGINE_METRICS, locations=['mmseg.evaluation'])
 # manage evaluator
 EVALUATOR = Registry(
     'evaluator', parent=MMENGINE_EVALUATOR, locations=['mmseg.evaluation'])
```

### Comparing `mmsegmentation-1.0.0rc6/mmseg/structures/sampler/ohem_pixel_sampler.py` & `mmsegmentation-1.1.0/mmseg/structures/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/structures/seg_data_sample.py` & `mmsegmentation-1.1.0/mmseg/structures/seg_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/utils/__init__.py` & `mmsegmentation-1.1.0/mmseg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/utils/io.py` & `mmsegmentation-1.1.0/mmseg/utils/io.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/utils/misc.py` & `mmsegmentation-1.1.0/mmseg/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/utils/set_env.py` & `mmsegmentation-1.1.0/mmseg/utils/set_env.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/utils/typing_utils.py` & `mmsegmentation-1.1.0/mmseg/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/mmseg/visualization/local_visualizer.py` & `mmsegmentation-1.1.0/mmseg/visualization/local_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         classes (list, optional): Input classes for result rendering, as the
             prediction of segmentation model is a segment map with label
             indices, `classes` is a list which includes items responding to the
             label indices. If classes is not defined, visualizer will take
             `cityscapes` classes by default. Defaults to None.
         palette (list, optional): Input palette for result rendering, which is
             a list of color palette responding to the classes. Defaults to None.
-        dataset_name (str, optional): `Dataset name or alias <https://github.com/open-mmlab/mmsegmentation/blob/dev-1.x/mmseg/utils/class_names.py#L302-L317>`_
+        dataset_name (str, optional): `Dataset name or alias <https://github.com/open-mmlab/mmsegmentation/blob/main/mmseg/utils/class_names.py#L302-L317>`_
             visulizer will use the meta information of the dataset i.e. classes
             and palette, but the `classes` and `palette` have higher priority.
             Defaults to None.
         alpha (int, float): The transparency of segmentation mask.
                 Defaults to 0.8.
 
     Examples:
@@ -104,22 +104,22 @@
         ids = np.unique(sem_seg)[::-1]
         legal_indices = ids < num_classes
         ids = ids[legal_indices]
         labels = np.array(ids, dtype=np.int64)
 
         colors = [palette[label] for label in labels]
 
-        self.set_image(image)
-
-        # draw semantic masks
+        mask = np.zeros_like(image, dtype=np.uint8)
         for label, color in zip(labels, colors):
-            self.draw_binary_masks(
-                sem_seg == label, colors=[color], alphas=self.alpha)
+            mask[sem_seg[0] == label, :] = color
 
-        return self.get_image()
+        color_seg = (image * (1 - self.alpha) + mask * self.alpha).astype(
+            np.uint8)
+        self.set_image(color_seg)
+        return color_seg
 
     def set_dataset_meta(self,
                          classes: Optional[List] = None,
                          palette: Optional[List] = None,
                          dataset_name: Optional[str] = None) -> None:
         """Set meta information to visualizer.
 
@@ -129,15 +129,15 @@
                 label indices, `classes` is a list which includes items
                 responding to the label indices. If classes is not defined,
                 visualizer will take `cityscapes` classes by default.
                 Defaults to None.
             palette (list, optional): Input palette for result rendering, which
                 is a list of color palette responding to the classes.
                 Defaults to None.
-            dataset_name (str, optional): `Dataset name or alias <https://github.com/open-mmlab/mmsegmentation/blob/dev-1.x/mmseg/utils/class_names.py#L302-L317>`_
+            dataset_name (str, optional): `Dataset name or alias <https://github.com/open-mmlab/mmsegmentation/blob/main/mmseg/utils/class_names.py#L302-L317>`_
                 visulizer will use the meta information of the dataset i.e.
                 classes and palette, but the `classes` and `palette` have
                 higher priority. Defaults to None.
         """ # noqa
         # Set default value. When calling
         # `SegLocalVisualizer().dataset_meta=xxx`,
         # it will override the default value.
@@ -222,10 +222,10 @@
         else:
             drawn_img = pred_img_data
 
         if show:
             self.show(drawn_img, win_name=name, wait_time=wait_time)
 
         if out_file is not None:
-            mmcv.imwrite(mmcv.bgr2rgb(drawn_img), out_file)
+            mmcv.imwrite(mmcv.rgb2bgr(drawn_img), out_file)
         else:
             self.add_image(name, drawn_img, step)
```

### Comparing `mmsegmentation-1.0.0rc6/mmsegmentation.egg-info/SOURCES.txt` & `mmsegmentation-1.1.0/mmsegmentation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py
 mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py
 mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py
 mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py
 mmseg/.mim/configs/_base_/datasets/drive.py
 mmseg/.mim/configs/_base_/datasets/hrf.py
 mmseg/.mim/configs/_base_/datasets/isaid.py
+mmseg/.mim/configs/_base_/datasets/levir_256x256.py
 mmseg/.mim/configs/_base_/datasets/loveda.py
+mmseg/.mim/configs/_base_/datasets/mapillary_v1.py
+mmseg/.mim/configs/_base_/datasets/mapillary_v1_65.py
+mmseg/.mim/configs/_base_/datasets/mapillary_v2.py
 mmseg/.mim/configs/_base_/datasets/pascal_context.py
 mmseg/.mim/configs/_base_/datasets/pascal_context_59.py
 mmseg/.mim/configs/_base_/datasets/pascal_voc12.py
 mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py
 mmseg/.mim/configs/_base_/datasets/potsdam.py
 mmseg/.mim/configs/_base_/datasets/refuge.py
 mmseg/.mim/configs/_base_/datasets/stare.py
@@ -75,18 +79,18 @@
 mmseg/.mim/configs/_base_/models/upernet_convnext.py
 mmseg/.mim/configs/_base_/models/upernet_mae.py
 mmseg/.mim/configs/_base_/models/upernet_r50.py
 mmseg/.mim/configs/_base_/models/upernet_swin.py
 mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py
 mmseg/.mim/configs/_base_/schedules/schedule_160k.py
 mmseg/.mim/configs/_base_/schedules/schedule_20k.py
+mmseg/.mim/configs/_base_/schedules/schedule_240k.py
 mmseg/.mim/configs/_base_/schedules/schedule_320k.py
 mmseg/.mim/configs/_base_/schedules/schedule_40k.py
 mmseg/.mim/configs/_base_/schedules/schedule_80k.py
-mmseg/.mim/configs/ann/ann.yml
 mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/ann/ann_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/ann/ann_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/ann/ann_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -95,50 +99,50 @@
 mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/ann/ann_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/ann/ann_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/ann/ann_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/ann/ann_r50-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/apcnet/apcnet.yml
+mmseg/.mim/configs/ann/metafile.yaml
 mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-80k_ade20k-512x512.py
+mmseg/.mim/configs/apcnet/metafile.yaml
 mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py
 mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py
 mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py
 mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py
-mmseg/.mim/configs/beit/beit.yml
-mmseg/.mim/configs/bisenetv1/bisenetv1.yml
+mmseg/.mim/configs/beit/metafile.yaml
 mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb8-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py
-mmseg/.mim/configs/bisenetv2/bisenetv2.yml
+mmseg/.mim/configs/bisenetv1/metafile.yaml
 mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-amp-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py
-mmseg/.mim/configs/ccnet/ccnet.yml
+mmseg/.mim/configs/bisenetv2/metafile.yaml
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -147,25 +151,25 @@
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/cgnet/cgnet.yml
+mmseg/.mim/configs/ccnet/metafile.yaml
 mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py
 mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py
+mmseg/.mim/configs/cgnet/metafile.yaml
 mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py
 mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py
 mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py
 mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py
 mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py
 mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py
-mmseg/.mim/configs/convnext/convnext.yml
-mmseg/.mim/configs/danet/danet.yml
+mmseg/.mim/configs/convnext/metafile.yaml
 mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/danet/danet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/danet/danet_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/danet/danet_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -174,15 +178,18 @@
 mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/danet/danet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/danet/danet_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/danet/danet_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/danet/danet_r50-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/deeplabv3/deeplabv3.yml
+mmseg/.mim/configs/danet/metafile.yaml
+mmseg/.mim/configs/ddrnet/ddrnet_23-slim_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
+mmseg/.mim/configs/ddrnet/ddrnet_23_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
+mmseg/.mim/configs/ddrnet/metafile.yaml
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
@@ -220,15 +227,15 @@
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-769x769.py
-mmseg/.mim/configs/deeplabv3plus/deeplabv3plus.yml
+mmseg/.mim/configs/deeplabv3/metafile.yaml
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
@@ -249,14 +256,15 @@
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_isaid-896x896.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_loveda-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_potsdam-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_vaihingen-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-769x769.py
+mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-300k_mapillay_v1_65-1280x1280.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py
@@ -267,48 +275,51 @@
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_loveda-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_potsdam-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_vaihingen-512x512.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-769x769.py
-mmseg/.mim/configs/dmnet/dmnet.yml
+mmseg/.mim/configs/deeplabv3plus/metafile.yaml
 mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-80k_ade20k-512x512.py
+mmseg/.mim/configs/dmnet/metafile.yaml
 mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/dnlnet/dnlnet.yml
-mmseg/.mim/configs/dpt/dpt.yml
+mmseg/.mim/configs/dnlnet/metafile.yaml
 mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py
-mmseg/.mim/configs/emanet/emanet.yml
+mmseg/.mim/configs/dpt/metafile.yaml
+mmseg/.mim/configs/dsdl/cityscapes.py
+mmseg/.mim/configs/dsdl/metafile.yaml
+mmseg/.mim/configs/dsdl/voc.py
 mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-769x769.py
-mmseg/.mim/configs/encnet/encnet.yml
+mmseg/.mim/configs/emanet/metafile.yaml
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -318,44 +329,44 @@
 mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/encnet/encnet_r50s-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/erfnet/erfnet.yml
+mmseg/.mim/configs/encnet/metafile.yaml
 mmseg/.mim/configs/erfnet/erfnet_fcn_4xb4-160k_cityscapes-512x1024.py
-mmseg/.mim/configs/fastfcn/fastfcn.yml
+mmseg/.mim/configs/erfnet/metafile.yaml
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_cityscapes-512x1024.py
+mmseg/.mim/configs/fastfcn/metafile.yaml
 mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py
-mmseg/.mim/configs/fastscnn/fastscnn.yml
+mmseg/.mim/configs/fastscnn/metafile.yaml
 mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-769x769.py
-mmseg/.mim/configs/fcn/fcn.yml
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-20k_voc12aug-512x512.py
@@ -381,15 +392,15 @@
 mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py
 mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py
 mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py
 mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-769x769.py
-mmseg/.mim/configs/gcnet/gcnet.yml
+mmseg/.mim/configs/fcn/metafile.yaml
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -398,14 +409,15 @@
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-80k_ade20k-512x512.py
+mmseg/.mim/configs/gcnet/metafile.yaml
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-160k_cityscapes-512x1024.py
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py
 mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py
@@ -443,29 +455,28 @@
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_isaid-896x896.py
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_loveda-512x512.py
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-480x480.py
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-59-480x480.py
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_potsdam-512x512.py
 mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_vaihingen-512x512.py
-mmseg/.mim/configs/hrnet/hrnet.yml
-mmseg/.mim/configs/icnet/icnet.yml
+mmseg/.mim/configs/hrnet/metafile.yaml
 mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-160k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-80k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-160k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-80k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-160k_cityscapes-832x832.py
 mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-80k_cityscapes-832x832.py
-mmseg/.mim/configs/isanet/isanet.yml
+mmseg/.mim/configs/icnet/metafile.yaml
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -474,59 +485,60 @@
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-80k_ade20k-512x512.py
+mmseg/.mim/configs/isanet/metafile.yaml
 mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py
 mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py
 mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py
 mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py
 mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py
 mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py
 mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py
-mmseg/.mim/configs/knet/knet.yml
+mmseg/.mim/configs/knet/metafile.yaml
 mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py
 mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py
-mmseg/.mim/configs/mae/mae.yml
-mmseg/.mim/configs/mask2former/mask2former.yml
+mmseg/.mim/configs/mae/metafile.yaml
 mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-90k_cityscapes-512x1024.py
 mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py
 mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py
 mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
 mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
 mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
 mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
 mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py
 mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py
-mmseg/.mim/configs/maskformer/maskformer.yml
+mmseg/.mim/configs/mask2former/metafile.yaml
 mmseg/.mim/configs/maskformer/maskformer_r101-d32_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py
+mmseg/.mim/configs/maskformer/metafile.yaml
+mmseg/.mim/configs/mobilenet_v2/metafile.yaml
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512.py
-mmseg/.mim/configs/mobilenet_v2/mobilenet_v2.yml
+mmseg/.mim/configs/mobilenet_v3/metafile.yaml
 mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024.py
 mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py
-mmseg/.mim/configs/mobilenet_v3/mobilenet_v3.yml
-mmseg/.mim/configs/nonlocal_net/nonlocal_net.yml
+mmseg/.mim/configs/nonlocal_net/metafile.yaml
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -535,15 +547,15 @@
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/ocrnet/ocrnet.yml
+mmseg/.mim/configs/ocrnet/metafile.yaml
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-160k_cityscapes-512x1024.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
@@ -560,26 +572,30 @@
 mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py
-mmseg/.mim/configs/point_rend/point_rend.yml
+mmseg/.mim/configs/pidnet/metafile.yaml
+mmseg/.mim/configs/pidnet/pidnet-l_2xb6-120k_1024x1024-cityscapes.py
+mmseg/.mim/configs/pidnet/pidnet-m_2xb6-120k_1024x1024-cityscapes.py
+mmseg/.mim/configs/pidnet/pidnet-s_2xb6-120k_1024x1024-cityscapes.py
+mmseg/.mim/configs/point_rend/metafile.yaml
 mmseg/.mim/configs/point_rend/pointrend_r101_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/point_rend/pointrend_r101_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/poolformer/fpn_poolformer_m36_8xb4-40k_ade20k-512x512.py
 mmseg/.mim/configs/poolformer/fpn_poolformer_m48_8xb4-40k_ade20k-512x512.py
 mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py
 mmseg/.mim/configs/poolformer/fpn_poolformer_s24_8xb4-40k_ade20k-512x512.py
 mmseg/.mim/configs/poolformer/fpn_poolformer_s36_8x4_512x512_40k_ade20k.py
-mmseg/.mim/configs/poolformer/poolformer.yml
-mmseg/.mim/configs/psanet/psanet.yml
+mmseg/.mim/configs/poolformer/metafile.yaml
+mmseg/.mim/configs/psanet/metafile.yaml
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-40k_voc12aug-512x512.py
@@ -588,15 +604,15 @@
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/pspnet/pspnet.yml
+mmseg/.mim/configs/pspnet/metafile.yaml
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
@@ -655,83 +671,90 @@
 mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py
 mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py
 mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_potsdam-512x512.py
 mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_vaihingen-512x512.py
 mmseg/.mim/configs/pspnet/pspnet_r50b-d32_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-769x769.py
-mmseg/.mim/configs/resnest/resnest.yml
+mmseg/.mim/configs/resnest/metafile.yaml
 mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb2-80k_cityscapes512x1024.py
 mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb4-160k_ade20k-512x512.py
-mmseg/.mim/configs/segformer/segformer.yml
+mmseg/.mim/configs/segformer/metafile.yaml
 mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/segformer/segformer_mit-b1_8xb1-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/segformer/segformer_mit-b1_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/segformer/segformer_mit-b2_8xb1-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/segformer/segformer_mit-b2_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/segformer/segformer_mit-b3_8xb1-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/segformer/segformer_mit-b3_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/segformer/segformer_mit-b4_8xb1-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/segformer/segformer_mit-b4_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/segformer/segformer_mit-b5_8xb1-160k_cityscapes-1024x1024.py
 mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py
-mmseg/.mim/configs/segmenter/segmenter.yml
+mmseg/.mim/configs/segmenter/metafile.yaml
 mmseg/.mim/configs/segmenter/segmenter_vit-b_mask_8xb1-160k_ade20k-512x512.py
 mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py
 mmseg/.mim/configs/segmenter/segmenter_vit-s_fcn_8xb1-160k_ade20k-512x512.py
 mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py
 mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py
+mmseg/.mim/configs/segnext/metafile.yaml
+mmseg/.mim/configs/segnext/segnext_mscan-b_1xb16-adamw-160k_ade20k-512x512.py
+mmseg/.mim/configs/segnext/segnext_mscan-l_1xb16-adamw-160k_ade20k-512x512.py
+mmseg/.mim/configs/segnext/segnext_mscan-s_1xb16-adamw-160k_ade20k-512x512.py
+mmseg/.mim/configs/segnext/segnext_mscan-t_1xb16-adamw-160k_ade20k-512x512.py
 mmseg/.mim/configs/sem_fpn/fpn_r101_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/sem_fpn/fpn_r101_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/sem_fpn/fpn_r50_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/sem_fpn/fpn_r50_4xb4-160k_ade20k-512x512.py
-mmseg/.mim/configs/sem_fpn/sem_fpn.yml
-mmseg/.mim/configs/setr/setr.yml
+mmseg/.mim/configs/sem_fpn/metafile.yaml
+mmseg/.mim/configs/setr/metafile.yaml
 mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py
 mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py
 mmseg/.mim/configs/setr/setr_vit-l_mla_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py
 mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py
 mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py
-mmseg/.mim/configs/stdc/stdc.yml
+mmseg/.mim/configs/stdc/metafile.yaml
 mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/stdc/stdc1_in1k-pre_4xb12-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/stdc/stdc2_4xb12-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/stdc/stdc2_in1k-pre_4xb12-80k_cityscapes-512x1024.py
+mmseg/.mim/configs/swin/metafile.yaml
 mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-base-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-large-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
-mmseg/.mim/configs/swin/swin.yml
-mmseg/.mim/configs/twins/twins.yml
+mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py
+mmseg/.mim/configs/twins/metafile.yaml
 mmseg/.mim/configs/twins/twins_pcpvt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_pcpvt-b_uperhead_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_pcpvt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_pcpvt-l_uperhead_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_pcpvt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_svt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_svt-b_uperhead_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_svt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py
+mmseg/.mim/configs/unet/metafile.yaml
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_drive-64x64.py
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_hrf-256x256.py
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_stare-128x128.py
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
 mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
@@ -748,17 +771,16 @@
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_drive-64x64.py
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_hrf-256x256.py
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_stare-128x128.py
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
 mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
-mmseg/.mim/configs/unet/unet.yml
 mmseg/.mim/configs/unet/unet_s5-d16_deeplabv3_4xb4-40k_chase-db1-128x128.py
-mmseg/.mim/configs/upernet/upernet.yml
+mmseg/.mim/configs/upernet/metafile.yaml
 mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-512x1024.py
 mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/upernet/upernet_r101_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/upernet/upernet_r101_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/upernet/upernet_r101_4xb4-40k_voc12aug-512x512.py
@@ -773,20 +795,20 @@
 mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-769x769.py
 mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/upernet/upernet_r50_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/upernet/upernet_r50_4xb4-20k_voc12aug-512x512.py
 mmseg/.mim/configs/upernet/upernet_r50_4xb4-40k_voc12aug-512x512.py
 mmseg/.mim/configs/upernet/upernet_r50_4xb4-80k_ade20k-512x512.py
-mmseg/.mim/configs/vit/vit.yml
+mmseg/.mim/configs/vit/metafile.yaml
 mmseg/.mim/configs/vit/vit_deit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_deit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-80k_ade20k-512x512.py
-mmseg/.mim/configs/vit/vit_deit-s16-ln_mln_upernet_512x512_160k_ade20k-512x512.py
+mmseg/.mim/configs/vit/vit_deit-s16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_deit-s16_mln_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-80k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py
 mmseg/.mim/tools/dist_test.sh
@@ -803,14 +825,15 @@
 mmseg/.mim/tools/dataset_converters/chase_db1.py
 mmseg/.mim/tools/dataset_converters/cityscapes.py
 mmseg/.mim/tools/dataset_converters/coco_stuff10k.py
 mmseg/.mim/tools/dataset_converters/coco_stuff164k.py
 mmseg/.mim/tools/dataset_converters/drive.py
 mmseg/.mim/tools/dataset_converters/hrf.py
 mmseg/.mim/tools/dataset_converters/isaid.py
+mmseg/.mim/tools/dataset_converters/levircd.py
 mmseg/.mim/tools/dataset_converters/loveda.py
 mmseg/.mim/tools/dataset_converters/pascal_context.py
 mmseg/.mim/tools/dataset_converters/potsdam.py
 mmseg/.mim/tools/dataset_converters/refuge.py
 mmseg/.mim/tools/dataset_converters/stare.py
 mmseg/.mim/tools/dataset_converters/synapse.py
 mmseg/.mim/tools/dataset_converters/vaihingen.py
@@ -838,19 +861,22 @@
 mmseg/datasets/chase_db1.py
 mmseg/datasets/cityscapes.py
 mmseg/datasets/coco_stuff.py
 mmseg/datasets/dark_zurich.py
 mmseg/datasets/dataset_wrappers.py
 mmseg/datasets/decathlon.py
 mmseg/datasets/drive.py
+mmseg/datasets/dsdl.py
 mmseg/datasets/hrf.py
 mmseg/datasets/isaid.py
 mmseg/datasets/isprs.py
+mmseg/datasets/levir.py
 mmseg/datasets/lip.py
 mmseg/datasets/loveda.py
+mmseg/datasets/mapillary.py
 mmseg/datasets/night_driving.py
 mmseg/datasets/pascal_context.py
 mmseg/datasets/potsdam.py
 mmseg/datasets/refuge.py
 mmseg/datasets/stare.py
 mmseg/datasets/synapse.py
 mmseg/datasets/voc.py
@@ -871,22 +897,25 @@
 mmseg/models/builder.py
 mmseg/models/data_preprocessor.py
 mmseg/models/backbones/__init__.py
 mmseg/models/backbones/beit.py
 mmseg/models/backbones/bisenetv1.py
 mmseg/models/backbones/bisenetv2.py
 mmseg/models/backbones/cgnet.py
+mmseg/models/backbones/ddrnet.py
 mmseg/models/backbones/erfnet.py
 mmseg/models/backbones/fast_scnn.py
 mmseg/models/backbones/hrnet.py
 mmseg/models/backbones/icnet.py
 mmseg/models/backbones/mae.py
 mmseg/models/backbones/mit.py
 mmseg/models/backbones/mobilenet_v2.py
 mmseg/models/backbones/mobilenet_v3.py
+mmseg/models/backbones/mscan.py
+mmseg/models/backbones/pidnet.py
 mmseg/models/backbones/resnest.py
 mmseg/models/backbones/resnet.py
 mmseg/models/backbones/resnext.py
 mmseg/models/backbones/stdc.py
 mmseg/models/backbones/swin.py
 mmseg/models/backbones/timm_backbone.py
 mmseg/models/backbones/twins.py
@@ -895,47 +924,53 @@
 mmseg/models/decode_heads/__init__.py
 mmseg/models/decode_heads/ann_head.py
 mmseg/models/decode_heads/apc_head.py
 mmseg/models/decode_heads/aspp_head.py
 mmseg/models/decode_heads/cascade_decode_head.py
 mmseg/models/decode_heads/cc_head.py
 mmseg/models/decode_heads/da_head.py
+mmseg/models/decode_heads/ddr_head.py
 mmseg/models/decode_heads/decode_head.py
 mmseg/models/decode_heads/dm_head.py
 mmseg/models/decode_heads/dnl_head.py
 mmseg/models/decode_heads/dpt_head.py
 mmseg/models/decode_heads/ema_head.py
 mmseg/models/decode_heads/enc_head.py
 mmseg/models/decode_heads/fcn_head.py
 mmseg/models/decode_heads/fpn_head.py
 mmseg/models/decode_heads/gc_head.py
+mmseg/models/decode_heads/ham_head.py
 mmseg/models/decode_heads/isa_head.py
 mmseg/models/decode_heads/knet_head.py
 mmseg/models/decode_heads/lraspp_head.py
 mmseg/models/decode_heads/mask2former_head.py
 mmseg/models/decode_heads/maskformer_head.py
 mmseg/models/decode_heads/nl_head.py
 mmseg/models/decode_heads/ocr_head.py
+mmseg/models/decode_heads/pid_head.py
 mmseg/models/decode_heads/point_head.py
 mmseg/models/decode_heads/psa_head.py
 mmseg/models/decode_heads/psp_head.py
 mmseg/models/decode_heads/segformer_head.py
 mmseg/models/decode_heads/segmenter_mask_head.py
 mmseg/models/decode_heads/sep_aspp_head.py
 mmseg/models/decode_heads/sep_fcn_head.py
 mmseg/models/decode_heads/setr_mla_head.py
 mmseg/models/decode_heads/setr_up_head.py
 mmseg/models/decode_heads/stdc_head.py
 mmseg/models/decode_heads/uper_head.py
 mmseg/models/losses/__init__.py
 mmseg/models/losses/accuracy.py
+mmseg/models/losses/boundary_loss.py
 mmseg/models/losses/cross_entropy_loss.py
 mmseg/models/losses/dice_loss.py
 mmseg/models/losses/focal_loss.py
+mmseg/models/losses/huasdorff_distance_loss.py
 mmseg/models/losses/lovasz_loss.py
+mmseg/models/losses/ohem_cross_entropy_loss.py
 mmseg/models/losses/tversky_loss.py
 mmseg/models/losses/utils.py
 mmseg/models/necks/__init__.py
 mmseg/models/necks/featurepyramid.py
 mmseg/models/necks/fpn.py
 mmseg/models/necks/ic_neck.py
 mmseg/models/necks/jpu.py
@@ -943,18 +978,20 @@
 mmseg/models/necks/multilevel_neck.py
 mmseg/models/segmentors/__init__.py
 mmseg/models/segmentors/base.py
 mmseg/models/segmentors/cascade_encoder_decoder.py
 mmseg/models/segmentors/encoder_decoder.py
 mmseg/models/segmentors/seg_tta.py
 mmseg/models/utils/__init__.py
+mmseg/models/utils/basic_block.py
 mmseg/models/utils/embed.py
 mmseg/models/utils/encoding.py
 mmseg/models/utils/inverted_residual.py
 mmseg/models/utils/make_divisible.py
+mmseg/models/utils/ppm.py
 mmseg/models/utils/res_layer.py
 mmseg/models/utils/se_layer.py
 mmseg/models/utils/self_attention_block.py
 mmseg/models/utils/shape_convert.py
 mmseg/models/utils/up_conv_block.py
 mmseg/models/utils/wrappers.py
 mmseg/registry/__init__.py
@@ -976,14 +1013,15 @@
 mmseg/visualization/local_visualizer.py
 mmsegmentation.egg-info/PKG-INFO
 mmsegmentation.egg-info/SOURCES.txt
 mmsegmentation.egg-info/dependency_links.txt
 mmsegmentation.egg-info/not-zip-safe
 mmsegmentation.egg-info/requires.txt
 mmsegmentation.egg-info/top_level.txt
+requirements/albu.txt
 requirements/docs.txt
 requirements/mminstall.txt
 requirements/optional.txt
 requirements/readthedocs.txt
 requirements/runtime.txt
 requirements/tests.txt
 tests/__init__.py
@@ -1002,14 +1040,16 @@
 tests/test_models/test_backbones/test_erfnet.py
 tests/test_models/test_backbones/test_fast_scnn.py
 tests/test_models/test_backbones/test_hrnet.py
 tests/test_models/test_backbones/test_icnet.py
 tests/test_models/test_backbones/test_mae.py
 tests/test_models/test_backbones/test_mit.py
 tests/test_models/test_backbones/test_mobilenet_v3.py
+tests/test_models/test_backbones/test_mscan.py
+tests/test_models/test_backbones/test_pidnet.py
 tests/test_models/test_backbones/test_resnest.py
 tests/test_models/test_backbones/test_resnet.py
 tests/test_models/test_backbones/test_resnext.py
 tests/test_models/test_backbones/test_stdc.py
 tests/test_models/test_backbones/test_swin.py
 tests/test_models/test_backbones/test_timm_backbone.py
 tests/test_models/test_backbones/test_twins.py
@@ -1024,20 +1064,22 @@
 tests/test_models/test_heads/test_decode_head.py
 tests/test_models/test_heads/test_dm_head.py
 tests/test_models/test_heads/test_dnl_head.py
 tests/test_models/test_heads/test_dpt_head.py
 tests/test_models/test_heads/test_ema_head.py
 tests/test_models/test_heads/test_fcn_head.py
 tests/test_models/test_heads/test_gc_head.py
+tests/test_models/test_heads/test_ham_head.py
 tests/test_models/test_heads/test_isa_head.py
 tests/test_models/test_heads/test_lraspp_head.py
 tests/test_models/test_heads/test_mask2former_head.py
 tests/test_models/test_heads/test_maskformer_head.py
 tests/test_models/test_heads/test_nl_head.py
 tests/test_models/test_heads/test_ocr_head.py
+tests/test_models/test_heads/test_pidnet_head.py
 tests/test_models/test_heads/test_psa_head.py
 tests/test_models/test_heads/test_psp_head.py
 tests/test_models/test_heads/test_segformer_head.py
 tests/test_models/test_heads/test_segmenter_mask_head.py
 tests/test_models/test_heads/test_setr_mla_head.py
 tests/test_models/test_heads/test_setr_up_head.py
 tests/test_models/test_heads/test_uper_head.py
```

### Comparing `mmsegmentation-1.0.0rc6/setup.cfg` & `mmsegmentation-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 no_lines_before = STDLIB,LOCALFOLDER
 default_section = THIRDPARTY
 
 [codespell]
 skip = *.po,*.ts,*.ipynb
 count = 
 quiet-level = 3
-ignore-words-list = formating,sur,hist,dota,warmup
+ignore-words-list = formating,sur,hist,dota,warmup,damon
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mmsegmentation-1.0.0rc6/setup.py` & `mmsegmentation-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         # installed by `pip install .`
         # or create source distribution by `python setup.py sdist`
         # set `copy` mode here since symlink fails with WinError on Windows.
         mode = 'copy'
     else:
         return
 
-    filenames = ['tools', 'configs', 'model-index.yml']
+    filenames = ['tools', 'configs', 'model-index.yml', 'dataset-index.yml']
     repo_path = osp.dirname(__file__)
     mim_path = osp.join(repo_path, 'mmseg', '.mim')
     os.makedirs(mim_path, exist_ok=True)
 
     for filename in filenames:
         if osp.exists(filename):
             src_path = osp.join(repo_path, filename)
@@ -171,15 +171,15 @@
         version=get_version(),
         description='Open MMLab Semantic Segmentation Toolbox and Benchmark',
         long_description=readme(),
         long_description_content_type='text/markdown',
         author='MMSegmentation Contributors',
         author_email='openmmlab@gmail.com',
         keywords='computer vision, semantic segmentation',
-        url='http://github.com/open-mmlab/mmsegmentation',
+        url='https://github.com/open-mmlab/mmsegmentation',
         packages=find_packages(exclude=('configs', 'tools', 'demo')),
         include_package_data=True,
         classifiers=[
             'Development Status :: 4 - Beta',
             'License :: OSI Approved :: Apache Software License',
             'Operating System :: OS Independent',
             'Programming Language :: Python :: 3.6',
```

### Comparing `mmsegmentation-1.0.0rc6/tests/test_config.py` & `mmsegmentation-1.1.0/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,19 @@
 
         # remove loading pipeline
         load_img_pipeline = config_mod.train_pipeline.pop(0)
         to_float32 = load_img_pipeline.get('to_float32', False)
         del config_mod.train_pipeline[0]
         del config_mod.test_pipeline[0]
         # remove loading annotation in test pipeline
-        del config_mod.test_pipeline[-2]
+        load_anno_idx = -1
+        for i in range(len(config_mod.test_pipeline)):
+            if config_mod.test_pipeline[i].type == 'LoadAnnotations':
+                load_anno_idx = i
+        del config_mod.test_pipeline[load_anno_idx]
 
         train_pipeline = Compose(config_mod.train_pipeline)
         test_pipeline = Compose(config_mod.test_pipeline)
 
         img = np.random.randint(0, 255, size=(1024, 2048, 3), dtype=np.uint8)
         if to_float32:
             img = img.astype(np.float32)
@@ -106,30 +110,35 @@
             filename='test_img.png',
             ori_filename='test_img.png',
             img=img,
             img_shape=img.shape,
             ori_shape=img.shape,
             gt_seg_map=seg)
         results['seg_fields'] = ['gt_seg_map']
-
+        _check_concat_cd_input(config_mod, results)
         print(f'Test training data pipeline: \n{train_pipeline!r}')
         output_results = train_pipeline(results)
         assert output_results is not None
 
-        results = dict(
-            filename='test_img.png',
-            ori_filename='test_img.png',
-            img=img,
-            img_shape=img.shape,
-            ori_shape=img.shape)
+        _check_concat_cd_input(config_mod, results)
         print(f'Test testing data pipeline: \n{test_pipeline!r}')
         output_results = test_pipeline(results)
         assert output_results is not None
 
 
+def _check_concat_cd_input(config_mod: Config, results: dict):
+    keys = []
+    pipeline = config_mod.train_pipeline.copy()
+    pipeline.extend(config_mod.test_pipeline)
+    for t in pipeline:
+        keys.append(t.type)
+    if 'ConcatCDInput' in keys:
+        results.update({'img2': results['img']})
+
+
 def _check_decode_head(decode_head_cfg, decode_head):
     if isinstance(decode_head_cfg, list):
         assert isinstance(decode_head, nn.ModuleList)
         assert len(decode_head_cfg) == len(decode_head)
         num_heads = len(decode_head)
         for i in range(num_heads):
             _check_decode_head(decode_head_cfg[i], decode_head[i])
```

### Comparing `mmsegmentation-1.0.0rc6/tests/test_digit_version.py` & `mmsegmentation-1.1.0/tests/test_digit_version.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_beit.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_beit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_bisenetv1.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_bisenetv2.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_blocks.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_blocks.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_cgnet.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_cgnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_erfnet.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_erfnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_fast_scnn.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_fast_scnn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_hrnet.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_hrnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_icnet.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_icnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_mae.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mae.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_mit.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_mobilenet_v3.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_resnest.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnest.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_resnet.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_resnext.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnext.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_stdc.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_stdc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_swin.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_swin.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_timm_backbone.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_timm_backbone.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_twins.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_twins.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_unet.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_unet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/test_vit.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_vit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_backbones/utils.py` & `mmsegmentation-1.1.0/tests/test_models/test_backbones/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_data_preprocessor.py` & `mmsegmentation-1.1.0/tests/test_models/test_data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_forward.py` & `mmsegmentation-1.1.0/tests/test_models/test_forward.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_ann_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ann_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_apc_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_apc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_aspp_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_aspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_cc_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_cc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_decode_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_decode_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_dm_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_dm_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_dnl_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_dnl_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_dpt_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_dpt_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_ema_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ema_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_fcn_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_fcn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_isa_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_isa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_lraspp_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_lraspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_mask2former_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_mask2former_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_maskformer_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_maskformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_ocr_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ocr_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_psa_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_psa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_psp_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_psp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_segformer_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_segformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_segmenter_mask_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_segmenter_mask_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_setr_mla_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_mla_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_setr_up_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_up_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/test_uper_head.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/test_uper_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_heads/utils.py` & `mmsegmentation-1.1.0/tests/test_models/test_heads/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_feature2pyramid.py` & `mmsegmentation-1.1.0/tests/test_models/test_necks/test_feature2pyramid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_fpn.py` & `mmsegmentation-1.1.0/tests/test_models/test_necks/test_fpn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_ic_neck.py` & `mmsegmentation-1.1.0/tests/test_models/test_necks/test_ic_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_jpu.py` & `mmsegmentation-1.1.0/tests/test_models/test_necks/test_jpu.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_mla_neck.py` & `mmsegmentation-1.1.0/tests/test_models/test_necks/test_mla_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_necks/test_multilevel_neck.py` & `mmsegmentation-1.1.0/tests/test_models/test_necks/test_multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py` & `mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/test_encoder_decoder.py` & `mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/test_seg_tta_model.py` & `mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_seg_tta_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import tempfile
+
 import torch
 from mmengine import ConfigDict
 from mmengine.model import BaseTTAModel
 from mmengine.registry import init_default_scope
 from mmengine.structures import PixelData
 
 from mmseg.registry import MODELS
@@ -33,15 +35,16 @@
         imgs.append(torch.randn(1, 3, 10 + i, 10 + i))
         data_samples.append([
             SegDataSample(
                 metainfo=dict(
                     ori_shape=(10, 10),
                     img_shape=(10 + i, 10 + i),
                     flip=(i % 2 == 0),
-                    flip_direction=flip_direction),
+                    flip_direction=flip_direction,
+                    img_path=tempfile.mktemp()),
                 gt_sem_seg=PixelData(data=torch.randint(0, 19, (1, 10, 10))))
         ])
 
     model.test_step(dict(inputs=imgs, data_samples=data_samples))
 
     # test out_channels == 1
     segmentor_cfg = ConfigDict(
```

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_segmentors/utils.py` & `mmsegmentation-1.1.0/tests/test_models/test_segmentors/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_utils/test_embed.py` & `mmsegmentation-1.1.0/tests/test_models/test_utils/test_embed.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_models/test_utils/test_shape_convert.py` & `mmsegmentation-1.1.0/tests/test_models/test_utils/test_shape_convert.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.0.0rc6/tests/test_sampler.py` & `mmsegmentation-1.1.0/tests/test_sampler.py`

 * *Files identical despite different names*

