# Comparing `tmp/mmdet3d-1.1.1.tar.gz` & `tmp/mmdet3d-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmdet3d-1.1.1.tar", last modified: Wed May 31 07:58:38 2023, max compression
+gzip compressed data, was "dist/mmdet3d-1.2.0.tar", last modified: Tue Jul  4 15:52:49 2023, max compression
```

## Comparing `mmdet3d-1.1.1.tar` & `mmdet3d-1.2.0.tar`

### file list

```diff
@@ -1,661 +1,665 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19598 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/3dssd/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/3dssd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/3dssd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/cylinder3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/fcaf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/fcos3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/groupfree3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/h3dnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/imvotenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/minkunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/paconv_ssg-cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/parta2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/point_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/spvcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/votenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/cylinder3d_4xb4-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/cylinder3d_8xb2-laser-polar-mix-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dfm/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcos3d/
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d_finetune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/fcos3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/h3dnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/h3dnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_2xb4_sunrgbd-3d-10class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet18_w16_torchsparse_8xb2-amp-15e_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet18_w20_torchsparse_8xb2-amp-15e_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet18_w32_torchsparse_8xb2-amp-15e_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34_w32_minkowski_8xb2-laser-polar-mix-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34_w32_spconv_8xb2-amp-laser-polar-mix-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34_w32_spconv_8xb2-laser-polar-mix-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34_w32_torchsparse_8xb2-amp-laser-polar-mix-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34_w32_torchsparse_8xb2-laser-polar-mix-3x_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34v2_w32_torchsparse_8xb2-amp-laser-polar-mix-3x_semantickitti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/monoflex/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/monoflex/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/mvxnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/mvxnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn-r50-fpn_coco-20e_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r101_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_coco-20e-1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_x101_32x4d_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e-1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r101_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_x101_32x4d_fpn_1x_nuim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d_finetune.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d_finetune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/point_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/point_rcnn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d-range100.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-amp-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-amp-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pv_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pv_rcnn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/sassd/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-3class.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-car.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/smoke/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/smoke/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/spvcnn_w16_8xb2-amp-15e_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/spvcnn_w20_8xb2-amp-15e_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-15e_semantickitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-laser-polar-mix-3x_semantickitti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/votenet_head-iouloss_8xb8_scannet-3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/get_flops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/create_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/create_data.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24939 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24694 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/semantickitti_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49931 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25658 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/test_torchserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/dist_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/print_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/visualize_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/publish_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/slurm_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/update_data_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/.mim/tools/update_data_coords.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/base_3d_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/lidar_det3d_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/lidar_seg3d_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/mono_det3d_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/apis/inferencers/multi_modality_det3d_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/det3d_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/kitti2d_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/kitti_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/lyft_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/nuscenes_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/s3dis_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/scannet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/seg3d_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/semantickitti_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/sunrgbd_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/data_augment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/dbsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)    51869 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)   102784 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/transforms/transforms_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/datasets/waymo_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/engine/hooks/benchmark_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/engine/hooks/disable_object_sample_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/indoor_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/instance_seg_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/kitti_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/kitti_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/kitti_utils/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/lyft_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/panoptic_seg_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/scannet_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/scannet_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/scannet_utils/util_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/seg_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/waymo_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/waymo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/indoor_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/instance_seg_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    28517 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/kitti_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/lyft_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    32405 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/nuscenes_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/panoptic_seg_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/seg_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/evaluation/metrics/waymo_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/base_pointnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/cylinder3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/dla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/mink_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/minkunet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/multi_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/nostem_regnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/pointnet2_sa_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/pointnet2_sa_ssg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/second.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/backbones/spvcnn_backone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/cylinder3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/dgcnn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/minkunet_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/paconv_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/decode_heads/pointnet2_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18722 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/anchor3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/base_3d_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/base_conv_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/base_mono3d_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    37182 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/centerpoint_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    29966 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/fcaf3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/fcos_mono3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/free_anchor3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    47808 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/groupfree3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/imvoxel_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    36543 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/monoflex_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/parta2_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    59511 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/pgd_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/point_rpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    22790 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/shape_aware_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/smoke_mono3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/ssd_3d_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/train_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/dense_heads/vote_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/centerpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/dfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/dynamic_voxelnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/fcos_mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/groupfree3dnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/h3dnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23036 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/imvotenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/imvoxelnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/mink_single_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/multiview_dfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/mvx_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/mvx_two_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/parta2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/point_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/pv_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/sassd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/single_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/single_stage_mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/smoke_mono3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/ssd3dnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/two_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/votenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/detectors/voxelnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/box3d_nms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/edge_fusion_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/coord_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/point_fusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/vote_fusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/minkowski_engine_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/paconv/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/paconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/paconv/paconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/paconv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/point_fp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/point_sa_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/sparse_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/spconv/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/spconv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/spconv/overwrite_spconv/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/spconv/overwrite_spconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/layers/torchsparse/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/torchsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/torchsparse/torchsparse_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/torchsparse_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/layers/vote_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/axis_aligned_iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/multibin_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/paconv_regularization_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/rotated_iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/losses/uncertain_smooth_l1_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/middle_encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/middle_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/middle_encoders/pillar_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/middle_encoders/sparse_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/middle_encoders/sparse_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/middle_encoders/voxel_set_abstraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/necks/dla_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/necks/imvoxel_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/necks/pointnet2_fp_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/necks/second_fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/base_3droi_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42934 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    26660 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/h3d_roi_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    46441 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/primitive_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/part_aggregation_roi_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/point_rcnn_roi_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/cylinder3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/minkunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/segmentors/seg3d_tta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/assigners/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/pseudosample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/voxel/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/task_modules/voxel/voxel_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/test_time_augs/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/test_time_augs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/test_time_augs/merge_augs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/add_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/clip_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/edge_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/gen_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/utils/handle_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/pillar_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/voxel_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/base_box3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/box_3d_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/cam_box3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/coord_3d_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/depth_box3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/lidar_box3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/det3d_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/structures/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30923 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/ops/box_np_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/ops/iou3d_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/ops/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/point_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/structures/points/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/points/base_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/points/cam_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/points/depth_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/structures/points/lidar_points.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/testing/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/testing/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14155 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/array_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/compat_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/utils/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44177 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/visualization/local_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/mmdet3d/visualization/vis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30357 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/mmdet3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 07:58:38.000000 mmdet3d-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-31 07:57:16.000000 mmdet3d-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/3dssd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/3dssd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/3dssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/cylinder3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/fcaf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/fcos3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/groupfree3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/h3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/imvotenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/minkunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/paconv_ssg-cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/parta2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/point_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/spvcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/votenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn-circlenms_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_head-dcn_8xb4-cyclic-20e_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/cylinder3d_4xb4-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/cylinder3d_8xb2-laser-polar-mix-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dfm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcos3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/fcos3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/h3dnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/h3dnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_2xb4_sunrgbd-3d-10class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet18_w16_torchsparse_8xb2-amp-15e_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet18_w20_torchsparse_8xb2-amp-15e_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet18_w32_torchsparse_8xb2-amp-15e_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34_w32_minkowski_8xb2-laser-polar-mix-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34_w32_spconv_8xb2-amp-laser-polar-mix-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34_w32_spconv_8xb2-laser-polar-mix-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34_w32_torchsparse_8xb2-amp-laser-polar-mix-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34_w32_torchsparse_8xb2-laser-polar-mix-3x_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34v2_w32_torchsparse_8xb2-amp-laser-polar-mix-3x_semantickitti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/monoflex/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/monoflex/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/mvxnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/mvxnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn-r50-fpn_coco-20e_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r101_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_coco-20e-1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_x101_32x4d_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e-1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_coco-20e_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r101_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_x101_32x4d_fpn_1x_nuim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-2x_nus-mono3d_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/point_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/point_rcnn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d-range100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb2-amp-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_fpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-amp-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pv_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pv_rcnn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/sassd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-3class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-amp-80e_kitti-3d-car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/smoke/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/smoke/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/spvcnn_w16_8xb2-amp-15e_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/spvcnn_w20_8xb2-amp-15e_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-15e_semantickitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-laser-polar-mix-3x_semantickitti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/votenet_head-iouloss_8xb8_scannet-3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d/.mim/dataset-index.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/get_flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/create_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/create_data.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24939 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      401 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/kitti_unzip.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24694 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/nuscenes_unzip.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/semantickitti_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/semantickitti_unzip.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49931 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25658 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/test_torchserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/dist_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/print_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/visualize_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/publish_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/slurm_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/update_data_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 15:51:28.000000 mmdet3d-1.2.0/mmdet3d/.mim/tools/update_data_coords.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/base_3d_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/lidar_det3d_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/lidar_seg3d_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/mono_det3d_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/apis/inferencers/multi_modality_det3d_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/det3d_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/kitti2d_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/kitti_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/lyft_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/nuscenes_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/s3dis_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/scannet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/seg3d_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/semantickitti_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/sunrgbd_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/data_augment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/dbsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52466 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102784 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/transforms/transforms_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/datasets/waymo_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/engine/hooks/benchmark_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/engine/hooks/disable_object_sample_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/indoor_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/instance_seg_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/kitti_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/kitti_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/kitti_utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/lyft_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/panoptic_seg_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/scannet_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/scannet_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/scannet_utils/util_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/seg_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/waymo_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/waymo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/indoor_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/instance_seg_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28517 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/kitti_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/lyft_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32405 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/nuscenes_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/panoptic_seg_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/seg_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/evaluation/metrics/waymo_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/base_pointnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/cylinder3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/dla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/mink_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/minkunet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/multi_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/nostem_regnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/pointnet2_sa_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/pointnet2_sa_ssg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/second.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/backbones/spvcnn_backone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/cylinder3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/dgcnn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/minkunet_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/paconv_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/decode_heads/pointnet2_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18722 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/anchor3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/base_3d_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/base_conv_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/base_mono3d_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37182 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/centerpoint_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29966 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/fcaf3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/fcos_mono3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/free_anchor3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47808 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/groupfree3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/imvoxel_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36543 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/monoflex_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/parta2_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59511 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/pgd_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/point_rpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22790 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/shape_aware_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/smoke_mono3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25624 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/ssd_3d_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/train_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/dense_heads/vote_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/centerpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/dfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/dynamic_voxelnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/fcos_mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/groupfree3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/h3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23036 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/imvotenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/imvoxelnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/mink_single_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/multiview_dfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/mvx_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/mvx_two_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/parta2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/point_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/pv_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/sassd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/single_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/single_stage_mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/smoke_mono3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/ssd3dnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/two_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/votenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/detectors/voxelnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/box3d_nms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/edge_fusion_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/coord_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/point_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/vote_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/minkowski_engine_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/paconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/paconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/paconv/paconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/paconv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/point_fp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/point_sa_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/sparse_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/spconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/spconv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/spconv/overwrite_spconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/spconv/overwrite_spconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/layers/torchsparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/torchsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/torchsparse/torchsparse_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/torchsparse_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/layers/vote_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/axis_aligned_iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/chamfer_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/multibin_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/paconv_regularization_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/rotated_iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/losses/uncertain_smooth_l1_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/middle_encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/middle_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/middle_encoders/pillar_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/middle_encoders/sparse_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/middle_encoders/sparse_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/middle_encoders/voxel_set_abstraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/necks/dla_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/necks/imvoxel_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/necks/pointnet2_fp_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/necks/second_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/base_3droi_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42934 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26660 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/h3d_roi_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46441 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/primitive_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/part_aggregation_roi_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/point_rcnn_roi_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/cylinder3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/minkunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/segmentors/seg3d_tta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/assigners/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/pseudosample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/voxel/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/task_modules/voxel/voxel_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/test_time_augs/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/test_time_augs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/test_time_augs/merge_augs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/add_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/clip_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/edge_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/gen_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/utils/handle_objs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/pillar_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/voxel_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/base_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/box_3d_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/cam_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/coord_3d_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/depth_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/lidar_box3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/det3d_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/structures/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30923 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/ops/box_np_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/ops/iou3d_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/ops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/point_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/structures/points/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/points/base_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/points/cam_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/points/depth_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/structures/points/lidar_points.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/testing/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/testing/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14155 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/array_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/compat_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/utils/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49588 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/visualization/local_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/mmdet3d/visualization/vis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30558 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/mmdet3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 15:52:48.000000 mmdet3d-1.2.0/mmdet3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-04 15:52:49.000000 mmdet3d-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-04 15:51:27.000000 mmdet3d-1.2.0/setup.py
```

### Comparing `mmdet3d-1.1.1/PKG-INFO` & `mmdet3d-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,354 +1,399 @@
-Metadata-Version: 2.1
-Name: mmdet3d
-Version: 1.1.1
-Summary: OpenMMLab's next-generation platformfor general 3D object detection.
-Home-page: https://github.com/open-mmlab/mmdetection3d
-Author: MMDetection3D Contributors
-Author-email: zwwdev@gmail.com
-License: Apache License 2.0
-Description: <div align="center">
-          <img src="resources/mmdet3d-logo.png" width="600"/>
-          <div>&nbsp;</div>
-          <div align="center">
-            <b><font size="5">OpenMMLab website</font></b>
-            <sup>
-              <a href="https://openmmlab.com">
-                <i><font size="4">HOT</font></i>
-              </a>
-            </sup>
-            &nbsp;&nbsp;&nbsp;&nbsp;
-            <b><font size="5">OpenMMLab platform</font></b>
-            <sup>
-              <a href="https://platform.openmmlab.com">
-                <i><font size="4">TRY IT OUT</font></i>
-              </a>
-            </sup>
-          </div>
-          <div>&nbsp;</div>
-        
-        [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/latest/)
-        [![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
-        [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
-        [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/LICENSE)
-        
-        </div>
-        
-        </div>
-        
-        <div align="center">
-          <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://discord.com/channels/1037617289144569886/1046608014234370059" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
-        </div>
-        
-        **News**:
-        
-        **We have renamed the branch `1.1`  to `main` and switched the default branch from `master` to `main`. We encourage
-        users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](docs/en/migration.md) for more details.**
-        
-        **v1.1.1** was released in 30/5/2023
-        
-        We have constructed a comprehensive LiDAR semantic segmentation benchmark on SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy, the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of SemanticKITTI. We have also supported the training of BEVFusion and an occupancy prediction method, TPVFomrer, in our `projects`. More new features about 3D perception are on the way. Please stay tuned!
-        
-        ## Introduction
-        
-        English | [简体中文](README_zh-CN.md)
-        
-        The main branch works with **PyTorch 1.8+**.
-        
-        MMDetection3D is an open source object detection toolbox based on PyTorch, towards the next-generation platform for general 3D detection. It is
-        a part of the OpenMMLab project developed by [MMLab](http://mmlab.ie.cuhk.edu.hk/).
-        
-        ![demo image](resources/mmdet3d_outdoor_demo.gif)
-        
-        ### Major features
-        
-        - **Support multi-modality/single-modality detectors out of box**
-        
-          It directly supports multi-modality/single-modality detectors including MVXNet, VoteNet, PointPillars, etc.
-        
-        - **Support indoor/outdoor 3D detection out of box**
-        
-          It directly supports popular indoor and outdoor 3D detection datasets, including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI.
-          For nuScenes dataset, we also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/nuimages).
-        
-        - **Natural integration with 2D detection**
-        
-          All the about **300+ models, methods of 40+ papers**, and modules supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
-        
-        - **High efficiency**
-        
-          It trains faster than other codebases. The main results are as below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the number of samples trained per second (the higher, the better). The models that are not supported by other codebases are marked by `✗`.
-        
-          |       Methods       | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) | [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://github.com/poodarchu/Det3D) |
-          | :-----------------: | :-----------: | :--------------------------------------------------: | :----------------------------------------------------: | :-----------------------------------------: |
-          |       VoteNet       |      358      |                          ✗                           |                           77                           |                      ✗                      |
-          |  PointPillars-car   |      141      |                          ✗                           |                           ✗                            |                     140                     |
-          | PointPillars-3class |      107      |                          44                          |                           ✗                            |                      ✗                      |
-          |       SECOND        |      40       |                          30                          |                           ✗                            |                      ✗                      |
-          |       Part-A2       |      17       |                          14                          |                           ✗                            |                      ✗                      |
-        
-        Like [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to support different projects on top of it.
-        
-        ## License
-        
-        This project is released under the [Apache 2.0 license](LICENSE).
-        
-        ## Changelog
-        
-        **1.1.0** was released in 6/4/2023.
-        
-        Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
-        
-        ## Benchmark and model zoo
-        
-        Results and models are available in the [model zoo](docs/en/model_zoo.md).
-        
-        <div align="center">
-          <b>Components</b>
-        </div>
-        <table align="center">
-          <tbody>
-            <tr align="center" valign="bottom">
-              <td>
-                <b>Backbones</b>
-              </td>
-              <td>
-                <b>Heads</b>
-              </td>
-              <td>
-                <b>Features</b>
-              </td>
-            </tr>
-            <tr valign="top">
-              <td>
-              <ul>
-                <li><a href="configs/pointnet2">PointNet (CVPR'2017)</a></li>
-                <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
-                <li><a href="configs/regnet">RegNet (CVPR'2020)</a></li>
-                <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
-                <li>DLA (CVPR'2018)</li>
-                <li>MinkResNet (CVPR'2019)</li>
-                <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
-                <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
-              </ul>
-              </td>
-              <td>
-              <ul>
-                <li><a href="configs/free_anchor">FreeAnchor (NeurIPS'2019)</a></li>
-              </ul>
-              </td>
-              <td>
-              <ul>
-                <li><a href="configs/dynamic_voxelization">Dynamic Voxelization (CoRL'2019)</a></li>
-              </ul>
-              </td>
-            </tr>
-        </td>
-            </tr>
-          </tbody>
-        </table>
-        
-        <div align="center">
-          <b>Architectures</b>
-        </div>
-        <table align="center">
-          <tbody>
-            <tr align="center" valign="middle">
-              <td>
-                <b>3D Object Detection</b>
-              </td>
-              <td>
-                <b>Monocular 3D Object Detection</b>
-              </td>
-              <td>
-                <b>Multi-modal 3D Object Detection</b>
-              </td>
-              <td>
-                <b>3D Semantic Segmentation</b>
-              </td>
-            </tr>
-            <tr valign="top">
-              <td>
-                <li><b>Outdoor</b></li>
-                <ul>
-                    <li><a href="configs/second">SECOND (Sensor'2018)</a></li>
-                    <li><a href="configs/pointpillars">PointPillars (CVPR'2019)</a></li>
-                    <li><a href="configs/ssn">SSN (ECCV'2020)</a></li>
-                    <li><a href="configs/3dssd">3DSSD (CVPR'2020)</a></li>
-                    <li><a href="configs/sassd">SA-SSD (CVPR'2020)</a></li>
-                    <li><a href="configs/point_rcnn">PointRCNN (CVPR'2019)</a></li>
-                    <li><a href="configs/parta2">Part-A2 (TPAMI'2020)</a></li>
-                    <li><a href="configs/centerpoint">CenterPoint (CVPR'2021)</a></li>
-                    <li><a href="configs/pv_rcnn">PV-RCNN (CVPR'2020)</a></li>
-                </ul>
-                <li><b>Indoor</b></li>
-                <ul>
-                    <li><a href="configs/votenet">VoteNet (ICCV'2019)</a></li>
-                    <li><a href="configs/h3dnet">H3DNet (ECCV'2020)</a></li>
-                    <li><a href="configs/groupfree3d">Group-Free-3D (ICCV'2021)</a></li>
-                    <li><a href="configs/fcaf3d">FCAF3D (ECCV'2022)</a></li>
-              </ul>
-              </td>
-              <td>
-                <li><b>Outdoor</b></li>
-                <ul>
-                  <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
-                  <li><a href="configs/smoke">SMOKE (CVPRW'2020)</a></li>
-                  <li><a href="configs/fcos3d">FCOS3D (ICCVW'2021)</a></li>
-                  <li><a href="configs/pgd">PGD (CoRL'2021)</a></li>
-                  <li><a href="configs/monoflex">MonoFlex (CVPR'2021)</a></li>
-                </ul>
-                <li><b>Indoor</b></li>
-                <ul>
-                  <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
-                </ul>
-              </td>
-              <td>
-                <li><b>Outdoor</b></li>
-                <ul>
-                  <li><a href="configs/mvxnet">MVXNet (ICRA'2019)</a></li>
-                </ul>
-                <li><b>Indoor</b></li>
-                <ul>
-                  <li><a href="configs/imvotenet">ImVoteNet (CVPR'2020)</a></li>
-                </ul>
-              </td>
-              <td>
-                <li><b>Outdoor</b></li>
-                <ul>
-                  <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
-                  <li><a href="configs/spvcnn">SPVCNN (ECCV'2020)</a></li>
-                  <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
-                </ul>
-                <li><b>Indoor</b></li>
-                <ul>
-                  <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
-                  <li><a href="configs/paconv">PAConv (CVPR'2021)</a></li>
-                  <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
-                </ul>
-              </ul>
-              </td>
-            </tr>
-        </td>
-            </tr>
-          </tbody>
-        </table>
-        
-        |               | ResNet | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet | Cylinder3D | MinkUNet |
-        | :-----------: | :----: | :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :------: |
-        |    SECOND     |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        | PointPillars  |   ✗    |     ✗      |   ✓    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  FreeAnchor   |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    VoteNet    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    H3DNet     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |     3DSSD     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    Part-A2    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    MVXNet     |   ✓    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  CenterPoint  |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |      SSN      |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |   ImVoteNet   |   ✓    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    FCOS3D     |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  PointNet++   |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        | Group-Free-3D |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  ImVoxelNet   |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    PAConv     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |     DGCNN     |   ✗    |     ✗      |   ✗    |   ✓   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |     SMOKE     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
-        |      PGD      |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |   MonoFlex    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
-        |    SA-SSD     |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    FCAF3D     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
-        |    PV-RCNN    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  Cylinder3D   |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✓      |    ✗     |
-        |   MinkUNet    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
-        |    SPVCNN     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
-        
-        **Note:** All the about **300+ models, methods of 40+ papers** in 2D detection supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
-        
-        ## Installation
-        
-        Please refer to [get_started.md](docs/en/get_started.md) for installation.
-        
-        ## Get Started
-        
-        Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMDetection3D. We provide guidance for quick run [with existing dataset](docs/en/user_guides/train_test.md) and [with new dataset](docs/en/user_guides/2_new_data_model.md) for beginners. There are also tutorials for [learning configuration systems](docs/en/user_guides/config.md), [customizing dataset](docs/en/advanced_guides/customize_dataset.md), [designing data pipeline](docs/en/user_guides/data_pipeline.md), [customizing models](docs/en/advanced_guides/customize_models.md), [customizing runtime settings](docs/en/advanced_guides/customize_runtime.md) and [Waymo dataset](docs/en/advanced_guides/datasets/waymo_det.md).
-        
-        Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions. When updating the version of MMDetection3D, please also check the [compatibility doc](docs/en/notes/compatibility.md) to be aware of the BC-breaking updates introduced in each version.
-        
-        ## Citation
-        
-        If you find this project useful in your research, please consider cite:
-        
-        ```latex
-        @misc{mmdet3d2020,
-            title={{MMDetection3D: OpenMMLab} next-generation platform for general {3D} object detection},
-            author={MMDetection3D Contributors},
-            howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}},
-            year={2020}
-        }
-        ```
-        
-        ## Contributing
-        
-        We appreciate all contributions to improve MMDetection3D. Please refer to [CONTRIBUTING.md](./docs/en/notes/contribution_guides.md) for the contributing guideline.
-        
-        ## Acknowledgement
-        
-        MMDetection3D is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors as well as users who give valuable feedbacks.
-        We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and develop their own new 3D detectors.
-        
-        ## Projects in OpenMMLab
-        
-        - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
-        - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
-        - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-        - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-        - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
-        - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-        - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
-        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-        - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-        - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-        - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-        - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
-        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
-        - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
-        
-Keywords: computer vision,3D object detection
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: tests
-Provides-Extra: build
-Provides-Extra: optional
-Provides-Extra: mim
+<div align="center">
+  <img src="resources/mmdet3d-logo.png" width="600"/>
+  <div>&nbsp;</div>
+  <div align="center">
+    <b><font size="5">OpenMMLab website</font></b>
+    <sup>
+      <a href="https://openmmlab.com">
+        <i><font size="4">HOT</font></i>
+      </a>
+    </sup>
+    &nbsp;&nbsp;&nbsp;&nbsp;
+    <b><font size="5">OpenMMLab platform</font></b>
+    <sup>
+      <a href="https://platform.openmmlab.com">
+        <i><font size="4">TRY IT OUT</font></i>
+      </a>
+    </sup>
+  </div>
+  <div>&nbsp;</div>
+
+[![PyPI](https://img.shields.io/pypi/v/mmdet3d)](https://pypi.org/project/mmdet3d)
+[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/latest/)
+[![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
+[![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
+[![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/main/LICENSE)
+[![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+[![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+
+[📘Documentation](https://mmdetection3d.readthedocs.io/en/latest/) |
+[🛠️Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html) |
+[👀Model Zoo](https://mmdetection3d.readthedocs.io/en/latest/model_zoo.html) |
+[🆕Update News](https://mmdetection3d.readthedocs.io/en/latest/notes/changelog.html) |
+[🚀Ongoing Projects](https://github.com/open-mmlab/mmdetection3d/projects) |
+[🤔Reporting Issues](https://github.com/open-mmlab/mmdetection3d/issues/new/choose)
+
+</div>
+
+<div align="center">
+
+English | [简体中文](README_zh-CN.md)
+
+</div>
+
+<div align="center">
+  <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://discord.com/channels/1037617289144569886/1046608014234370059" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
+</div>
+
+## Introduction
+
+MMDetection3D is an open source object detection toolbox based on PyTorch, towards the next-generation platform for general 3D detection. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
+
+The main branch works with **PyTorch 1.8+**.
+
+![demo image](resources/mmdet3d_outdoor_demo.gif)
+
+<details open>
+<summary>Major features</summary>
+
+- **Support multi-modality/single-modality detectors out of box**
+
+  It directly supports multi-modality/single-modality detectors including MVXNet, VoteNet, PointPillars, etc.
+
+- **Support indoor/outdoor 3D detection out of box**
+
+  It directly supports popular indoor and outdoor 3D detection datasets, including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes dataset, we also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/nuimages).
+
+- **Natural integration with 2D detection**
+
+  All the about **300+ models, methods of 40+ papers**, and modules supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
+
+- **High efficiency**
+
+  It trains faster than other codebases. The main results are as below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the number of samples trained per second (the higher, the better). The models that are not supported by other codebases are marked by `✗`.
+
+  |       Methods       | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) | [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://github.com/poodarchu/Det3D) |
+  | :-----------------: | :-----------: | :--------------------------------------------------: | :----------------------------------------------------: | :-----------------------------------------: |
+  |       VoteNet       |      358      |                          ✗                           |                           77                           |                      ✗                      |
+  |  PointPillars-car   |      141      |                          ✗                           |                           ✗                            |                     140                     |
+  | PointPillars-3class |      107      |                          44                          |                           ✗                            |                      ✗                      |
+  |       SECOND        |      40       |                          30                          |                           ✗                            |                      ✗                      |
+  |       Part-A2       |      17       |                          14                          |                           ✗                            |                      ✗                      |
+
+</details>
+
+Like [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to support different projects on top of it.
+
+## What's New
+
+### Highlight
+
+**We have renamed the branch `1.1` to `main` and switched the default branch from `master` to `main`. We encourage users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](docs/en/migration.md) for more details.**
+
+We have constructed a comprehensive LiDAR semantic segmentation benchmark on SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy, the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of SemanticKITTI. We have also supported the training of BEVFusion and an occupancy prediction method, TPVFomrer, in our `projects`. More new features about 3D perception are on the way. Please stay tuned!
+
+**v1.2.0** was released in 4/7/2023
+
+- Support [New Config Type](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) in `mmdet3d/config`
+- Support the inference of [DSVT](<(https://arxiv.org/abs/2301.06051)>) in `projects`
+- Support downloading datasets from [OpenDataLab](https://opendatalab.com/) using `mim`
+
+**v1.1.1** was released in 30/5/2023:
+
+- Support [TPVFormer](https://arxiv.org/pdf/2302.07817.pdf) in `projects`
+- Support the training of BEVFusion in `projects`
+- Support lidar-based 3D semantic segmentation benchmark
+
+## Installation
+
+Please refer to [Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html) for installation instructions.
+
+## Getting Started
+
+For detailed user guides and advanced guides, please refer to our [documentation](https://mmdetection3d.readthedocs.io/en/latest/):
+
+<details>
+<summary>User Guides</summary>
+
+- [Train & Test](https://mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#train-test)
+  - [Learn about Configs](https://mmdetection3d.readthedocs.io/en/latest/user_guides/config.html)
+  - [Coordinate System](https://mmdetection3d.readthedocs.io/en/latest/user_guides/coord_sys_tutorial.html)
+  - [Dataset Preparation](https://mmdetection3d.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
+  - [Customize Data Pipelines](https://mmdetection3d.readthedocs.io/en/latest/user_guides/data_pipeline.html)
+  - [Test and Train on Standard Datasets](https://mmdetection3d.readthedocs.io/en/latest/user_guides/train_test.html)
+  - [Inference](https://mmdetection3d.readthedocs.io/en/latest/user_guides/inference.html)
+  - [Train with Customized Datasets](https://mmdetection3d.readthedocs.io/en/latest/user_guides/new_data_model.html)
+- [Useful Tools](https://mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#useful-tools)
+
+</details>
+
+<details>
+<summary>Advanced Guides</summary>
+
+- [Datasets](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#datasets)
+  - [KITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/kitti.html)
+  - [NuScenes Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/nuscenes.html)
+  - [Lyft Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/lyft.html)
+  - [Waymo Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/waymo.html)
+  - [SUN RGB-D Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/sunrgbd.html)
+  - [ScanNet Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/scannet.html)
+  - [S3DIS Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/s3dis.html)
+  - [SemanticKITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/semantickitti.html)
+- [Supported Tasks](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#supported-tasks)
+  - [LiDAR-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/lidar_det3d.html)
+  - [Vision-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/vision_det3d.html)
+  - [LiDAR-Based 3D Semantic Segmentation](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/lidar_sem_seg3d.html)
+- [Customization](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#customization)
+  - [Customize Datasets](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_dataset.html)
+  - [Customize Models](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_models.html)
+  - [Customize Runtime Settings](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_runtime.html)
+
+</details>
+
+## Overview of Benchmark and Model Zoo
+
+Results and models are available in the [model zoo](docs/en/model_zoo.md).
+
+<div align="center">
+  <b>Components</b>
+</div>
+<table align="center">
+  <tbody>
+    <tr align="center" valign="bottom">
+      <td>
+        <b>Backbones</b>
+      </td>
+      <td>
+        <b>Heads</b>
+      </td>
+      <td>
+        <b>Features</b>
+      </td>
+    </tr>
+    <tr valign="top">
+      <td>
+      <ul>
+        <li><a href="configs/pointnet2">PointNet (CVPR'2017)</a></li>
+        <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
+        <li><a href="configs/regnet">RegNet (CVPR'2020)</a></li>
+        <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
+        <li>DLA (CVPR'2018)</li>
+        <li>MinkResNet (CVPR'2019)</li>
+        <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
+        <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
+      </ul>
+      </td>
+      <td>
+      <ul>
+        <li><a href="configs/free_anchor">FreeAnchor (NeurIPS'2019)</a></li>
+      </ul>
+      </td>
+      <td>
+      <ul>
+        <li><a href="configs/dynamic_voxelization">Dynamic Voxelization (CoRL'2019)</a></li>
+      </ul>
+      </td>
+    </tr>
+</td>
+    </tr>
+  </tbody>
+</table>
+
+<div align="center">
+  <b>Architectures</b>
+</div>
+<table align="center">
+  <tbody>
+    <tr align="center" valign="middle">
+      <td>
+        <b>LiDAR-based 3D Object Detection</b>
+      </td>
+      <td>
+        <b>Camera-based 3D Object Detection</b>
+      </td>
+      <td>
+        <b>Multi-modal 3D Object Detection</b>
+      </td>
+      <td>
+        <b>3D Semantic Segmentation</b>
+      </td>
+    </tr>
+    <tr valign="top">
+      <td>
+        <li><b>Outdoor</b></li>
+        <ul>
+            <li><a href="configs/second">SECOND (Sensor'2018)</a></li>
+            <li><a href="configs/pointpillars">PointPillars (CVPR'2019)</a></li>
+            <li><a href="configs/ssn">SSN (ECCV'2020)</a></li>
+            <li><a href="configs/3dssd">3DSSD (CVPR'2020)</a></li>
+            <li><a href="configs/sassd">SA-SSD (CVPR'2020)</a></li>
+            <li><a href="configs/point_rcnn">PointRCNN (CVPR'2019)</a></li>
+            <li><a href="configs/parta2">Part-A2 (TPAMI'2020)</a></li>
+            <li><a href="configs/centerpoint">CenterPoint (CVPR'2021)</a></li>
+            <li><a href="configs/pv_rcnn">PV-RCNN (CVPR'2020)</a></li>
+            <li><a href="projects/CenterFormer">CenterFormer (ECCV'2022)</a></li>
+        </ul>
+        <li><b>Indoor</b></li>
+        <ul>
+            <li><a href="configs/votenet">VoteNet (ICCV'2019)</a></li>
+            <li><a href="configs/h3dnet">H3DNet (ECCV'2020)</a></li>
+            <li><a href="configs/groupfree3d">Group-Free-3D (ICCV'2021)</a></li>
+            <li><a href="configs/fcaf3d">FCAF3D (ECCV'2022)</a></li>
+            <li><a href="projects/TR3D">TR3D (ArXiv'2023)</a></li>
+      </ul>
+      </td>
+      <td>
+        <li><b>Outdoor</b></li>
+        <ul>
+          <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
+          <li><a href="configs/smoke">SMOKE (CVPRW'2020)</a></li>
+          <li><a href="configs/fcos3d">FCOS3D (ICCVW'2021)</a></li>
+          <li><a href="configs/pgd">PGD (CoRL'2021)</a></li>
+          <li><a href="configs/monoflex">MonoFlex (CVPR'2021)</a></li>
+          <li><a href="projects/DETR3D">DETR3D (CoRL'2021)</a></li>
+          <li><a href="projects/PETR">PETR (ECCV'2022)</a></li>
+        </ul>
+        <li><b>Indoor</b></li>
+        <ul>
+          <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
+        </ul>
+      </td>
+      <td>
+        <li><b>Outdoor</b></li>
+        <ul>
+          <li><a href="configs/mvxnet">MVXNet (ICRA'2019)</a></li>
+          <li><a href="projects/BEVFusion">BEVFusion (ICRA'2023)</a></li>
+        </ul>
+        <li><b>Indoor</b></li>
+        <ul>
+          <li><a href="configs/imvotenet">ImVoteNet (CVPR'2020)</a></li>
+        </ul>
+      </td>
+      <td>
+        <li><b>Outdoor</b></li>
+        <ul>
+          <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
+          <li><a href="configs/spvcnn">SPVCNN (ECCV'2020)</a></li>
+          <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
+          <li><a href="projects/TPVFormer">TPVFormer (CVPR'2023)</a></li>
+        </ul>
+        <li><b>Indoor</b></li>
+        <ul>
+          <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
+          <li><a href="configs/paconv">PAConv (CVPR'2021)</a></li>
+          <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
+        </ul>
+      </ul>
+      </td>
+    </tr>
+</td>
+    </tr>
+  </tbody>
+</table>
+
+|               | ResNet | VoVNet | Swin-T | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet | Cylinder3D | MinkUNet |
+| :-----------: | :----: | :----: | :----: | :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :------: |
+|    SECOND     |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+| PointPillars  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+|  FreeAnchor   |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    VoteNet    |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    H3DNet     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|     3DSSD     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    Part-A2    |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    MVXNet     |   ✓    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|  CenterPoint  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|      SSN      |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+|   ImVoteNet   |   ✓    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    FCOS3D     |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|  PointNet++   |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+| Group-Free-3D |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|  ImVoxelNet   |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    PAConv     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|     DGCNN     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✓   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|     SMOKE     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
+|      PGD      |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|   MonoFlex    |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
+|    SA-SSD     |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|    FCAF3D     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
+|    PV-RCNN    |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|  Cylinder3D   |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✓      |    ✗     |
+|   MinkUNet    |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+|    SPVCNN     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+|   BEVFusion   |   ✗    |   ✗    |   ✓    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+| CenterFormer  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|     TR3D      |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
+|    DETR3D     |   ✓    |   ✓    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|     PETR      |   ✗    |   ✓    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+|   TPVFormer   |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+
+**Note:** All the about **500+ models, methods of 90+ papers** in 2D detection supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
+
+## FAQ
+
+Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions.
+
+## Contributing
+
+We appreciate all contributions to improve MMDetection3D. Please refer to [CONTRIBUTING.md](docs/en/notes/contribution_guides.md) for the contributing guideline.
+
+## Acknowledgement
+
+MMDetection3D is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors as well as users who give valuable feedbacks. We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and develop their own new 3D detectors.
+
+## Citation
+
+If you find this project useful in your research, please consider cite:
+
+```latex
+@misc{mmdet3d2020,
+    title={{MMDetection3D: OpenMMLab} next-generation platform for general {3D} object detection},
+    author={MMDetection3D Contributors},
+    howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}},
+    year={2020}
+}
+```
+
+## License
+
+This project is released under the [Apache 2.0 license](LICENSE).
+
+## Projects in OpenMMLab
+
+- [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+- [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
+- [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
+- [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
+- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
+- [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
+- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
+- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
+- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
+- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
+- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
+- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
+- [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
+- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+- [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
```

#### html2text {}

```diff
@@ -1,171 +1,230 @@
-Metadata-Version: 2.1 Name: mmdet3d Version: 1.1.1 Summary: OpenMMLab's next-
-generation platformfor general 3D object detection. Home-page: https://
-github.com/open-mmlab/mmdetection3d Author: MMDetection3D Contributors Author-
-email: zwwdev@gmail.com License: Apache License 2.0 Description:
                          [resources/mmdet3d-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
-       [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
+  [![PyPI](https://img.shields.io/pypi/v/mmdet3d)](https://pypi.org/project/
+  mmdet3d) [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
   mmdetection3d.readthedocs.io/en/latest/) [![badge](https://github.com/open-
 mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/
      mmdetection3d/actions) [![codecov](https://codecov.io/gh/open-mmlab/
-mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
+ mmdetection3d/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
  mmdetection3d) [![license](https://img.shields.io/github/license/open-mmlab/
- mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/
-                                   LICENSE)
+  mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/main/
+  LICENSE) [![open issues](https://isitmaintained.com/badge/open/open-mmlab/
+  mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues) [!
+  [issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/
+   mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+    [ðDocumentation](https://mmdetection3d.readthedocs.io/en/latest/) |
+     [ð ï¸Installation](https://mmdetection3d.readthedocs.io/en/latest/
+ get_started.html) | [ðModel Zoo](https://mmdetection3d.readthedocs.io/en/
+              latest/model_zoo.html) | [ðUpdate News](https://
+  mmdetection3d.readthedocs.io/en/latest/notes/changelog.html) | [ðOngoing
+      Projects](https://github.com/open-mmlab/mmdetection3d/projects) |
+[ð¤Reporting Issues](https://github.com/open-mmlab/mmdetection3d/issues/new/
+                                    choose)
+                   English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-**News**: **We have renamed the branch `1.1` to `main` and switched the default
-branch from `master` to `main`. We encourage users to migrate to the latest
-version, though it comes with some cost. Please refer to [Migration Guide]
-(docs/en/migration.md) for more details.** **v1.1.1** was released in 30/5/2023
-We have constructed a comprehensive LiDAR semantic segmentation benchmark on
-SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy,
-the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of
-SemanticKITTI. We have also supported the training of BEVFusion and an
-occupancy prediction method, TPVFomrer, in our `projects`. More new features
-about 3D perception are on the way. Please stay tuned! ## Introduction English
-| [ç®ä½ä¸­æ](README_zh-CN.md) The main branch works with **PyTorch 1.8+**.
-MMDetection3D is an open source object detection toolbox based on PyTorch,
-towards the next-generation platform for general 3D detection. It is a part of
-the OpenMMLab project developed by [MMLab](http://mmlab.ie.cuhk.edu.hk/). !
-[demo image](resources/mmdet3d_outdoor_demo.gif) ### Major features - **Support
-multi-modality/single-modality detectors out of box** It directly supports
-multi-modality/single-modality detectors including MVXNet, VoteNet,
-PointPillars, etc. - **Support indoor/outdoor 3D detection out of box** It
-directly supports popular indoor and outdoor 3D detection datasets, including
-ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes dataset, we
-also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/
-tree/main/configs/nuimages). - **Natural integration with 2D detection** All
-the about **300+ models, methods of 40+ papers**, and modules supported in
-[MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/
-model_zoo.md) can be trained or used in this codebase. - **High efficiency** It
-trains faster than other codebases. The main results are as below. Details can
-be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the
-number of samples trained per second (the higher, the better). The models that
-are not supported by other codebases are marked by `â`. | Methods |
-MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) |
-[votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://
+## Introduction MMDetection3D is an open source object detection toolbox based
+on PyTorch, towards the next-generation platform for general 3D detection. It
+is a part of the [OpenMMLab](https://openmmlab.com/) project. The main branch
+works with **PyTorch 1.8+**. ![demo image](resources/mmdet3d_outdoor_demo.gif)
+Major features - **Support multi-modality/single-modality detectors out of
+box** It directly supports multi-modality/single-modality detectors including
+MVXNet, VoteNet, PointPillars, etc. - **Support indoor/outdoor 3D detection out
+of box** It directly supports popular indoor and outdoor 3D detection datasets,
+including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes
+dataset, we also support [nuImages dataset](https://github.com/open-mmlab/
+mmdetection3d/tree/main/configs/nuimages). - **Natural integration with 2D
+detection** All the about **300+ models, methods of 40+ papers**, and modules
+supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/
+docs/en/model_zoo.md) can be trained or used in this codebase. - **High
+efficiency** It trains faster than other codebases. The main results are as
+below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md).
+We compare the number of samples trained per second (the higher, the better).
+The models that are not supported by other codebases are marked by `â`. |
+Methods | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet)
+| [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://
 github.com/poodarchu/Det3D) | | :-----------------: | :-----------: | :--------
 ------------------------------------------: | :--------------------------------
 --------------------: | :-----------------------------------------: | | VoteNet
 | 358 | â | 77 | â | | PointPillars-car | 141 | â | â | 140 | |
 PointPillars-3class | 107 | 44 | â | â | | SECOND | 40 | 30 | â | â | |
-Part-A2 | 17 | 14 | â | â | Like [MMDetection](https://github.com/open-
+Part-A2 | 17 | 14 | â | â |  Like [MMDetection](https://github.com/open-
 mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv),
 MMDetection3D can also be used as a library to support different projects on
-top of it. ## License This project is released under the [Apache 2.0 license]
-(LICENSE). ## Changelog **1.1.0** was released in 6/4/2023. Please refer to
-[changelog.md](docs/en/notes/changelog.md) for details and release history. ##
-Benchmark and model zoo Results and models are available in the [model zoo]
-(docs/en/model_zoo.md).
+top of it. ## What's New ### Highlight **We have renamed the branch `1.1` to
+`main` and switched the default branch from `master` to `main`. We encourage
+users to migrate to the latest version, though it comes with some cost. Please
+refer to [Migration Guide](docs/en/migration.md) for more details.** We have
+constructed a comprehensive LiDAR semantic segmentation benchmark on
+SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy,
+the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of
+SemanticKITTI. We have also supported the training of BEVFusion and an
+occupancy prediction method, TPVFomrer, in our `projects`. More new features
+about 3D perception are on the way. Please stay tuned! **v1.2.0** was released
+in 4/7/2023 - Support [New Config Type](https://mmengine.readthedocs.io/en/
+latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
+beta) in `mmdet3d/config` - Support the inference of [DSVT](<(https://
+arxiv.org/abs/2301.06051)>) in `projects` - Support downloading datasets from
+[OpenDataLab](https://opendatalab.com/) using `mim` **v1.1.1** was released in
+30/5/2023: - Support [TPVFormer](https://arxiv.org/pdf/2302.07817.pdf) in
+`projects` - Support the training of BEVFusion in `projects` - Support lidar-
+based 3D semantic segmentation benchmark ## Installation Please refer to
+[Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html)
+for installation instructions. ## Getting Started For detailed user guides and
+advanced guides, please refer to our [documentation](https://
+mmdetection3d.readthedocs.io/en/latest/):  User Guides - [Train & Test](https:/
+/mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#train-test) -
+[Learn about Configs](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/config.html) - [Coordinate System](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/coord_sys_tutorial.html) -
+[Dataset Preparation](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/dataset_prepare.html) - [Customize Data Pipelines](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/data_pipeline.html) - [Test
+and Train on Standard Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/train_test.html) - [Inference](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/inference.html) - [Train
+with Customized Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/new_data_model.html) - [Useful Tools](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#useful-tools)
+Advanced Guides - [Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/index.html#datasets) - [KITTI Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/kitti.html) -
+[NuScenes Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/nuscenes.html) - [Lyft Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/lyft.html) -
+[Waymo Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+datasets/waymo.html) - [SUN RGB-D Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/sunrgbd.html) -
+[ScanNet Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/scannet.html) - [S3DIS Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/s3dis.html) -
+[SemanticKITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/semantickitti.html) - [Supported Tasks](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#supported-
+tasks) - [LiDAR-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/
+latest/advanced_guides/supported_tasks/lidar_det3d.html) - [Vision-Based 3D
+Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+supported_tasks/vision_det3d.html) - [LiDAR-Based 3D Semantic Segmentation]
+(https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+supported_tasks/lidar_sem_seg3d.html) - [Customization](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+index.html#customization) - [Customize Datasets](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_dataset.html)
+- [Customize Models](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/customize_models.html) - [Customize Runtime Settings](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_runtime.html)
+## Overview of Benchmark and Model Zoo Results and models are available in the
+[model zoo](docs/en/model_zoo.md).
                                   Components
                Backbones                 Heads                   Features
      * PointNet_(CVPR'2017)       * FreeAnchor_        * Dynamic_Voxelization_
      * PointNet++_                  (NeurIPS'2019)       (CoRL'2019)
        (NeurIPS'2017)
      * RegNet_(CVPR'2020)
      * DGCNN_(TOG'2019)
      * DLA (CVPR'2018)
      * MinkResNet (CVPR'2019)
      * MinkUNet_(CVPR'2019)
      * Cylinder3D_(CVPR'2021)
                                  Architectures
-3D Object Detection  Monocular 3D Object  Multi-modal 3D         3D Semantic
-                          Detection      Object Detection        Segmentation
-Outdoor              Outdoor             Outdoor           Outdoor
-    * SECOND_            * ImVoxelNet_       * MVXNet_         * MinkUNet_
-      (Sensor'2018)        (WACV'2022)         (ICRA'2019)       (CVPR'2019)
-    * PointPillars_      * SMOKE_        Indoor                * SPVCNN_
-      (CVPR'2019)          (CVPRW'2020)      * ImVoteNet_        (ECCV'2020)
-    * SSN_               * FCOS3D_             (CVPR'2020)     * Cylinder3D_
-      (ECCV'2020)          (ICCVW'2021)                          (CVPR'2021)
-    * 3DSSD_             * PGD_                            Indoor
-      (CVPR'2020)          (CoRL'2021)                         * PointNet++_
-    * SA-SSD_            * MonoFlex_                             (NeurIPS'2017)
-      (CVPR'2020)          (CVPR'2021)                         * PAConv_
-    * PointRCNN_     Indoor                                      (CVPR'2021)
-      (CVPR'2019)        * ImVoxelNet_                         * DGCNN_
-    * Part-A2_             (WACV'2022)                           (TOG'2019)
-      (TPAMI'2020)
-    * CenterPoint_
-      (CVPR'2021)
-    * PV-RCNN_
+    LiDAR-based 3D    Camera-based 3D    Multi-modal 3D         3D Semantic
+   Object Detection   Object Detection  Object Detection        Segmentation
+Outdoor              Outdoor            Outdoor           Outdoor
+    * SECOND_            * ImVoxelNet_      * MVXNet_         * MinkUNet_
+      (Sensor'2018)        (WACV'2022)        (ICRA'2019)       (CVPR'2019)
+    * PointPillars_      * SMOKE_           * BEVFusion_      * SPVCNN_
+      (CVPR'2019)          (CVPRW'2020)       (ICRA'2023)       (ECCV'2020)
+    * SSN_               * FCOS3D_      Indoor                * Cylinder3D_
+      (ECCV'2020)          (ICCVW'2021)     * ImVoteNet_        (CVPR'2021)
+    * 3DSSD_             * PGD_               (CVPR'2020)     * TPVFormer_
+      (CVPR'2020)          (CoRL'2021)                          (CVPR'2023)
+    * SA-SSD_            * MonoFlex_                      Indoor
+      (CVPR'2020)          (CVPR'2021)                        * PointNet++_
+    * PointRCNN_         * DETR3D_                              (NeurIPS'2017)
+      (CVPR'2019)          (CoRL'2021)                        * PAConv_
+    * Part-A2_           * PETR_                                (CVPR'2021)
+      (TPAMI'2020)         (ECCV'2022)                        * DGCNN_
+    * CenterPoint_   Indoor                                     (TOG'2019)
+      (CVPR'2021)        * ImVoxelNet_
+    * PV-RCNN_             (WACV'2022)
       (CVPR'2020)
+    * CenterFormer_
+      (ECCV'2022)
 Indoor
     * VoteNet_
       (ICCV'2019)
     * H3DNet_
       (ECCV'2020)
     * Group-Free-3D_
       (ICCV'2021)
     * FCAF3D_
       (ECCV'2022)
-| | ResNet | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet |
-Cylinder3D | MinkUNet | | :-----------: | :----: | :--------: | :----: | :---:
-| :-----: | :-: | :--------: | :--------: | :------: | | SECOND | â | â |
-â | â | â | â | â | â | â | | PointPillars | â | â | â |
-â | â | â | â | â | â | | FreeAnchor | â | â | â | â | â
-| â | â | â | â | | VoteNet | â | â | â | â | â | â | â |
-â | â | | H3DNet | â | â | â | â | â | â | â | â | â | |
-3DSSD | â | â | â | â | â | â | â | â | â | | Part-A2 | â |
-â | â | â | â | â | â | â | â | | MVXNet | â | â | â |
-â | â | â | â | â | â | | CenterPoint | â | â | â | â | â
-| â | â | â | â | | SSN | â | â | â | â | â | â | â | â
-| â | | ImVoteNet | â | â | â | â | â | â | â | â | â | |
-FCOS3D | â | â | â | â | â | â | â | â | â | | PointNet++ |
-â | â | â | â | â | â | â | â | â | | Group-Free-3D | â |
-â | â | â | â | â | â | â | â | | ImVoxelNet | â | â | â
-| â | â | â | â | â | â | | PAConv | â | â | â | â | â |
-â | â | â | â | | DGCNN | â | â | â | â | â | â | â | â
-| â | | SMOKE | â | â | â | â | â | â | â | â | â | | PGD |
-â | â | â | â | â | â | â | â | â | | MonoFlex | â | â |
-â | â | â | â | â | â | â | | SA-SSD | â | â | â | â |
-â | â | â | â | â | | FCAF3D | â | â | â | â | â | â |
-â | â | â | | PV-RCNN | â | â | â | â | â | â | â | â |
-â | | Cylinder3D | â | â | â | â | â | â | â | â | â | |
-MinkUNet | â | â | â | â | â | â | â | â | â | | SPVCNN | â
-| â | â | â | â | â | â | â | â | **Note:** All the about
-**300+ models, methods of 40+ papers** in 2D detection supported by
-[MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/
-model_zoo.md) can be trained or used in this codebase. ## Installation Please
-refer to [get_started.md](docs/en/get_started.md) for installation. ## Get
-Started Please see [get_started.md](docs/en/get_started.md) for the basic usage
-of MMDetection3D. We provide guidance for quick run [with existing dataset]
-(docs/en/user_guides/train_test.md) and [with new dataset](docs/en/user_guides/
-2_new_data_model.md) for beginners. There are also tutorials for [learning
-configuration systems](docs/en/user_guides/config.md), [customizing dataset]
-(docs/en/advanced_guides/customize_dataset.md), [designing data pipeline](docs/
-en/user_guides/data_pipeline.md), [customizing models](docs/en/advanced_guides/
-customize_models.md), [customizing runtime settings](docs/en/advanced_guides/
-customize_runtime.md) and [Waymo dataset](docs/en/advanced_guides/datasets/
-waymo_det.md). Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked
-questions. When updating the version of MMDetection3D, please also check the
-[compatibility doc](docs/en/notes/compatibility.md) to be aware of the BC-
-breaking updates introduced in each version. ## Citation If you find this
-project useful in your research, please consider cite: ```latex @misc
-{mmdet3d2020, title={{MMDetection3D: OpenMMLab} next-generation platform for
-general {3D} object detection}, author={MMDetection3D Contributors},
-howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}}, year={2020}
-} ``` ## Contributing We appreciate all contributions to improve MMDetection3D.
-Please refer to [CONTRIBUTING.md](./docs/en/notes/contribution_guides.md) for
-the contributing guideline. ## Acknowledgement MMDetection3D is an open source
+    * TR3D_
+      (ArXiv'2023)
+| | ResNet | VoVNet | Swin-T | PointNet++ | SECOND | DGCNN | RegNetX | DLA |
+MinkResNet | Cylinder3D | MinkUNet | | :-----------: | :----: | :----: | :----:
+| :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :----
+--: | | SECOND | â | â | â | â | â | â | â | â | â | â |
+â | | PointPillars | â | â | â | â | â | â | â | â | â |
+â | â | | FreeAnchor | â | â | â | â | â | â | â | â | â
+| â | â | | VoteNet | â | â | â | â | â | â | â | â | â |
+â | â | | H3DNet | â | â | â | â | â | â | â | â | â |
+â | â | | 3DSSD | â | â | â | â | â | â | â | â | â | â
+| â | | Part-A2 | â | â | â | â | â | â | â | â | â | â |
+â | | MVXNet | â | â | â | â | â | â | â | â | â | â |
+â | | CenterPoint | â | â | â | â | â | â | â | â | â | â
+| â | | SSN | â | â | â | â | â | â | â | â | â | â | â
+| | ImVoteNet | â | â | â | â | â | â | â | â | â | â | â
+| | FCOS3D | â | â | â | â | â | â | â | â | â | â | â |
+| PointNet++ | â | â | â | â | â | â | â | â | â | â | â
+| | Group-Free-3D | â | â | â | â | â | â | â | â | â | â |
+â | | ImVoxelNet | â | â | â | â | â | â | â | â | â | â
+| â | | PAConv | â | â | â | â | â | â | â | â | â | â |
+â | | DGCNN | â | â | â | â | â | â | â | â | â | â | â
+| | SMOKE | â | â | â | â | â | â | â | â | â | â | â | |
+PGD | â | â | â | â | â | â | â | â | â | â | â | |
+MonoFlex | â | â | â | â | â | â | â | â | â | â | â | |
+SA-SSD | â | â | â | â | â | â | â | â | â | â | â | |
+FCAF3D | â | â | â | â | â | â | â | â | â | â | â | |
+PV-RCNN | â | â | â | â | â | â | â | â | â | â | â | |
+Cylinder3D | â | â | â | â | â | â | â | â | â | â | â |
+| MinkUNet | â | â | â | â | â | â | â | â | â | â | â |
+| SPVCNN | â | â | â | â | â | â | â | â | â | â | â | |
+BEVFusion | â | â | â | â | â | â | â | â | â | â | â | |
+CenterFormer | â | â | â | â | â | â | â | â | â | â | â
+| | TR3D | â | â | â | â | â | â | â | â | â | â | â | |
+DETR3D | â | â | â | â | â | â | â | â | â | â | â | |
+PETR | â | â | â | â | â | â | â | â | â | â | â | |
+TPVFormer | â | â | â | â | â | â | â | â | â | â | â |
+**Note:** All the about **500+ models, methods of 90+ papers** in 2D detection
+supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/
+docs/en/model_zoo.md) can be trained or used in this codebase. ## FAQ Please
+refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions. ##
+Contributing We appreciate all contributions to improve MMDetection3D. Please
+refer to [CONTRIBUTING.md](docs/en/notes/contribution_guides.md) for the
+contributing guideline. ## Acknowledgement MMDetection3D is an open source
 project that is contributed by researchers and engineers from various colleges
 and companies. We appreciate all the contributors as well as users who give
 valuable feedbacks. We wish that the toolbox and benchmark could serve the
 growing research community by providing a flexible toolkit to reimplement
-existing methods and develop their own new 3D detectors. ## Projects in
-OpenMMLab - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab
-foundational library for training deep learning models. - [MMCV](https://
-github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
-vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation
-library for multiple machine learning libraries. - [MIM](https://github.com/
-open-mmlab/mim): MIM installs OpenMMLab packages. - [MMPreTrain](https://
-github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+existing methods and develop their own new 3D detectors. ## Citation If you
+find this project useful in your research, please consider cite: ```latex @misc
+{mmdet3d2020, title={{MMDetection3D: OpenMMLab} next-generation platform for
+general {3D} object detection}, author={MMDetection3D Contributors},
+howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}}, year={2020}
+} ``` ## License This project is released under the [Apache 2.0 license]
+(LICENSE). ## Projects in OpenMMLab - [MMEngine](https://github.com/open-mmlab/
+mmengine): OpenMMLab foundational library for training deep learning models. -
+[MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for
+computer vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified
+evaluation library for multiple machine learning libraries. - [MIM](https://
+github.com/open-mmlab/mim): MIM installs OpenMMLab packages. - [MMPreTrain]
+(https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
 benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection):
 OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
 github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
 general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
 mmrotate): OpenMMLab rotated object detection toolbox and benchmark. - [MMYOLO]
 (https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and
 benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
@@ -183,15 +242,8 @@
 benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
 mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMagic](https:/
 /github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
 **I**ntelligent **C**reation toolbox. - [MMGeneration](https://github.com/open-
 mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
 [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
-framework. Keywords: computer vision,3D object detection Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown Provides-Extra: all Provides-Extra: tests Provides-
-Extra: build Provides-Extra: optional Provides-Extra: mim
+framework.
```

### Comparing `mmdet3d-1.1.1/README.md` & `mmdet3d-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,330 +1,423 @@
-<div align="center">
-  <img src="resources/mmdet3d-logo.png" width="600"/>
-  <div>&nbsp;</div>
-  <div align="center">
-    <b><font size="5">OpenMMLab website</font></b>
-    <sup>
-      <a href="https://openmmlab.com">
-        <i><font size="4">HOT</font></i>
-      </a>
-    </sup>
-    &nbsp;&nbsp;&nbsp;&nbsp;
-    <b><font size="5">OpenMMLab platform</font></b>
-    <sup>
-      <a href="https://platform.openmmlab.com">
-        <i><font size="4">TRY IT OUT</font></i>
-      </a>
-    </sup>
-  </div>
-  <div>&nbsp;</div>
-
-[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/latest/)
-[![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
-[![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
-[![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/LICENSE)
-
-</div>
-
-</div>
-
-<div align="center">
-  <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://discord.com/channels/1037617289144569886/1046608014234370059" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
-</div>
-
-**News**:
-
-**We have renamed the branch `1.1`  to `main` and switched the default branch from `master` to `main`. We encourage
-users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](docs/en/migration.md) for more details.**
-
-**v1.1.1** was released in 30/5/2023
-
-We have constructed a comprehensive LiDAR semantic segmentation benchmark on SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy, the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of SemanticKITTI. We have also supported the training of BEVFusion and an occupancy prediction method, TPVFomrer, in our `projects`. More new features about 3D perception are on the way. Please stay tuned!
-
-## Introduction
-
-English | [简体中文](README_zh-CN.md)
-
-The main branch works with **PyTorch 1.8+**.
-
-MMDetection3D is an open source object detection toolbox based on PyTorch, towards the next-generation platform for general 3D detection. It is
-a part of the OpenMMLab project developed by [MMLab](http://mmlab.ie.cuhk.edu.hk/).
-
-![demo image](resources/mmdet3d_outdoor_demo.gif)
-
-### Major features
-
-- **Support multi-modality/single-modality detectors out of box**
-
-  It directly supports multi-modality/single-modality detectors including MVXNet, VoteNet, PointPillars, etc.
-
-- **Support indoor/outdoor 3D detection out of box**
-
-  It directly supports popular indoor and outdoor 3D detection datasets, including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI.
-  For nuScenes dataset, we also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/nuimages).
-
-- **Natural integration with 2D detection**
-
-  All the about **300+ models, methods of 40+ papers**, and modules supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
-
-- **High efficiency**
-
-  It trains faster than other codebases. The main results are as below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the number of samples trained per second (the higher, the better). The models that are not supported by other codebases are marked by `✗`.
-
-  |       Methods       | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) | [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://github.com/poodarchu/Det3D) |
-  | :-----------------: | :-----------: | :--------------------------------------------------: | :----------------------------------------------------: | :-----------------------------------------: |
-  |       VoteNet       |      358      |                          ✗                           |                           77                           |                      ✗                      |
-  |  PointPillars-car   |      141      |                          ✗                           |                           ✗                            |                     140                     |
-  | PointPillars-3class |      107      |                          44                          |                           ✗                            |                      ✗                      |
-  |       SECOND        |      40       |                          30                          |                           ✗                            |                      ✗                      |
-  |       Part-A2       |      17       |                          14                          |                           ✗                            |                      ✗                      |
-
-Like [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to support different projects on top of it.
-
-## License
-
-This project is released under the [Apache 2.0 license](LICENSE).
-
-## Changelog
-
-**1.1.0** was released in 6/4/2023.
-
-Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
-
-## Benchmark and model zoo
-
-Results and models are available in the [model zoo](docs/en/model_zoo.md).
-
-<div align="center">
-  <b>Components</b>
-</div>
-<table align="center">
-  <tbody>
-    <tr align="center" valign="bottom">
-      <td>
-        <b>Backbones</b>
-      </td>
-      <td>
-        <b>Heads</b>
-      </td>
-      <td>
-        <b>Features</b>
-      </td>
-    </tr>
-    <tr valign="top">
-      <td>
-      <ul>
-        <li><a href="configs/pointnet2">PointNet (CVPR'2017)</a></li>
-        <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
-        <li><a href="configs/regnet">RegNet (CVPR'2020)</a></li>
-        <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
-        <li>DLA (CVPR'2018)</li>
-        <li>MinkResNet (CVPR'2019)</li>
-        <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
-        <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
-      </ul>
-      </td>
-      <td>
-      <ul>
-        <li><a href="configs/free_anchor">FreeAnchor (NeurIPS'2019)</a></li>
-      </ul>
-      </td>
-      <td>
-      <ul>
-        <li><a href="configs/dynamic_voxelization">Dynamic Voxelization (CoRL'2019)</a></li>
-      </ul>
-      </td>
-    </tr>
-</td>
-    </tr>
-  </tbody>
-</table>
-
-<div align="center">
-  <b>Architectures</b>
-</div>
-<table align="center">
-  <tbody>
-    <tr align="center" valign="middle">
-      <td>
-        <b>3D Object Detection</b>
-      </td>
-      <td>
-        <b>Monocular 3D Object Detection</b>
-      </td>
-      <td>
-        <b>Multi-modal 3D Object Detection</b>
-      </td>
-      <td>
-        <b>3D Semantic Segmentation</b>
-      </td>
-    </tr>
-    <tr valign="top">
-      <td>
-        <li><b>Outdoor</b></li>
-        <ul>
-            <li><a href="configs/second">SECOND (Sensor'2018)</a></li>
-            <li><a href="configs/pointpillars">PointPillars (CVPR'2019)</a></li>
-            <li><a href="configs/ssn">SSN (ECCV'2020)</a></li>
-            <li><a href="configs/3dssd">3DSSD (CVPR'2020)</a></li>
-            <li><a href="configs/sassd">SA-SSD (CVPR'2020)</a></li>
-            <li><a href="configs/point_rcnn">PointRCNN (CVPR'2019)</a></li>
-            <li><a href="configs/parta2">Part-A2 (TPAMI'2020)</a></li>
-            <li><a href="configs/centerpoint">CenterPoint (CVPR'2021)</a></li>
-            <li><a href="configs/pv_rcnn">PV-RCNN (CVPR'2020)</a></li>
-        </ul>
-        <li><b>Indoor</b></li>
-        <ul>
-            <li><a href="configs/votenet">VoteNet (ICCV'2019)</a></li>
-            <li><a href="configs/h3dnet">H3DNet (ECCV'2020)</a></li>
-            <li><a href="configs/groupfree3d">Group-Free-3D (ICCV'2021)</a></li>
-            <li><a href="configs/fcaf3d">FCAF3D (ECCV'2022)</a></li>
-      </ul>
-      </td>
-      <td>
-        <li><b>Outdoor</b></li>
-        <ul>
-          <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
-          <li><a href="configs/smoke">SMOKE (CVPRW'2020)</a></li>
-          <li><a href="configs/fcos3d">FCOS3D (ICCVW'2021)</a></li>
-          <li><a href="configs/pgd">PGD (CoRL'2021)</a></li>
-          <li><a href="configs/monoflex">MonoFlex (CVPR'2021)</a></li>
-        </ul>
-        <li><b>Indoor</b></li>
-        <ul>
-          <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
-        </ul>
-      </td>
-      <td>
-        <li><b>Outdoor</b></li>
-        <ul>
-          <li><a href="configs/mvxnet">MVXNet (ICRA'2019)</a></li>
-        </ul>
-        <li><b>Indoor</b></li>
-        <ul>
-          <li><a href="configs/imvotenet">ImVoteNet (CVPR'2020)</a></li>
-        </ul>
-      </td>
-      <td>
-        <li><b>Outdoor</b></li>
-        <ul>
-          <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
-          <li><a href="configs/spvcnn">SPVCNN (ECCV'2020)</a></li>
-          <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
-        </ul>
-        <li><b>Indoor</b></li>
-        <ul>
-          <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
-          <li><a href="configs/paconv">PAConv (CVPR'2021)</a></li>
-          <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
-        </ul>
-      </ul>
-      </td>
-    </tr>
-</td>
-    </tr>
-  </tbody>
-</table>
-
-|               | ResNet | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet | Cylinder3D | MinkUNet |
-| :-----------: | :----: | :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :------: |
-|    SECOND     |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-| PointPillars  |   ✗    |     ✗      |   ✓    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-|  FreeAnchor   |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    VoteNet    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    H3DNet     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|     3DSSD     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    Part-A2    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    MVXNet     |   ✓    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|  CenterPoint  |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|      SSN      |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-|   ImVoteNet   |   ✓    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    FCOS3D     |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|  PointNet++   |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-| Group-Free-3D |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|  ImVoxelNet   |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    PAConv     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|     DGCNN     |   ✗    |     ✗      |   ✗    |   ✓   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|     SMOKE     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
-|      PGD      |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|   MonoFlex    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
-|    SA-SSD     |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|    FCAF3D     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
-|    PV-RCNN    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-|  Cylinder3D   |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✓      |    ✗     |
-|   MinkUNet    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
-|    SPVCNN     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
-
-**Note:** All the about **300+ models, methods of 40+ papers** in 2D detection supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
-
-## Installation
-
-Please refer to [get_started.md](docs/en/get_started.md) for installation.
-
-## Get Started
-
-Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMDetection3D. We provide guidance for quick run [with existing dataset](docs/en/user_guides/train_test.md) and [with new dataset](docs/en/user_guides/2_new_data_model.md) for beginners. There are also tutorials for [learning configuration systems](docs/en/user_guides/config.md), [customizing dataset](docs/en/advanced_guides/customize_dataset.md), [designing data pipeline](docs/en/user_guides/data_pipeline.md), [customizing models](docs/en/advanced_guides/customize_models.md), [customizing runtime settings](docs/en/advanced_guides/customize_runtime.md) and [Waymo dataset](docs/en/advanced_guides/datasets/waymo_det.md).
-
-Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions. When updating the version of MMDetection3D, please also check the [compatibility doc](docs/en/notes/compatibility.md) to be aware of the BC-breaking updates introduced in each version.
-
-## Citation
-
-If you find this project useful in your research, please consider cite:
-
-```latex
-@misc{mmdet3d2020,
-    title={{MMDetection3D: OpenMMLab} next-generation platform for general {3D} object detection},
-    author={MMDetection3D Contributors},
-    howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}},
-    year={2020}
-}
-```
-
-## Contributing
-
-We appreciate all contributions to improve MMDetection3D. Please refer to [CONTRIBUTING.md](./docs/en/notes/contribution_guides.md) for the contributing guideline.
-
-## Acknowledgement
-
-MMDetection3D is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors as well as users who give valuable feedbacks.
-We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and develop their own new 3D detectors.
-
-## Projects in OpenMMLab
-
-- [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
-- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
-- [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-- [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-- [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
-- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-- [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
-- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-- [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
-- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
-- [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+Metadata-Version: 2.1
+Name: mmdet3d
+Version: 1.2.0
+Summary: OpenMMLab's next-generation platformfor general 3D object detection.
+Home-page: https://github.com/open-mmlab/mmdetection3d
+Author: MMDetection3D Contributors
+Author-email: zwwdev@gmail.com
+License: Apache License 2.0
+Description: <div align="center">
+          <img src="resources/mmdet3d-logo.png" width="600"/>
+          <div>&nbsp;</div>
+          <div align="center">
+            <b><font size="5">OpenMMLab website</font></b>
+            <sup>
+              <a href="https://openmmlab.com">
+                <i><font size="4">HOT</font></i>
+              </a>
+            </sup>
+            &nbsp;&nbsp;&nbsp;&nbsp;
+            <b><font size="5">OpenMMLab platform</font></b>
+            <sup>
+              <a href="https://platform.openmmlab.com">
+                <i><font size="4">TRY IT OUT</font></i>
+              </a>
+            </sup>
+          </div>
+          <div>&nbsp;</div>
+        
+        [![PyPI](https://img.shields.io/pypi/v/mmdet3d)](https://pypi.org/project/mmdet3d)
+        [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/latest/)
+        [![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
+        [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
+        [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/main/LICENSE)
+        [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+        [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+        
+        [📘Documentation](https://mmdetection3d.readthedocs.io/en/latest/) |
+        [🛠️Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html) |
+        [👀Model Zoo](https://mmdetection3d.readthedocs.io/en/latest/model_zoo.html) |
+        [🆕Update News](https://mmdetection3d.readthedocs.io/en/latest/notes/changelog.html) |
+        [🚀Ongoing Projects](https://github.com/open-mmlab/mmdetection3d/projects) |
+        [🤔Reporting Issues](https://github.com/open-mmlab/mmdetection3d/issues/new/choose)
+        
+        </div>
+        
+        <div align="center">
+        
+        English | [简体中文](README_zh-CN.md)
+        
+        </div>
+        
+        <div align="center">
+          <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://discord.com/channels/1037617289144569886/1046608014234370059" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
+        </div>
+        
+        ## Introduction
+        
+        MMDetection3D is an open source object detection toolbox based on PyTorch, towards the next-generation platform for general 3D detection. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
+        
+        The main branch works with **PyTorch 1.8+**.
+        
+        ![demo image](resources/mmdet3d_outdoor_demo.gif)
+        
+        <details open>
+        <summary>Major features</summary>
+        
+        - **Support multi-modality/single-modality detectors out of box**
+        
+          It directly supports multi-modality/single-modality detectors including MVXNet, VoteNet, PointPillars, etc.
+        
+        - **Support indoor/outdoor 3D detection out of box**
+        
+          It directly supports popular indoor and outdoor 3D detection datasets, including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes dataset, we also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/nuimages).
+        
+        - **Natural integration with 2D detection**
+        
+          All the about **300+ models, methods of 40+ papers**, and modules supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
+        
+        - **High efficiency**
+        
+          It trains faster than other codebases. The main results are as below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the number of samples trained per second (the higher, the better). The models that are not supported by other codebases are marked by `✗`.
+        
+          |       Methods       | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) | [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://github.com/poodarchu/Det3D) |
+          | :-----------------: | :-----------: | :--------------------------------------------------: | :----------------------------------------------------: | :-----------------------------------------: |
+          |       VoteNet       |      358      |                          ✗                           |                           77                           |                      ✗                      |
+          |  PointPillars-car   |      141      |                          ✗                           |                           ✗                            |                     140                     |
+          | PointPillars-3class |      107      |                          44                          |                           ✗                            |                      ✗                      |
+          |       SECOND        |      40       |                          30                          |                           ✗                            |                      ✗                      |
+          |       Part-A2       |      17       |                          14                          |                           ✗                            |                      ✗                      |
+        
+        </details>
+        
+        Like [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to support different projects on top of it.
+        
+        ## What's New
+        
+        ### Highlight
+        
+        **We have renamed the branch `1.1` to `main` and switched the default branch from `master` to `main`. We encourage users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](docs/en/migration.md) for more details.**
+        
+        We have constructed a comprehensive LiDAR semantic segmentation benchmark on SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy, the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of SemanticKITTI. We have also supported the training of BEVFusion and an occupancy prediction method, TPVFomrer, in our `projects`. More new features about 3D perception are on the way. Please stay tuned!
+        
+        **v1.2.0** was released in 4/7/2023
+        
+        - Support [New Config Type](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) in `mmdet3d/config`
+        - Support the inference of [DSVT](<(https://arxiv.org/abs/2301.06051)>) in `projects`
+        - Support downloading datasets from [OpenDataLab](https://opendatalab.com/) using `mim`
+        
+        **v1.1.1** was released in 30/5/2023:
+        
+        - Support [TPVFormer](https://arxiv.org/pdf/2302.07817.pdf) in `projects`
+        - Support the training of BEVFusion in `projects`
+        - Support lidar-based 3D semantic segmentation benchmark
+        
+        ## Installation
+        
+        Please refer to [Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html) for installation instructions.
+        
+        ## Getting Started
+        
+        For detailed user guides and advanced guides, please refer to our [documentation](https://mmdetection3d.readthedocs.io/en/latest/):
+        
+        <details>
+        <summary>User Guides</summary>
+        
+        - [Train & Test](https://mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#train-test)
+          - [Learn about Configs](https://mmdetection3d.readthedocs.io/en/latest/user_guides/config.html)
+          - [Coordinate System](https://mmdetection3d.readthedocs.io/en/latest/user_guides/coord_sys_tutorial.html)
+          - [Dataset Preparation](https://mmdetection3d.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
+          - [Customize Data Pipelines](https://mmdetection3d.readthedocs.io/en/latest/user_guides/data_pipeline.html)
+          - [Test and Train on Standard Datasets](https://mmdetection3d.readthedocs.io/en/latest/user_guides/train_test.html)
+          - [Inference](https://mmdetection3d.readthedocs.io/en/latest/user_guides/inference.html)
+          - [Train with Customized Datasets](https://mmdetection3d.readthedocs.io/en/latest/user_guides/new_data_model.html)
+        - [Useful Tools](https://mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#useful-tools)
+        
+        </details>
+        
+        <details>
+        <summary>Advanced Guides</summary>
+        
+        - [Datasets](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#datasets)
+          - [KITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/kitti.html)
+          - [NuScenes Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/nuscenes.html)
+          - [Lyft Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/lyft.html)
+          - [Waymo Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/waymo.html)
+          - [SUN RGB-D Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/sunrgbd.html)
+          - [ScanNet Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/scannet.html)
+          - [S3DIS Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/s3dis.html)
+          - [SemanticKITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/semantickitti.html)
+        - [Supported Tasks](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#supported-tasks)
+          - [LiDAR-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/lidar_det3d.html)
+          - [Vision-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/vision_det3d.html)
+          - [LiDAR-Based 3D Semantic Segmentation](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/lidar_sem_seg3d.html)
+        - [Customization](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#customization)
+          - [Customize Datasets](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_dataset.html)
+          - [Customize Models](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_models.html)
+          - [Customize Runtime Settings](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_runtime.html)
+        
+        </details>
+        
+        ## Overview of Benchmark and Model Zoo
+        
+        Results and models are available in the [model zoo](docs/en/model_zoo.md).
+        
+        <div align="center">
+          <b>Components</b>
+        </div>
+        <table align="center">
+          <tbody>
+            <tr align="center" valign="bottom">
+              <td>
+                <b>Backbones</b>
+              </td>
+              <td>
+                <b>Heads</b>
+              </td>
+              <td>
+                <b>Features</b>
+              </td>
+            </tr>
+            <tr valign="top">
+              <td>
+              <ul>
+                <li><a href="configs/pointnet2">PointNet (CVPR'2017)</a></li>
+                <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
+                <li><a href="configs/regnet">RegNet (CVPR'2020)</a></li>
+                <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
+                <li>DLA (CVPR'2018)</li>
+                <li>MinkResNet (CVPR'2019)</li>
+                <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
+                <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
+              </ul>
+              </td>
+              <td>
+              <ul>
+                <li><a href="configs/free_anchor">FreeAnchor (NeurIPS'2019)</a></li>
+              </ul>
+              </td>
+              <td>
+              <ul>
+                <li><a href="configs/dynamic_voxelization">Dynamic Voxelization (CoRL'2019)</a></li>
+              </ul>
+              </td>
+            </tr>
+        </td>
+            </tr>
+          </tbody>
+        </table>
+        
+        <div align="center">
+          <b>Architectures</b>
+        </div>
+        <table align="center">
+          <tbody>
+            <tr align="center" valign="middle">
+              <td>
+                <b>LiDAR-based 3D Object Detection</b>
+              </td>
+              <td>
+                <b>Camera-based 3D Object Detection</b>
+              </td>
+              <td>
+                <b>Multi-modal 3D Object Detection</b>
+              </td>
+              <td>
+                <b>3D Semantic Segmentation</b>
+              </td>
+            </tr>
+            <tr valign="top">
+              <td>
+                <li><b>Outdoor</b></li>
+                <ul>
+                    <li><a href="configs/second">SECOND (Sensor'2018)</a></li>
+                    <li><a href="configs/pointpillars">PointPillars (CVPR'2019)</a></li>
+                    <li><a href="configs/ssn">SSN (ECCV'2020)</a></li>
+                    <li><a href="configs/3dssd">3DSSD (CVPR'2020)</a></li>
+                    <li><a href="configs/sassd">SA-SSD (CVPR'2020)</a></li>
+                    <li><a href="configs/point_rcnn">PointRCNN (CVPR'2019)</a></li>
+                    <li><a href="configs/parta2">Part-A2 (TPAMI'2020)</a></li>
+                    <li><a href="configs/centerpoint">CenterPoint (CVPR'2021)</a></li>
+                    <li><a href="configs/pv_rcnn">PV-RCNN (CVPR'2020)</a></li>
+                    <li><a href="projects/CenterFormer">CenterFormer (ECCV'2022)</a></li>
+                </ul>
+                <li><b>Indoor</b></li>
+                <ul>
+                    <li><a href="configs/votenet">VoteNet (ICCV'2019)</a></li>
+                    <li><a href="configs/h3dnet">H3DNet (ECCV'2020)</a></li>
+                    <li><a href="configs/groupfree3d">Group-Free-3D (ICCV'2021)</a></li>
+                    <li><a href="configs/fcaf3d">FCAF3D (ECCV'2022)</a></li>
+                    <li><a href="projects/TR3D">TR3D (ArXiv'2023)</a></li>
+              </ul>
+              </td>
+              <td>
+                <li><b>Outdoor</b></li>
+                <ul>
+                  <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
+                  <li><a href="configs/smoke">SMOKE (CVPRW'2020)</a></li>
+                  <li><a href="configs/fcos3d">FCOS3D (ICCVW'2021)</a></li>
+                  <li><a href="configs/pgd">PGD (CoRL'2021)</a></li>
+                  <li><a href="configs/monoflex">MonoFlex (CVPR'2021)</a></li>
+                  <li><a href="projects/DETR3D">DETR3D (CoRL'2021)</a></li>
+                  <li><a href="projects/PETR">PETR (ECCV'2022)</a></li>
+                </ul>
+                <li><b>Indoor</b></li>
+                <ul>
+                  <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
+                </ul>
+              </td>
+              <td>
+                <li><b>Outdoor</b></li>
+                <ul>
+                  <li><a href="configs/mvxnet">MVXNet (ICRA'2019)</a></li>
+                  <li><a href="projects/BEVFusion">BEVFusion (ICRA'2023)</a></li>
+                </ul>
+                <li><b>Indoor</b></li>
+                <ul>
+                  <li><a href="configs/imvotenet">ImVoteNet (CVPR'2020)</a></li>
+                </ul>
+              </td>
+              <td>
+                <li><b>Outdoor</b></li>
+                <ul>
+                  <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
+                  <li><a href="configs/spvcnn">SPVCNN (ECCV'2020)</a></li>
+                  <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
+                  <li><a href="projects/TPVFormer">TPVFormer (CVPR'2023)</a></li>
+                </ul>
+                <li><b>Indoor</b></li>
+                <ul>
+                  <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
+                  <li><a href="configs/paconv">PAConv (CVPR'2021)</a></li>
+                  <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
+                </ul>
+              </ul>
+              </td>
+            </tr>
+        </td>
+            </tr>
+          </tbody>
+        </table>
+        
+        |               | ResNet | VoVNet | Swin-T | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet | Cylinder3D | MinkUNet |
+        | :-----------: | :----: | :----: | :----: | :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :------: |
+        |    SECOND     |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        | PointPillars  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  FreeAnchor   |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    VoteNet    |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    H3DNet     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     3DSSD     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    Part-A2    |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    MVXNet     |   ✓    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  CenterPoint  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |      SSN      |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |   ImVoteNet   |   ✓    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    FCOS3D     |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  PointNet++   |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        | Group-Free-3D |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  ImVoxelNet   |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    PAConv     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     DGCNN     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✓   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     SMOKE     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
+        |      PGD      |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |   MonoFlex    |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
+        |    SA-SSD     |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    FCAF3D     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
+        |    PV-RCNN    |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  Cylinder3D   |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✓      |    ✗     |
+        |   MinkUNet    |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+        |    SPVCNN     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+        |   BEVFusion   |   ✗    |   ✗    |   ✓    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        | CenterFormer  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     TR3D      |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
+        |    DETR3D     |   ✓    |   ✓    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     PETR      |   ✗    |   ✓    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |   TPVFormer   |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        
+        **Note:** All the about **500+ models, methods of 90+ papers** in 2D detection supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
+        
+        ## FAQ
+        
+        Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions.
+        
+        ## Contributing
+        
+        We appreciate all contributions to improve MMDetection3D. Please refer to [CONTRIBUTING.md](docs/en/notes/contribution_guides.md) for the contributing guideline.
+        
+        ## Acknowledgement
+        
+        MMDetection3D is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors as well as users who give valuable feedbacks. We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and develop their own new 3D detectors.
+        
+        ## Citation
+        
+        If you find this project useful in your research, please consider cite:
+        
+        ```latex
+        @misc{mmdet3d2020,
+            title={{MMDetection3D: OpenMMLab} next-generation platform for general {3D} object detection},
+            author={MMDetection3D Contributors},
+            howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}},
+            year={2020}
+        }
+        ```
+        
+        ## License
+        
+        This project is released under the [Apache 2.0 license](LICENSE).
+        
+        ## Projects in OpenMMLab
+        
+        - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+        - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+        - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
+        - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
+        - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+        - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
+        - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
+        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
+        - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
+        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
+        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
+        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+        - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
+        - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
+        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+        - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
+        - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
+        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+        - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+        
+Keywords: computer vision,3D object detection
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: tests
+Provides-Extra: build
+Provides-Extra: optional
+Provides-Extra: mim
```

#### html2text {}

```diff
@@ -1,167 +1,234 @@
+Metadata-Version: 2.1 Name: mmdet3d Version: 1.2.0 Summary: OpenMMLab's next-
+generation platformfor general 3D object detection. Home-page: https://
+github.com/open-mmlab/mmdetection3d Author: MMDetection3D Contributors Author-
+email: zwwdev@gmail.com License: Apache License 2.0 Description:
                          [resources/mmdet3d-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
-       [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
+  [![PyPI](https://img.shields.io/pypi/v/mmdet3d)](https://pypi.org/project/
+  mmdet3d) [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
   mmdetection3d.readthedocs.io/en/latest/) [![badge](https://github.com/open-
 mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/
      mmdetection3d/actions) [![codecov](https://codecov.io/gh/open-mmlab/
-mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
+ mmdetection3d/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
  mmdetection3d) [![license](https://img.shields.io/github/license/open-mmlab/
- mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/
-                                   LICENSE)
+  mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/main/
+  LICENSE) [![open issues](https://isitmaintained.com/badge/open/open-mmlab/
+  mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues) [!
+  [issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/
+   mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+    [ðDocumentation](https://mmdetection3d.readthedocs.io/en/latest/) |
+     [ð ï¸Installation](https://mmdetection3d.readthedocs.io/en/latest/
+ get_started.html) | [ðModel Zoo](https://mmdetection3d.readthedocs.io/en/
+              latest/model_zoo.html) | [ðUpdate News](https://
+  mmdetection3d.readthedocs.io/en/latest/notes/changelog.html) | [ðOngoing
+      Projects](https://github.com/open-mmlab/mmdetection3d/projects) |
+[ð¤Reporting Issues](https://github.com/open-mmlab/mmdetection3d/issues/new/
+                                    choose)
+                   English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-**News**: **We have renamed the branch `1.1` to `main` and switched the default
-branch from `master` to `main`. We encourage users to migrate to the latest
-version, though it comes with some cost. Please refer to [Migration Guide]
-(docs/en/migration.md) for more details.** **v1.1.1** was released in 30/5/2023
-We have constructed a comprehensive LiDAR semantic segmentation benchmark on
-SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy,
-the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of
-SemanticKITTI. We have also supported the training of BEVFusion and an
-occupancy prediction method, TPVFomrer, in our `projects`. More new features
-about 3D perception are on the way. Please stay tuned! ## Introduction English
-| [ç®ä½ä¸­æ](README_zh-CN.md) The main branch works with **PyTorch 1.8+**.
-MMDetection3D is an open source object detection toolbox based on PyTorch,
-towards the next-generation platform for general 3D detection. It is a part of
-the OpenMMLab project developed by [MMLab](http://mmlab.ie.cuhk.edu.hk/). !
-[demo image](resources/mmdet3d_outdoor_demo.gif) ### Major features - **Support
-multi-modality/single-modality detectors out of box** It directly supports
-multi-modality/single-modality detectors including MVXNet, VoteNet,
-PointPillars, etc. - **Support indoor/outdoor 3D detection out of box** It
-directly supports popular indoor and outdoor 3D detection datasets, including
-ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes dataset, we
-also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/
-tree/main/configs/nuimages). - **Natural integration with 2D detection** All
-the about **300+ models, methods of 40+ papers**, and modules supported in
-[MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/
-model_zoo.md) can be trained or used in this codebase. - **High efficiency** It
-trains faster than other codebases. The main results are as below. Details can
-be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the
-number of samples trained per second (the higher, the better). The models that
-are not supported by other codebases are marked by `â`. | Methods |
-MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) |
-[votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://
+## Introduction MMDetection3D is an open source object detection toolbox based
+on PyTorch, towards the next-generation platform for general 3D detection. It
+is a part of the [OpenMMLab](https://openmmlab.com/) project. The main branch
+works with **PyTorch 1.8+**. ![demo image](resources/mmdet3d_outdoor_demo.gif)
+Major features - **Support multi-modality/single-modality detectors out of
+box** It directly supports multi-modality/single-modality detectors including
+MVXNet, VoteNet, PointPillars, etc. - **Support indoor/outdoor 3D detection out
+of box** It directly supports popular indoor and outdoor 3D detection datasets,
+including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes
+dataset, we also support [nuImages dataset](https://github.com/open-mmlab/
+mmdetection3d/tree/main/configs/nuimages). - **Natural integration with 2D
+detection** All the about **300+ models, methods of 40+ papers**, and modules
+supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/
+docs/en/model_zoo.md) can be trained or used in this codebase. - **High
+efficiency** It trains faster than other codebases. The main results are as
+below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md).
+We compare the number of samples trained per second (the higher, the better).
+The models that are not supported by other codebases are marked by `â`. |
+Methods | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet)
+| [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://
 github.com/poodarchu/Det3D) | | :-----------------: | :-----------: | :--------
 ------------------------------------------: | :--------------------------------
 --------------------: | :-----------------------------------------: | | VoteNet
 | 358 | â | 77 | â | | PointPillars-car | 141 | â | â | 140 | |
 PointPillars-3class | 107 | 44 | â | â | | SECOND | 40 | 30 | â | â | |
-Part-A2 | 17 | 14 | â | â | Like [MMDetection](https://github.com/open-
+Part-A2 | 17 | 14 | â | â |  Like [MMDetection](https://github.com/open-
 mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv),
 MMDetection3D can also be used as a library to support different projects on
-top of it. ## License This project is released under the [Apache 2.0 license]
-(LICENSE). ## Changelog **1.1.0** was released in 6/4/2023. Please refer to
-[changelog.md](docs/en/notes/changelog.md) for details and release history. ##
-Benchmark and model zoo Results and models are available in the [model zoo]
-(docs/en/model_zoo.md).
+top of it. ## What's New ### Highlight **We have renamed the branch `1.1` to
+`main` and switched the default branch from `master` to `main`. We encourage
+users to migrate to the latest version, though it comes with some cost. Please
+refer to [Migration Guide](docs/en/migration.md) for more details.** We have
+constructed a comprehensive LiDAR semantic segmentation benchmark on
+SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy,
+the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of
+SemanticKITTI. We have also supported the training of BEVFusion and an
+occupancy prediction method, TPVFomrer, in our `projects`. More new features
+about 3D perception are on the way. Please stay tuned! **v1.2.0** was released
+in 4/7/2023 - Support [New Config Type](https://mmengine.readthedocs.io/en/
+latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
+beta) in `mmdet3d/config` - Support the inference of [DSVT](<(https://
+arxiv.org/abs/2301.06051)>) in `projects` - Support downloading datasets from
+[OpenDataLab](https://opendatalab.com/) using `mim` **v1.1.1** was released in
+30/5/2023: - Support [TPVFormer](https://arxiv.org/pdf/2302.07817.pdf) in
+`projects` - Support the training of BEVFusion in `projects` - Support lidar-
+based 3D semantic segmentation benchmark ## Installation Please refer to
+[Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html)
+for installation instructions. ## Getting Started For detailed user guides and
+advanced guides, please refer to our [documentation](https://
+mmdetection3d.readthedocs.io/en/latest/):  User Guides - [Train & Test](https:/
+/mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#train-test) -
+[Learn about Configs](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/config.html) - [Coordinate System](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/coord_sys_tutorial.html) -
+[Dataset Preparation](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/dataset_prepare.html) - [Customize Data Pipelines](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/data_pipeline.html) - [Test
+and Train on Standard Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/train_test.html) - [Inference](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/inference.html) - [Train
+with Customized Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/new_data_model.html) - [Useful Tools](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#useful-tools)
+Advanced Guides - [Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/index.html#datasets) - [KITTI Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/kitti.html) -
+[NuScenes Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/nuscenes.html) - [Lyft Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/lyft.html) -
+[Waymo Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+datasets/waymo.html) - [SUN RGB-D Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/sunrgbd.html) -
+[ScanNet Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/scannet.html) - [S3DIS Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/s3dis.html) -
+[SemanticKITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/semantickitti.html) - [Supported Tasks](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#supported-
+tasks) - [LiDAR-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/
+latest/advanced_guides/supported_tasks/lidar_det3d.html) - [Vision-Based 3D
+Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+supported_tasks/vision_det3d.html) - [LiDAR-Based 3D Semantic Segmentation]
+(https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+supported_tasks/lidar_sem_seg3d.html) - [Customization](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+index.html#customization) - [Customize Datasets](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_dataset.html)
+- [Customize Models](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/customize_models.html) - [Customize Runtime Settings](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_runtime.html)
+## Overview of Benchmark and Model Zoo Results and models are available in the
+[model zoo](docs/en/model_zoo.md).
                                   Components
                Backbones                 Heads                   Features
      * PointNet_(CVPR'2017)       * FreeAnchor_        * Dynamic_Voxelization_
      * PointNet++_                  (NeurIPS'2019)       (CoRL'2019)
        (NeurIPS'2017)
      * RegNet_(CVPR'2020)
      * DGCNN_(TOG'2019)
      * DLA (CVPR'2018)
      * MinkResNet (CVPR'2019)
      * MinkUNet_(CVPR'2019)
      * Cylinder3D_(CVPR'2021)
                                  Architectures
-3D Object Detection  Monocular 3D Object  Multi-modal 3D         3D Semantic
-                          Detection      Object Detection        Segmentation
-Outdoor              Outdoor             Outdoor           Outdoor
-    * SECOND_            * ImVoxelNet_       * MVXNet_         * MinkUNet_
-      (Sensor'2018)        (WACV'2022)         (ICRA'2019)       (CVPR'2019)
-    * PointPillars_      * SMOKE_        Indoor                * SPVCNN_
-      (CVPR'2019)          (CVPRW'2020)      * ImVoteNet_        (ECCV'2020)
-    * SSN_               * FCOS3D_             (CVPR'2020)     * Cylinder3D_
-      (ECCV'2020)          (ICCVW'2021)                          (CVPR'2021)
-    * 3DSSD_             * PGD_                            Indoor
-      (CVPR'2020)          (CoRL'2021)                         * PointNet++_
-    * SA-SSD_            * MonoFlex_                             (NeurIPS'2017)
-      (CVPR'2020)          (CVPR'2021)                         * PAConv_
-    * PointRCNN_     Indoor                                      (CVPR'2021)
-      (CVPR'2019)        * ImVoxelNet_                         * DGCNN_
-    * Part-A2_             (WACV'2022)                           (TOG'2019)
-      (TPAMI'2020)
-    * CenterPoint_
-      (CVPR'2021)
-    * PV-RCNN_
+    LiDAR-based 3D    Camera-based 3D    Multi-modal 3D         3D Semantic
+   Object Detection   Object Detection  Object Detection        Segmentation
+Outdoor              Outdoor            Outdoor           Outdoor
+    * SECOND_            * ImVoxelNet_      * MVXNet_         * MinkUNet_
+      (Sensor'2018)        (WACV'2022)        (ICRA'2019)       (CVPR'2019)
+    * PointPillars_      * SMOKE_           * BEVFusion_      * SPVCNN_
+      (CVPR'2019)          (CVPRW'2020)       (ICRA'2023)       (ECCV'2020)
+    * SSN_               * FCOS3D_      Indoor                * Cylinder3D_
+      (ECCV'2020)          (ICCVW'2021)     * ImVoteNet_        (CVPR'2021)
+    * 3DSSD_             * PGD_               (CVPR'2020)     * TPVFormer_
+      (CVPR'2020)          (CoRL'2021)                          (CVPR'2023)
+    * SA-SSD_            * MonoFlex_                      Indoor
+      (CVPR'2020)          (CVPR'2021)                        * PointNet++_
+    * PointRCNN_         * DETR3D_                              (NeurIPS'2017)
+      (CVPR'2019)          (CoRL'2021)                        * PAConv_
+    * Part-A2_           * PETR_                                (CVPR'2021)
+      (TPAMI'2020)         (ECCV'2022)                        * DGCNN_
+    * CenterPoint_   Indoor                                     (TOG'2019)
+      (CVPR'2021)        * ImVoxelNet_
+    * PV-RCNN_             (WACV'2022)
       (CVPR'2020)
+    * CenterFormer_
+      (ECCV'2022)
 Indoor
     * VoteNet_
       (ICCV'2019)
     * H3DNet_
       (ECCV'2020)
     * Group-Free-3D_
       (ICCV'2021)
     * FCAF3D_
       (ECCV'2022)
-| | ResNet | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet |
-Cylinder3D | MinkUNet | | :-----------: | :----: | :--------: | :----: | :---:
-| :-----: | :-: | :--------: | :--------: | :------: | | SECOND | â | â |
-â | â | â | â | â | â | â | | PointPillars | â | â | â |
-â | â | â | â | â | â | | FreeAnchor | â | â | â | â | â
-| â | â | â | â | | VoteNet | â | â | â | â | â | â | â |
-â | â | | H3DNet | â | â | â | â | â | â | â | â | â | |
-3DSSD | â | â | â | â | â | â | â | â | â | | Part-A2 | â |
-â | â | â | â | â | â | â | â | | MVXNet | â | â | â |
-â | â | â | â | â | â | | CenterPoint | â | â | â | â | â
-| â | â | â | â | | SSN | â | â | â | â | â | â | â | â
-| â | | ImVoteNet | â | â | â | â | â | â | â | â | â | |
-FCOS3D | â | â | â | â | â | â | â | â | â | | PointNet++ |
-â | â | â | â | â | â | â | â | â | | Group-Free-3D | â |
-â | â | â | â | â | â | â | â | | ImVoxelNet | â | â | â
-| â | â | â | â | â | â | | PAConv | â | â | â | â | â |
-â | â | â | â | | DGCNN | â | â | â | â | â | â | â | â
-| â | | SMOKE | â | â | â | â | â | â | â | â | â | | PGD |
-â | â | â | â | â | â | â | â | â | | MonoFlex | â | â |
-â | â | â | â | â | â | â | | SA-SSD | â | â | â | â |
-â | â | â | â | â | | FCAF3D | â | â | â | â | â | â |
-â | â | â | | PV-RCNN | â | â | â | â | â | â | â | â |
-â | | Cylinder3D | â | â | â | â | â | â | â | â | â | |
-MinkUNet | â | â | â | â | â | â | â | â | â | | SPVCNN | â
-| â | â | â | â | â | â | â | â | **Note:** All the about
-**300+ models, methods of 40+ papers** in 2D detection supported by
-[MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/
-model_zoo.md) can be trained or used in this codebase. ## Installation Please
-refer to [get_started.md](docs/en/get_started.md) for installation. ## Get
-Started Please see [get_started.md](docs/en/get_started.md) for the basic usage
-of MMDetection3D. We provide guidance for quick run [with existing dataset]
-(docs/en/user_guides/train_test.md) and [with new dataset](docs/en/user_guides/
-2_new_data_model.md) for beginners. There are also tutorials for [learning
-configuration systems](docs/en/user_guides/config.md), [customizing dataset]
-(docs/en/advanced_guides/customize_dataset.md), [designing data pipeline](docs/
-en/user_guides/data_pipeline.md), [customizing models](docs/en/advanced_guides/
-customize_models.md), [customizing runtime settings](docs/en/advanced_guides/
-customize_runtime.md) and [Waymo dataset](docs/en/advanced_guides/datasets/
-waymo_det.md). Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked
-questions. When updating the version of MMDetection3D, please also check the
-[compatibility doc](docs/en/notes/compatibility.md) to be aware of the BC-
-breaking updates introduced in each version. ## Citation If you find this
-project useful in your research, please consider cite: ```latex @misc
-{mmdet3d2020, title={{MMDetection3D: OpenMMLab} next-generation platform for
-general {3D} object detection}, author={MMDetection3D Contributors},
-howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}}, year={2020}
-} ``` ## Contributing We appreciate all contributions to improve MMDetection3D.
-Please refer to [CONTRIBUTING.md](./docs/en/notes/contribution_guides.md) for
-the contributing guideline. ## Acknowledgement MMDetection3D is an open source
+    * TR3D_
+      (ArXiv'2023)
+| | ResNet | VoVNet | Swin-T | PointNet++ | SECOND | DGCNN | RegNetX | DLA |
+MinkResNet | Cylinder3D | MinkUNet | | :-----------: | :----: | :----: | :----:
+| :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :----
+--: | | SECOND | â | â | â | â | â | â | â | â | â | â |
+â | | PointPillars | â | â | â | â | â | â | â | â | â |
+â | â | | FreeAnchor | â | â | â | â | â | â | â | â | â
+| â | â | | VoteNet | â | â | â | â | â | â | â | â | â |
+â | â | | H3DNet | â | â | â | â | â | â | â | â | â |
+â | â | | 3DSSD | â | â | â | â | â | â | â | â | â | â
+| â | | Part-A2 | â | â | â | â | â | â | â | â | â | â |
+â | | MVXNet | â | â | â | â | â | â | â | â | â | â |
+â | | CenterPoint | â | â | â | â | â | â | â | â | â | â
+| â | | SSN | â | â | â | â | â | â | â | â | â | â | â
+| | ImVoteNet | â | â | â | â | â | â | â | â | â | â | â
+| | FCOS3D | â | â | â | â | â | â | â | â | â | â | â |
+| PointNet++ | â | â | â | â | â | â | â | â | â | â | â
+| | Group-Free-3D | â | â | â | â | â | â | â | â | â | â |
+â | | ImVoxelNet | â | â | â | â | â | â | â | â | â | â
+| â | | PAConv | â | â | â | â | â | â | â | â | â | â |
+â | | DGCNN | â | â | â | â | â | â | â | â | â | â | â
+| | SMOKE | â | â | â | â | â | â | â | â | â | â | â | |
+PGD | â | â | â | â | â | â | â | â | â | â | â | |
+MonoFlex | â | â | â | â | â | â | â | â | â | â | â | |
+SA-SSD | â | â | â | â | â | â | â | â | â | â | â | |
+FCAF3D | â | â | â | â | â | â | â | â | â | â | â | |
+PV-RCNN | â | â | â | â | â | â | â | â | â | â | â | |
+Cylinder3D | â | â | â | â | â | â | â | â | â | â | â |
+| MinkUNet | â | â | â | â | â | â | â | â | â | â | â |
+| SPVCNN | â | â | â | â | â | â | â | â | â | â | â | |
+BEVFusion | â | â | â | â | â | â | â | â | â | â | â | |
+CenterFormer | â | â | â | â | â | â | â | â | â | â | â
+| | TR3D | â | â | â | â | â | â | â | â | â | â | â | |
+DETR3D | â | â | â | â | â | â | â | â | â | â | â | |
+PETR | â | â | â | â | â | â | â | â | â | â | â | |
+TPVFormer | â | â | â | â | â | â | â | â | â | â | â |
+**Note:** All the about **500+ models, methods of 90+ papers** in 2D detection
+supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/
+docs/en/model_zoo.md) can be trained or used in this codebase. ## FAQ Please
+refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions. ##
+Contributing We appreciate all contributions to improve MMDetection3D. Please
+refer to [CONTRIBUTING.md](docs/en/notes/contribution_guides.md) for the
+contributing guideline. ## Acknowledgement MMDetection3D is an open source
 project that is contributed by researchers and engineers from various colleges
 and companies. We appreciate all the contributors as well as users who give
 valuable feedbacks. We wish that the toolbox and benchmark could serve the
 growing research community by providing a flexible toolkit to reimplement
-existing methods and develop their own new 3D detectors. ## Projects in
-OpenMMLab - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab
-foundational library for training deep learning models. - [MMCV](https://
-github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
-vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation
-library for multiple machine learning libraries. - [MIM](https://github.com/
-open-mmlab/mim): MIM installs OpenMMLab packages. - [MMPreTrain](https://
-github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+existing methods and develop their own new 3D detectors. ## Citation If you
+find this project useful in your research, please consider cite: ```latex @misc
+{mmdet3d2020, title={{MMDetection3D: OpenMMLab} next-generation platform for
+general {3D} object detection}, author={MMDetection3D Contributors},
+howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}}, year={2020}
+} ``` ## License This project is released under the [Apache 2.0 license]
+(LICENSE). ## Projects in OpenMMLab - [MMEngine](https://github.com/open-mmlab/
+mmengine): OpenMMLab foundational library for training deep learning models. -
+[MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for
+computer vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified
+evaluation library for multiple machine learning libraries. - [MIM](https://
+github.com/open-mmlab/mim): MIM installs OpenMMLab packages. - [MMPreTrain]
+(https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
 benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection):
 OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
 github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
 general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
 mmrotate): OpenMMLab rotated object detection toolbox and benchmark. - [MMYOLO]
 (https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and
 benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
@@ -179,8 +246,15 @@
 benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
 mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMagic](https:/
 /github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
 **I**ntelligent **C**reation toolbox. - [MMGeneration](https://github.com/open-
 mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
 [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
-framework.
+framework. Keywords: computer vision,3D object detection Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
+Content-Type: text/markdown Provides-Extra: all Provides-Extra: tests Provides-
+Extra: build Provides-Extra: optional Provides-Extra: mim
```

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/3dssd/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/3dssd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/lyft-3d-range100.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/nuim-instance.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/nus-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/s3dis-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/scannet-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/semantickitti.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         with_label_3d=False,
         with_seg_3d=True,
         seg_3d_dtype='np.int32',
         seg_offset=2**16,
         dataset_type='semantickitti',
         backend_args=backend_args),
     dict(type='PointSegClassMapping'),
-    dict(type='Pack3DDetInputs', keys=['points'])
+    dict(type='Pack3DDetInputs', keys=['points', 'pts_semantic_mask'])
 ]
 # construct a pipeline for data and gt loading in show function
 # please keep its loading function consistent with test_pipeline (e.g. client)
 eval_pipeline = [
     dict(
         type='LoadPointsFromFile',
         coord_type='LIDAR',
```

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-fov-mono3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv-mono3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/datasets/waymoD5-mv3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/default_runtime.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/3dssd.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/3dssd.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/cascade-mask-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/centerpoint_pillar02_second_secfpn_nus.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/centerpoint_voxel01_second_secfpn_nus.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/cylinder3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/cylinder3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/dgcnn.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/dgcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/fcaf3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/fcaf3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/fcos3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/fcos3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/groupfree3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/groupfree3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/h3dnet.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/h3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/imvotenet.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/imvotenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/mask-rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/minkunet.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/minkunet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/multiview_dfm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/paconv_ssg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/parta2.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/parta2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pgd.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pgd.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/point_rcnn.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/point_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointnet2_msg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointnet2_ssg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_lyft.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_nus.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_fpn_range100_lyft.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_kitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/pointpillars_hv_secfpn_waymo.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_kitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/second_hv_secfpn_waymo.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/smoke.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/smoke.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/spvcnn.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/spvcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/models/votenet.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/models/votenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/cosine.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/cosine.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/cyclic-20e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/cyclic-40e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/mmdet-schedule-1x.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/schedule-2x.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/schedule-3x.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-100e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-150e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-200e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/_base_/schedules/seg-cosine-50e.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_PartA2_secfpn_4x8_cyclic_80e_pcdet_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_3x8_100e_det3d_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_pointpillars_secfpn_4x8_80e_pcdet_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/benchmark/hv_second_secfpn_4x8_80e_pcdet_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_pillar02_second_secfpn_8xb4-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_8xb4-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn-circlenms_8xb4-flip-tta-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-flip-tta-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel0075_second_secfpn_head-dcn_8xb4-tta-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/centerpoint_voxel01_second_secfpn_8xb4-cyclic-20e_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/centerpoint/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/centerpoint/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/cylinder3d_4xb4-3x_semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/cylinder3d_4xb4-3x_semantickitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/cylinder3d_8xb2-laser-polar-mix-3x_semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/cylinder3d_8xb2-laser-polar-mix-3x_semantickitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/cylinder3d/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/cylinder3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_16xb2_waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dfm/multiview-dfm_r101-dcn_centerhead_16xb2_waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area1.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area3.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area4.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area5.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/dgcnn_4xb32-cosine-100e_s3dis-seg_test-area6.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dgcnn/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dgcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/pointpillars_dv_secfpn_8xb6-160e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb2-cosine-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/dynamic_voxelization/second_dv_secfpn_8xb6-80e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_s3dis-3d-5class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_scannet-3d-18class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/fcaf3d_2xb8_sunrgbd-3d-10class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/fcaf3d/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/fcaf3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/fcos3d/fcos3d_r101-caffe-dcn_fpn_head-gn_8xb2-1x_nus-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/fcos3d/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/fcos3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-1.6gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-3.2gf_fpn_head-free-anchor_sbn-all_8xb4-strong-aug-3x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/free_anchor/pointpillars_hv_regnet-400mf_fpn_head-free-anchor_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L12-O256_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_head-L6-O256_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O256_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/groupfree3d_w2x-head-L12-O512_4xb8_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/groupfree3d/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/groupfree3d/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/h3dnet/h3dnet_8xb3_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/h3dnet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/h3dnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/imvotenet_faster-rcnn-r50_fpn_4xb2_sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/imvotenet_stage2_8xb16_sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/imvotenet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/imvotenet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_2xb4_sunrgbd-3d-10class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_2xb4_sunrgbd-3d-10class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/imvoxelnet_8xb4_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/imvoxelnet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/imvoxelnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet18_w32_torchsparse_8xb2-amp-15e_semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet18_w32_torchsparse_8xb2-amp-15e_semantickitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/minkunet/minkunet34_w32_torchsparse_8xb2-laser-polar-mix-3x_semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/minkunet/minkunet34_w32_torchsparse_8xb2-laser-polar-mix-3x_semantickitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/monoflex/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/monoflex/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/mvxnet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/mvxnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/cascade-mask-rcnn_r50_fpn_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_r50_fpn_head-without-semantic_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/htc_x101_64x4d_fpn_dconv_c3-c5_coco-20e-1xb16_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_1x_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_caffe_fpn_coco-3x_20e_nuim.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/mask-rcnn_r50_fpn_coco-2x_1x_nus-2d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/nuimages/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/nuimages/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/paconv_ssg-cuda_8xb8-cosine-200e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/paconv/paconv_ssg_8xb8-cosine-150e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/parta2/parta2_hv_secfpn_8xb2-cyclic-80e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_16xb2-1x_nus-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101-caffe_fpn_head-gn_4xb3-4x_kitti-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-fov-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pgd/pgd_r101_fpn-head_dcn_16xb3_waymoD5-mv-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/point_rcnn/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/point_rcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/point_rcnn/point-rcnn_8xb2_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg-xyz-only.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-250e_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_msg_2xb16-cosine-80e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg-xyz-only.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-200e_scannet-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointnet2/pointnet2_ssg_2xb16-cosine-50e_s3dis-seg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_8xb6-160e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymo-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d-range100.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pointpillars/pointpillars_hv_secfpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pv_rcnn/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pv_rcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-1.6gf_fpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_fpn_sbn-all_range100_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_8xb4-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/regnet/pointpillars_hv_regnet-400mf_secfpn_sbn-all_range100_8xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/second/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/second/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_8xb6-80e_kitti-3d-car.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/second/second_hv_secfpn_sbn-all_16xb2-2x_waymoD5-3d-3class.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/smoke/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/smoke/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/smoke/smoke_dla34_dlaneck_gn-all_4xb8-6x_kitti-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-15e_semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-15e_semantickitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-laser-polar-mix-3x_semantickitti.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/spvcnn/spvcnn_w32_8xb2-amp-laser-polar-mix-3x_semantickitti.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb1-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_regnet-400mf_secfpn_sbn-all_16xb2-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_lyft-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/ssn/ssn_hv_secfpn_sbn-all_16xb2-2x_nus-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/metafile.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/votenet_8xb16_sunrgbd-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py` & `mmdet3d-1.2.0/mmdet3d/.mim/configs/votenet/votenet_8xb8_scannet-3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/model-index.yml` & `mmdet3d-1.2.0/mmdet3d/.mim/model-index.yml`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/benchmark.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/analysis_tools/get_flops.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/create_data.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/create_data.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/create_data.sh` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/create_data.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/create_gt_database.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/indoor_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/kitti_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/lyft_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/semantickitti_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/semantickitti_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/dataset_converters/waymo_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/mmdet3d_handler.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/deployment/test_torchserver.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/deployment/test_torchserver.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/browse_dataset.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/fuse_conv_bn.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/print_config.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/misc/visualize_results.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/misc/visualize_results.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/convert_h3dnet_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/convert_votenet_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/publish_model.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/model_converters/regnet2mmdet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/slurm_test.sh` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/slurm_train.sh` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/test.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/test.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/train.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/train.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/update_data_coords.py` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/update_data_coords.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/.mim/tools/update_data_coords.sh` & `mmdet3d-1.2.0/mmdet3d/.mim/tools/update_data_coords.sh`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/__init__.py` & `mmdet3d-1.2.0/mmdet3d/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 from .version import __version__, version_info
 
 mmcv_minimum_version = '2.0.0rc4'
 mmcv_maximum_version = '2.1.0'
 mmcv_version = digit_version(mmcv.__version__)
 
-mmengine_minimum_version = '0.7.1'
+mmengine_minimum_version = '0.8.0'
 mmengine_maximum_version = '1.0.0'
 mmengine_version = digit_version(mmengine.__version__)
 
 mmdet_minimum_version = '3.0.0'
-mmdet_maximum_version = '3.1.0'
+mmdet_maximum_version = '3.2.0'
 mmdet_version = digit_version(mmdet.__version__)
 
 assert (mmcv_version >= digit_version(mmcv_minimum_version)
         and mmcv_version < digit_version(mmcv_maximum_version)), \
     f'MMCV=={mmcv.__version__} is used but incompatible. ' \
     f'Please install mmcv>={mmcv_minimum_version}, <{mmcv_maximum_version}.'
```

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/__init__.py` & `mmdet3d-1.2.0/mmdet3d/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/inference.py` & `mmdet3d-1.2.0/mmdet3d/apis/inference.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/inferencers/base_3d_inferencer.py` & `mmdet3d-1.2.0/mmdet3d/apis/inferencers/base_3d_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/inferencers/lidar_det3d_inferencer.py` & `mmdet3d-1.2.0/mmdet3d/apis/inferencers/lidar_det3d_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/inferencers/lidar_seg3d_inferencer.py` & `mmdet3d-1.2.0/mmdet3d/apis/inferencers/lidar_seg3d_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/inferencers/mono_det3d_inferencer.py` & `mmdet3d-1.2.0/mmdet3d/apis/inferencers/mono_det3d_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/apis/inferencers/multi_modality_det3d_inferencer.py` & `mmdet3d-1.2.0/mmdet3d/apis/inferencers/multi_modality_det3d_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/__init__.py` & `mmdet3d-1.2.0/mmdet3d/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/convert_utils.py` & `mmdet3d-1.2.0/mmdet3d/datasets/convert_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/dataset_wrappers.py` & `mmdet3d-1.2.0/mmdet3d/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/det3d_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/det3d_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/kitti2d_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/kitti2d_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/kitti_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/kitti_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/lyft_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/lyft_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/nuscenes_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/nuscenes_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/s3dis_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/s3dis_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/scannet_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/scannet_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/seg3d_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/seg3d_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/semantickitti_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/semantickitti_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/sunrgbd_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/sunrgbd_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/__init__.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/data_augment_utils.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/data_augment_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/dbsampler.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/dbsampler.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/formating.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/formating.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
                             'img_norm_cfg', 'num_pts_feats', 'pcd_trans',
                             'sample_idx', 'pcd_scale_factor', 'pcd_rotation',
                             'pcd_rotation_angle', 'lidar_path',
                             'transformation_3d_flow', 'trans_mat',
                             'affine_aug', 'sweep_img_metas', 'ori_cam2img',
                             'cam2global', 'crop_offset', 'img_crop_offset',
                             'resize_img_shape', 'lidar2cam', 'ori_lidar2img',
-                            'num_ref_frames', 'num_views', 'ego2global')
+                            'num_ref_frames', 'num_views', 'ego2global',
+                            'axis_align_matrix')
     ) -> None:
         self.keys = keys
         self.meta_keys = meta_keys
 
     def _remove_prefix(self, key: str) -> str:
         if key.startswith('gt_'):
             key = key[3:]
```

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/loading.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -575,38 +575,42 @@
         use_dim (list[int] | int): Which dimensions of the points to use.
             Defaults to [0, 1, 2]. For KITTI dataset, set use_dim=4
             or use_dim=[0, 1, 2, 3] to use the intensity dimension.
         shift_height (bool): Whether to use shifted height. Defaults to False.
         use_color (bool): Whether to use color features. Defaults to False.
         norm_intensity (bool): Whether to normlize the intensity. Defaults to
             False.
+        norm_elongation (bool): Whether to normlize the elongation. This is
+            usually used in Waymo dataset.Defaults to False.
         backend_args (dict, optional): Arguments to instantiate the
             corresponding backend. Defaults to None.
     """
 
     def __init__(self,
                  coord_type: str,
                  load_dim: int = 6,
                  use_dim: Union[int, List[int]] = [0, 1, 2],
                  shift_height: bool = False,
                  use_color: bool = False,
                  norm_intensity: bool = False,
+                 norm_elongation: bool = False,
                  backend_args: Optional[dict] = None) -> None:
         self.shift_height = shift_height
         self.use_color = use_color
         if isinstance(use_dim, int):
             use_dim = list(range(use_dim))
         assert max(use_dim) < load_dim, \
             f'Expect all used dimensions < {load_dim}, got {use_dim}'
         assert coord_type in ['CAMERA', 'LIDAR', 'DEPTH']
 
         self.coord_type = coord_type
         self.load_dim = load_dim
         self.use_dim = use_dim
         self.norm_intensity = norm_intensity
+        self.norm_elongation = norm_elongation
         self.backend_args = backend_args
 
     def _load_points(self, pts_filename: str) -> np.ndarray:
         """Private function to load point clouds data.
 
         Args:
             pts_filename (str): Filename of point clouds data.
@@ -642,14 +646,18 @@
         points = self._load_points(pts_file_path)
         points = points.reshape(-1, self.load_dim)
         points = points[:, self.use_dim]
         if self.norm_intensity:
             assert len(self.use_dim) >= 4, \
                 f'When using intensity norm, expect used dimensions >= 4, got {len(self.use_dim)}'  # noqa: E501
             points[:, 3] = np.tanh(points[:, 3])
+        if self.norm_elongation:
+            assert len(self.use_dim) >= 5, \
+                f'When using elongation norm, expect used dimensions >= 5, got {len(self.use_dim)}'  # noqa: E501
+            points[:, 4] = np.tanh(points[:, 4])
         attribute_dims = None
 
         if self.shift_height:
             floor_height = np.percentile(points[:, 2], 0.99)
             height = points[:, 2] - floor_height
             points = np.concatenate(
                 [points[:, :3],
@@ -678,14 +686,16 @@
         """str: Return a string that describes the module."""
         repr_str = self.__class__.__name__ + '('
         repr_str += f'shift_height={self.shift_height}, '
         repr_str += f'use_color={self.use_color}, '
         repr_str += f'backend_args={self.backend_args}, '
         repr_str += f'load_dim={self.load_dim}, '
         repr_str += f'use_dim={self.use_dim})'
+        repr_str += f'norm_intensity={self.norm_intensity})'
+        repr_str += f'norm_elongation={self.norm_elongation})'
         return repr_str
 
 
 @TRANSFORMS.register_module()
 class LoadPointsFromDict(LoadPointsFromFile):
     """Load Points From Dict."""
```

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/test_time_aug.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/transforms/transforms_3d.py` & `mmdet3d-1.2.0/mmdet3d/datasets/transforms/transforms_3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/utils.py` & `mmdet3d-1.2.0/mmdet3d/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/datasets/waymo_dataset.py` & `mmdet3d-1.2.0/mmdet3d/datasets/waymo_dataset.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/engine/hooks/benchmark_hook.py` & `mmdet3d-1.2.0/mmdet3d/engine/hooks/benchmark_hook.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/engine/hooks/disable_object_sample_hook.py` & `mmdet3d-1.2.0/mmdet3d/engine/hooks/disable_object_sample_hook.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/engine/hooks/visualization_hook.py` & `mmdet3d-1.2.0/mmdet3d/engine/hooks/visualization_hook.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 from typing import Optional, Sequence
 
 import mmcv
 import numpy as np
 from mmengine.fileio import get
 from mmengine.hooks import Hook
+from mmengine.logging import print_log
 from mmengine.runner import Runner
 from mmengine.utils import mkdir_or_exist
 from mmengine.visualization import Visualizer
 
 from mmdet3d.registry import HOOKS
 from mmdet3d.structures import Det3DDataSample
 
@@ -38,47 +39,64 @@
             it means that no drawing will be done. Defaults to False.
         interval (int): The interval of visualization. Defaults to 50.
         score_thr (float): The threshold to visualize the bboxes
             and masks. Defaults to 0.3.
         show (bool): Whether to display the drawn image. Default to False.
         vis_task (str): Visualization task. Defaults to 'mono_det'.
         wait_time (float): The interval of show (s). Defaults to 0.
+        draw_gt (bool): Whether to draw ground truth. Defaults to True.
+        draw_pred (bool): Whether to draw prediction. Defaults to True.
+        show_pcd_rgb (bool): Whether to show RGB point cloud. Defaults to
+            False.
         test_out_dir (str, optional): directory where painted images
             will be saved in testing process.
         backend_args (dict, optional): Arguments to instantiate the
             corresponding backend. Defaults to None.
     """
 
     def __init__(self,
                  draw: bool = False,
                  interval: int = 50,
                  score_thr: float = 0.3,
                  show: bool = False,
                  vis_task: str = 'mono_det',
                  wait_time: float = 0.,
                  test_out_dir: Optional[str] = None,
+                 draw_gt: bool = False,
+                 draw_pred: bool = True,
+                 show_pcd_rgb: bool = False,
                  backend_args: Optional[dict] = None):
         self._visualizer: Visualizer = Visualizer.get_current_instance()
         self.interval = interval
         self.score_thr = score_thr
         self.show = show
         if self.show:
             # No need to think about vis backends.
             self._visualizer._vis_backends = {}
             warnings.warn('The show is True, it means that only '
                           'the prediction results are visualized '
                           'without storing data, so vis_backends '
                           'needs to be excluded.')
         self.vis_task = vis_task
 
+        if wait_time == -1:
+            print_log(
+                'Manual control mode, press [Right] to next sample.',
+                logger='current')
+        else:
+            print_log(
+                'Autoplay mode, press [SPACE] to pause.', logger='current')
         self.wait_time = wait_time
         self.backend_args = backend_args
         self.draw = draw
         self.test_out_dir = test_out_dir
         self._test_index = 0
+        self.draw_gt = draw_gt
+        self.draw_pred = draw_pred
+        self.show_pcd_rgb = show_pcd_rgb
 
     def after_val_iter(self, runner: Runner, batch_idx: int, data_batch: dict,
                        outputs: Sequence[Det3DDataSample]) -> None:
         """Run after every ``self.interval`` validation iterations.
 
         Args:
             runner (:obj:`Runner`): The runner of the validation process.
@@ -126,19 +144,22 @@
             data_input['points'] = points
 
         if total_curr_iter % self.interval == 0:
             self._visualizer.add_datasample(
                 'val sample',
                 data_input,
                 data_sample=outputs[0],
+                draw_gt=self.draw_gt,
+                draw_pred=self.draw_pred,
                 show=self.show,
                 vis_task=self.vis_task,
                 wait_time=self.wait_time,
                 pred_score_thr=self.score_thr,
-                step=total_curr_iter)
+                step=total_curr_iter,
+                show_pcd_rgb=self.show_pcd_rgb)
 
     def after_test_iter(self, runner: Runner, batch_idx: int, data_batch: dict,
                         outputs: Sequence[Det3DDataSample]) -> None:
         """Run after every testing iterations.
 
         Args:
             runner (:obj:`Runner`): The runner of the testing process.
@@ -204,14 +225,17 @@
                         '.')[0] + '.png'
                     o3d_save_path = osp.join(self.test_out_dir, o3d_save_path)
 
             self._visualizer.add_datasample(
                 'test sample',
                 data_input,
                 data_sample=data_sample,
+                draw_gt=self.draw_gt,
+                draw_pred=self.draw_pred,
                 show=self.show,
                 vis_task=self.vis_task,
                 wait_time=self.wait_time,
                 pred_score_thr=self.score_thr,
                 out_file=out_file,
                 o3d_save_path=o3d_save_path,
-                step=self._test_index)
+                step=self._test_index,
+                show_pcd_rgb=self.show_pcd_rgb)
```

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/__init__.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/__init__.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/indoor_eval.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/indoor_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/instance_seg_eval.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/instance_seg_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/kitti_utils/eval.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/kitti_utils/eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/kitti_utils/rotate_iou.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/lyft_eval.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/lyft_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/panoptic_seg_eval.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/panoptic_seg_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/scannet_utils/evaluate_semantic_instance.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/scannet_utils/util_3d.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/scannet_utils/util_3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/seg_eval.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/seg_eval.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/functional/waymo_utils/prediction_to_waymo.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/__init__.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/indoor_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/indoor_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/instance_seg_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/instance_seg_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/kitti_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/kitti_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/lyft_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/lyft_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/nuscenes_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/nuscenes_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/panoptic_seg_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/panoptic_seg_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/seg_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/seg_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/evaluation/metrics/waymo_metric.py` & `mmdet3d-1.2.0/mmdet3d/evaluation/metrics/waymo_metric.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/base_pointnet.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/base_pointnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/cylinder3d.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/cylinder3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/dgcnn.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/dgcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/dla.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/dla.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/mink_resnet.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/mink_resnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/minkunet_backbone.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/minkunet_backbone.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/multi_backbone.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/multi_backbone.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/nostem_regnet.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/nostem_regnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/pointnet2_sa_msg.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/pointnet2_sa_msg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/pointnet2_sa_ssg.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/pointnet2_sa_ssg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/second.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/second.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/backbones/spvcnn_backone.py` & `mmdet3d-1.2.0/mmdet3d/models/backbones/spvcnn_backone.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/data_preprocessor.py` & `mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/utils.py` & `mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/data_preprocessors/voxelize.py` & `mmdet3d-1.2.0/mmdet3d/models/data_preprocessors/voxelize.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/decode_heads/cylinder3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/decode_heads/cylinder3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/decode_heads/decode_head.py` & `mmdet3d-1.2.0/mmdet3d/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/decode_heads/dgcnn_head.py` & `mmdet3d-1.2.0/mmdet3d/models/decode_heads/dgcnn_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/decode_heads/minkunet_head.py` & `mmdet3d-1.2.0/mmdet3d/models/decode_heads/minkunet_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/decode_heads/paconv_head.py` & `mmdet3d-1.2.0/mmdet3d/models/decode_heads/paconv_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/decode_heads/pointnet2_head.py` & `mmdet3d-1.2.0/mmdet3d/models/decode_heads/pointnet2_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/anchor3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/anchor3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/anchor_free_mono3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/base_3d_dense_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/base_3d_dense_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/base_conv_bbox_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/base_conv_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/base_mono3d_dense_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/base_mono3d_dense_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/centerpoint_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/centerpoint_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/fcaf3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/fcaf3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/fcos_mono3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/fcos_mono3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/free_anchor3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/free_anchor3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/groupfree3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/groupfree3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/imvoxel_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/imvoxel_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/monoflex_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/monoflex_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/parta2_rpn_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/parta2_rpn_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/pgd_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/pgd_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/point_rpn_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/point_rpn_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/shape_aware_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/shape_aware_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/smoke_mono3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/smoke_mono3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/ssd_3d_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/ssd_3d_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/train_mixins.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/train_mixins.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/dense_heads/vote_head.py` & `mmdet3d-1.2.0/mmdet3d/models/dense_heads/vote_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/base.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/base.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/centerpoint.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/centerpoint.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/dfm.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/dfm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/dynamic_voxelnet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/dynamic_voxelnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/fcos_mono3d.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/fcos_mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/groupfree3dnet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/groupfree3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/h3dnet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/h3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/imvotenet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/imvotenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/imvoxelnet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/imvoxelnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/mink_single_stage.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/mink_single_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/multiview_dfm.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/multiview_dfm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/mvx_faster_rcnn.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/mvx_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/mvx_two_stage.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/mvx_two_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/parta2.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/parta2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/point_rcnn.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/point_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/pv_rcnn.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/pv_rcnn.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/sassd.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/sassd.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/single_stage.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/single_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/single_stage_mono3d.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/single_stage_mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/smoke_mono3d.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/smoke_mono3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/ssd3dnet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/ssd3dnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/two_stage.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/two_stage.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/votenet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/votenet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/detectors/voxelnet.py` & `mmdet3d-1.2.0/mmdet3d/models/detectors/voxelnet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/box3d_nms.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/box3d_nms.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/dgcnn_fa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/dgcnn_fp_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/dgcnn_modules/dgcnn_gf_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/edge_fusion_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/edge_fusion_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/coord_transform.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/coord_transform.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/point_fusion.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/point_fusion.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/fusion_layers/vote_fusion.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/fusion_layers/vote_fusion.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/minkowski_engine_block.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/minkowski_engine_block.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/mlp.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/norm.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/norm.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/paconv/paconv.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/paconv/paconv.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/paconv/utils.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/paconv/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/builder.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/builder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/paconv_sa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/point_fp_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/point_fp_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/point_sa_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/point_sa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/pointnet_modules/stack_point_sa_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/sparse_block.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/sparse_block.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/spconv/overwrite_spconv/write_spconv2.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/torchsparse/torchsparse_wrapper.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/torchsparse/torchsparse_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/torchsparse_block.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/torchsparse_block.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/transformer.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/layers/vote_module.py` & `mmdet3d-1.2.0/mmdet3d/models/layers/vote_module.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/axis_aligned_iou_loss.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/axis_aligned_iou_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/chamfer_distance.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/lovasz_loss.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/multibin_loss.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/multibin_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/paconv_regularization_loss.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/paconv_regularization_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/rotated_iou_loss.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/rotated_iou_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/losses/uncertain_smooth_l1_loss.py` & `mmdet3d-1.2.0/mmdet3d/models/losses/uncertain_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/middle_encoders/pillar_scatter.py` & `mmdet3d-1.2.0/mmdet3d/models/middle_encoders/pillar_scatter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/middle_encoders/sparse_encoder.py` & `mmdet3d-1.2.0/mmdet3d/models/middle_encoders/sparse_encoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/middle_encoders/sparse_unet.py` & `mmdet3d-1.2.0/mmdet3d/models/middle_encoders/sparse_unet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/middle_encoders/voxel_set_abstraction.py` & `mmdet3d-1.2.0/mmdet3d/models/middle_encoders/voxel_set_abstraction.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/necks/dla_neck.py` & `mmdet3d-1.2.0/mmdet3d/models/necks/dla_neck.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/necks/imvoxel_neck.py` & `mmdet3d-1.2.0/mmdet3d/models/necks/imvoxel_neck.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/necks/pointnet2_fp_neck.py` & `mmdet3d-1.2.0/mmdet3d/models/necks/pointnet2_fp_neck.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/necks/second_fpn.py` & `mmdet3d-1.2.0/mmdet3d/models/necks/second_fpn.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,15 +70,16 @@
                 dict(type='Constant', layer='NaiveSyncBatchNorm2d', val=1.0)
             ]
 
     def forward(self, x):
         """Forward function.
 
         Args:
-            x (torch.Tensor): 4D Tensor in (N, C, H, W) shape.
+            x (List[torch.Tensor]): Multi-level features with 4D Tensor in
+                (N, C, H, W) shape.
 
         Returns:
             list[torch.Tensor]: Multi-level feature maps.
         """
         assert len(x) == len(self.in_channels)
         ups = [deblock(x[i]) for i, deblock in enumerate(self.deblocks)]
```

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/base_3droi_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/base_3droi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/h3d_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/parta2_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/point_rcnn_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/bbox_heads/pv_rcnn_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/h3d_roi_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/h3d_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/foreground_segmentation_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/pointwise_semantic_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/mask_heads/primitive_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/mask_heads/primitive_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/part_aggregation_roi_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/part_aggregation_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/point_rcnn_roi_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/point_rcnn_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/pv_rcnn_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/batch_roigridpoint_extractor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/single_roiaware_extractor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py` & `mmdet3d-1.2.0/mmdet3d/models/roi_heads/roi_extractors/single_roipoint_extractor.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/segmentors/base.py` & `mmdet3d-1.2.0/mmdet3d/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/segmentors/cylinder3d.py` & `mmdet3d-1.2.0/mmdet3d/models/segmentors/cylinder3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/segmentors/encoder_decoder.py` & `mmdet3d-1.2.0/mmdet3d/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/segmentors/minkunet.py` & `mmdet3d-1.2.0/mmdet3d/models/segmentors/minkunet.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/segmentors/seg3d_tta.py` & `mmdet3d-1.2.0/mmdet3d/models/segmentors/seg3d_tta.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/anchor_3d_generator.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/anchor/builder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/anchor/builder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/assigners/max_3d_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/builder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/builder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/anchor_free_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/centerpoint_bbox_coders.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/delta_xyzwhlr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/fcos3d_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/groupfree3d_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/monoflex_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/partial_bin_based_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/pgd_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/point_xyzwhlr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/coders/smoke_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/iou_neg_piecewise_sampler.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/samplers/pseudosample.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/samplers/pseudosample.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/task_modules/voxel/voxel_generator.py` & `mmdet3d-1.2.0/mmdet3d/models/task_modules/voxel/voxel_generator.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/test_time_augs/merge_augs.py` & `mmdet3d-1.2.0/mmdet3d/models/test_time_augs/merge_augs.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/utils/__init__.py` & `mmdet3d-1.2.0/mmdet3d/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/utils/edge_indices.py` & `mmdet3d-1.2.0/mmdet3d/models/utils/edge_indices.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/utils/gaussian.py` & `mmdet3d-1.2.0/mmdet3d/models/utils/gaussian.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/utils/gen_keypoints.py` & `mmdet3d-1.2.0/mmdet3d/models/utils/gen_keypoints.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/utils/handle_objs.py` & `mmdet3d-1.2.0/mmdet3d/models/utils/handle_objs.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/pillar_encoder.py` & `mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/pillar_encoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/utils.py` & `mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/models/voxel_encoders/voxel_encoder.py` & `mmdet3d-1.2.0/mmdet3d/models/voxel_encoders/voxel_encoder.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/registry.py` & `mmdet3d-1.2.0/mmdet3d/registry.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/__init__.py` & `mmdet3d-1.2.0/mmdet3d/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/__init__.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/base_box3d.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/base_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/box_3d_mode.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/box_3d_mode.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/cam_box3d.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/cam_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/coord_3d_mode.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/coord_3d_mode.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/depth_box3d.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/depth_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/lidar_box3d.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/lidar_box3d.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/bbox_3d/utils.py` & `mmdet3d-1.2.0/mmdet3d/structures/bbox_3d/utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/det3d_data_sample.py` & `mmdet3d-1.2.0/mmdet3d/structures/det3d_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/ops/__init__.py` & `mmdet3d-1.2.0/mmdet3d/structures/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/ops/box_np_ops.py` & `mmdet3d-1.2.0/mmdet3d/structures/ops/box_np_ops.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/ops/iou3d_calculator.py` & `mmdet3d-1.2.0/mmdet3d/structures/ops/iou3d_calculator.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/ops/transforms.py` & `mmdet3d-1.2.0/mmdet3d/structures/ops/transforms.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/point_data.py` & `mmdet3d-1.2.0/mmdet3d/structures/point_data.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/points/__init__.py` & `mmdet3d-1.2.0/mmdet3d/structures/points/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/points/base_points.py` & `mmdet3d-1.2.0/mmdet3d/structures/points/base_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/points/cam_points.py` & `mmdet3d-1.2.0/mmdet3d/structures/points/cam_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/points/depth_points.py` & `mmdet3d-1.2.0/mmdet3d/structures/points/depth_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/structures/points/lidar_points.py` & `mmdet3d-1.2.0/mmdet3d/structures/points/lidar_points.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/testing/__init__.py` & `mmdet3d-1.2.0/mmdet3d/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/testing/data_utils.py` & `mmdet3d-1.2.0/mmdet3d/testing/data_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/testing/model_utils.py` & `mmdet3d-1.2.0/mmdet3d/testing/model_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/__init__.py` & `mmdet3d-1.2.0/mmdet3d/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/array_converter.py` & `mmdet3d-1.2.0/mmdet3d/utils/array_converter.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/collect_env.py` & `mmdet3d-1.2.0/mmdet3d/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/compat_cfg.py` & `mmdet3d-1.2.0/mmdet3d/utils/compat_cfg.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/misc.py` & `mmdet3d-1.2.0/mmdet3d/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/setup_env.py` & `mmdet3d-1.2.0/mmdet3d/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/utils/typing_utils.py` & `mmdet3d-1.2.0/mmdet3d/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d/version.py` & `mmdet3d-1.2.0/mmdet3d/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) Open-MMLab. All rights reserved.
 
-__version__ = '1.1.1'
+__version__ = '1.2.0'
 short_version = __version__
 
 
 def parse_version_info(version_str: str) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
```

### Comparing `mmdet3d-1.1.1/mmdet3d/visualization/local_visualizer.py` & `mmdet3d-1.2.0/mmdet3d/visualization/local_visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 import math
+import sys
 import time
 from typing import List, Optional, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import mmcv
 import numpy as np
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 from mmdet.visualization import DetLocalVisualizer, get_palette
 from mmengine.dist import master_only
+from mmengine.logging import print_log
 from mmengine.structures import InstanceData
 from mmengine.visualization import Visualizer as MMENGINE_Visualizer
 from mmengine.visualization.utils import (check_type, color_val_matplotlib,
                                           tensor2ndarray)
 from torch import Tensor
 
 from mmdet3d.registry import VISUALIZERS
 from mmdet3d.structures import (BaseInstance3DBoxes, Box3DMode,
                                 CameraInstance3DBoxes, Coord3DMode,
-                                DepthInstance3DBoxes, Det3DDataSample,
-                                LiDARInstance3DBoxes, PointData,
-                                points_cam2img)
+                                DepthInstance3DBoxes, DepthPoints,
+                                Det3DDataSample, LiDARInstance3DBoxes,
+                                PointData, points_cam2img)
 from .vis_utils import (proj_camera_bbox3d_to_img, proj_depth_bbox3d_to_img,
                         proj_lidar_bbox3d_to_img, to_depth_mode)
 
 try:
     import open3d as o3d
     from open3d import geometry
     from open3d.visualization import Visualizer
@@ -132,44 +134,54 @@
             bbox_color=bbox_color,
             text_color=text_color,
             mask_color=mask_color,
             line_width=line_width,
             alpha=alpha)
         if points is not None:
             self.set_points(points, pcd_mode=pcd_mode, frame_cfg=frame_cfg)
-        self.pts_seg_num = 0
         self.multi_imgs_col = multi_imgs_col
         self.fig_show_cfg.update(fig_show_cfg)
 
+        self.flag_pause = False
+        self.flag_next = False
+        self.flag_exit = False
+
     def _clear_o3d_vis(self) -> None:
         """Clear open3d vis."""
 
         if hasattr(self, 'o3d_vis'):
             del self.o3d_vis
-            del self.pcd
             del self.points_colors
+            del self.view_control
+            if hasattr(self, 'pcd'):
+                del self.pcd
 
-    def _initialize_o3d_vis(self, frame_cfg: dict) -> Visualizer:
+    def _initialize_o3d_vis(self) -> Visualizer:
         """Initialize open3d vis according to frame_cfg.
 
         Args:
             frame_cfg (dict): The config to create coordinate frame in open3d
                 vis.
 
         Returns:
             :obj:`o3d.visualization.Visualizer`: Created open3d vis.
         """
         if o3d is None or geometry is None:
             raise ImportError(
                 'Please run "pip install open3d" to install open3d first.')
-        o3d_vis = o3d.visualization.Visualizer()
+        glfw_key_escape = 256  # Esc
+        glfw_key_space = 32  # Space
+        glfw_key_right = 262  # Right
+        o3d_vis = o3d.visualization.VisualizerWithKeyCallback()
+        o3d_vis.register_key_callback(glfw_key_escape, self.escape_callback)
+        o3d_vis.register_key_action_callback(glfw_key_space,
+                                             self.space_action_callback)
+        o3d_vis.register_key_callback(glfw_key_right, self.right_callback)
         o3d_vis.create_window()
-        # create coordinate frame
-        mesh_frame = geometry.TriangleMesh.create_coordinate_frame(**frame_cfg)
-        o3d_vis.add_geometry(mesh_frame)
+        self.view_control = o3d_vis.get_view_control()
         return o3d_vis
 
     @master_only
     def set_points(self,
                    points: np.ndarray,
                    pcd_mode: int = 0,
                    vis_mode: str = 'replace',
@@ -201,15 +213,15 @@
                 ['xyz', 'xyzrgb']. Defaults to 'xyz'.
         """
         assert points is not None
         assert vis_mode in ('replace', 'add')
         check_type('points', points, np.ndarray)
 
         if not hasattr(self, 'o3d_vis'):
-            self.o3d_vis = self._initialize_o3d_vis(frame_cfg)
+            self.o3d_vis = self._initialize_o3d_vis()
 
         # for now we convert points into depth mode for visualization
         if pcd_mode != Coord3DMode.DEPTH:
             points = Coord3DMode.convert(points, pcd_mode, Coord3DMode.DEPTH)
 
         if hasattr(self, 'pcd') and vis_mode != 'add':
             self.o3d_vis.remove_geometry(self.pcd)
@@ -231,14 +243,18 @@
             points_colors = points[:, 3:6]
             # normalize to [0, 1] for Open3D drawing
             if not ((points_colors >= 0.0) & (points_colors <= 1.0)).all():
                 points_colors /= 255.0
         else:
             raise NotImplementedError
 
+        # create coordinate frame
+        mesh_frame = geometry.TriangleMesh.create_coordinate_frame(**frame_cfg)
+        self.o3d_vis.add_geometry(mesh_frame)
+
         pcd.colors = o3d.utility.Vector3dVector(points_colors)
         self.o3d_vis.add_geometry(pcd)
         self.pcd = pcd
         self.points_colors = points_colors
 
     # TODO: assign 3D Box color according to pred / GT labels
     # We draw GT / pred bboxes on the same point cloud scenes
@@ -273,15 +289,15 @@
 
         if not isinstance(bboxes_3d, DepthInstance3DBoxes):
             bboxes_3d = bboxes_3d.convert_to(Box3DMode.DEPTH)
 
         # convert bboxes to numpy dtype
         bboxes_3d = tensor2ndarray(bboxes_3d.tensor)
 
-        in_box_color = np.array(points_in_box_color)
+        # in_box_color = np.array(points_in_box_color)
 
         for i in range(len(bboxes_3d)):
             center = bboxes_3d[i, 0:3]
             dim = bboxes_3d[i, 3:6]
             yaw = np.zeros(3)
             yaw[rot_axis] = bboxes_3d[i, 6]
             rot_mat = geometry.get_rotation_matrix_from_xyz(yaw)
@@ -300,15 +316,15 @@
             # draw bboxes on visualizer
             self.o3d_vis.add_geometry(line_set)
 
             # change the color of points which are in box
             if self.pcd is not None and mode == 'xyz':
                 indices = box3d.get_point_indices_within_bounding_box(
                     self.pcd.points)
-                self.points_colors[indices] = in_box_color
+                self.points_colors[indices] = np.array(bbox_color[i]) / 255.
 
         # update points colors
         if self.pcd is not None:
             self.pcd.colors = o3d.utility.Vector3dVector(self.points_colors)
             self.o3d_vis.update_geometry(self.pcd)
 
     def set_bev_image(self,
@@ -568,39 +584,44 @@
             seg_mask_colors (np.ndarray): The segmentation mask with shape
                 (N, 6), whose first 3 dims are point coordinates and last 3
                 dims are converted colors.
         """
         # we can't draw the colors on existing points
         # in case gt and pred mask would overlap
         # instead we set a large offset along x-axis for each seg mask
-        self.pts_seg_num += 1
-        offset = (np.array(self.pcd.points).max(0) -
-                  np.array(self.pcd.points).min(0))[0] * 1.2 * self.pts_seg_num
-        mesh_frame = geometry.TriangleMesh.create_coordinate_frame(
-            size=1, origin=[offset, 0, 0])  # create coordinate frame for seg
-        self.o3d_vis.add_geometry(mesh_frame)
+        if hasattr(self, 'pcd'):
+            offset = (np.array(self.pcd.points).max(0) -
+                      np.array(self.pcd.points).min(0))[0] * 1.2
+            mesh_frame = geometry.TriangleMesh.create_coordinate_frame(
+                size=1, origin=[offset, 0,
+                                0])  # create coordinate frame for seg
+            self.o3d_vis.add_geometry(mesh_frame)
+        else:
+            offset = 0
         seg_points = copy.deepcopy(seg_mask_colors)
         seg_points[:, 0] += offset
         self.set_points(seg_points, pcd_mode=2, vis_mode='add', mode='xyzrgb')
 
     def _draw_instances_3d(self,
                            data_input: dict,
                            instances: InstanceData,
                            input_meta: dict,
                            vis_task: str,
+                           show_pcd_rgb: bool = False,
                            palette: Optional[List[tuple]] = None) -> dict:
         """Draw 3D instances of GT or prediction.
 
         Args:
             data_input (dict): The input dict to draw.
             instances (:obj:`InstanceData`): Data structure for instance-level
                 annotations or predictions.
             input_meta (dict): Meta information.
             vis_task (str): Visualization task, it includes: 'lidar_det',
                 'multi-modality_det', 'mono_det'.
+            show_pcd_rgb (bool): Whether to show RGB point cloud.
             palette (List[tuple], optional): Palette information corresponding
                 to the category. Defaults to None.
 
         Returns:
             dict: The drawn point cloud and image whose channel is RGB.
         """
 
@@ -620,21 +641,30 @@
             points = tensor2ndarray(points)
 
             if not isinstance(bboxes_3d, DepthInstance3DBoxes):
                 points, bboxes_3d_depth = to_depth_mode(points, bboxes_3d)
             else:
                 bboxes_3d_depth = bboxes_3d.clone()
 
+            if 'axis_align_matrix' in input_meta:
+                points = DepthPoints(points, points_dim=points.shape[1])
+                rot_mat = input_meta['axis_align_matrix'][:3, :3]
+                trans_vec = input_meta['axis_align_matrix'][:3, -1]
+                points.rotate(rot_mat.T)
+                points.translate(trans_vec)
+                points = tensor2ndarray(points.tensor)
+
             max_label = int(max(labels_3d) if len(labels_3d) > 0 else 0)
             bbox_color = palette if self.bbox_color is None \
                 else self.bbox_color
             bbox_palette = get_palette(bbox_color, max_label + 1)
             colors = [bbox_palette[label] for label in labels_3d]
 
-            self.set_points(points, pcd_mode=2)
+            self.set_points(
+                points, pcd_mode=2, mode='xyzrgb' if show_pcd_rgb else 'xyz')
             self.draw_bboxes_3d(bboxes_3d_depth, bbox_color=colors)
 
             data_3d['bboxes_3d'] = tensor2ndarray(bboxes_3d_depth.tensor)
             data_3d['points'] = points
 
         if vis_task in ['mono_det', 'multi-modality_det']:
             assert 'img' in data_input
@@ -712,15 +742,15 @@
 
         return data_3d
 
     def _draw_pts_sem_seg(self,
                           points: Union[Tensor, np.ndarray],
                           pts_seg: PointData,
                           palette: Optional[List[tuple]] = None,
-                          ignore_index: Optional[int] = None) -> None:
+                          keep_index: Optional[int] = None) -> None:
         """Draw 3D semantic mask of GT or prediction.
 
         Args:
             points (Tensor or np.ndarray): The input point cloud to draw.
             pts_seg (:obj:`PointData`): Data structure for pixel-level
                 annotations or predictions.
             palette (List[tuple], optional): Palette information corresponding
@@ -729,32 +759,32 @@
         """
         check_type('points', points, (np.ndarray, Tensor))
 
         points = tensor2ndarray(points)
         pts_sem_seg = tensor2ndarray(pts_seg.pts_semantic_mask)
         palette = np.array(palette)
 
-        if ignore_index is not None:
-            points = points[pts_sem_seg != ignore_index]
-            pts_sem_seg = pts_sem_seg[pts_sem_seg != ignore_index]
+        if keep_index is not None:
+            keep_index = tensor2ndarray(keep_index)
+            points = points[keep_index]
+            pts_sem_seg = pts_sem_seg[keep_index]
 
         pts_color = palette[pts_sem_seg]
         seg_color = np.concatenate([points[:, :3], pts_color], axis=1)
 
-        self.set_points(points, pcd_mode=2, vis_mode='add')
         self.draw_seg_mask(seg_color)
 
     @master_only
     def show(self,
              save_path: Optional[str] = None,
              drawn_img_3d: Optional[np.ndarray] = None,
              drawn_img: Optional[np.ndarray] = None,
              win_name: str = 'image',
-             wait_time: int = 0,
-             continue_key: str = ' ',
+             wait_time: int = -1,
+             continue_key: str = 'right',
              vis_task: str = 'lidar_det') -> None:
         """Show the drawn point cloud/image.
 
         Args:
             save_path (str, optional): Path to save open3d visualized results.
                 Defaults to None.
             drawn_img_3d (np.ndarray, optional): The image to show. If
@@ -764,53 +794,134 @@
                 is not None, it will show the image got by Visualizer.
                 Defaults to None.
             win_name (str): The image title. Defaults to 'image'.
             wait_time (int): Delay in milliseconds. 0 is the special value that
                 means "forever". Defaults to 0.
             continue_key (str): The key for users to continue. Defaults to ' '.
         """
-        if vis_task == 'multi-modality_det':
-            img_wait_time = 0.5
-        else:
-            img_wait_time = wait_time
 
         # In order to show multi-modal results at the same time, we show image
         # firstly and then show point cloud since the running of
         # Open3D will block the process
         if hasattr(self, '_image'):
             if drawn_img is None and drawn_img_3d is None:
                 # use the image got by Visualizer.get_image()
-                super().show(drawn_img_3d, win_name, img_wait_time,
-                             continue_key)
-            else:
-                if drawn_img_3d is not None:
-                    super().show(drawn_img_3d, win_name, img_wait_time,
-                                 continue_key)
-                if drawn_img is not None:
-                    super().show(drawn_img, win_name, img_wait_time,
+                if vis_task == 'multi-modality_det':
+                    import matplotlib.pyplot as plt
+                    is_inline = 'inline' in plt.get_backend()
+                    img = self.get_image() if drawn_img is None else drawn_img
+                    self._init_manager(win_name)
+                    fig = self.manager.canvas.figure
+                    # remove white edges by set subplot margin
+                    fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
+                    fig.clear()
+                    ax = fig.add_subplot()
+                    ax.axis(False)
+                    ax.imshow(img)
+                    self.manager.canvas.draw()
+                    if is_inline:
+                        return fig
+                    else:
+                        fig.show()
+                    self.manager.canvas.flush_events()
+                else:
+                    super().show(drawn_img_3d, win_name, wait_time,
                                  continue_key)
+            else:
+                if vis_task == 'multi-modality_det':
+                    import matplotlib.pyplot as plt
+                    is_inline = 'inline' in plt.get_backend()
+                    img = drawn_img if drawn_img_3d is None else drawn_img_3d
+                    self._init_manager(win_name)
+                    fig = self.manager.canvas.figure
+                    # remove white edges by set subplot margin
+                    fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
+                    fig.clear()
+                    ax = fig.add_subplot()
+                    ax.axis(False)
+                    ax.imshow(img)
+                    self.manager.canvas.draw()
+                    if is_inline:
+                        return fig
+                    else:
+                        fig.show()
+                    self.manager.canvas.flush_events()
+                else:
+                    if drawn_img_3d is not None:
+                        super().show(drawn_img_3d, win_name, wait_time,
+                                     continue_key)
+                    if drawn_img is not None:
+                        super().show(drawn_img, win_name, wait_time,
+                                     continue_key)
 
         if hasattr(self, 'o3d_vis'):
-            self.o3d_vis.poll_events()
+            if hasattr(self, 'view_port'):
+                self.view_control.convert_from_pinhole_camera_parameters(
+                    self.view_port)
+            self.flag_exit = not self.o3d_vis.poll_events()
             self.o3d_vis.update_renderer()
-            if wait_time > 0:
-                time.sleep(wait_time)
+            self.view_port = \
+                self.view_control.convert_to_pinhole_camera_parameters()  # noqa: E501
+            if wait_time != -1:
+                self.last_time = time.time()
+                while time.time(
+                ) - self.last_time < wait_time and self.o3d_vis.poll_events():
+                    self.o3d_vis.update_renderer()
+                    self.view_port = \
+                        self.view_control.convert_to_pinhole_camera_parameters()  # noqa: E501
+                while self.flag_pause and self.o3d_vis.poll_events():
+                    self.o3d_vis.update_renderer()
+                    self.view_port = \
+                        self.view_control.convert_to_pinhole_camera_parameters()  # noqa: E501
+
             else:
-                self.o3d_vis.run()
+                while not self.flag_next and self.o3d_vis.poll_events():
+                    self.o3d_vis.update_renderer()
+                    self.view_port = \
+                        self.view_control.convert_to_pinhole_camera_parameters()  # noqa: E501
+                self.flag_next = False
+            self.o3d_vis.clear_geometries()
+            try:
+                del self.pcd
+            except (KeyError, AttributeError):
+                pass
             if save_path is not None:
                 if not (save_path.endswith('.png')
                         or save_path.endswith('.jpg')):
                     save_path += '.png'
                 self.o3d_vis.capture_screen_image(save_path)
-
-            # TODO: support more flexible window control
-            self.o3d_vis.clear_geometries()
-            self.o3d_vis.destroy_window()
-            self.o3d_vis.close()
-            self._clear_o3d_vis()
+            if self.flag_exit:
+                self.o3d_vis.destroy_window()
+                self.o3d_vis.close()
+                self._clear_o3d_vis()
+                sys.exit(0)
+
+    def escape_callback(self, vis):
+        self.o3d_vis.clear_geometries()
+        self.o3d_vis.destroy_window()
+        self.o3d_vis.close()
+        self._clear_o3d_vis()
+        sys.exit(0)
+
+    def space_action_callback(self, vis, action, mods):
+        if action == 1:
+            if self.flag_pause:
+                print_log(
+                    'Playback continued, press [SPACE] to pause.',
+                    logger='current')
+            else:
+                print_log(
+                    'Playback paused, press [SPACE] to continue.',
+                    logger='current')
+            self.flag_pause = not self.flag_pause
+        return True
+
+    def right_callback(self, vis):
+        self.flag_next = True
+        return False
 
     # TODO: Support Visualize the 3D results from image and point cloud
     # respectively
     @master_only
     def add_datasample(self,
                        name: str,
                        data_input: dict,
@@ -819,15 +930,16 @@
                        draw_pred: bool = True,
                        show: bool = False,
                        wait_time: float = 0,
                        out_file: Optional[str] = None,
                        o3d_save_path: Optional[str] = None,
                        vis_task: str = 'mono_det',
                        pred_score_thr: float = 0.3,
-                       step: int = 0) -> None:
+                       step: int = 0,
+                       show_pcd_rgb: bool = False) -> None:
         """Draw datasample and save to all backends.
 
         - If GT and prediction are plotted at the same time, they are displayed
           in a stitched image where the left image is the ground truth and the
           right image is the prediction.
         - If ``show`` is True, all storage backends are ignored, and the images
           will be displayed in a local window.
@@ -850,33 +962,39 @@
             out_file (str, optional): Path to output file. Defaults to None.
             o3d_save_path (str, optional): Path to save open3d visualized
                 results. Defaults to None.
             vis_task (str): Visualization task. Defaults to 'mono_det'.
             pred_score_thr (float): The threshold to visualize the bboxes
                 and masks. Defaults to 0.3.
             step (int): Global step value to record. Defaults to 0.
+            show_pcd_rgb (bool): Whether to show RGB point cloud. Defaults to
+                False.
         """
         assert vis_task in (
             'mono_det', 'multi-view_det', 'lidar_det', 'lidar_seg',
             'multi-modality_det'), f'got unexpected vis_task {vis_task}.'
         classes = self.dataset_meta.get('classes', None)
         # For object detection datasets, no palette is saved
         palette = self.dataset_meta.get('palette', None)
         ignore_index = self.dataset_meta.get('ignore_index', None)
+        if ignore_index is not None and 'gt_pts_seg' in data_sample and vis_task == 'lidar_seg':  # noqa: E501
+            keep_index = data_sample.gt_pts_seg.pts_semantic_mask != ignore_index  # noqa: E501
+        else:
+            keep_index = None
 
         gt_data_3d = None
         pred_data_3d = None
         gt_img_data = None
         pred_img_data = None
 
         if draw_gt and data_sample is not None:
             if 'gt_instances_3d' in data_sample:
                 gt_data_3d = self._draw_instances_3d(
                     data_input, data_sample.gt_instances_3d,
-                    data_sample.metainfo, vis_task, palette)
+                    data_sample.metainfo, vis_task, show_pcd_rgb, palette)
             if 'gt_instances' in data_sample:
                 if len(data_sample.gt_instances) > 0:
                     assert 'img' in data_input
                     img = data_input['img']
                     if isinstance(data_input['img'], Tensor):
                         img = data_input['img'].permute(1, 2, 0).numpy()
                         img = img[..., [2, 1, 0]]  # bgr to rgb
@@ -886,27 +1004,28 @@
                 assert classes is not None, 'class information is ' \
                                             'not provided when ' \
                                             'visualizing semantic ' \
                                             'segmentation results.'
                 assert 'points' in data_input
                 self._draw_pts_sem_seg(data_input['points'],
                                        data_sample.gt_pts_seg, palette,
-                                       ignore_index)
+                                       keep_index)
 
         if draw_pred and data_sample is not None:
             if 'pred_instances_3d' in data_sample:
                 pred_instances_3d = data_sample.pred_instances_3d
                 # .cpu can not be used for BaseInstance3DBoxes
                 # so we need to use .to('cpu')
                 pred_instances_3d = pred_instances_3d[
                     pred_instances_3d.scores_3d > pred_score_thr].to('cpu')
                 pred_data_3d = self._draw_instances_3d(data_input,
                                                        pred_instances_3d,
                                                        data_sample.metainfo,
-                                                       vis_task, palette)
+                                                       vis_task, show_pcd_rgb,
+                                                       palette)
             if 'pred_instances' in data_sample:
                 if 'img' in data_input and len(data_sample.pred_instances) > 0:
                     pred_instances = data_sample.pred_instances
                     pred_instances = pred_instances[
                         pred_instances.scores > pred_score_thr].cpu()
                     img = data_input['img']
                     if isinstance(data_input['img'], Tensor):
@@ -918,15 +1037,15 @@
                 assert classes is not None, 'class information is ' \
                                             'not provided when ' \
                                             'visualizing semantic ' \
                                             'segmentation results.'
                 assert 'points' in data_input
                 self._draw_pts_sem_seg(data_input['points'],
                                        data_sample.pred_pts_seg, palette,
-                                       ignore_index)
+                                       keep_index)
 
         # monocular 3d object detection image
         if vis_task in ['mono_det', 'multi-modality_det']:
             if gt_data_3d is not None and pred_data_3d is not None:
                 drawn_img_3d = np.concatenate(
                     (gt_data_3d['img'], pred_data_3d['img']), axis=1)
             elif gt_data_3d is not None:
```

### Comparing `mmdet3d-1.1.1/mmdet3d/visualization/vis_utils.py` & `mmdet3d-1.2.0/mmdet3d/visualization/vis_utils.py`

 * *Files identical despite different names*

### Comparing `mmdet3d-1.1.1/mmdet3d.egg-info/PKG-INFO` & `mmdet3d-1.2.0/mmdet3d.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdet3d
-Version: 1.1.1
+Version: 1.2.0
 Summary: OpenMMLab's next-generation platformfor general 3D object detection.
 Home-page: https://github.com/open-mmlab/mmdetection3d
 Author: MMDetection3D Contributors
 Author-email: zwwdev@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmdet3d-logo.png" width="600"/>
@@ -22,21 +22,35 @@
               <a href="https://platform.openmmlab.com">
                 <i><font size="4">TRY IT OUT</font></i>
               </a>
             </sup>
           </div>
           <div>&nbsp;</div>
         
+        [![PyPI](https://img.shields.io/pypi/v/mmdet3d)](https://pypi.org/project/mmdet3d)
         [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdetection3d.readthedocs.io/en/latest/)
         [![badge](https://github.com/open-mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdetection3d/actions)
-        [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
-        [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/LICENSE)
+        [![codecov](https://codecov.io/gh/open-mmlab/mmdetection3d/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdetection3d)
+        [![license](https://img.shields.io/github/license/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/main/LICENSE)
+        [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+        [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+        
+        [📘Documentation](https://mmdetection3d.readthedocs.io/en/latest/) |
+        [🛠️Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html) |
+        [👀Model Zoo](https://mmdetection3d.readthedocs.io/en/latest/model_zoo.html) |
+        [🆕Update News](https://mmdetection3d.readthedocs.io/en/latest/notes/changelog.html) |
+        [🚀Ongoing Projects](https://github.com/open-mmlab/mmdetection3d/projects) |
+        [🤔Reporting Issues](https://github.com/open-mmlab/mmdetection3d/issues/new/choose)
         
         </div>
         
+        <div align="center">
+        
+        English | [简体中文](README_zh-CN.md)
+        
         </div>
         
         <div align="center">
           <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://discord.com/channels/1037617289144569886/1046608014234370059" style="text-decoration:none;">
@@ -51,44 +65,32 @@
           <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
           <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
           <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
             <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
         </div>
         
-        **News**:
-        
-        **We have renamed the branch `1.1`  to `main` and switched the default branch from `master` to `main`. We encourage
-        users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](docs/en/migration.md) for more details.**
-        
-        **v1.1.1** was released in 30/5/2023
-        
-        We have constructed a comprehensive LiDAR semantic segmentation benchmark on SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy, the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of SemanticKITTI. We have also supported the training of BEVFusion and an occupancy prediction method, TPVFomrer, in our `projects`. More new features about 3D perception are on the way. Please stay tuned!
-        
         ## Introduction
         
-        English | [简体中文](README_zh-CN.md)
+        MMDetection3D is an open source object detection toolbox based on PyTorch, towards the next-generation platform for general 3D detection. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
         
         The main branch works with **PyTorch 1.8+**.
         
-        MMDetection3D is an open source object detection toolbox based on PyTorch, towards the next-generation platform for general 3D detection. It is
-        a part of the OpenMMLab project developed by [MMLab](http://mmlab.ie.cuhk.edu.hk/).
-        
         ![demo image](resources/mmdet3d_outdoor_demo.gif)
         
-        ### Major features
+        <details open>
+        <summary>Major features</summary>
         
         - **Support multi-modality/single-modality detectors out of box**
         
           It directly supports multi-modality/single-modality detectors including MVXNet, VoteNet, PointPillars, etc.
         
         - **Support indoor/outdoor 3D detection out of box**
         
-          It directly supports popular indoor and outdoor 3D detection datasets, including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI.
-          For nuScenes dataset, we also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/nuimages).
+          It directly supports popular indoor and outdoor 3D detection datasets, including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes dataset, we also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/nuimages).
         
         - **Natural integration with 2D detection**
         
           All the about **300+ models, methods of 40+ papers**, and modules supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
         
         - **High efficiency**
         
@@ -98,27 +100,85 @@
           | :-----------------: | :-----------: | :--------------------------------------------------: | :----------------------------------------------------: | :-----------------------------------------: |
           |       VoteNet       |      358      |                          ✗                           |                           77                           |                      ✗                      |
           |  PointPillars-car   |      141      |                          ✗                           |                           ✗                            |                     140                     |
           | PointPillars-3class |      107      |                          44                          |                           ✗                            |                      ✗                      |
           |       SECOND        |      40       |                          30                          |                           ✗                            |                      ✗                      |
           |       Part-A2       |      17       |                          14                          |                           ✗                            |                      ✗                      |
         
+        </details>
+        
         Like [MMDetection](https://github.com/open-mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv), MMDetection3D can also be used as a library to support different projects on top of it.
         
-        ## License
+        ## What's New
         
-        This project is released under the [Apache 2.0 license](LICENSE).
+        ### Highlight
+        
+        **We have renamed the branch `1.1` to `main` and switched the default branch from `master` to `main`. We encourage users to migrate to the latest version, though it comes with some cost. Please refer to [Migration Guide](docs/en/migration.md) for more details.**
+        
+        We have constructed a comprehensive LiDAR semantic segmentation benchmark on SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy, the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of SemanticKITTI. We have also supported the training of BEVFusion and an occupancy prediction method, TPVFomrer, in our `projects`. More new features about 3D perception are on the way. Please stay tuned!
+        
+        **v1.2.0** was released in 4/7/2023
         
-        ## Changelog
+        - Support [New Config Type](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-beta) in `mmdet3d/config`
+        - Support the inference of [DSVT](<(https://arxiv.org/abs/2301.06051)>) in `projects`
+        - Support downloading datasets from [OpenDataLab](https://opendatalab.com/) using `mim`
         
-        **1.1.0** was released in 6/4/2023.
+        **v1.1.1** was released in 30/5/2023:
         
-        Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
+        - Support [TPVFormer](https://arxiv.org/pdf/2302.07817.pdf) in `projects`
+        - Support the training of BEVFusion in `projects`
+        - Support lidar-based 3D semantic segmentation benchmark
         
-        ## Benchmark and model zoo
+        ## Installation
+        
+        Please refer to [Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html) for installation instructions.
+        
+        ## Getting Started
+        
+        For detailed user guides and advanced guides, please refer to our [documentation](https://mmdetection3d.readthedocs.io/en/latest/):
+        
+        <details>
+        <summary>User Guides</summary>
+        
+        - [Train & Test](https://mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#train-test)
+          - [Learn about Configs](https://mmdetection3d.readthedocs.io/en/latest/user_guides/config.html)
+          - [Coordinate System](https://mmdetection3d.readthedocs.io/en/latest/user_guides/coord_sys_tutorial.html)
+          - [Dataset Preparation](https://mmdetection3d.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
+          - [Customize Data Pipelines](https://mmdetection3d.readthedocs.io/en/latest/user_guides/data_pipeline.html)
+          - [Test and Train on Standard Datasets](https://mmdetection3d.readthedocs.io/en/latest/user_guides/train_test.html)
+          - [Inference](https://mmdetection3d.readthedocs.io/en/latest/user_guides/inference.html)
+          - [Train with Customized Datasets](https://mmdetection3d.readthedocs.io/en/latest/user_guides/new_data_model.html)
+        - [Useful Tools](https://mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#useful-tools)
+        
+        </details>
+        
+        <details>
+        <summary>Advanced Guides</summary>
+        
+        - [Datasets](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#datasets)
+          - [KITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/kitti.html)
+          - [NuScenes Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/nuscenes.html)
+          - [Lyft Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/lyft.html)
+          - [Waymo Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/waymo.html)
+          - [SUN RGB-D Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/sunrgbd.html)
+          - [ScanNet Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/scannet.html)
+          - [S3DIS Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/s3dis.html)
+          - [SemanticKITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/semantickitti.html)
+        - [Supported Tasks](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#supported-tasks)
+          - [LiDAR-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/lidar_det3d.html)
+          - [Vision-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/vision_det3d.html)
+          - [LiDAR-Based 3D Semantic Segmentation](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/supported_tasks/lidar_sem_seg3d.html)
+        - [Customization](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#customization)
+          - [Customize Datasets](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_dataset.html)
+          - [Customize Models](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_models.html)
+          - [Customize Runtime Settings](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_runtime.html)
+        
+        </details>
+        
+        ## Overview of Benchmark and Model Zoo
         
         Results and models are available in the [model zoo](docs/en/model_zoo.md).
         
         <div align="center">
           <b>Components</b>
         </div>
         <table align="center">
@@ -166,18 +226,18 @@
         <div align="center">
           <b>Architectures</b>
         </div>
         <table align="center">
           <tbody>
             <tr align="center" valign="middle">
               <td>
-                <b>3D Object Detection</b>
+                <b>LiDAR-based 3D Object Detection</b>
               </td>
               <td>
-                <b>Monocular 3D Object Detection</b>
+                <b>Camera-based 3D Object Detection</b>
               </td>
               <td>
                 <b>Multi-modal 3D Object Detection</b>
               </td>
               <td>
                 <b>3D Semantic Segmentation</b>
               </td>
@@ -191,53 +251,59 @@
                     <li><a href="configs/ssn">SSN (ECCV'2020)</a></li>
                     <li><a href="configs/3dssd">3DSSD (CVPR'2020)</a></li>
                     <li><a href="configs/sassd">SA-SSD (CVPR'2020)</a></li>
                     <li><a href="configs/point_rcnn">PointRCNN (CVPR'2019)</a></li>
                     <li><a href="configs/parta2">Part-A2 (TPAMI'2020)</a></li>
                     <li><a href="configs/centerpoint">CenterPoint (CVPR'2021)</a></li>
                     <li><a href="configs/pv_rcnn">PV-RCNN (CVPR'2020)</a></li>
+                    <li><a href="projects/CenterFormer">CenterFormer (ECCV'2022)</a></li>
                 </ul>
                 <li><b>Indoor</b></li>
                 <ul>
                     <li><a href="configs/votenet">VoteNet (ICCV'2019)</a></li>
                     <li><a href="configs/h3dnet">H3DNet (ECCV'2020)</a></li>
                     <li><a href="configs/groupfree3d">Group-Free-3D (ICCV'2021)</a></li>
                     <li><a href="configs/fcaf3d">FCAF3D (ECCV'2022)</a></li>
+                    <li><a href="projects/TR3D">TR3D (ArXiv'2023)</a></li>
               </ul>
               </td>
               <td>
                 <li><b>Outdoor</b></li>
                 <ul>
                   <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
                   <li><a href="configs/smoke">SMOKE (CVPRW'2020)</a></li>
                   <li><a href="configs/fcos3d">FCOS3D (ICCVW'2021)</a></li>
                   <li><a href="configs/pgd">PGD (CoRL'2021)</a></li>
                   <li><a href="configs/monoflex">MonoFlex (CVPR'2021)</a></li>
+                  <li><a href="projects/DETR3D">DETR3D (CoRL'2021)</a></li>
+                  <li><a href="projects/PETR">PETR (ECCV'2022)</a></li>
                 </ul>
                 <li><b>Indoor</b></li>
                 <ul>
                   <li><a href="configs/imvoxelnet">ImVoxelNet (WACV'2022)</a></li>
                 </ul>
               </td>
               <td>
                 <li><b>Outdoor</b></li>
                 <ul>
                   <li><a href="configs/mvxnet">MVXNet (ICRA'2019)</a></li>
+                  <li><a href="projects/BEVFusion">BEVFusion (ICRA'2023)</a></li>
                 </ul>
                 <li><b>Indoor</b></li>
                 <ul>
                   <li><a href="configs/imvotenet">ImVoteNet (CVPR'2020)</a></li>
                 </ul>
               </td>
               <td>
                 <li><b>Outdoor</b></li>
                 <ul>
                   <li><a href="configs/minkunet">MinkUNet (CVPR'2019)</a></li>
                   <li><a href="configs/spvcnn">SPVCNN (ECCV'2020)</a></li>
                   <li><a href="configs/cylinder3d">Cylinder3D (CVPR'2021)</a></li>
+                  <li><a href="projects/TPVFormer">TPVFormer (CVPR'2023)</a></li>
                 </ul>
                 <li><b>Indoor</b></li>
                 <ul>
                   <li><a href="configs/pointnet2">PointNet++ (NeurIPS'2017)</a></li>
                   <li><a href="configs/paconv">PAConv (CVPR'2021)</a></li>
                   <li><a href="configs/dgcnn">DGCNN (TOG'2019)</a></li>
                 </ul>
@@ -245,76 +311,79 @@
               </td>
             </tr>
         </td>
             </tr>
           </tbody>
         </table>
         
-        |               | ResNet | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet | Cylinder3D | MinkUNet |
-        | :-----------: | :----: | :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :------: |
-        |    SECOND     |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        | PointPillars  |   ✗    |     ✗      |   ✓    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  FreeAnchor   |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    VoteNet    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    H3DNet     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |     3DSSD     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    Part-A2    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    MVXNet     |   ✓    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  CenterPoint  |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |      SSN      |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |   ImVoteNet   |   ✓    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    FCOS3D     |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  PointNet++   |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        | Group-Free-3D |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  ImVoxelNet   |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    PAConv     |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |     DGCNN     |   ✗    |     ✗      |   ✗    |   ✓   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |     SMOKE     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
-        |      PGD      |   ✓    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |   MonoFlex    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
-        |    SA-SSD     |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |    FCAF3D     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
-        |    PV-RCNN    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
-        |  Cylinder3D   |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✓      |    ✗     |
-        |   MinkUNet    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
-        |    SPVCNN     |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+        |               | ResNet | VoVNet | Swin-T | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet | Cylinder3D | MinkUNet |
+        | :-----------: | :----: | :----: | :----: | :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :------: |
+        |    SECOND     |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        | PointPillars  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  FreeAnchor   |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    VoteNet    |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    H3DNet     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     3DSSD     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    Part-A2    |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    MVXNet     |   ✓    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  CenterPoint  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |      SSN      |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✓    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |   ImVoteNet   |   ✓    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    FCOS3D     |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  PointNet++   |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        | Group-Free-3D |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  ImVoxelNet   |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    PAConv     |   ✗    |   ✗    |   ✗    |     ✓      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     DGCNN     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✓   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     SMOKE     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
+        |      PGD      |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |   MonoFlex    |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✓  |     ✗      |     ✗      |    ✗     |
+        |    SA-SSD     |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |    FCAF3D     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
+        |    PV-RCNN    |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |  Cylinder3D   |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✓      |    ✗     |
+        |   MinkUNet    |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+        |    SPVCNN     |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✓     |
+        |   BEVFusion   |   ✗    |   ✗    |   ✓    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        | CenterFormer  |   ✗    |   ✗    |   ✗    |     ✗      |   ✓    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     TR3D      |   ✗    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✓      |     ✗      |    ✗     |
+        |    DETR3D     |   ✓    |   ✓    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |     PETR      |   ✗    |   ✓    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
+        |   TPVFormer   |   ✓    |   ✗    |   ✗    |     ✗      |   ✗    |   ✗   |    ✗    |  ✗  |     ✗      |     ✗      |    ✗     |
         
-        **Note:** All the about **300+ models, methods of 40+ papers** in 2D detection supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
+        **Note:** All the about **500+ models, methods of 90+ papers** in 2D detection supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/model_zoo.md) can be trained or used in this codebase.
         
-        ## Installation
+        ## FAQ
         
-        Please refer to [get_started.md](docs/en/get_started.md) for installation.
+        Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions.
         
-        ## Get Started
+        ## Contributing
+        
+        We appreciate all contributions to improve MMDetection3D. Please refer to [CONTRIBUTING.md](docs/en/notes/contribution_guides.md) for the contributing guideline.
         
-        Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMDetection3D. We provide guidance for quick run [with existing dataset](docs/en/user_guides/train_test.md) and [with new dataset](docs/en/user_guides/2_new_data_model.md) for beginners. There are also tutorials for [learning configuration systems](docs/en/user_guides/config.md), [customizing dataset](docs/en/advanced_guides/customize_dataset.md), [designing data pipeline](docs/en/user_guides/data_pipeline.md), [customizing models](docs/en/advanced_guides/customize_models.md), [customizing runtime settings](docs/en/advanced_guides/customize_runtime.md) and [Waymo dataset](docs/en/advanced_guides/datasets/waymo_det.md).
+        ## Acknowledgement
         
-        Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions. When updating the version of MMDetection3D, please also check the [compatibility doc](docs/en/notes/compatibility.md) to be aware of the BC-breaking updates introduced in each version.
+        MMDetection3D is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors as well as users who give valuable feedbacks. We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and develop their own new 3D detectors.
         
         ## Citation
         
         If you find this project useful in your research, please consider cite:
         
         ```latex
         @misc{mmdet3d2020,
             title={{MMDetection3D: OpenMMLab} next-generation platform for general {3D} object detection},
             author={MMDetection3D Contributors},
             howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}},
             year={2020}
         }
         ```
         
-        ## Contributing
-        
-        We appreciate all contributions to improve MMDetection3D. Please refer to [CONTRIBUTING.md](./docs/en/notes/contribution_guides.md) for the contributing guideline.
-        
-        ## Acknowledgement
+        ## License
         
-        MMDetection3D is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors as well as users who give valuable feedbacks.
-        We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and develop their own new 3D detectors.
+        This project is released under the [Apache 2.0 license](LICENSE).
         
         ## Projects in OpenMMLab
         
         - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
         - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
         - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
```

#### html2text {}

```diff
@@ -1,171 +1,234 @@
-Metadata-Version: 2.1 Name: mmdet3d Version: 1.1.1 Summary: OpenMMLab's next-
+Metadata-Version: 2.1 Name: mmdet3d Version: 1.2.0 Summary: OpenMMLab's next-
 generation platformfor general 3D object detection. Home-page: https://
 github.com/open-mmlab/mmdetection3d Author: MMDetection3D Contributors Author-
 email: zwwdev@gmail.com License: Apache License 2.0 Description:
                          [resources/mmdet3d-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
-       [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
+  [![PyPI](https://img.shields.io/pypi/v/mmdet3d)](https://pypi.org/project/
+  mmdet3d) [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
   mmdetection3d.readthedocs.io/en/latest/) [![badge](https://github.com/open-
 mmlab/mmdetection3d/workflows/build/badge.svg)](https://github.com/open-mmlab/
      mmdetection3d/actions) [![codecov](https://codecov.io/gh/open-mmlab/
-mmdetection3d/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
+ mmdetection3d/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
  mmdetection3d) [![license](https://img.shields.io/github/license/open-mmlab/
- mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/master/
-                                   LICENSE)
+  mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/blob/main/
+  LICENSE) [![open issues](https://isitmaintained.com/badge/open/open-mmlab/
+  mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues) [!
+  [issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/
+   mmdetection3d.svg)](https://github.com/open-mmlab/mmdetection3d/issues)
+    [ðDocumentation](https://mmdetection3d.readthedocs.io/en/latest/) |
+     [ð ï¸Installation](https://mmdetection3d.readthedocs.io/en/latest/
+ get_started.html) | [ðModel Zoo](https://mmdetection3d.readthedocs.io/en/
+              latest/model_zoo.html) | [ðUpdate News](https://
+  mmdetection3d.readthedocs.io/en/latest/notes/changelog.html) | [ðOngoing
+      Projects](https://github.com/open-mmlab/mmdetection3d/projects) |
+[ð¤Reporting Issues](https://github.com/open-mmlab/mmdetection3d/issues/new/
+                                    choose)
+                   English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
-**News**: **We have renamed the branch `1.1` to `main` and switched the default
-branch from `master` to `main`. We encourage users to migrate to the latest
-version, though it comes with some cost. Please refer to [Migration Guide]
-(docs/en/migration.md) for more details.** **v1.1.1** was released in 30/5/2023
-We have constructed a comprehensive LiDAR semantic segmentation benchmark on
-SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy,
-the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of
-SemanticKITTI. We have also supported the training of BEVFusion and an
-occupancy prediction method, TPVFomrer, in our `projects`. More new features
-about 3D perception are on the way. Please stay tuned! ## Introduction English
-| [ç®ä½ä¸­æ](README_zh-CN.md) The main branch works with **PyTorch 1.8+**.
-MMDetection3D is an open source object detection toolbox based on PyTorch,
-towards the next-generation platform for general 3D detection. It is a part of
-the OpenMMLab project developed by [MMLab](http://mmlab.ie.cuhk.edu.hk/). !
-[demo image](resources/mmdet3d_outdoor_demo.gif) ### Major features - **Support
-multi-modality/single-modality detectors out of box** It directly supports
-multi-modality/single-modality detectors including MVXNet, VoteNet,
-PointPillars, etc. - **Support indoor/outdoor 3D detection out of box** It
-directly supports popular indoor and outdoor 3D detection datasets, including
-ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes dataset, we
-also support [nuImages dataset](https://github.com/open-mmlab/mmdetection3d/
-tree/main/configs/nuimages). - **Natural integration with 2D detection** All
-the about **300+ models, methods of 40+ papers**, and modules supported in
-[MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/
-model_zoo.md) can be trained or used in this codebase. - **High efficiency** It
-trains faster than other codebases. The main results are as below. Details can
-be found in [benchmark.md](./docs/en/notes/benchmarks.md). We compare the
-number of samples trained per second (the higher, the better). The models that
-are not supported by other codebases are marked by `â`. | Methods |
-MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet) |
-[votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://
+## Introduction MMDetection3D is an open source object detection toolbox based
+on PyTorch, towards the next-generation platform for general 3D detection. It
+is a part of the [OpenMMLab](https://openmmlab.com/) project. The main branch
+works with **PyTorch 1.8+**. ![demo image](resources/mmdet3d_outdoor_demo.gif)
+Major features - **Support multi-modality/single-modality detectors out of
+box** It directly supports multi-modality/single-modality detectors including
+MVXNet, VoteNet, PointPillars, etc. - **Support indoor/outdoor 3D detection out
+of box** It directly supports popular indoor and outdoor 3D detection datasets,
+including ScanNet, SUNRGB-D, Waymo, nuScenes, Lyft, and KITTI. For nuScenes
+dataset, we also support [nuImages dataset](https://github.com/open-mmlab/
+mmdetection3d/tree/main/configs/nuimages). - **Natural integration with 2D
+detection** All the about **300+ models, methods of 40+ papers**, and modules
+supported in [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/
+docs/en/model_zoo.md) can be trained or used in this codebase. - **High
+efficiency** It trains faster than other codebases. The main results are as
+below. Details can be found in [benchmark.md](./docs/en/notes/benchmarks.md).
+We compare the number of samples trained per second (the higher, the better).
+The models that are not supported by other codebases are marked by `â`. |
+Methods | MMDetection3D | [OpenPCDet](https://github.com/open-mmlab/OpenPCDet)
+| [votenet](https://github.com/facebookresearch/votenet) | [Det3D](https://
 github.com/poodarchu/Det3D) | | :-----------------: | :-----------: | :--------
 ------------------------------------------: | :--------------------------------
 --------------------: | :-----------------------------------------: | | VoteNet
 | 358 | â | 77 | â | | PointPillars-car | 141 | â | â | 140 | |
 PointPillars-3class | 107 | 44 | â | â | | SECOND | 40 | 30 | â | â | |
-Part-A2 | 17 | 14 | â | â | Like [MMDetection](https://github.com/open-
+Part-A2 | 17 | 14 | â | â |  Like [MMDetection](https://github.com/open-
 mmlab/mmdetection) and [MMCV](https://github.com/open-mmlab/mmcv),
 MMDetection3D can also be used as a library to support different projects on
-top of it. ## License This project is released under the [Apache 2.0 license]
-(LICENSE). ## Changelog **1.1.0** was released in 6/4/2023. Please refer to
-[changelog.md](docs/en/notes/changelog.md) for details and release history. ##
-Benchmark and model zoo Results and models are available in the [model zoo]
-(docs/en/model_zoo.md).
+top of it. ## What's New ### Highlight **We have renamed the branch `1.1` to
+`main` and switched the default branch from `master` to `main`. We encourage
+users to migrate to the latest version, though it comes with some cost. Please
+refer to [Migration Guide](docs/en/migration.md) for more details.** We have
+constructed a comprehensive LiDAR semantic segmentation benchmark on
+SemanticKITTI, including Cylinder3D, MinkUNet and SPVCNN methods. Noteworthy,
+the improved MinkUNetv2 can achieve 70.3 mIoU on the validation set of
+SemanticKITTI. We have also supported the training of BEVFusion and an
+occupancy prediction method, TPVFomrer, in our `projects`. More new features
+about 3D perception are on the way. Please stay tuned! **v1.2.0** was released
+in 4/7/2023 - Support [New Config Type](https://mmengine.readthedocs.io/en/
+latest/advanced_tutorials/config.html#a-pure-python-style-configuration-file-
+beta) in `mmdet3d/config` - Support the inference of [DSVT](<(https://
+arxiv.org/abs/2301.06051)>) in `projects` - Support downloading datasets from
+[OpenDataLab](https://opendatalab.com/) using `mim` **v1.1.1** was released in
+30/5/2023: - Support [TPVFormer](https://arxiv.org/pdf/2302.07817.pdf) in
+`projects` - Support the training of BEVFusion in `projects` - Support lidar-
+based 3D semantic segmentation benchmark ## Installation Please refer to
+[Installation](https://mmdetection3d.readthedocs.io/en/latest/get_started.html)
+for installation instructions. ## Getting Started For detailed user guides and
+advanced guides, please refer to our [documentation](https://
+mmdetection3d.readthedocs.io/en/latest/):  User Guides - [Train & Test](https:/
+/mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#train-test) -
+[Learn about Configs](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/config.html) - [Coordinate System](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/coord_sys_tutorial.html) -
+[Dataset Preparation](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/dataset_prepare.html) - [Customize Data Pipelines](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/data_pipeline.html) - [Test
+and Train on Standard Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/train_test.html) - [Inference](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/inference.html) - [Train
+with Customized Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+user_guides/new_data_model.html) - [Useful Tools](https://
+mmdetection3d.readthedocs.io/en/latest/user_guides/index.html#useful-tools)
+Advanced Guides - [Datasets](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/index.html#datasets) - [KITTI Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/kitti.html) -
+[NuScenes Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/nuscenes.html) - [Lyft Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/lyft.html) -
+[Waymo Dataset](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+datasets/waymo.html) - [SUN RGB-D Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/sunrgbd.html) -
+[ScanNet Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/scannet.html) - [S3DIS Dataset](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/datasets/s3dis.html) -
+[SemanticKITTI Dataset](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/datasets/semantickitti.html) - [Supported Tasks](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/index.html#supported-
+tasks) - [LiDAR-Based 3D Detection](https://mmdetection3d.readthedocs.io/en/
+latest/advanced_guides/supported_tasks/lidar_det3d.html) - [Vision-Based 3D
+Detection](https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+supported_tasks/vision_det3d.html) - [LiDAR-Based 3D Semantic Segmentation]
+(https://mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+supported_tasks/lidar_sem_seg3d.html) - [Customization](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/
+index.html#customization) - [Customize Datasets](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_dataset.html)
+- [Customize Models](https://mmdetection3d.readthedocs.io/en/latest/
+advanced_guides/customize_models.html) - [Customize Runtime Settings](https://
+mmdetection3d.readthedocs.io/en/latest/advanced_guides/customize_runtime.html)
+## Overview of Benchmark and Model Zoo Results and models are available in the
+[model zoo](docs/en/model_zoo.md).
                                   Components
                Backbones                 Heads                   Features
      * PointNet_(CVPR'2017)       * FreeAnchor_        * Dynamic_Voxelization_
      * PointNet++_                  (NeurIPS'2019)       (CoRL'2019)
        (NeurIPS'2017)
      * RegNet_(CVPR'2020)
      * DGCNN_(TOG'2019)
      * DLA (CVPR'2018)
      * MinkResNet (CVPR'2019)
      * MinkUNet_(CVPR'2019)
      * Cylinder3D_(CVPR'2021)
                                  Architectures
-3D Object Detection  Monocular 3D Object  Multi-modal 3D         3D Semantic
-                          Detection      Object Detection        Segmentation
-Outdoor              Outdoor             Outdoor           Outdoor
-    * SECOND_            * ImVoxelNet_       * MVXNet_         * MinkUNet_
-      (Sensor'2018)        (WACV'2022)         (ICRA'2019)       (CVPR'2019)
-    * PointPillars_      * SMOKE_        Indoor                * SPVCNN_
-      (CVPR'2019)          (CVPRW'2020)      * ImVoteNet_        (ECCV'2020)
-    * SSN_               * FCOS3D_             (CVPR'2020)     * Cylinder3D_
-      (ECCV'2020)          (ICCVW'2021)                          (CVPR'2021)
-    * 3DSSD_             * PGD_                            Indoor
-      (CVPR'2020)          (CoRL'2021)                         * PointNet++_
-    * SA-SSD_            * MonoFlex_                             (NeurIPS'2017)
-      (CVPR'2020)          (CVPR'2021)                         * PAConv_
-    * PointRCNN_     Indoor                                      (CVPR'2021)
-      (CVPR'2019)        * ImVoxelNet_                         * DGCNN_
-    * Part-A2_             (WACV'2022)                           (TOG'2019)
-      (TPAMI'2020)
-    * CenterPoint_
-      (CVPR'2021)
-    * PV-RCNN_
+    LiDAR-based 3D    Camera-based 3D    Multi-modal 3D         3D Semantic
+   Object Detection   Object Detection  Object Detection        Segmentation
+Outdoor              Outdoor            Outdoor           Outdoor
+    * SECOND_            * ImVoxelNet_      * MVXNet_         * MinkUNet_
+      (Sensor'2018)        (WACV'2022)        (ICRA'2019)       (CVPR'2019)
+    * PointPillars_      * SMOKE_           * BEVFusion_      * SPVCNN_
+      (CVPR'2019)          (CVPRW'2020)       (ICRA'2023)       (ECCV'2020)
+    * SSN_               * FCOS3D_      Indoor                * Cylinder3D_
+      (ECCV'2020)          (ICCVW'2021)     * ImVoteNet_        (CVPR'2021)
+    * 3DSSD_             * PGD_               (CVPR'2020)     * TPVFormer_
+      (CVPR'2020)          (CoRL'2021)                          (CVPR'2023)
+    * SA-SSD_            * MonoFlex_                      Indoor
+      (CVPR'2020)          (CVPR'2021)                        * PointNet++_
+    * PointRCNN_         * DETR3D_                              (NeurIPS'2017)
+      (CVPR'2019)          (CoRL'2021)                        * PAConv_
+    * Part-A2_           * PETR_                                (CVPR'2021)
+      (TPAMI'2020)         (ECCV'2022)                        * DGCNN_
+    * CenterPoint_   Indoor                                     (TOG'2019)
+      (CVPR'2021)        * ImVoxelNet_
+    * PV-RCNN_             (WACV'2022)
       (CVPR'2020)
+    * CenterFormer_
+      (ECCV'2022)
 Indoor
     * VoteNet_
       (ICCV'2019)
     * H3DNet_
       (ECCV'2020)
     * Group-Free-3D_
       (ICCV'2021)
     * FCAF3D_
       (ECCV'2022)
-| | ResNet | PointNet++ | SECOND | DGCNN | RegNetX | DLA | MinkResNet |
-Cylinder3D | MinkUNet | | :-----------: | :----: | :--------: | :----: | :---:
-| :-----: | :-: | :--------: | :--------: | :------: | | SECOND | â | â |
-â | â | â | â | â | â | â | | PointPillars | â | â | â |
-â | â | â | â | â | â | | FreeAnchor | â | â | â | â | â
-| â | â | â | â | | VoteNet | â | â | â | â | â | â | â |
-â | â | | H3DNet | â | â | â | â | â | â | â | â | â | |
-3DSSD | â | â | â | â | â | â | â | â | â | | Part-A2 | â |
-â | â | â | â | â | â | â | â | | MVXNet | â | â | â |
-â | â | â | â | â | â | | CenterPoint | â | â | â | â | â
-| â | â | â | â | | SSN | â | â | â | â | â | â | â | â
-| â | | ImVoteNet | â | â | â | â | â | â | â | â | â | |
-FCOS3D | â | â | â | â | â | â | â | â | â | | PointNet++ |
-â | â | â | â | â | â | â | â | â | | Group-Free-3D | â |
-â | â | â | â | â | â | â | â | | ImVoxelNet | â | â | â
-| â | â | â | â | â | â | | PAConv | â | â | â | â | â |
-â | â | â | â | | DGCNN | â | â | â | â | â | â | â | â
-| â | | SMOKE | â | â | â | â | â | â | â | â | â | | PGD |
-â | â | â | â | â | â | â | â | â | | MonoFlex | â | â |
-â | â | â | â | â | â | â | | SA-SSD | â | â | â | â |
-â | â | â | â | â | | FCAF3D | â | â | â | â | â | â |
-â | â | â | | PV-RCNN | â | â | â | â | â | â | â | â |
-â | | Cylinder3D | â | â | â | â | â | â | â | â | â | |
-MinkUNet | â | â | â | â | â | â | â | â | â | | SPVCNN | â
-| â | â | â | â | â | â | â | â | **Note:** All the about
-**300+ models, methods of 40+ papers** in 2D detection supported by
-[MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/docs/en/
-model_zoo.md) can be trained or used in this codebase. ## Installation Please
-refer to [get_started.md](docs/en/get_started.md) for installation. ## Get
-Started Please see [get_started.md](docs/en/get_started.md) for the basic usage
-of MMDetection3D. We provide guidance for quick run [with existing dataset]
-(docs/en/user_guides/train_test.md) and [with new dataset](docs/en/user_guides/
-2_new_data_model.md) for beginners. There are also tutorials for [learning
-configuration systems](docs/en/user_guides/config.md), [customizing dataset]
-(docs/en/advanced_guides/customize_dataset.md), [designing data pipeline](docs/
-en/user_guides/data_pipeline.md), [customizing models](docs/en/advanced_guides/
-customize_models.md), [customizing runtime settings](docs/en/advanced_guides/
-customize_runtime.md) and [Waymo dataset](docs/en/advanced_guides/datasets/
-waymo_det.md). Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked
-questions. When updating the version of MMDetection3D, please also check the
-[compatibility doc](docs/en/notes/compatibility.md) to be aware of the BC-
-breaking updates introduced in each version. ## Citation If you find this
-project useful in your research, please consider cite: ```latex @misc
-{mmdet3d2020, title={{MMDetection3D: OpenMMLab} next-generation platform for
-general {3D} object detection}, author={MMDetection3D Contributors},
-howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}}, year={2020}
-} ``` ## Contributing We appreciate all contributions to improve MMDetection3D.
-Please refer to [CONTRIBUTING.md](./docs/en/notes/contribution_guides.md) for
-the contributing guideline. ## Acknowledgement MMDetection3D is an open source
+    * TR3D_
+      (ArXiv'2023)
+| | ResNet | VoVNet | Swin-T | PointNet++ | SECOND | DGCNN | RegNetX | DLA |
+MinkResNet | Cylinder3D | MinkUNet | | :-----------: | :----: | :----: | :----:
+| :--------: | :----: | :---: | :-----: | :-: | :--------: | :--------: | :----
+--: | | SECOND | â | â | â | â | â | â | â | â | â | â |
+â | | PointPillars | â | â | â | â | â | â | â | â | â |
+â | â | | FreeAnchor | â | â | â | â | â | â | â | â | â
+| â | â | | VoteNet | â | â | â | â | â | â | â | â | â |
+â | â | | H3DNet | â | â | â | â | â | â | â | â | â |
+â | â | | 3DSSD | â | â | â | â | â | â | â | â | â | â
+| â | | Part-A2 | â | â | â | â | â | â | â | â | â | â |
+â | | MVXNet | â | â | â | â | â | â | â | â | â | â |
+â | | CenterPoint | â | â | â | â | â | â | â | â | â | â
+| â | | SSN | â | â | â | â | â | â | â | â | â | â | â
+| | ImVoteNet | â | â | â | â | â | â | â | â | â | â | â
+| | FCOS3D | â | â | â | â | â | â | â | â | â | â | â |
+| PointNet++ | â | â | â | â | â | â | â | â | â | â | â
+| | Group-Free-3D | â | â | â | â | â | â | â | â | â | â |
+â | | ImVoxelNet | â | â | â | â | â | â | â | â | â | â
+| â | | PAConv | â | â | â | â | â | â | â | â | â | â |
+â | | DGCNN | â | â | â | â | â | â | â | â | â | â | â
+| | SMOKE | â | â | â | â | â | â | â | â | â | â | â | |
+PGD | â | â | â | â | â | â | â | â | â | â | â | |
+MonoFlex | â | â | â | â | â | â | â | â | â | â | â | |
+SA-SSD | â | â | â | â | â | â | â | â | â | â | â | |
+FCAF3D | â | â | â | â | â | â | â | â | â | â | â | |
+PV-RCNN | â | â | â | â | â | â | â | â | â | â | â | |
+Cylinder3D | â | â | â | â | â | â | â | â | â | â | â |
+| MinkUNet | â | â | â | â | â | â | â | â | â | â | â |
+| SPVCNN | â | â | â | â | â | â | â | â | â | â | â | |
+BEVFusion | â | â | â | â | â | â | â | â | â | â | â | |
+CenterFormer | â | â | â | â | â | â | â | â | â | â | â
+| | TR3D | â | â | â | â | â | â | â | â | â | â | â | |
+DETR3D | â | â | â | â | â | â | â | â | â | â | â | |
+PETR | â | â | â | â | â | â | â | â | â | â | â | |
+TPVFormer | â | â | â | â | â | â | â | â | â | â | â |
+**Note:** All the about **500+ models, methods of 90+ papers** in 2D detection
+supported by [MMDetection](https://github.com/open-mmlab/mmdetection/blob/3.x/
+docs/en/model_zoo.md) can be trained or used in this codebase. ## FAQ Please
+refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions. ##
+Contributing We appreciate all contributions to improve MMDetection3D. Please
+refer to [CONTRIBUTING.md](docs/en/notes/contribution_guides.md) for the
+contributing guideline. ## Acknowledgement MMDetection3D is an open source
 project that is contributed by researchers and engineers from various colleges
 and companies. We appreciate all the contributors as well as users who give
 valuable feedbacks. We wish that the toolbox and benchmark could serve the
 growing research community by providing a flexible toolkit to reimplement
-existing methods and develop their own new 3D detectors. ## Projects in
-OpenMMLab - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab
-foundational library for training deep learning models. - [MMCV](https://
-github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
-vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation
-library for multiple machine learning libraries. - [MIM](https://github.com/
-open-mmlab/mim): MIM installs OpenMMLab packages. - [MMPreTrain](https://
-github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+existing methods and develop their own new 3D detectors. ## Citation If you
+find this project useful in your research, please consider cite: ```latex @misc
+{mmdet3d2020, title={{MMDetection3D: OpenMMLab} next-generation platform for
+general {3D} object detection}, author={MMDetection3D Contributors},
+howpublished = {\url{https://github.com/open-mmlab/mmdetection3d}}, year={2020}
+} ``` ## License This project is released under the [Apache 2.0 license]
+(LICENSE). ## Projects in OpenMMLab - [MMEngine](https://github.com/open-mmlab/
+mmengine): OpenMMLab foundational library for training deep learning models. -
+[MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for
+computer vision. - [MMEval](https://github.com/open-mmlab/mmeval): A unified
+evaluation library for multiple machine learning libraries. - [MIM](https://
+github.com/open-mmlab/mim): MIM installs OpenMMLab packages. - [MMPreTrain]
+(https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
 benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection):
 OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
 github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
 general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
 mmrotate): OpenMMLab rotated object detection toolbox and benchmark. - [MMYOLO]
 (https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and
 benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
```

### Comparing `mmdet3d-1.1.1/mmdet3d.egg-info/SOURCES.txt` & `mmdet3d-1.2.0/mmdet3d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mmdet3d/version.py
 mmdet3d.egg-info/PKG-INFO
 mmdet3d.egg-info/SOURCES.txt
 mmdet3d.egg-info/dependency_links.txt
 mmdet3d.egg-info/not-zip-safe
 mmdet3d.egg-info/requires.txt
 mmdet3d.egg-info/top_level.txt
+mmdet3d/.mim/dataset-index.yml
 mmdet3d/.mim/model-index.yml
 mmdet3d/.mim/configs/3dssd/3dssd_4xb4_kitti-3d-car.py
 mmdet3d/.mim/configs/3dssd/metafile.yml
 mmdet3d/.mim/configs/_base_/default_runtime.py
 mmdet3d/.mim/configs/_base_/datasets/kitti-3d-3class.py
 mmdet3d/.mim/configs/_base_/datasets/kitti-3d-car.py
 mmdet3d/.mim/configs/_base_/datasets/kitti-mono3d.py
@@ -254,21 +255,24 @@
 mmdet3d/.mim/tools/analysis_tools/analyze_logs.py
 mmdet3d/.mim/tools/analysis_tools/benchmark.py
 mmdet3d/.mim/tools/analysis_tools/get_flops.py
 mmdet3d/.mim/tools/dataset_converters/create_gt_database.py
 mmdet3d/.mim/tools/dataset_converters/indoor_converter.py
 mmdet3d/.mim/tools/dataset_converters/kitti_converter.py
 mmdet3d/.mim/tools/dataset_converters/kitti_data_utils.py
+mmdet3d/.mim/tools/dataset_converters/kitti_unzip.sh
 mmdet3d/.mim/tools/dataset_converters/lyft_converter.py
 mmdet3d/.mim/tools/dataset_converters/lyft_data_fixer.py
 mmdet3d/.mim/tools/dataset_converters/nuimage_converter.py
 mmdet3d/.mim/tools/dataset_converters/nuscenes_converter.py
+mmdet3d/.mim/tools/dataset_converters/nuscenes_unzip.sh
 mmdet3d/.mim/tools/dataset_converters/s3dis_data_utils.py
 mmdet3d/.mim/tools/dataset_converters/scannet_data_utils.py
 mmdet3d/.mim/tools/dataset_converters/semantickitti_converter.py
+mmdet3d/.mim/tools/dataset_converters/semantickitti_unzip.sh
 mmdet3d/.mim/tools/dataset_converters/sunrgbd_data_utils.py
 mmdet3d/.mim/tools/dataset_converters/update_infos_to_v2.py
 mmdet3d/.mim/tools/dataset_converters/waymo_converter.py
 mmdet3d/.mim/tools/deployment/mmdet3d2torchserve.py
 mmdet3d/.mim/tools/deployment/mmdet3d_handler.py
 mmdet3d/.mim/tools/deployment/test_torchserver.py
 mmdet3d/.mim/tools/misc/browse_dataset.py
```

### Comparing `mmdet3d-1.1.1/mmdet3d.egg-info/requires.txt` & `mmdet3d-1.2.0/mmdet3d.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 lyft_dataset_sdk
 networkx>=2.5
 numba
 numpy
 nuscenes-devkit
-open3d
+open3d==0.16.0
 plyfile
 scikit-image
 tensorboard
 trimesh
 
 [all]
 black==20.8b1
 typing-extensions
 waymo-open-dataset-tf-2-6-0
 lyft_dataset_sdk
 networkx>=2.5
 numba
 numpy
 nuscenes-devkit
-open3d
+open3d==0.16.0
 plyfile
 scikit-image
 tensorboard
 trimesh
 codecov
 flake8
 interrogate
@@ -36,15 +36,15 @@
 xdoctest>=0.10.0
 yapf
 
 [build]
 
 [mim]
 mmcv<2.1.0,>=2.0.0rc4
-mmdet<3.1.0,>=3.0.0
+mmdet<3.2.0,>=3.0.0
 mmengine<1.0.0,>=0.7.1
 
 [optional]
 black==20.8b1
 typing-extensions
 waymo-open-dataset-tf-2-6-0
```

### Comparing `mmdet3d-1.1.1/setup.cfg` & `mmdet3d-1.2.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -11,11 +11,14 @@
 known_third_party = cv2,imageio,indoor3d_util,load_scannet_data,lyft_dataset_sdk,m2r,matplotlib,mmcv,mmdet,mmengine,nuimages,numba,numpy,nuscenes,pandas,plyfile,pycocotools,pyquaternion,pytest,pytorch_sphinx_theme,recommonmark,requests,scannet_utils,scipy,seaborn,shapely,skimage,sphinx,tensorflow,terminaltables,torch,trimesh,ts,waymo_open_dataset
 no_lines_before = STDLIB,LOCALFOLDER
 default_section = THIRDPARTY
 
 [codespell]
 ignore-words-list = ans,refridgerator,crate,hist,formating,dout,wan,nd,fo,avod,AVOD,warmup
 
+[flake8]
+per-file-ignores = mmdet3d/configs/*:F401,F403,F405
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mmdet3d-1.1.1/setup.py` & `mmdet3d-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,17 @@
     elif 'sdist' in sys.argv or 'bdist_wheel' in sys.argv:
         # installed by `pip install .`
         # or create source distribution by `python setup.py sdist`
         mode = 'copy'
     else:
         return
 
-    filenames = ['tools', 'configs', 'demo', 'model-index.yml']
+    filenames = [
+        'tools', 'configs', 'demo', 'model-index.yml', 'dataset-index.yml'
+    ]
     repo_path = osp.dirname(__file__)
     mim_path = osp.join(repo_path, 'mmdet3d', '.mim')
     os.makedirs(mim_path, exist_ok=True)
 
     for filename in filenames:
         if osp.exists(filename):
             src_path = osp.join(repo_path, filename)
```

