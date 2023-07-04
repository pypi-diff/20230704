# Comparing `tmp/tomni-1.9.2.tar.gz` & `tmp/tomni-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tomni-1.9.2.tar", last modified: Mon Jan  3 15:11:05 2022, max compression
+gzip compressed data, was "dist/tomni-2.0.0b1.tar", last modified: Thu Jun 29 12:39:38 2023, max compression
```

## Comparing `tomni-1.9.2.tar` & `tomni-2.0.0b1.tar`

### file list

```diff
@@ -1,183 +1,258 @@
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3786 2022-01-03 15:10:17.000000 tomni-1.9.2/HISTORY.rst
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)    13066 2022-01-03 15:10:17.000000 tomni-1.9.2/LICENSE
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      241 2022-01-03 15:10:17.000000 tomni-1.9.2/MANIFEST.in
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)    19405 2022-01-03 15:11:05.000000 tomni-1.9.2/PKG-INFO
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1894 2022-01-03 15:10:17.000000 tomni-1.9.2/README.md
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      122 2022-01-03 15:10:17.000000 tomni-1.9.2/requirements.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      531 2022-01-03 15:11:05.000000 tomni-1.9.2/setup.cfg
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1553 2022-01-03 15:10:17.000000 tomni-1.9.2/setup.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      550 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/bbox_fitting/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      130 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       31 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     2030 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     6501 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting_center/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       65 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting_center/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1098 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting_center/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3248 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/bbox_operations/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       50 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_operations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/bbox_operations/check_overlap_bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       36 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_operations/check_overlap_bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      916 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_operations/check_overlap_bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1722 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/contour_operations/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       34 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/contour_operations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/contour_operations/get_center/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       28 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/contour_operations/get_center/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      374 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/contour_operations/get_center/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      780 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/contour_operations/get_center/test_get_center.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/illumination_correction/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      105 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/illumination_correction/absolute_difference/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       37 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/absolute_difference/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1476 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/absolute_difference/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     2486 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/absolute_difference/test_absolute_difference.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/illumination_correction/fluo_tophat/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       29 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/fluo_tophat/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1845 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/fluo_tophat/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      953 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/illumination_correction/relative_difference/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       37 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/relative_difference/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     2146 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/relative_difference/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3302 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/illumination_correction/relative_difference/test_ratio_based.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/img_dim/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       25 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/img_dim/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      528 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/img_dim/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      936 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/img_dim/test_imgDim.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/img_paste/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/img_paste/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1778 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/img_paste/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)    14165 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/img_paste/test_img_paste.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      324 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/add_area/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       26 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_area/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      780 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_area/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3132 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_area/test_add_area.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/add_center/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       28 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_center/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      430 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_center/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     2098 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_center/test_add_center.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/add_circularity/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       33 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_circularity/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1110 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_circularity/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1357 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/add_circularity/test_add_circularity.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/cropping/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/cropping/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     4282 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/cropping/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     7281 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/cropping/test_crop_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/flipping/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/flipping/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1261 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/flipping/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1125 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/flipping/test_flip_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/rotation/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       29 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/rotation/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3396 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/rotation/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     4236 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/rotation/test_rotate_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/scale_json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       28 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/scale_json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1674 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/scale_json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1784 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/scale_json/test_scaleResults.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/summary_json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       30 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/summary_json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1807 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/summary_json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     6663 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/summary_json/test_summary_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/json_operations/translation/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       34 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/translation/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1589 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/translation/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1931 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/json_operations/translation/test_translation_json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/make_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      200 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/make_mask/circlair_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       71 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/circlair_mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1397 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/circlair_mask/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     2951 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/circlair_mask/test_circle_mask.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/make_mask/contour_mask_maker/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       35 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/contour_mask_maker/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      949 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/contour_mask_maker/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     5681 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/contour_mask_maker/test_make_mask_contour.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/make_mask/ellipse_mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       65 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/ellipse_mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3297 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/ellipse_mask/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)    14243 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/shape_fitting/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       53 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/shape_fitting/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/shape_fitting/fit_rect_ellipse/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       41 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/shape_fitting/fit_rect_ellipse/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      835 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/shape_fitting/fit_rect_ellipse/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1875 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      490 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/__init__.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/contour2bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       30 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/contour2bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1134 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/contour2bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1222 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/contour2bbox/test_contour2bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/contours2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       31 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/contours2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      651 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/contours2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      913 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/contours2json/test_contours2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/ellipse2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       30 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/ellipse2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      794 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/ellipse2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      863 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/ellipse2json/test_ellipse2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/json2contours/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       31 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2contours/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      532 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2contours/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1593 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2contours/test_contours2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/json2dict/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2dict/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1458 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2dict/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     4245 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2dict/test_json2dict.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/json2labels/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       29 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2labels/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1258 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2labels/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3901 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2labels/test_json2labels.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/json2mask/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2mask/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     3153 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2mask/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)    12317 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2mask/test_json2mask.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/json2vgg/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       26 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2vgg/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1941 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2vgg/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     4183 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/json2vgg/test_json2vgg.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/labels2contours/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       34 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2contours/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      651 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2contours/main.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/labels2contours/positions2contour/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       35 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2contours/positions2contour/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      862 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2contours/positions2contour/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1006 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2contours/test_labels2contours.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/labels2listsOfPoints/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       38 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2listsOfPoints/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      578 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2listsOfPoints/integration_real_data.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      820 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2listsOfPoints/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1070 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/list_of_points2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       37 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/list_of_points2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      640 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/list_of_points2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1310 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/list_of_points2json/test_list_of_points2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/mask2bbox/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/mask2bbox/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1642 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/mask2bbox/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     5346 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/mask2bbox/test_mask2bbox.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/mask2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       27 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/mask2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1734 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/mask2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     9351 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/mask2json/test_mask2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni/transformers/vgg2json/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       26 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/vgg2json/__init__.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     1909 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/vgg2json/main.py
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     7053 2022-01-03 15:10:17.000000 tomni-1.9.2/tomni/transformers/vgg2json/test_vgg2json.py
-drwxr-xr-x   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        0 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)    19405 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/PKG-INFO
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)     5831 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/SOURCES.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        1 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/dependency_links.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)       46 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/entry_points.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        1 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/not-zip-safe
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)      120 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/requires.txt
--rw-r--r--   0 vsts_azpcontainer  (1001) vsts_azpcontainer  (1001)        6 2022-01-03 15:11:05.000000 tomni-1.9.2/tomni.egg-info/top_level.txt
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5709 2023-06-29 12:39:00.000000 tomni-2.0.0b1/HISTORY.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    13065 2023-06-29 12:39:00.000000 tomni-2.0.0b1/LICENSE
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      241 2023-06-29 12:39:00.000000 tomni-2.0.0b1/MANIFEST.in
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    21882 2023-06-29 12:39:38.000000 tomni-2.0.0b1/PKG-INFO
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2451 2023-06-29 12:39:00.000000 tomni-2.0.0b1/README.md
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/docs/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      634 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/Makefile
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      924 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/apidocs.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2214 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/conf.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      471 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/index.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      760 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/make.bat
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      333 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/quickstart.rst
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/docs/tutorials/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2859 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/tutorials/roundness_vs_circularity.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      296 2023-06-29 12:39:00.000000 tomni-2.0.0b1/docs/tutorials.rst
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      150 2023-06-29 12:39:00.000000 tomni-2.0.0b1/requirements.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      790 2023-06-29 12:39:38.000000 tomni-2.0.0b1/setup.cfg
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1526 2023-06-29 12:39:00.000000 tomni-2.0.0b1/setup.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      666 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      109 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      154 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      955 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/annotation/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      834 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/binary_mask/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7640 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6586 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/test_ellipse.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2764 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/ellipse/test_ellipse_comparing.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       24 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       82 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      533 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/point/test_point_comparing.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7582 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    10074 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/test_polygon.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2580 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/annotations/polygon/test_polygon_comparing.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    12861 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    17618 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/test_annotation_manager.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      232 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      723 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1127 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/are_lines_equal/test_lines_equal.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       42 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      843 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2640 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/compress_polygon_points/test_compress_polygon_points.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      310 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       33 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4291 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5955 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/overlap_object/test_overlap_object.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1072 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2798 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/simplify_line/test_polygon_simplify.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1435 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/annotation_manager/utils/test_utils.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_fitting/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      131 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2379 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6932 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       66 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1200 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3727 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_operations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       51 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       37 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      917 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1722 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      172 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       45 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      606 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      538 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/approximate_circle_by_area/test_get_approx_circle_by_area.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      963 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1962 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/circularity/test_circularity.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      519 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      782 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/get_center/test_get_center.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      660 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1899 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/contour_operations/roundness/test_roundness.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/convert_color/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/convert_color/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2803 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/convert_color/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3934 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/convert_color/test_colorConvert.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      106 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1477 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2487 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/test_absolute_difference.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1832 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      950 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2260 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3410 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/illumination_correction/relative_difference/test_ratio_based.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/img_dim/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       26 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_dim/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      530 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_dim/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      937 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_dim/test_imgDim.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/img_paste/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_paste/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1756 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_paste/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    14725 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/img_paste/test_img_paste.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      325 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/add_area/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_area/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      780 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_area/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3132 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_area/test_add_area.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/add_center/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_center/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      434 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_center/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2158 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_center/test_add_center.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      881 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1356 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/add_circularity/test_add_circularity.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/cropping/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/cropping/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4284 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/cropping/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7257 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/cropping/test_crop_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/flipping/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/flipping/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1262 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/flipping/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1036 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/flipping/test_flip_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/rotation/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/rotation/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3397 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/rotation/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4236 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/rotation/test_rotate_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       29 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1663 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1785 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/scale_json/test_scaleResults.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1807 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     6663 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/summary_json/test_summary_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/json_operations/translation/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       35 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/translation/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1576 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/translation/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1931 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/json_operations/translation/test_translation_json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      200 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       71 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1388 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3163 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/circlair_mask/test_circle_mask.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      949 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5774 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/test_make_mask_contour.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       65 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3275 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    36148 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/make_mask/ellipse_mask/test_make_mask_ellipse.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/shape_fitting/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       54 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       42 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      827 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1875 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      573 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/__init__.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1134 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1222 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contour2bbox/test_contour2bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/contours2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contours2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      648 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contours2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1011 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/contours2json/test_contours2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       31 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      794 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      921 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/ellipse2json/test_ellipse2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1902 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4228 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2bbox/test_json2bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2contours/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       32 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2contours/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      553 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2contours/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1594 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2contours/test_contours2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2dict/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2dict/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1459 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2dict/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4246 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2dict/test_json2dict.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2labels/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       30 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2labels/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1296 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2labels/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3120 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2labels/test_json2labels.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2mask/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2mask/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3160 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2mask/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    12303 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2mask/test_json2mask.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1941 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     4183 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/json2vgg/test_json2vgg.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       34 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      973 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     3877 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2contours/test_labels2contours.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       39 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      578 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/integration_real_data.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      817 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1066 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       38 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      603 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1312 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/list_of_points2json/test_list_of_points2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1642 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     5347 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/mask2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       28 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     2811 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    15757 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/mask2json/test_mask2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/positions2contour/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       36 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/positions2contour/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1877 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/positions2contour/main.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)       27 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/__init__.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     1909 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/main.py
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     7052 2023-06-29 12:39:00.000000 tomni-2.0.0b1/tomni/transformers/vgg2json/test_vgg2json.py
+drwxr-xr-x   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        0 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)    21882 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/PKG-INFO
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)     8601 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        1 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        1 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/not-zip-safe
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)      145 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/requires.txt
+-rw-r--r--   0 vsts_azpcontainer  (1001) docker_azpcontainer   (123)        6 2023-06-29 12:39:38.000000 tomni-2.0.0b1/tomni.egg-info/top_level.txt
```

### Comparing `tomni-1.9.2/LICENSE` & `tomni-2.0.0b1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 similar to the well-known GNU General Public License, yet it retains the
 possibility for LuxConnector authors to financially support the development by
 selling commercial licenses. In fact, if you intend to use LuxConnector in a
 "for-profit" environment, where research is conducted to develop or enhance
 a product, is used in a commercial service offering, or when an entity uses
 LuxConnector to participate in government-funded, EU-funded, military or similar
 research projects, then you need to obtain a commercial license.
-In that case, or if you are unsure, please contact the Author info@cytosmart.com 
+In that case, or if you are unsure, please contact the Author info@cytosmart.com
 to inquire about commercial licenses.
 
   What are the rights given to noncommercial users? Similarly to GPL, you
 have the right to use the software, to distribute copies, to receive source
 code, to change the software and distribute your modifications or the
 modified software. Also similarly to the GPL, if you distribute verbatim or
 modified copies of this software, they must be distributed under this
@@ -232,9 +232,9 @@
 TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
 YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
 PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGES.
 
                      END OF TERMS AND CONDITIONS
 
-Initially written by Andras Varga (public domain) for OMNeT++ https://omnetpp.org/intro/license, 
-adapted by CytoSMART TECHNOLOGIES BV. The adaptation is licensed under CC0 1.0 (Public Domain Dedication).
+Initially written by Andras Varga (public domain) for OMNeT++ https://omnetpp.org/intro/license,
+adapted by CytoSMART TECHNOLOGIES BV. The adaptation is licensed under CC0 1.0 (Public Domain Dedication).
```

### Comparing `tomni-1.9.2/PKG-INFO` & `tomni-2.0.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,166 @@
 Metadata-Version: 2.1
 Name: tomni
-Version: 1.9.2
+Version: 2.0.0b1
 Summary: Tomni is a collection of image analysis functions usefull for CytoSmart solution.
 Home-page: https://github.com/cytosmart-bv/tomni
 Author: Tom Nijhof
-License: UNKNOWN
+License: ACADEMIC PUBLIC LICENSE
 Keywords: tomni
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Tomni
-=====
+# Tomni
 
-Tomni is a python package that contains a collection of helper functions based on OpenCV and NumPy. It can be used for any python based computer vision or image analysis problem. The package simplifies the code and takes care of edge cages, everything from simplifying code like img_dim to compute optimization like labels2contours or illumination correction image processing. Tomni uses the image coordinates (same as OpenCV). 
+[![Build Status](https://cytosmart.visualstudio.com/CytoSmartImageAnalysis/_apis/build/status/cytosmart-bv.tomni?branchName=main)](https://cytosmart.visualstudio.com/CytoSmartImageAnalysis/_build/latest?definitionId=384&branchName=main)
+[![Downloads](https://pepy.tech/badge/tomni)](https://pepy.tech/project/tomni)
+
+Tomni is a python package that contains a collection of helper functions based on OpenCV and NumPy. It can be used for any python based computer vision or image analysis problem. The package simplifies the code and takes care of edge cages, everything from simplifying code like img_dim to compute optimization like labels2contours or illumination correction image processing. Tomni uses the image coordinates (same as OpenCV).
 
 Tomni is created by [CytoSMART](https://cytosmart.com).
 
 The package was developed in-house to centralize the helper function for computer vision problems. In 2021, CytoSMART engineers turned it to open source, enabling researchers and educators to use it for free.
 
 ## Getting Tomni
 
-``` cmd
+```cmd
 pip install tomni
 ```
 
 ## License
 
 Tomni is free for academic and educational use.
 
 For commercial use please contact [CytoSMART](https://cytosmart.com/contact).
 
 ## The name
 
-The name Tomni is a combination of creator (Tom) and other CytoSMART product he was working on, [the Omni](https://cytosmart.com/products/omni). Tomni name was proposed by Denissa Daroţi, a former CytoSMART intern, who won a bet with her mentor by getting a (well deserved) 9/10 for her internship. 
-
-
+The name Tomni is a combination of creator (Tom) and other CytoSMART product he was working on, [the Omni](https://cytosmart.com/products/omni). Tomni name was proposed by Denissa Daroţi, a former CytoSMART intern, who won a bet with her mentor by getting a (well deserved) 9/10 for her internship.
 
 ## Features
 
-* Bounding box fitting (bbox fitting)
-  * Center bounding box fit
-  * Custom location box fit
-* Illumination correction 
-  * Brightfield
-  * Fluorescence
-* Json operation
-  * Add circularity property
-  * Scale object
-  * Translate object
-* Make a mask
-  * Ellipse
-  * Polygon
-* Shape fitting
-  * Rect around ellipse
-* Transformers of data format
-  * Contours to json
-  * Ellipse to json
-  * Json 2 contours
-  * Json 2 label
-  * Labels 2 contours
-  * Labels 2 lists of points
+- Bounding box fitting (bbox fitting)
+  - Center bounding box fit
+  - Custom location box fit
+- Image helpers
+  - Get image dimensions
+  - Convert color of an image
+- Illumination correction
+  - Brightfield
+  - Fluorescence
+- Contour operations
+  - Get center
+  - Approximate circle by area
+  - Get roundness
+  - Get circularity
+- CytoSMART data format
+  - Tba
+- Json operation
+  - Add circularity property
+  - Scale object
+  - Translate object
+- Make a mask
+  - Ellipse
+  - Polygon
+- Shape fitting
+  - Rect around ellipse
+- Transformers of data format
+  - Contours to json
+  - Ellipse to json
+  - Json 2 contours
+  - Json 2 label
+  - Json 2 bbox
+  - Labels 2 contours
+  - Labels 2 lists of points
+
 
 ## Credits
+
 Sorted alphabetically
 
 - Coenraad Stijne
 - Denisa Daroţi
 - Hristo Atanasov
+- Jan-Niklas Schneider
 - Jelle van Kerkvoorde
 - Kirsten Koopman
 - Manon van Erp
 - Marina Tzenkova
 - Tom de Vries
 - Tom Nijhof
 
+
 # History
+
+2.0.0-b0 (2022-11-29)
+------------------
+- CDF-Main: Implement `filter` to allow filtering of annotations by feature values (aka gating).
+- CDF-Main: Implement `from_contours`.
+- CDF-Main: Implement `to_contours`.
+- CDF-Main: Implement `from_dict`.
+- CDF-Main: Implement `to_dict`. Includes rounding.
+- CDF-Main: Implement `__len__`.
+- CDF-Main: Implement `__iter__` and `__next__`.
+- Add polygon annotation class.
+- CDF-polygon: Implement `__eq__`
+- CDF-polygon: Remove useless point
+- Add ellipse annotation class.
+- CDF-ellipse: Implement `__eq__`
+- CDF-ellipse: Set all rotations between 0 and 90, flip radii if needed
+- Renamed `CytoSmartDataFormat` to `AnnotationManager`
+- Add `is_in_mask` for `Ellipse` and `Polygon`
+- Add `min_overlap`-parameter in `to_dict` to apply masks to filter annotations
+- Add `to_binary_mask` and `to_labeled_mask` for `AnnotationManager`, `Ellipse` and `Polygon`
+- Add init-function `from_binary_mask` and `from_labeled_mask` to `AnnotationManager`
+- Bugfix: Fixed a bug where `simplify_line` returns empty list when passing two points.
+- Add option to to compress polygons in `to_dict()`.
+
+1.15.0 (2022-12-05)
+------------------
+- Add json2bbox for ellipse with angle of rotation
+
+1.14.0 (2022-11-11)
+------------------
+- Add convert to color
+
+1.13.0 (2022-10-24)
+------------------
+- Add json2bbox for polygon and ellipse
+
+1.12.1 (2022-10-06)
+------------------
+- Update Json-circularity with circularity calculation from contour ops.
+
+1.12.0 (2022-04-15)
+------------------
+- BUGFIX: Import approximate_circle_by_area
+- Add roundness
+- Add contour operation circularity
+
+1.11.0 (2022-04-11)
+------------------
+- Add inner contours to labels2contours
+- Add inner contours to mask2json
+
+1.10.0 (2022-02-17)
+------------------
+- Add approximate_circle_by_area to contour operations
+- BUGFIX: Change type np.array to np.ndarray
+- DEPRECATE: Remove simplification so python 3.8+ can be used
+
 1.9.2 (2022-01-03)
 ------------------
-- BUGFIX: Bufferoverflow make_mask_ellipse (again/still) 
+- BUGFIX: Bufferoverflow make_mask_ellipse (again/still)
     remove times 2 for all values in the function
 
 1.9.1 (2021-10-26)
 ------------------
 - add ellipse to json2mask
 - BUGFIX: Bufferoverflow make_mask_ellipse
 - BUGFIX: Make make_mask_ellipse accept floats
@@ -123,15 +194,15 @@
 ------------------
 updated setup file simplification<0.6
 
 1.7.0 (2020-12-03)
 ------------------
 added new functions
 - add_area
-- summary_json 
+- summary_json
 - json2dict
 
 1.6.4 (2020-11-26)
 ------------------
 - add  missing requirements in setup file
 
 1.6.3 (2020-11-25)
@@ -171,15 +242,15 @@
 - add vgg2json
 
 1.3.0
 ------------------
 Updating of relative illumination correction.
 - add (optional) smoothing step
 - add (optional) resize step
-- add (optional) normalization 
+- add (optional) normalization
 
 1.2.0 (2020-07-02)
 ------------------
 - Add translation of json functions
 
 1.1.0 (2020-03-11)
 ------------------
@@ -196,15 +267,15 @@
 1.0.0 (2020-02-28)
 ------------------
 Restructuring of tomni:
 - Migrated Visualization to cytoBoom
 - Migrated validation to manVal
 - Made sure every function followed:
     function_name
-    - __init__.py 
+    - __init__.py
     - main.py
     - test_function_name
 - removed following function:
 -- channel_selecting (was only used for old cell counter)
 -- select_labels (complete replaceable by transformers.labels2listsOfPoints
 - Added docstring to all functions
 - Added typing to all functions
@@ -265,15 +336,15 @@
 similar to the well-known GNU General Public License, yet it retains the
 possibility for LuxConnector authors to financially support the development by
 selling commercial licenses. In fact, if you intend to use LuxConnector in a
 "for-profit" environment, where research is conducted to develop or enhance
 a product, is used in a commercial service offering, or when an entity uses
 LuxConnector to participate in government-funded, EU-funded, military or similar
 research projects, then you need to obtain a commercial license.
-In that case, or if you are unsure, please contact the Author info@cytosmart.com 
+In that case, or if you are unsure, please contact the Author info@cytosmart.com
 to inquire about commercial licenses.
 
   What are the rights given to noncommercial users? Similarly to GPL, you
 have the right to use the software, to distribute copies, to receive source
 code, to change the software and distribute your modifications or the
 modified software. Also similarly to the GPL, if you distribute verbatim or
 modified copies of this software, they must be distributed under this
@@ -484,10 +555,9 @@
 TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
 YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
 PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGES.
 
                      END OF TERMS AND CONDITIONS
 
-Initially written by Andras Varga (public domain) for OMNeT++ https://omnetpp.org/intro/license, 
+Initially written by Andras Varga (public domain) for OMNeT++ https://omnetpp.org/intro/license,
 adapted by CytoSMART TECHNOLOGIES BV. The adaptation is licensed under CC0 1.0 (Public Domain Dedication).
-
```

### Comparing `tomni-1.9.2/setup.py` & `tomni-2.0.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """The setup script."""
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
@@ -29,22 +29,22 @@
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     description="Tomni is a collection of image analysis functions usefull for CytoSmart solution.",
-    entry_points={"console_scripts": ["tomni=tomni.cli:__init__"]},
     install_requires=requirements,
     long_description=readme + "\n\n" + history + "\n\n" + license,
+    license="ACADEMIC PUBLIC LICENSE",
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="tomni",
     name="tomni",
     packages=find_packages(include=["tomni*"], exclude=["docs*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cytosmart-bv/tomni",
-    version="1.9.2",
+    version="2.0.0b1",
     zip_safe=False,
 )
```

### Comparing `tomni-1.9.2/tomni/__init__.py` & `tomni-2.0.0b1/tomni/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 """Tomni is a collection of image analysis functions useful for CytoSmart solution."""
 
 __author__ = """Tom Nijhof & Jelle van Kerkvoorde"""
 __email__ = "tom.nijhof@cytosmart.com"
-__version__ = "1.9.2"
+__version__ = "2.0.0b1"
 
 from .bbox_fitting import bbox_fitting, bbox_fitting_center
+from .bbox_operations import check_overlap_bbox
+from .convert_color import convert_color
+from .illumination_correction import absolute_difference, fluo_tophat, relative_difference
+from .img_dim import img_dim
 from .img_paste import img_paste
+from .json_operations import *
+from .make_mask import *
 from .shape_fitting import fit_rect_around_ellipse
-from .img_dim import img_dim
-
-from . import illumination_correction
-from . import make_mask
-from . import transformers
-from . import json_operations
-from . import bbox_operations
+from .transformers import *
```

### Comparing `tomni-1.9.2/tomni/bbox_fitting/bbox_fitting/main.py` & `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,86 @@
 import cv2
-import numpy as np 
+import numpy as np
 
-def bbox_fitting(img, x1, y1, x2, y2, padding_value=0):
+
+def bbox_fitting(
+    img: np.ndarray, x1: int, y1: int, x2: int, y2: int, padding_value: int = 0
+) -> np.ndarray:
     """
     Bounding box fitting:
     Using cropping and padding to fit an image to the bounding box.
     Relative to the 0,0 of the input image the image gets cropped and padded to fit with x1, y1, x2 and y2.
     The result is including the pixels x1, x2, y1 and y2.
     So a 0, 0, 9, 9 gives an 10x10 result.
 
     WARNING:
     Coordinates are IMAGE-coordinates. So that is the same pillow and OpenCV uses but swapped from what Numpy and Scipy use (ARRAY-coordinates).
     Yes, I hate it too.
+
+    Args:
+        img: (np.ndarray): The image the bounding box will be extracted from
+
+        x1: (int): Lowest value of X
+
+        y1: (int): Lowest value of Y
+
+        x2: (int): Highest value of X
+
+        y2: (int): Highest value of Y
+
+        padding_value: (int, optional): Every pixel outside the image bit inside the bounding box will get this value.
+        Defaults to 0.
+
+    Returns:
+        np.ndarray: Extracted patch within the bounding box from the image
+    """
+    """
+
     """
 
     if not isinstance(img, np.ndarray):
         raise TypeError("Img needs to be a numpy.ndarry not {}".format(type(img)))
-    
-    if not isinstance(x1, int) or not isinstance(x2, int) or not isinstance(y1, int) or not isinstance(y2, int):
-        raise ValueError("x1, y1, x2 and y2 need to be a positive int not {}, {}, {}, {}".format(type(x1), type(y1), type(x2), type(y2)))
 
-    # if x1 < 0 or y1 < 0 or x2 < 0 or y2 < 0:
-    #     raise ValueError("x1, y1, x2 and y2 needs to be a possitive int. Given: {}, {}, {}, {}".format(x1, y1, x2, y2))
+    if (
+        not isinstance(x1, int)
+        or not isinstance(x2, int)
+        or not isinstance(y1, int)
+        or not isinstance(y2, int)
+    ):
+        raise ValueError(
+            "x1, y1, x2 and y2 need to be a positive int not {}, {}, {}, {}".format(
+                type(x1), type(y1), type(x2), type(y2)
+            )
+        )
 
     if x2 < 0:
-        return np.zeros((y2 - y1, x2 -x1))
+        return np.zeros((y2 - y1, x2 - x1))
     if y2 < 0:
-        return np.zeros((y2 - y1, x2 -x1))
+        return np.zeros((y2 - y1, x2 - x1))
     if x1 >= img.shape[1]:
-        return np.zeros((y2 - y1, x2 -x1))
+        return np.zeros((y2 - y1, x2 - x1))
     if y1 >= img.shape[0]:
-        return np.zeros((y2 - y1, x2 -x1))
+        return np.zeros((y2 - y1, x2 - x1))
 
     cy1 = max(0, y1)
     cy2 = min(img.shape[0], y2)
     cx1 = max(0, x1)
     cx2 = min(img.shape[1], x2)
-    
-    pad_left = - min(0, x1)
+
+    pad_left = -min(0, x1)
     pad_right = max(x2 - img.shape[1], 0)
-    pad_top = - min(0, y1)
+    pad_top = -min(0, y1)
     pad_bottom = max(y2 - img.shape[0], 0)
-    
+
     img = img[cy1:cy2, cx1:cx2]
-    
-    img = cv2.copyMakeBorder(img,
-                            top=pad_top, 
-                            bottom=pad_bottom,
-                            left=pad_left, 
-                            right=pad_right, 
-                            borderType=cv2.BORDER_CONSTANT, 
-                            value=padding_value)
+
+    img = cv2.copyMakeBorder(
+        img,
+        top=pad_top,
+        bottom=pad_bottom,
+        left=pad_left,
+        right=pad_right,
+        borderType=cv2.BORDER_CONSTANT,
+        value=padding_value,
+    )
 
     return img
```

### Comparing `tomni-1.9.2/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py` & `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting/test_bbox_fitting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,236 +1,252 @@
 from __future__ import absolute_import
 from unittest import TestCase
 from . import bbox_fitting
 import numpy as np
 
+
 class TestBbox_fitting(TestCase):
     def test_raise_warning_image(self):
         input_array = [
             [0, 1, 1, 1, 0],
             [1, 1, 1, 1, 1],
             [1, 1, 1, 2, 1],
             [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]]
+            [0, 1, 1, 1, 0],
+        ]
         with self.assertRaises(TypeError):
             result = bbox_fitting(input_array, 1, 1, 3, 3)
 
     def test_raise_warning_float_cor(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
         with self.assertRaises(ValueError):
             result = bbox_fitting(input_array, 1.1, 1, 3, 3)
         with self.assertRaises(ValueError):
             result = bbox_fitting(input_array, 1, 1.3, 3, 3)
         with self.assertRaises(ValueError):
             result = bbox_fitting(input_array, 1, 1, 3.9, 3)
         with self.assertRaises(ValueError):
             result = bbox_fitting(input_array, 1, 1, 3, 3.0)
 
     def test_crop_5x5_3x3(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
-
-        expected = np.array([
-            [1, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [1, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
 
         result = bbox_fitting(input_array, 1, 1, 4, 4)
         np.testing.assert_array_equal(expected, result)
 
     def test_crop_7x5_3x3(self):
-        input_array = np.array([
-            [0, 1, 0, 1, 0],
-            [0, 1, 1, 1, 0],
-            [1, 1, 4, 1, 1],
-            [1, 1, 5, 1, 1],
-            [1, 1, 1, 1, 1],
-            [0, 1, 1, 1, 0],
-            [0, 1, 0, 1, 0]
-        ])
-
-        expected = np.array([
-            [1, 4, 1],
-            [1, 5, 1],
-            [1, 1, 1],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 0, 1, 0],
+                [0, 1, 1, 1, 0],
+                [1, 1, 4, 1, 1],
+                [1, 1, 5, 1, 1],
+                [1, 1, 1, 1, 1],
+                [0, 1, 1, 1, 0],
+                [0, 1, 0, 1, 0],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [1, 4, 1],
+                [1, 5, 1],
+                [1, 1, 1],
+            ]
+        )
 
         result = bbox_fitting(input_array, 1, 2, 4, 5)
         np.testing.assert_array_equal(expected, result)
 
-    
     def test_padding_3x3_5x5(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [0, 0, 0, 0, 0],
-            [0, 5, 1, 1, 0],
-            [0, 1, 1, 2, 0],
-            [0, 1, 1, 3, 0],
-            [0, 0, 0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [0, 0, 0, 0, 0],
+                [0, 5, 1, 1, 0],
+                [0, 1, 1, 2, 0],
+                [0, 1, 1, 3, 0],
+                [0, 0, 0, 0, 0],
+            ]
+        )
 
         result = bbox_fitting(input_array, -1, -1, 4, 4)
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_3x3_5x7(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [0, 0, 0, 0, 0],
-            [0, 5, 1, 1, 0],
-            [0, 1, 1, 2, 0],
-            [0, 1, 1, 3, 0],
-            [0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [0, 0, 0, 0, 0],
+                [0, 5, 1, 1, 0],
+                [0, 1, 1, 2, 0],
+                [0, 1, 1, 3, 0],
+                [0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0],
+            ]
+        )
 
         result = bbox_fitting(input_array, -1, -1, 4, 6)
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_and_cropping_3x3_3x4(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [1, 1, 0],
-            [1, 2, 0],
-            [1, 3, 0],
-            [0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array([[1, 1, 0], [1, 2, 0], [1, 3, 0], [0, 0, 0]])
 
         result = bbox_fitting(input_array, 1, 0, 4, 4)
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_and_cropping_3x3_3x4_color(self):
-        input_array = np.array([
-            [[5, 4, 3], [1, 9, 2], [1, 8, 2]],
-            [[1, 2, 2],[1, 1, 2], [1, 7, 2]],
-            [[1, 4, 2], [1, 5, 2], [1, 6, 2]],
-        ])
-        
-        expected = np.array([
-            [[1, 9, 2], [1, 8, 2], [0, 0, 0]],
-            [[1, 1, 2], [1, 7, 2], [0, 0, 0]],
-            [[1, 5, 2], [1, 6, 2], [0, 0, 0]],
-            [[0, 0, 0], [0, 0, 0], [0, 0, 0]]
-        ])
+        input_array = np.array(
+            [
+                [[5, 4, 3], [1, 9, 2], [1, 8, 2]],
+                [[1, 2, 2], [1, 1, 2], [1, 7, 2]],
+                [[1, 4, 2], [1, 5, 2], [1, 6, 2]],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [[1, 9, 2], [1, 8, 2], [0, 0, 0]],
+                [[1, 1, 2], [1, 7, 2], [0, 0, 0]],
+                [[1, 5, 2], [1, 6, 2], [0, 0, 0]],
+                [[0, 0, 0], [0, 0, 0], [0, 0, 0]],
+            ]
+        )
 
         result = bbox_fitting(input_array, 1, 0, 4, 4)
         np.testing.assert_array_equal(expected, result)
-    
+
     def test_underflow_left(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0]]
+        )
 
         result = bbox_fitting(input_array, -5, 1, -1, 6)
         np.testing.assert_array_equal(expected, result)
-    
+
     def test_overflow_right(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0]]
+        )
 
         result = bbox_fitting(input_array, 3, 1, 7, 6)
         np.testing.assert_array_equal(expected, result)
+
     def test_overflow_down(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [0, 0, 0],
-            [0, 0, 0],
-            [0, 0, 0],
-            [0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array([[0, 0, 0], [0, 0, 0], [0, 0, 0], [0, 0, 0]])
 
         result = bbox_fitting(input_array, 1, 9, 4, 13)
         np.testing.assert_array_equal(expected, result)
-    
+
     def test_underflow_up(self):
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0]
-        ])
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0]]
+        )
 
         result = bbox_fitting(input_array, 1, -7, 5, -2)
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_3x3_5x7_different_color(self):
-        '''
+        """
         Don't argure about how color is writen. It is color without, because I don't like u.
-        '''
-        input_array = np.array([
-            [5, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
-        
-        expected = np.array([
-            [255, 255, 255, 255, 255],
-            [255, 5, 1, 1, 255],
-            [255, 1, 1, 2, 255],
-            [255, 1, 1, 3, 255],
-            [255, 255, 255, 255, 255],
-            [255, 255, 255, 255, 255],
-            [255, 255, 255, 255, 255],
-        ])
+        """
+        input_array = np.array(
+            [
+                [5, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [255, 255, 255, 255, 255],
+                [255, 5, 1, 1, 255],
+                [255, 1, 1, 2, 255],
+                [255, 1, 1, 3, 255],
+                [255, 255, 255, 255, 255],
+                [255, 255, 255, 255, 255],
+                [255, 255, 255, 255, 255],
+            ]
+        )
 
         result = bbox_fitting(input_array, -1, -1, 4, 6, padding_value=255)
-        np.testing.assert_array_equal(expected, result)
+        np.testing.assert_array_equal(expected, result)
```

### Comparing `tomni-1.9.2/tomni/bbox_fitting/bbox_fitting_center/main.py` & `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from __future__ import absolute_import, division
+from typing import List
 from . import bbox_fitting
-from math import ceil, floor
+from math import ceil
 import numpy as np
 
-def bbox_fitting_center(img, size, padding_value=0):
-    '''
+
+def bbox_fitting_center(img: np.ndarray, size, padding_value: int = 0) -> np.ndarray:
+    """
     Creates an image of size 'size' ([(int) x, (int) y]) in IMAGE-Coordinates).
     The orignal image will be centered and padded and/or cropped to fit the size.
 
     img: numpy.ndarray
     size: [int, int]
 
     output: numpy.ndarray
-    '''
+    """
     if not isinstance(img, np.ndarray):
         raise TypeError("Img needs to be a numpy.ndarry not {}".format(type(img)))
-    
+
     if not isinstance(size[0], int) or not isinstance(size[1], int):
-        raise ValueError("x1, y1, x2 and y2 need to be a positive int not {}, {}".format(type(size[0]), type(size[1])))
-    x1 = - (size[0] - img.shape[1])/2
-    y1 = - (size[1] - img.shape[0])/2
+        raise ValueError(
+            "x1, y1, x2 and y2 need to be a positive int not {}, {}".format(
+                type(size[0]), type(size[1])
+            )
+        )
+    x1 = -(size[0] - img.shape[1]) / 2
+    y1 = -(size[1] - img.shape[0]) / 2
     x2 = x1 + size[0]
     y2 = y1 + size[1]
 
     # Round the number to fit exactly with the pixels
     x1 = int(ceil(x1))
     y1 = int(ceil(y1))
     x2 = int(ceil(x2))
     y2 = int(ceil(y2))
 
-    return bbox_fitting(img, x1=x1, y1=y1, x2=x2, y2=y2, padding_value=padding_value)
+    return bbox_fitting(img, x1=x1, y1=y1, x2=x2, y2=y2, padding_value=padding_value)
```

### Comparing `tomni-1.9.2/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py` & `tomni-2.0.0b1/tomni/bbox_fitting/bbox_fitting_center/test_bbox_fitting_center.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,141 @@
 from __future__ import absolute_import
 from unittest import TestCase
 from . import bbox_fitting_center
 import numpy as np
 
+
 class TestBbox_fitting(TestCase):
     def test_raise_warning_image(self):
         input_array = [
             [0, 1, 1, 1, 0],
             [1, 1, 1, 1, 1],
             [1, 1, 1, 2, 1],
             [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]]
+            [0, 1, 1, 1, 0],
+        ]
         with self.assertRaises(TypeError):
             bbox_fitting_center(input_array, [3, 3])
 
     def test_raise_warning_float_cor(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
         with self.assertRaises(ValueError):
             bbox_fitting_center(input_array, [3.9, 3])
         with self.assertRaises(ValueError):
             bbox_fitting_center(input_array, [3, 3.0])
 
     def test_crop_5x5_3x3(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
-
-        expected = np.array([
-            [1, 1, 1],
-            [1, 1, 2],
-            [1, 1, 3],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [1, 1, 1],
+                [1, 1, 2],
+                [1, 1, 3],
+            ]
+        )
 
         result = bbox_fitting_center(input_array, (3, 3))
         np.testing.assert_array_equal(expected, result)
 
     def test_crop_5x5_5x3(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
-
-        expected = np.array([
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+            ]
+        )
 
         result = bbox_fitting_center(input_array, (5, 3))
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_and_cropping_5x5_7x3(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
-
-        expected = np.array([
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 2, 1, 0],
-            [0, 1, 1, 1, 3, 1, 0],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 2, 1, 0],
+                [0, 1, 1, 1, 3, 1, 0],
+            ]
+        )
 
         result = bbox_fitting_center(input_array, (7, 3))
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_and_cropping_5x5_6x3(self):
-        input_array = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 2, 1],
-            [1, 1, 1, 3, 1],
-            [0, 1, 1, 1, 0]
-        ])
-
-        expected = np.array([
-            [1, 1, 1, 1, 1, 0],
-            [1, 1, 1, 2, 1, 0],
-            [1, 1, 1, 3, 1, 0],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 2, 1],
+                [1, 1, 1, 3, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [1, 1, 1, 1, 1, 0],
+                [1, 1, 1, 2, 1, 0],
+                [1, 1, 1, 3, 1, 0],
+            ]
+        )
 
         result = bbox_fitting_center(input_array, (6, 3))
         np.testing.assert_array_equal(expected, result)
 
     def test_padding_and_cropping_4x4_6x3(self):
-        input_array = np.array([
-            [0, 1, 1, 1],
-            [1, 1, 1, 1],
-            [1, 1, 1, 2],
-            [1, 1, 1, 3],
-        ])
-
-        expected = np.array([
-            [0, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 2, 0],
-            [0, 1, 1, 1, 3, 0],
-        ])
+        input_array = np.array(
+            [
+                [0, 1, 1, 1],
+                [1, 1, 1, 1],
+                [1, 1, 1, 2],
+                [1, 1, 1, 3],
+            ]
+        )
+
+        expected = np.array(
+            [
+                [0, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 2, 0],
+                [0, 1, 1, 1, 3, 0],
+            ]
+        )
 
         result = bbox_fitting_center(input_array, (6, 3))
-        np.testing.assert_array_equal(expected, result)
+        np.testing.assert_array_equal(expected, result)
```

### Comparing `tomni-1.9.2/tomni/bbox_operations/check_overlap_bbox/main.py` & `tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         raise ValueError("The bounding boxes must be tuples or list of length 4")
 
     if (bb1[0] >= bb2[2]) or (bb2[0] >= bb1[2]):
         return False
     elif (bb1[1] >= bb2[3]) or (bb2[1] >= bb1[3]):
         return False
     else:
-        return True
+        return True
```

### Comparing `tomni-1.9.2/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py` & `tomni-2.0.0b1/tomni/bbox_operations/check_overlap_bbox/test_check_overlap_bbox.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/contour_operations/get_center/test_get_center.py` & `tomni-2.0.0b1/tomni/contour_operations/get_center/test_get_center.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import TestCase
 import numpy as np
 from .main import get_center
 
+
 class TestGetCenterContour(TestCase):
     def test_happy_flow(self):
         contour = np.array([[[500, 50]], [[500, 99]], [[539, 99]], [[539, 50]]])
 
         expectedResult = (519, 74)
 
         result = get_center(contour=contour)
@@ -19,8 +20,8 @@
 
         expectedResult = (500, 50)
 
         result = get_center(contour=contour)
 
         self.assertEqual(len(result), len(expectedResult))
         for i in range(len(result)):
-            self.assertEqual(result[i], expectedResult[i])
+            self.assertEqual(result[i], expectedResult[i])
```

### Comparing `tomni-1.9.2/tomni/illumination_correction/absolute_difference/main.py` & `tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import numpy as np
 import cv2
 import warnings
 
 
 def absolute_difference(
-    img: np.array, gauss_size: int = 21, new_median: int = 128
-) -> np.array:
+    img: np.ndarray, gauss_size: int = 21, new_median: int = 128
+) -> np.ndarray:
     """
     Remove big blurry artifact from the image.
     It will do this by taking the absolute difference between the blurred and raw image.
 
     # Usage
     Best not to use this for human vision.
     The algorithm can have weird artifacts.
     This is good as algorithm input for algorithms that rely on absolute pixel difference.
 
     # Fractal
-    This algorithm is fractal. 
+    This algorithm is fractal.
     Meaning the illumination correction followed by cropping will given the same result than first cropping.
 
     img (np.array): input image
-    gauss_size (int): needs to be an odd number. 
+    gauss_size (int): needs to be an odd number.
         This is corralated to the size of the big artifact to remove.
     """
 
     img = np.array(img, dtype=np.int16)
 
     if gauss_size % 2 == 0:
         gauss_size += 1  # Only works with odd gauss size
@@ -32,15 +32,15 @@
             "the gauss_size needs to be odd. It is {}. One is added to it".format(
                 gauss_size
             ),
             SyntaxWarning,
         )
 
     """
-    The illumination is every detail bigger than the gauss_size. 
+    The illumination is every detail bigger than the gauss_size.
     This includes the inside of square bigger than gauss_size, but not its borders.
     """
     img -= cv2.GaussianBlur(img, (gauss_size, gauss_size), 0)
 
     img += new_median
 
     # All overhead needs to be rounded down
```

### Comparing `tomni-1.9.2/tomni/illumination_correction/absolute_difference/test_absolute_difference.py` & `tomni-2.0.0b1/tomni/illumination_correction/absolute_difference/test_absolute_difference.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
         dist = xx
         img = (dist >= 100) * 128 + (dist >= 200) * 128
 
         with self.assertWarns(SyntaxWarning):
             illum_img = absolute_difference(img, gauss_size=20)
 
         self.assertGreaterEqual(np.min(illum_img), 0)
-        self.assertLessEqual(np.max(illum_img), 255)
+        self.assertLessEqual(np.max(illum_img), 255)
```

### Comparing `tomni-1.9.2/tomni/illumination_correction/fluo_tophat/main.py` & `tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     This is the background subtraction of the fluorescent channel.
     This subtraction can be used for the green and the red channel
     It uses a morphological white tophat filter to create a map of the subtraction.
 
     input:
         img: A standard grayscale image
         normalize: Normalizes the image from 0 to 255, this looks better but data will be lost
-    
+
     output:
         img: The result image after background subtraction
         p2 : The lower bound value where an x-amount of pixels are included
-        p98: The higher bound value where an y-amount of pixels are included  
+        p98: The higher bound value where an y-amount of pixels are included
 
     The p2 and p98 values are used to normalize the image, but won't be automatically applied
-    due to loss of data. These values should be given later to the integration part so they can 
-    pass these values to the front-end. 
-    
+    due to loss of data. These values should be given later to the integration part so they can
+    pass these values to the front-end.
+
     """
     img = img.astype(np.uint8)
     img = cv2.GaussianBlur(img, (5, 5), 0)
     filterSize = (25, 25)
     kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, filterSize)
     img = cv2.morphologyEx(img, cv2.MORPH_TOPHAT, kernel, iterations=10)
 
@@ -43,8 +43,7 @@
             img = rescale_intensity(img, p2, p98)
     else:
         p2, p98 = np.percentile(img, (15, 100), interpolation="linear")
         if normalize == 1:
             img = rescale_intensity(img, p2, p98)
 
     return img, p2, p98
-
```

### Comparing `tomni-1.9.2/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py` & `tomni-2.0.0b1/tomni/illumination_correction/fluo_tophat/test_fluo_tophat.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,10 +22,7 @@
 
     def test_random_image(self):
         img = np.random.randint(0, 255, (1000, 1000))
         img[0:400, 0:400] = np.zeros((400, 400))
         illum_img, _, _ = fluo_tophat(img)
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
-
-
-
```

### Comparing `tomni-1.9.2/tomni/illumination_correction/relative_difference/main.py` & `tomni-2.0.0b1/tomni/illumination_correction/relative_difference/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,70 @@
-
 import numpy as np
 import cv2
 
-def relative_difference(img: np.array, gauss_size: int = 301, smooth_size=None, do_normalize: bool= False, resize_ratio= None) -> np.array:
+
+def relative_difference(
+    img: np.ndarray,
+    gauss_size: int = 301,
+    smooth_size=None,
+    do_normalize: bool = False,
+    resize_ratio=None,
+) -> np.array:
     """
     Remove big blurry artifact from the image.
     It will do this by taking the ratio difference between the blurred and raw image.
-    
+
     # Usage
     This can be used for human vision.
     This is good as algorithm input for algorithm that rely on relative pixel difference.
 
     # NOT fractal
-    This algorithm is NOT fractal. 
+    This algorithm is NOT fractal.
     Meaning the illumination correction followed by cropping will given a different result than first cropping.
 
     img (np.array): input image
-    gauss_size (int): needs to be an odd number. 
+    gauss_size (int): needs to be an odd number.
         This is corralated to the size of the big artifact to remove.
     smooth_size (int): need to be an odd number.
         Is the size of the kernal of the gaussian filter that is used on the image before division.
     resize_ratio (float): the img is resized according to this ration before using a GaussianBlur.
         This is done to increase the speed of the function.
     do_normalize (bool): if true, the output img is normalized between the minimum and maximum
-        value of the smoothed img. 
+        value of the smoothed img.
     """
     img = np.float32(img)
-    
+
     if gauss_size % 2 == 0:
         gauss_size += 1
 
     if smooth_size:
-        img = cv2.GaussianBlur(img, (smooth_size,smooth_size), 0)
-    
+        img = cv2.GaussianBlur(img, (smooth_size, smooth_size), 0)
+
     max_img = np.max(img)
     min_img = np.min(img)
 
     if resize_ratio:
-        gb = cv2.resize(img, (0, 0), fx=resize_ratio, fy=resize_ratio, interpolation=cv2.INTER_LINEAR)
-        gb = cv2.GaussianBlur(gb, (gauss_size, gauss_size), 0, borderType=cv2.BORDER_REPLICATE)
-        gb = cv2.resize(gb, (img.shape[1], img.shape[0]), interpolation=cv2.INTER_LINEAR)
+        gb = cv2.resize(
+            img,
+            (0, 0),
+            fx=resize_ratio,
+            fy=resize_ratio,
+            interpolation=cv2.INTER_LINEAR,
+        )
+        gb = cv2.GaussianBlur(
+            gb, (gauss_size, gauss_size), 0, borderType=cv2.BORDER_REPLICATE
+        )
+        gb = cv2.resize(
+            gb, (img.shape[1], img.shape[0]), interpolation=cv2.INTER_LINEAR
+        )
     else:
         gb = cv2.GaussianBlur(img, (gauss_size, gauss_size), 0)
         gb = np.float32(gb)
 
     img = np.divide(img, gb + 1e-15, dtype=np.float32)
-    
-    
+
     if do_normalize:
         img = cv2.normalize(img, img, max_img, min_img, cv2.NORM_MINMAX)
     else:
         img = np.divide(img, np.max(img) + 1e-15, dtype=np.float32) * 255
-    
-    return img.astype(np.uint8)
+
+    return img.astype(np.uint8)
```

### Comparing `tomni-1.9.2/tomni/illumination_correction/relative_difference/test_ratio_based.py` & `tomni-2.0.0b1/tomni/illumination_correction/relative_difference/test_ratio_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
     def test_black_image(self):
         img = np.ones((1000, 1000)) * 0
         illum_img = relative_difference(img)
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
 
-
     def test_illumination_black_white(self):
         # BLACK GREY WHITE TEST
         xx, yy = np.mgrid[:300, :300]
         dist = xx
         img = (dist >= 100) * 128 + (dist >= 200) * 128
         illum_img = relative_difference(img, gauss_size=21)
         self.assertGreaterEqual(np.min(illum_img), 0)
@@ -40,42 +39,50 @@
         img = (dist >= 100) * 50 + (dist >= 200) * 50 + 50
         illum_img = relative_difference(img, gauss_size=21)
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
 
     def test_grey_image_adj(self):
         img = np.ones((1000, 1000)) * 128
-        illum_img = relative_difference(img, smooth_size=3, do_normalize=True, resize_ratio=0.125)
+        illum_img = relative_difference(
+            img, smooth_size=3, do_normalize=True, resize_ratio=0.125
+        )
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
 
     def test_white_image_adj(self):
         img = np.ones((1000, 1000)) * 255
-        illum_img = relative_difference(img, smooth_size=3, do_normalize=True, resize_ratio=0.125)
+        illum_img = relative_difference(
+            img, smooth_size=3, do_normalize=True, resize_ratio=0.125
+        )
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
 
     def test_black_image_adj(self):
         img = np.ones((1000, 1000)) * 0
-        illum_img = relative_difference(img,smooth_size=3, do_normalize=True, resize_ratio=0.125)
+        illum_img = relative_difference(
+            img, smooth_size=3, do_normalize=True, resize_ratio=0.125
+        )
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
 
-
     def test_illumination_black_white_adj(self):
         # BLACK GREY WHITE TEST
         xx, yy = np.mgrid[:300, :300]
         dist = xx
         img = (dist >= 100) * 128 + (dist >= 200) * 128
-        illum_img = relative_difference(img, gauss_size=21, smooth_size=3, do_normalize=True, resize_ratio=0.125)
+        illum_img = relative_difference(
+            img, gauss_size=21, smooth_size=3, do_normalize=True, resize_ratio=0.125
+        )
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
 
     def test_illumination_3_shades_of_grey_adj(self):
         print("\nSTART 3 SHADES OF GREY TEST")
         xx, yy = np.mgrid[:300, :300]
         dist = xx
         img = (dist >= 100) * 50 + (dist >= 200) * 50 + 50
-        illum_img = relative_difference(img, gauss_size=21, smooth_size=3, do_normalize=True, resize_ratio=0.125)
+        illum_img = relative_difference(
+            img, gauss_size=21, smooth_size=3, do_normalize=True, resize_ratio=0.125
+        )
         self.assertGreaterEqual(np.min(illum_img), 0)
         self.assertLessEqual(np.max(illum_img), 255)
-
```

### Comparing `tomni-1.9.2/tomni/img_dim/main.py` & `tomni-2.0.0b1/tomni/img_dim/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
 
+
 def img_dim(arr, showChannels=False):
-    '''
+    """
     This function gives the image dimensions and optional channel of a numpy array.
     arr: (numpy.ndarray) the image represented as numpy array
     showChannels: (boolean) if you want to output the number of color channels e.q. 1 for greyscale, 3 for BGR, 4 for BGRA
-    '''
+    """
     s = np.shape(arr)
 
     if showChannels:
         if len(s) > 2:
             return s[1], s[0], s[2]
         else:
             return s[1], s[0], 1
     else:
-        return s[1], s[0]
+        return s[1], s[0]
```

### Comparing `tomni-1.9.2/tomni/img_dim/test_imgDim.py` & `tomni-2.0.0b1/tomni/img_dim/test_imgDim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import TestCase
-import numpy as np 
+import numpy as np
 from .main import img_dim
 
+
 class Test_img_dim(TestCase):
     def test_happyflow_no_channel(self):
         inArr = np.zeros((10, 20))
         expected = [20, 10]
         result = img_dim(inArr, False)
 
         np.testing.assert_array_equal(result, expected)
@@ -25,8 +26,8 @@
         np.testing.assert_array_equal(result, expected)
 
     def test_happyflow_with_noshow_channel(self):
         inArr = np.zeros((10, 20, 3))
         expected = [20, 10]
         result = img_dim(inArr, False)
 
-        np.testing.assert_array_equal(result, expected)
+        np.testing.assert_array_equal(result, expected)
```

### Comparing `tomni-1.9.2/tomni/img_paste/main.py` & `tomni-2.0.0b1/tomni/img_paste/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import numpy as np 
+import numpy as np
+
 
 def img_paste(big_img, small_img, x, y):
-    '''
+    """
     This function adds a small image to a bigger image by translating it to position x, y (img coordinates).
     :big_img: (numpy.ndarray) the big image that gets altered
     :small_img: (numpy.ndarray) the smaller image that gets added to the big_img
     :x: (int) image coordinate x
     :y: (int) image coordinate y
-    
+
     return: None (big_img gets altered)
-    '''
+    """
     size_bimg = (big_img.shape[1], big_img.shape[0])
     size_simg = (small_img.shape[1], small_img.shape[0])
 
     # calculate position in big image
     # START
     if x < 0:
         start_x = 0
@@ -28,37 +29,37 @@
         start_y = 0
         crop_y_start = -y
     elif y > size_bimg[1] - 1:
         return
     else:
         start_y = y
         crop_y_start = 0
-    
-    #STOP
+
+    # STOP
     if x + size_simg[0] > size_bimg[0]:
         stop_x = size_bimg[0]
         if x >= 0:
             crop_x_stop = size_bimg[0] - x
         else:
             crop_x_stop = size_bimg[0] + crop_x_start
-        
+
     elif x + size_simg[0] < 0:
         return
     else:
         stop_x = x + size_simg[0]
         crop_x_stop = size_simg[0]
-    
+
     if y + size_simg[1] > size_bimg[1]:
         stop_y = size_bimg[1]
         if y >= 0:
             crop_y_stop = size_bimg[1] - y
         else:
             crop_y_stop = size_bimg[1] + crop_y_start
     elif y + size_simg[1] < 0:
         return
     else:
         stop_y = y + size_simg[1]
         crop_y_stop = size_simg[1]
-    
+
     # Crop smaller image to fit
     overlay_img = small_img[crop_y_start:crop_y_stop, crop_x_start:crop_x_stop]
-    big_img[start_y:stop_y, start_x:stop_x] = overlay_img
+    big_img[start_y:stop_y, start_x:stop_x] = overlay_img
```

### Comparing `tomni-1.9.2/tomni/json_operations/add_area/main.py` & `tomni-2.0.0b1/tomni/json_operations/add_area/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/json_operations/add_area/test_add_area.py` & `tomni-2.0.0b1/tomni/json_operations/add_area/test_add_area.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/json_operations/add_center/test_add_center.py` & `tomni-2.0.0b1/tomni/json_operations/add_center/test_add_center.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,27 @@
         add_center(json_object)
 
         self.assertDictEqual(json_object, expected_result)
 
     def test_single_point(self):
         json_object = {
             "type": "polygon",
-            "points": [{"x": 500, "y": 50},],
+            "points": [
+                {"x": 500, "y": 50},
+            ],
             "id": "unicorn",
             "parents": [],
             "children": [],
         }
 
         expected_result = {
             "type": "polygon",
-            "points": [{"x": 500, "y": 50},],
+            "points": [
+                {"x": 500, "y": 50},
+            ],
             "id": "unicorn",
             "parents": [],
             "children": [],
             "center": {"x": 500, "y": 50},
         }
 
         add_center(json_object)
```

### Comparing `tomni-1.9.2/tomni/json_operations/add_circularity/main.py` & `tomni-2.0.0b1/tomni/json_operations/add_circularity/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-import cv2
 import math
+
+import cv2
+
+from ...contour_operations import circularity
 from ...transformers import json2contours
 
 
 def add_circularity(json_object: dict) -> None:
     """
     This function adds the property 'circularity' to the current json object.
     circularity is calculated by drawing a circle around the object,
@@ -11,22 +14,15 @@
     The bigger the difference between those 2 areas, the lower the circularity.
 
     json_object: (dict) a json object of type polygon
     """
     if json_object["type"] == "polygon":
         cnt = json2contours(json_object)
 
-        # Calculate the area of enclosing circle
-        enclosing_circle = cv2.minEnclosingCircle(cnt)
-        radius = enclosing_circle[1]
-        area_circle = radius ** 2 * math.pi
-
-        # Calculate the area of contour
-        area_contour = cv2.contourArea(cnt)
-        circularity = area_contour / area_circle
+        _circularity = circularity(cnt)
 
         # Add results to current object
-        json_object["circularity"] = circularity
+        json_object["circularity"] = _circularity
     else:
         raise ValueError(
-            f"currently only the polygon objects are supported not {json_object['type']}"
+            f"Currently only the polygon objects are supported; not {json_object['type']}"
         )
```

### Comparing `tomni-1.9.2/tomni/json_operations/add_circularity/test_add_circularity.py` & `tomni-2.0.0b1/tomni/json_operations/add_circularity/test_add_circularity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
+
 from .main import add_circularity
-import math
 
 
-class TestScaleObject(TestCase):
+class TestAddCircularity(TestCase):
     def test_square(self):
         input_json_object = {
             "type": "polygon",
             "points": [
                 {"x": 5000, "y": 0},
                 {"x": 5000, "y": 10000},
                 {"x": 15000, "y": 10000},
@@ -21,15 +21,15 @@
             "points": [
                 {"x": 5000, "y": 0},
                 {"x": 5000, "y": 10000},
                 {"x": 15000, "y": 10000},
                 {"x": 15000, "y": 0},
             ],
             "id": "unicorn",
-            "circularity": 2 / math.pi,
+            "circularity": 0.7853981633974482,
         }
 
         add_circularity(input_json_object)
         self.assertAlmostEqual(
             input_json_object["circularity"], expected_json_object["circularity"], 5
         )
```

### Comparing `tomni-1.9.2/tomni/json_operations/cropping/main.py` & `tomni-2.0.0b1/tomni/json_operations/cropping/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     """
 
     new_json_list = []
 
     json_list_copy = copy.deepcopy(json_list)
 
     for c, json_object in enumerate(json_list):
-        json_copy= copy.deepcopy(json_object)
+        json_copy = copy.deepcopy(json_object)
         to_keep = json_object_to_keep(
             json_copy,
             (x_translation, x_translation + crop_dim[0]),
             (y_translation, y_translation + crop_dim[1]),
             crop_mode,
         )
         if to_keep:
@@ -109,8 +109,8 @@
             )
 
         else:
             continue
 
         new_json_list.append(json_list_copy[c])
 
-    return new_json_list
+    return new_json_list
```

### Comparing `tomni-1.9.2/tomni/json_operations/cropping/test_crop_json.py` & `tomni-2.0.0b1/tomni/json_operations/cropping/test_crop_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase
 from .main import crop_json
 
+
 class TestRandomCropBbox(TestCase):
     def test_ellipse_x_movement(self):
         input_json = [
             {
                 "type": "ellipse",
                 "center": {"x": 2, "y": 3},
                 "radiusX": 5,
@@ -24,46 +25,45 @@
                 "center": {"x": 0, "y": 3},
                 "radiusX": 5,
                 "radiusY": 5,
                 "angleOfRotation": 0,
             }
         ]
 
-        result_json = crop_json(input_json,x_move, y_move, inputDim)
+        result_json = crop_json(input_json, x_move, y_move, inputDim)
         self.assertListEqual(result_json, expected_json)
 
     def test_ellipse_xy_movement(self):
-        
 
         input_json = [
             {
                 "type": "ellipse",
                 "center": {"x": 2, "y": 3},
                 "radiusX": 5,
                 "radiusY": 5,
                 "angleOfRotation": 0,
             },
             {"type": "ellipse", "center": {"x": 4, "y": 8}, "radiusX": 6, "radiusY": 6},
         ]
 
         inputDim = (5, 6)
-        x_move = 2 
+        x_move = 2
         y_move = 1
 
         expected_json = [
             {
                 "type": "ellipse",
                 "center": {"x": 0, "y": 2},
                 "radiusX": 5,
                 "radiusY": 5,
                 "angleOfRotation": 0,
             }
         ]
 
-        result_json = crop_json(input_json,x_move, y_move, inputDim)
+        result_json = crop_json(input_json, x_move, y_move, inputDim)
 
         self.assertListEqual(result_json, expected_json)
 
         expected_input_json = [
             {
                 "type": "ellipse",
                 "center": {"x": 2, "y": 3},
@@ -71,17 +71,17 @@
                 "radiusY": 5,
                 "angleOfRotation": 0,
             },
             {"type": "ellipse", "center": {"x": 4, "y": 8}, "radiusX": 6, "radiusY": 6},
         ]
 
         self.assertListEqual(input_json, expected_input_json)
-    
+
     def test_polygon_x_movement(self):
-    
+
         # [p, bx, by, bw, bh, c1, c2, c3]
         input_json = [
             {
                 "type": "polygon",
                 "points": [
                     {"x": 0, "y": 2},
                     {"x": 2, "y": 2},
@@ -97,15 +97,15 @@
                     {"x": 6, "y": 4},
                     {"x": 4, "y": 6},
                 ],
             },
         ]
 
         inputDim = (5, 6)
-        x_move = 2 
+        x_move = 2
         y_move = 0
 
         expected_json = [
             {
                 "type": "polygon",
                 "points": [
                     {"x": 2, "y": 6},
@@ -132,15 +132,15 @@
                     {"x": 4, "y": 6},
                     {"x": 6, "y": 6},
                     {"x": 6, "y": 4},
                     {"x": 4, "y": 6},
                 ],
             },
         ]
-        result_json = crop_json(input_json,x_move, y_move, inputDim)
+        result_json = crop_json(input_json, x_move, y_move, inputDim)
         self.assertListEqual(result_json, expected_json)
 
         self.assertEqual(len(input_json), len(expected_input_json))
         for i in range(len(input_json)):
             self.assertDictEqual(input_json[i], expected_input_json[i])
 
     def test_polygon_xy_movement(self):
@@ -165,28 +165,28 @@
                 ],
             },
         ]
 
         inputDim = (5, 6)
         x_move = 2
         y_move = 1
-        
+
         expected_json = [
             {
                 "type": "polygon",
                 "points": [
                     {"x": 2, "y": 5},
                     {"x": 4, "y": 5},
                     {"x": 4, "y": 3},
                     {"x": 2, "y": 5},
                 ],
             }
         ]
 
-        result_json = crop_json(input_json,x_move, y_move,  inputDim)
+        result_json = crop_json(input_json, x_move, y_move, inputDim)
         self.assertListEqual(result_json, expected_json)
 
     def test_expected_polygon_no_crop(self):
 
         input_json = [
             {
                 "type": "polygon",
@@ -260,10 +260,9 @@
 
         inputDim = (2, 2)
         x_move = 8
         y_move = 0
 
         expected_json = []
 
-        result_json = crop_json(input_json,x_move, y_move,  inputDim)
+        result_json = crop_json(input_json, x_move, y_move, inputDim)
         self.assertListEqual(result_json, expected_json)
-
```

### Comparing `tomni-1.9.2/tomni/json_operations/flipping/main.py` & `tomni-2.0.0b1/tomni/json_operations/flipping/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
                 img_dim - json_object["points"][point_n]["y"] - 1
             )
     else:
         raise TypeError(
             f"The type {json_object['type']} is not found in flipping augmentation"
         )
 
-    return newjson_object
+    return newjson_object
```

### Comparing `tomni-1.9.2/tomni/json_operations/flipping/test_flip_json.py` & `tomni-2.0.0b1/tomni/json_operations/flipping/test_flip_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from unittest import TestCase
 from .main import flip_json
 
 
-
 class TestFlipPatch(TestCase):
     def test_flips(self):
         input_json = {
-                "type": "ellipse",
-                "center": {"x": 9, "y": 3},
-                "radiusX": 5,
-                "radiusY": 5,
-                "angleOfRotation": 0,
-            }
-        
-        result_json = flip_json(input_json,10)
+            "type": "ellipse",
+            "center": {"x": 9, "y": 3},
+            "radiusX": 5,
+            "radiusY": 5,
+            "angleOfRotation": 0,
+        }
+
+        result_json = flip_json(input_json, 10)
         expected_json = {
-                "type": "ellipse",
-                "center": {"x": 9, "y": 6},
-                "radiusX": 5,
-                "radiusY": 5,
-                "angleOfRotation": 0,
-            }
+            "type": "ellipse",
+            "center": {"x": 9, "y": 6},
+            "radiusX": 5,
+            "radiusY": 5,
+            "angleOfRotation": 0,
+        }
 
-        
         self.assertDictEqual(result_json, expected_json)
 
     def test_flips_polygon(self):
         input_json = {
-                "type": "polygon",
-                "points": [{"x": 7, "y": 2}, {"x": 7, "y": 6}, {"x": 12, "y": 5}],
-            }
-        result_json = flip_json(input_json,10)
+            "type": "polygon",
+            "points": [{"x": 7, "y": 2}, {"x": 7, "y": 6}, {"x": 12, "y": 5}],
+        }
+        result_json = flip_json(input_json, 10)
         expected_json = {
-                "type": "polygon",
-                "points": [{"x": 7, "y": 7}, {"x": 7, "y": 3}, {"x": 12, "y": 4}],
-            }
+            "type": "polygon",
+            "points": [{"x": 7, "y": 7}, {"x": 7, "y": 3}, {"x": 12, "y": 4}],
+        }
         self.assertDictEqual(result_json, expected_json)
-
```

### Comparing `tomni-1.9.2/tomni/json_operations/rotation/main.py` & `tomni-2.0.0b1/tomni/json_operations/rotation/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,8 @@
                 newjson_object["points"][point_n]["y"] = (
                     img_shape[1] - json_object["points"][point_n]["x"] - 1
                 )
 
         else:
             raise ValueError("Unkown Angle should be 0, 90, 180 or 270")
 
-    return newjson_object
+    return newjson_object
```

### Comparing `tomni-1.9.2/tomni/json_operations/rotation/test_rotate_json.py` & `tomni-2.0.0b1/tomni/json_operations/rotation/test_rotate_json.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/json_operations/scale_json/main.py` & `tomni-2.0.0b1/tomni/json_operations/scale_json/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,28 @@
     """
     Takes in a json object (ellipse or polygon) and makes it scaling_factor bigger
     json_object: (dict) following the standard format
     scaling_factor: (float) the multiplier of the object
 
     example:
     json_object = {
-        "type": "ellipse", 
-        "center": {"x": 100, "y": 200}, 
-        "radiusX": 50, 
-        "radiusY": 100, 
-        "angleOfRotation": 0, 
+        "type": "ellipse",
+        "center": {"x": 100, "y": 200},
+        "radiusX": 50,
+        "radiusY": 100,
+        "angleOfRotation": 0,
         "id": "12345-abcde"}
     scaling_factor = 2
 
     result = {
-        "type": "ellipse", 
-        "center": {"x": 200, "y": 400}, 
-        "radiusX": 100, 
-        "radiusY": 200, 
-        "angleOfRotation": 0, 
+        "type": "ellipse",
+        "center": {"x": 200, "y": 400},
+        "radiusX": 100,
+        "radiusY": 200,
+        "angleOfRotation": 0,
         "id": "12345-abcde"}
 
     """
     newjson_object = json_object.copy()
     if json_object["type"] == "ellipse":
         newjson_object["radiusX"] = int(round(json_object["radiusX"] * scaling_factor))
         newjson_object["radiusY"] = int(round(json_object["radiusY"] * scaling_factor))
@@ -44,8 +44,7 @@
                 }
             )
         newjson_object["points"] = all_points
     else:
         raise ValueError(f"type {json_object['type']} is not supported")
 
     return newjson_object
-
```

### Comparing `tomni-1.9.2/tomni/json_operations/scale_json/test_scaleResults.py` & `tomni-2.0.0b1/tomni/json_operations/scale_json/test_scaleResults.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 
     def test_unknown_type(self):
         inputDict = {
             "type": "unicornType",
         }
         inputScaling = 1.02
         with self.assertRaises(ValueError):
-            result = scale_json(inputDict, inputScaling)
+            result = scale_json(inputDict, inputScaling)
```

### Comparing `tomni-1.9.2/tomni/json_operations/summary_json/main.py` & `tomni-2.0.0b1/tomni/json_operations/summary_json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/json_operations/summary_json/test_summary_json.py` & `tomni-2.0.0b1/tomni/json_operations/summary_json/test_summary_json.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/json_operations/translation/main.py` & `tomni-2.0.0b1/tomni/json_operations/translation/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-
-
 def translation_json(json_object: dict, x_translation: int, y_translation: int):
     """
     Takes in a json object (ellipse or polygon) and translates it
     json_object: (dict) following the standard format
     x_translation: (int) The translation in the x-direction
     y_translation: (int) The translation in the y-direction
 
     example:
     json_object = {
-        "type": "ellipse", 
-        "center": {"x": 100, "y": 200}, 
-        "radiusX": 50, 
-        "radiusY": 100, 
-        "angleOfRotation": 0, 
+        "type": "ellipse",
+        "center": {"x": 100, "y": 200},
+        "radiusX": 50,
+        "radiusY": 100,
+        "angleOfRotation": 0,
         "id": "12345-abcde"}
     x_translation = 100
     y_translation = -20
 
     result = {
-        "type": "ellipse", 
-        "center": {"x": 200, "y": 180}, 
-        "radiusX": 50, 
-        "radiusY": 100, 
-        "angleOfRotation": 0, 
+        "type": "ellipse",
+        "center": {"x": 200, "y": 180},
+        "radiusX": 50,
+        "radiusY": 100,
+        "angleOfRotation": 0,
         "id": "12345-abcde"}
 
     """
     newjson_object = json_object.copy()
     if json_object["type"] == "ellipse":
         newjson_object["center"]["x"] = int(
             round(json_object["center"]["x"] + x_translation)
@@ -46,8 +44,7 @@
                 }
             )
         newjson_object["points"] = all_points
     else:
         raise ValueError(f"type {json_object['type']} is not supported")
 
     return newjson_object
-
```

### Comparing `tomni-1.9.2/tomni/json_operations/translation/test_translation_json.py` & `tomni-2.0.0b1/tomni/json_operations/translation/test_translation_json.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/make_mask/circlair_mask/main.py` & `tomni-2.0.0b1/tomni/make_mask/circlair_mask/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
     xx = xx.astype(np.int32)
     yy = yy.astype(np.int32)
 
     xx -= img_shape[1] - 1
     yy -= img_shape[0] - 1
 
-    circle = xx ** 2 + yy ** 2
-    kernel = circle <= diameter ** 2
+    circle = xx**2 + yy**2
+    kernel = circle <= diameter**2
 
     return kernel
 
 
 def make_big_mask_circle(img_shape, diameter):
     out = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (diameter, diameter))
     out = bbox_fitting_center(out, img_shape)
-    return out.astype(np.bool)
+    return out.astype(bool)
```

### Comparing `tomni-1.9.2/tomni/make_mask/circlair_mask/test_circle_mask.py` & `tomni-2.0.0b1/tomni/make_mask/circlair_mask/test_circle_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 from __future__ import absolute_import
 from unittest import TestCase
 from .main import make_mask_circle
 import numpy as np
 
+
 class TestCircle_mask_selector(TestCase):
     def test_5x5_5(self):
-        expected = np.array([
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 1, 1],
-            [0, 1, 1, 1, 0]
-        ])
+        expected = np.array(
+            [
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 1, 1],
+                [0, 1, 1, 1, 0],
+            ]
+        )
 
         result = make_mask_circle((5, 5), 5)
         np.testing.assert_array_equal(result, expected)
 
     def test_5x7_5(self):
-        expected = np.array([
-            [0, 0, 0, 0, 0],
-            [0, 1, 1, 1, 0],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 1, 1],
-            [1, 1, 1, 1, 1],
-            [0, 1, 1, 1, 0],
-            [0, 0, 0, 0, 0],
-        ])
+        expected = np.array(
+            [
+                [0, 0, 0, 0, 0],
+                [0, 1, 1, 1, 0],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 1, 1],
+                [1, 1, 1, 1, 1],
+                [0, 1, 1, 1, 0],
+                [0, 0, 0, 0, 0],
+            ]
+        )
 
         result = make_mask_circle((5, 7), 5)
         np.testing.assert_array_equal(result, expected)
-    
+
     def test_7x7_5(self):
-        expected = np.array([
-            [0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 1, 1, 1, 0, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 0, 1, 1, 1, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0],
-        ])
+        expected = np.array(
+            [
+                [0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 1, 1, 1, 0, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 0, 1, 1, 1, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0],
+            ]
+        )
 
         result = make_mask_circle((7, 7), 5)
         np.testing.assert_array_equal(result, expected)
 
     def test_7x10_6(self):
-        expected = np.array([
-            [0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 1, 1, 1, 0, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 1, 1, 1, 1, 1, 0],
-            [0, 0, 1, 1, 1, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0],
-        ])
+        expected = np.array(
+            [
+                [0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 1, 1, 1, 0, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 1, 1, 1, 1, 1, 0],
+                [0, 0, 1, 1, 1, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0],
+            ]
+        )
 
         result = make_mask_circle((7, 10), 6)
         np.testing.assert_array_equal(result, expected)
 
     def test_big_301x201(self):
-        result = make_mask_circle((301, 201),101)
+        result = make_mask_circle((301, 201), 101)
         self.assertEqual(np.shape(result), (201, 301))
         self.assertEqual(result[0, 0], False)
         self.assertEqual(result[0, 150], False)
         self.assertEqual(result[25, 75], False)
         self.assertEqual(result[100, 150], True)
         self.assertEqual(result[63, 117], True)
-        
+
     def test_overflow_5001(self):
-        result = make_mask_circle((5001, 5001),5000)
+        result = make_mask_circle((5001, 5001), 5000)
 
         self.assertEqual(result[0, 0], False)
         self.assertEqual(result[5000, 5000], False)
         self.assertEqual(result[4300, 4300], False)
         self.assertEqual(result[2500, 2500], True)
         self.assertEqual(result[3300, 3300], True)
```

### Comparing `tomni-1.9.2/tomni/make_mask/contour_mask_maker/main.py` & `tomni-2.0.0b1/tomni/make_mask/contour_mask_maker/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/make_mask/ellipse_mask/main.py` & `tomni-2.0.0b1/tomni/make_mask/ellipse_mask/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
     :param image_size: the size of the image
     :param x1: x coordinate of the center of the ellipse
     :param y1: y coordinate of the center of the ellipse
     :param rx: the length of the radius on the x axis of the ellipse
     :param ry: the length of the radius on the y axis of the ellipse
     :return: an image with an ellipse of True surrounded by False
-    
+
     Futere request: Variable Alpha.
-    
+
     For rotated ellipses, the alpha value is used to find the translated points
     alpha = angle of rotation (in degrees)
     alpha = 0 gives no rotation of the ellipse
 
     The sin() and cos() values are calculated using math library
 
     The following formula can be used to calculate the coordinates:
@@ -57,25 +57,25 @@
 
     yy, xx = np.mgrid[: image_size[1], : image_size[0]]
 
     xx = xx.astype(np.int32)
     yy = yy.astype(np.int32)
 
     # Center point of the ellipse becomes the (0, 0) point of the image
-    xx -= x1 
-    yy -= y1 
+    xx -= x1
+    yy -= y1
 
     # The ellipse formula used to calculate the points is
     # x^2 * (ry)^2 + y^2 * (rx)^2
     # Calculating the value of each point depending on the ellipse equation
-    ellipse = (xx ** 2) * (ry ** 2) + (yy ** 2) * (rx ** 2)
+    ellipse = (xx**2) * (ry**2) + (yy**2) * (rx**2)
 
     # The ellipse formula determines if a point is inside the ellipse or not
     # x^2 * (ry)^2 + y^2 * (rx)^2 <= (rx)^2 * (ry)^2
-    kernel = ellipse <= (rx ** 2) * (ry ** 2)
+    kernel = ellipse <= (rx**2) * (ry**2)
     kernel = kernel * (np.abs(xx) <= rx)
     kernel = kernel * (np.abs(yy) <= ry)
     return kernel
 
 
 def make_big_mask_ellipse(image_size, xe, ye, rex, rey):
     """
```

### Comparing `tomni-1.9.2/tomni/shape_fitting/fit_rect_ellipse/main.py` & `tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     x, y: (int, int) middle point of ellipse
     r1: (float) longest radius
     r2: (float) shortest radius. By definition 90 degrees away from r1
     alpha: (float) degrees between r1 and x-axis.
     Special thanks to: https://math.stackexchange.com/questions/91132/how-to-get-the-limits-of-rotated-ellipse
     """
     alpha = alpha / 180 * np.pi
-    a = np.sqrt(r1 ** 2 * np.cos(alpha) ** 2 + r2 ** 2 * np.sin(alpha) ** 2)
-    b = np.sqrt(r1 ** 2 * np.sin(alpha) ** 2 + r2 ** 2 * np.cos(alpha) ** 2)
+    a = np.sqrt(r1**2 * np.cos(alpha) ** 2 + r2**2 * np.sin(alpha) ** 2)
+    b = np.sqrt(r1**2 * np.sin(alpha) ** 2 + r2**2 * np.cos(alpha) ** 2)
     x1 = int(round(x - a))
     y1 = int(round(y - b))
     x2 = int(round(x + a))
     y2 = int(round(y + b))
     return x1, y1, x2, y2
```

### Comparing `tomni-1.9.2/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py` & `tomni-2.0.0b1/tomni/shape_fitting/fit_rect_ellipse/test_fitRectEllipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import absolute_import
 from unittest import TestCase
 from .main import fit_rect_around_ellipse
 import numpy as np
 
+
 class Testfit_rect_around_ellipse(TestCase):
     def test_fit_circle(self):
         x = 0
         y = 100
         r1 = 900
         r2 = 900
         alpha = 0
@@ -38,19 +39,18 @@
         x1, y1, x2, y2 = fit_rect_around_ellipse(x, y, r1, r2, alpha)
 
         self.assertEqual(x1, expectedX1)
         self.assertEqual(y1, expectedY1)
         self.assertEqual(x2, expectedX2)
         self.assertEqual(y2, expectedY2)
 
-
     def test_fit_ellipse_with_rotation(self):
-        '''
-        These number where measured using InkScape 
-        '''
+        """
+        These number where measured using InkScape
+        """
         x = 108
         y = 185
         r1 = 79
         r2 = 50
         alpha = 30
 
         expectedX1 = 35
@@ -62,8 +62,8 @@
 
         print(x1, y1, x2, y2)
         print("width {} expected width {}".format(x2 - x1, expectedX2 - expectedX1))
         print("height {} expected height {}".format(y2 - y1, expectedY2 - expectedY1))
         self.assertAlmostEqual(x1, expectedX1, 0)
         self.assertAlmostEqual(y1, expectedY1, 0)
         self.assertAlmostEqual(x2, expectedX2, 0)
-        self.assertAlmostEqual(y2, expectedY2, 0)
+        self.assertAlmostEqual(y2, expectedY2, 0)
```

### Comparing `tomni-1.9.2/tomni/transformers/contour2bbox/main.py` & `tomni-2.0.0b1/tomni/transformers/contour2bbox/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/contour2bbox/test_contour2bbox.py` & `tomni-2.0.0b1/tomni/transformers/contour2bbox/test_contour2bbox.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/contours2json/main.py` & `tomni-2.0.0b1/tomni/transformers/contours2json/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import uuid
 import numpy as np
 from typing import List, Union
 
+
 def contours2json(contours: Union[np.ndarray, List[list]]) -> List[dict]:
     """
     Transforms a list or array of contours into list of jsons
     contours: (numpy.array, list) needs to be the contours produced by opencv
-    """ 
+    """
     result = []
     for contour in contours:
         shape = {"type": "polygon", "points": []}
         for point in contour:
-            shape["points"].append(dict(x = int(point[0][0]), y = int(point[0][1])))
-        shape['id'] = str(uuid.uuid4())
-        shape['parents'] = []
-        shape['children'] = []
+            shape["points"].append(dict(x=int(point[0][0]), y=int(point[0][1])))
+        shape["id"] = str(uuid.uuid4())
+        shape["parents"] = []
+        shape["children"] = []
         result.append(shape)
-    return result
+    return result
```

### Comparing `tomni-1.9.2/tomni/transformers/contours2json/test_contours2json.py` & `tomni-2.0.0b1/tomni/transformers/contours2json/test_contours2json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from unittest import TestCase
 import numpy as np
 from .main import contours2json
 
+
 class TestContour2json(TestCase):
     def test_happy_flow(self):
         inputContours = np.array([[[[500, 50]], [[500, 99]], [[539, 99]], [[539, 50]]]])
 
-        expectedResult = [{
-            "type": "polygon",
-            "points": [
-                {"x": 500, "y": 50},
-                {"x": 500, "y": 99},
-                {"x": 539, "y": 99},
-                {"x": 539, "y": 50},
-            ],
-            "id": "unicorn",
-            "parents": [],
-            "children": [],
-        }]
+        expectedResult = [
+            {
+                "type": "polygon",
+                "points": [
+                    {"x": 500, "y": 50},
+                    {"x": 500, "y": 99},
+                    {"x": 539, "y": 99},
+                    {"x": 539, "y": 50},
+                ],
+                "id": "unicorn",
+                "parents": [],
+                "children": [],
+            }
+        ]
 
         result = contours2json(inputContours)
         result[0]["id"] = "unicorn"
 
         self.assertEqual(len(result), len(expectedResult))
         for i in range(len(result)):
-            print(f"future {i}: \n input \n {result[i]} \n expected \n {expectedResult[i]}")
-            self.assertDictEqual(result[i], expectedResult[i])
+            print(
+                f"future {i}: \n input \n {result[i]} \n expected \n {expectedResult[i]}"
+            )
+            self.assertDictEqual(result[i], expectedResult[i])
```

### Comparing `tomni-1.9.2/tomni/transformers/ellipse2json/main.py` & `tomni-2.0.0b1/tomni/transformers/ellipse2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/ellipse2json/test_ellipse2json.py` & `tomni-2.0.0b1/tomni/transformers/ellipse2json/test_ellipse2json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from unittest import TestCase
 import numpy as np
 from .main import ellipse2json
 
+
 class TestEllipse2json(TestCase):
     def test_happy_flow_circle(self):
         expectedResult = {
-        "type": "ellipse",
-        "center": {"x": 20, "y": 30},
-        "radiusX": 10,
-        "radiusY": 10,
-        "angleOfRotation": 0,
-        "id": "unicorn",
-    }
+            "type": "ellipse",
+            "center": {"x": 20, "y": 30},
+            "radiusX": 10,
+            "radiusY": 10,
+            "angleOfRotation": 0,
+            "id": "unicorn",
+        }
 
         result = ellipse2json(20, 30, 10)
         result["id"] = "unicorn"
 
         self.assertDictEqual(result, expectedResult)
 
     def test_happy_flow_ellipse(self):
         expectedResult = {
-        "type": "ellipse",
-        "center": {"x": 20, "y": 30},
-        "radiusX": 10,
-        "radiusY": 15,
-        "angleOfRotation": 0.98,
-        "id": "unicorn",
-    }
+            "type": "ellipse",
+            "center": {"x": 20, "y": 30},
+            "radiusX": 10,
+            "radiusY": 15,
+            "angleOfRotation": 0.98,
+            "id": "unicorn",
+        }
 
         result = ellipse2json(20, 30, 10, 15, 0.98)
         result["id"] = "unicorn"
 
-        self.assertDictEqual(result, expectedResult)
+        self.assertDictEqual(result, expectedResult)
```

### Comparing `tomni-1.9.2/tomni/transformers/json2contours/main.py` & `tomni-2.0.0b1/tomni/transformers/json2contours/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import numpy as np
 
 
 def json2contours(json: dict) -> np.ndarray:
-    '''
+    """
     Set a default json format object to a contour.
     json: (dict) the objects needs:
         'points': (if polygon) list of dict of form {x: ..., y: ...}
-        'type': needs to be polygon 
-    '''
-    if json.get('type', '').lower() == 'polygon':
+        'type': needs to be polygon
+    """
+    if json.get("type", "").lower() == "polygon":
         result = [[[i["x"], i["y"]]] for i in json["points"]]
     else:
-        raise ValueError(f"The type {json.get('type', 'NO TYPE GIVEN')} is not supported")
+        raise ValueError(
+            f"The type {json.get('type', 'NO TYPE GIVEN')} is not supported"
+        )
     return np.array(result, dtype=np.int32)
```

### Comparing `tomni-1.9.2/tomni/transformers/json2contours/test_contours2json.py` & `tomni-2.0.0b1/tomni/transformers/json2contours/test_contours2json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from unittest import TestCase
 import numpy as np
 from .main import json2contours
 
+
 class TestJson2contours(TestCase):
     def test_happy_flow(self):
-        expectedResult  = np.array([[[500, 50]], [[500, 99]], [[539, 99]], [[539, 50]]])
+        expectedResult = np.array([[[500, 50]], [[500, 99]], [[539, 99]], [[539, 50]]])
 
         inputContours = {
             "type": "polygon",
             "points": [
                 {"x": 500, "y": 50},
                 {"x": 500, "y": 99},
                 {"x": 539, "y": 99},
@@ -50,8 +51,8 @@
             ],
             "id": "unicorn",
             "parents": [],
             "children": [],
         }
 
         with self.assertRaises(ValueError):
-            json2contours(inputContours)
+            json2contours(inputContours)
```

### Comparing `tomni-1.9.2/tomni/transformers/json2dict/main.py` & `tomni-2.0.0b1/tomni/transformers/json2dict/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
             else:
                 if isinstance(json_object[key], dict):
                     variable = [json_object[key][x] for x in json_object[key].keys()]
                 else:
                     variable = json_object[key]
                 json_dict[key].append(variable)
 
-    return json_dict
+    return json_dict
```

### Comparing `tomni-1.9.2/tomni/transformers/json2dict/test_json2dict.py` & `tomni-2.0.0b1/tomni/transformers/json2dict/test_json2dict.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -148,8 +148,8 @@
         expected_output = {
             "cytosmart": [None, None],
             "index": [0, 1],
         }
 
         result = json2dict(input_json_list, ["cytosmart"])
 
-        self.assertDictEqual(result, expected_output)
+        self.assertDictEqual(result, expected_output)
```

### Comparing `tomni-1.9.2/tomni/transformers/json2labels/main.py` & `tomni-2.0.0b1/tomni/transformers/json2labels/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,15 @@
                 360,
                 color=i + 1,
                 thickness=-1,
             )
         elif obj["type"] == "polygon":
             points = np.empty((len(obj["points"]), 2))
             for j in range(len(obj["points"])):
-                points[j,] = [obj["points"][j]["x"], obj["points"][j]["y"]]
+                points[
+                    j,
+                ] = [obj["points"][j]["x"], obj["points"][j]["y"]]
             cv2.fillConvexPoly(seg_map, np.int32([points]), i + 1)
         else:
             raise ValueError("Object type not supported")
 
     return seg_map
```

### Comparing `tomni-1.9.2/tomni/transformers/json2mask/main.py` & `tomni-2.0.0b1/tomni/transformers/json2mask/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from ... import img_dim
+from ...img_dim import img_dim
 from ...make_mask import make_mask_contour, make_mask_ellipse
 from ..json2contours import json2contours
 
 
 def contour2mask(mask: np.ndarray, contour: list) -> np.ndarray:
     """Converts contour to mask"""
     add_mask = make_mask_contour(img_dim(mask), contour)
```

### Comparing `tomni-1.9.2/tomni/transformers/json2mask/test_json2mask.py` & `tomni-2.0.0b1/tomni/transformers/json2mask/test_json2mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from numpy.testing import assert_array_equal
 from unittest import TestCase
 
 from .main import json2mask
 from ...make_mask import make_mask_circle
 
+
 class TestJson2Mask(TestCase):
     @classmethod
     def setUp(self):
         self.json_objects = [
             {
                 "type": "polygon",
                 "points": [
@@ -224,17 +225,17 @@
         assert_array_equal(expected_result, result)
 
     def test_circle_floats(self):
         size = (11, 13)
         json_objects = [
             {
                 "type": "ellipse",
-                "center": {"x": 6., "y": 4.},
-                "radiusX": 6.,
-                "radiusY": 4.,
+                "center": {"x": 6.0, "y": 4.0},
+                "radiusX": 6.0,
+                "radiusY": 4.0,
                 "angleOfRotation": 0,
                 "id": "unicorn",
             }
         ]
 
         expected = np.array(
             [
@@ -263,62 +264,62 @@
                 "type": "ellipse",
                 "center": {"x": 5000, "y": 2467},
                 "radiusX": 3200,
                 "radiusY": 1692,
                 "angleOfRotation": 0,
                 "id": "unicorn",
             }
-        ]    
+        ]
 
         mask = json2mask(json_objects, size, 0)
         self.assertEqual(True, mask[2467][5000])
         self.assertEqual(True, mask[3000][5000])
 
         # X minimum
         self.assertEqual(False, mask[2467][1798])
         self.assertEqual(True, mask[2467][1801])
 
         # X Maximum
         self.assertEqual(True, mask[2467][8198])
         self.assertEqual(False, mask[2467][8201])
-        
+
         # Y minimum
         self.assertEqual(False, mask[773][5000])
         self.assertEqual(True, mask[777][5000])
 
         # Y maximum
         self.assertEqual(True, mask[4157][5000])
         self.assertEqual(False, mask[4161][5000])
 
     def test_big_circle_floats(self):
         size = (10000, 10001)
 
         json_objects = [
             {
                 "type": "ellipse",
-                "center": {"x": 5000., "y": 2467.},
-                "radiusX": 3200.,
-                "radiusY": 1692.,
+                "center": {"x": 5000.0, "y": 2467.0},
+                "radiusX": 3200.0,
+                "radiusY": 1692.0,
                 "angleOfRotation": 0,
                 "id": "unicorn",
             }
-        ]    
+        ]
 
         mask = json2mask(json_objects, size, 0)
         self.assertEqual(True, mask[2467][5000])
         self.assertEqual(True, mask[3000][5000])
 
         # X minimum
         self.assertEqual(False, mask[2467][1798])
         self.assertEqual(True, mask[2467][1801])
 
         # X Maximum
         self.assertEqual(True, mask[2467][8198])
         self.assertEqual(False, mask[2467][8201])
-        
+
         # Y minimum
         self.assertEqual(False, mask[773][5000])
         self.assertEqual(True, mask[777][5000])
 
         # Y maximum
         self.assertEqual(True, mask[4157][5000])
         self.assertEqual(False, mask[4161][5000])
@@ -376,8 +377,8 @@
             }
         ]
 
         expected = np.zeros((500, 500), dtype=np.uint8)
         expected[75:126, 75:126] = make_mask_circle((51, 51), 50)
 
         result = json2mask(json_objects, size, 0)
-        assert_array_equal(result, expected)
+        assert_array_equal(result, expected)
```

### Comparing `tomni-1.9.2/tomni/transformers/json2vgg/main.py` & `tomni-2.0.0b1/tomni/transformers/json2vgg/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/json2vgg/test_json2vgg.py` & `tomni-2.0.0b1/tomni/transformers/json2vgg/test_json2vgg.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/labels2contours/test_labels2contours.py` & `tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/test_labels2listsOfPoints.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import absolute_import
 from unittest import TestCase
 import numpy as np
 from numpy import array, uint8, uint16, uint32, int64
-from .main import labels2contours
+from .main import labels2listsOfPoints
 
 
-class TestSelect_labels2Contours(TestCase):
-    def test_happy_flow(self):
+class TestSelect_labels2ListOfPoints(TestCase):
+    def test_select_labels_as_indices(self):
         data = array(
             [
                 [0, 5, 5, 0, 0, 0],
-                [0, 5, 5, 0, 0, 0],
-                [1, 1, 1, 0, 0, 0],
+                [0, 0, 0, 0, 3, 3],
+                [1, 0, 0, 0, 0, 0],
                 [0, 2, 0, 0, 0, 0],
                 [0, 2, 2, 0, 0, 0],
-                [0, 2, 2, 2, 0, 0],
-                [0, 2, 2, 2, 2, 0],
+                [0, 2, 2, 0, 8, 0],
+                [0, 2, 2, 0, 0, 0],
             ]
         )
 
         expected_output = [
-            [[[0, 2]], [[2, 2]]], #1
-            [[[1, 3]], [[1, 6]], [[4, 6]]], #2
-            [[[1, 0]], [[1, 1]], [[2, 1]], [[2, 0]]], #5
+            [[0, 2]],
+            [[1, 3], [1, 4], [1, 5], [1, 6], [2, 4], [2, 5], [2, 6]],
+            [[4, 1], [5, 1]],
+            [[1, 0], [2, 0]],
+            [[4, 5]],
         ]
 
-        result = labels2contours(data)
+        result = labels2listsOfPoints(data)
 
         self.assertEqual(len(expected_output), len(result))
 
         for i in range(len(expected_output)):
             x = result[i]
             print(x)
             np.testing.assert_array_equal(x, expected_output[i])
-
```

### Comparing `tomni-1.9.2/tomni/transformers/labels2listsOfPoints/integration_real_data.py` & `tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/integration_real_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #%%
-import numpy as np 
+import numpy as np
 from time import time
 
 from tomni.select_labels.main import select_labels_as_indices
 import pickle
 
 path = r"C:\Users\tomni\Downloads\labels.dump"
-fileObject = open(path,'rb')
+fileObject = open(path, "rb")
 data = pickle.load(fileObject)
 
 # #%% version 3
 # start = time()
 # result = select_labels_as_indices(data)
 # print("0.3.3 timing", time() - start)
 
 #%% version 2
-import numpy as np 
+import numpy as np
 from time import time
 
 from main_0_4 import select_labels_as_indices as select_labels_as_indices_v2
 
 start = time()
 result = select_labels_as_indices_v2(data)
-print("scipy timing", time() - start)
+print("scipy timing", time() - start)
```

### Comparing `tomni-1.9.2/tomni/transformers/labels2listsOfPoints/main.py` & `tomni-2.0.0b1/tomni/transformers/labels2listsOfPoints/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import numpy as np
 from scipy.sparse import csr_matrix, find
 import numpy_indexed as npi
 
+
 def labels2listsOfPoints(labels: np.ndarray) -> np.ndarray:
-    '''
+    """
     Transforms each label into a list of points.
     These points are for every point in the label.
 
     labels: (numpy.array) An array where every pixel is labeled to which object it belongs
-    '''
+    """
     if np.max(labels) < 256:
         dataType = np.uint8
     elif np.max(labels) < 65536:
         dataType = np.uint16
     elif np.max(labels) < 4294967296:
         dataType = np.uint32
     else:
         raise ValueError("There are to many labels")
-    
+
     # Memory check number of labels
     c = csr_matrix(labels, dtype=dataType)
     x, y, v = find(c)
     g = npi.group_by(v)
     output = g.split_array_as_list(np.array([y, x]).transpose())
     return output
```

### Comparing `tomni-1.9.2/tomni/transformers/list_of_points2json/main.py` & `tomni-2.0.0b1/tomni/transformers/list_of_points2json/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from typing import Union
 import numpy as np
 from ..contours2json import contours2json
 
 
 def list_of_points2json(list_of_points: Union[list, np.array]) -> dict:
-    ''''
+    """'
     From a list of points in the form of [[x1, y1], [x2, y2], ... ,[xn, yn]] a json is made
 
     list_of_points: (list or numpy array) the list of points that discripe a polygon.
         In the form of [[x1, y1], [x2, y2], ... ,[xn, yn]].
-    '''
+    """
     contours = np.array(list_of_points)
-    contours = contours.reshape((
-        1,
-        contours.shape[0],
-        1,
-        contours.shape[1]
-    ))
+    contours = contours.reshape((1, contours.shape[0], 1, contours.shape[1]))
 
     json_object = contours2json(contours)[0]
-    return json_object
+    return json_object
```

### Comparing `tomni-1.9.2/tomni/transformers/list_of_points2json/test_list_of_points2json.py` & `tomni-2.0.0b1/tomni/transformers/list_of_points2json/test_list_of_points2json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import TestCase
 import numpy as np
 from .main import list_of_points2json
 
+
 class TestContour2json(TestCase):
     def test_happy_flow_np_array(self):
         list_of_points = np.array([[500, 50], [500, 99], [539, 99], [539, 50]])
 
         expectedResult = {
             "type": "polygon",
             "points": [
@@ -39,8 +40,8 @@
             "parents": [],
             "children": [],
         }
 
         result = list_of_points2json(list_of_points)
         result["id"] = "unicorn"
 
-        self.assertDictEqual(result, expectedResult)
+        self.assertDictEqual(result, expectedResult)
```

### Comparing `tomni-1.9.2/tomni/transformers/mask2bbox/main.py` & `tomni-2.0.0b1/tomni/transformers/mask2bbox/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/mask2bbox/test_mask2bbox.py` & `tomni-2.0.0b1/tomni/transformers/mask2bbox/test_mask2bbox.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -135,8 +135,8 @@
                 [0, 0, 0, 0, 0, 0, 0, 0, 1, 1],
                 [0, 0, 0, 0, 0, 0, 0, 0, 1, 1],
             ],
             dtype=np.uint8,
         )
         output_function = mask2bbox(input, 1)
         expected_output = (7, 7, 10, 10)
-        self.assertEqual(output_function, expected_output)
+        self.assertEqual(output_function, expected_output)
```

### Comparing `tomni-1.9.2/tomni/transformers/mask2json/main.py` & `tomni-2.0.0b1/tomni/transformers/mask2json/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 from ..contours2json import contours2json
 from ..labels2contours import labels2contours
 
 
 def get_edges(mask: np.ndarray):
-    """ get edges of the mask"""
+    """get edges of the mask"""
     mask_copy = cv2.copyMakeBorder(
         mask,
         top=1,
         bottom=1,
         left=1,
         right=1,
         borderType=cv2.BORDER_CONSTANT,
@@ -24,40 +24,72 @@
     edges = edges.astype(np.uint8)
     edges = edges[1:-1, 1:-1]
 
     return edges
 
 
 def mask2json(
-    mask: np.ndarray, minimum_size_contours: int = 3, is_diagonal_connected=True
+    mask: np.ndarray,
+    minimum_size_contours: int = 3,
+    is_diagonal_connected=True,
+    return_inner_contours: bool = False,
 ) -> list:
     """
     Converts binary mask to standard cytosmart format
 
     Args:
         mask (np.ndarray): binary mask
         minimum_size_contours (int, optional): The minimum number of points an contour should have to be included. Defaults to 3.
         is_diagonal_connected (bool, optional): If true diagonal pixels [[1, 0][0,1]] will be seen as the same object. Defaults to True.
+        return_inner_contours (bool, optional): return the internal contours.
+            These contours are around the holes with the contour
+            default: False
 
     Returns:
-        list: json_objects, e.g [{'type':'polygon', 'points':[{'x':1,'y':4},{'x':2,'y':3},{'x':4,'y':4} ]
+        list: json_objects,
+            e.g [
+                    {
+                        'type':'polygon',
+                        'points':[
+                            {'x':1,'y':4},
+                            {'x':2,'y':3},
+                            {'x':4,'y':4}
+                        ],
+                        "innerObjects": [
+                            {
+                                'type':'polygon',
+                                'points':[
+                                    {'x':3,'y':2}
+                                ]
+                            }
+                        ]
+                    }
+                ]
     """
     connectivity = 4
     if is_diagonal_connected:
         connectivity = 8
 
     labels = cv2.connectedComponents(mask.astype(np.uint8), connectivity=connectivity)[
         1
     ]
     edges = get_edges(mask)
 
     edges = edges * labels
     del labels
-    contours = labels2contours(edges)
-    json_objects = contours2json(contours)
+    contours = labels2contours(edges, return_inner_contours=return_inner_contours)
+
+    if return_inner_contours:
+        json_objects = []
+        for contour in contours:
+            json_object = contours2json([contour[0]])[0]
+            json_object["innerObjects"] = contours2json(contour[1])
+            json_objects.append(json_object)
+    else:
+        json_objects = contours2json(contours)
     json_objects = [
         json_object
         for i, json_object in enumerate(json_objects)
         if len(json_objects[i]["points"]) >= minimum_size_contours
     ]
 
     return json_objects
```

### Comparing `tomni-1.9.2/tomni/transformers/vgg2json/main.py` & `tomni-2.0.0b1/tomni/transformers/vgg2json/main.py`

 * *Files identical despite different names*

### Comparing `tomni-1.9.2/tomni/transformers/vgg2json/test_vgg2json.py` & `tomni-2.0.0b1/tomni/transformers/vgg2json/test_vgg2json.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                         "region_attributes": {"name": "organoid"},
                     },
                     {
                         "shape_attributes": {
                             "name": "circle",
                             "cx": 769,
                             "cy": 649,
-                            "r": 24
+                            "r": 24,
                         },
                         "region_attributes": {},
                     },
                 ],
             },
         }
 
@@ -211,9 +211,7 @@
         result[0][0]["id"] = "unicorn"
         result[1][0]["id"] = "unicorn"
 
         self.assertEqual(len(result), len(expected_output))
         for i in range(len(result)):
             for j in range(len(result[i])):
                 self.assertDictEqual(result[i][j], expected_output[i][j])
-
-
```

### Comparing `tomni-1.9.2/tomni.egg-info/PKG-INFO` & `tomni-2.0.0b1/tomni.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,166 @@
 Metadata-Version: 2.1
 Name: tomni
-Version: 1.9.2
+Version: 2.0.0b1
 Summary: Tomni is a collection of image analysis functions usefull for CytoSmart solution.
 Home-page: https://github.com/cytosmart-bv/tomni
 Author: Tom Nijhof
-License: UNKNOWN
+License: ACADEMIC PUBLIC LICENSE
 Keywords: tomni
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Tomni
-=====
+# Tomni
 
-Tomni is a python package that contains a collection of helper functions based on OpenCV and NumPy. It can be used for any python based computer vision or image analysis problem. The package simplifies the code and takes care of edge cages, everything from simplifying code like img_dim to compute optimization like labels2contours or illumination correction image processing. Tomni uses the image coordinates (same as OpenCV). 
+[![Build Status](https://cytosmart.visualstudio.com/CytoSmartImageAnalysis/_apis/build/status/cytosmart-bv.tomni?branchName=main)](https://cytosmart.visualstudio.com/CytoSmartImageAnalysis/_build/latest?definitionId=384&branchName=main)
+[![Downloads](https://pepy.tech/badge/tomni)](https://pepy.tech/project/tomni)
+
+Tomni is a python package that contains a collection of helper functions based on OpenCV and NumPy. It can be used for any python based computer vision or image analysis problem. The package simplifies the code and takes care of edge cages, everything from simplifying code like img_dim to compute optimization like labels2contours or illumination correction image processing. Tomni uses the image coordinates (same as OpenCV).
 
 Tomni is created by [CytoSMART](https://cytosmart.com).
 
 The package was developed in-house to centralize the helper function for computer vision problems. In 2021, CytoSMART engineers turned it to open source, enabling researchers and educators to use it for free.
 
 ## Getting Tomni
 
-``` cmd
+```cmd
 pip install tomni
 ```
 
 ## License
 
 Tomni is free for academic and educational use.
 
 For commercial use please contact [CytoSMART](https://cytosmart.com/contact).
 
 ## The name
 
-The name Tomni is a combination of creator (Tom) and other CytoSMART product he was working on, [the Omni](https://cytosmart.com/products/omni). Tomni name was proposed by Denissa Daroţi, a former CytoSMART intern, who won a bet with her mentor by getting a (well deserved) 9/10 for her internship. 
-
-
+The name Tomni is a combination of creator (Tom) and other CytoSMART product he was working on, [the Omni](https://cytosmart.com/products/omni). Tomni name was proposed by Denissa Daroţi, a former CytoSMART intern, who won a bet with her mentor by getting a (well deserved) 9/10 for her internship.
 
 ## Features
 
-* Bounding box fitting (bbox fitting)
-  * Center bounding box fit
-  * Custom location box fit
-* Illumination correction 
-  * Brightfield
-  * Fluorescence
-* Json operation
-  * Add circularity property
-  * Scale object
-  * Translate object
-* Make a mask
-  * Ellipse
-  * Polygon
-* Shape fitting
-  * Rect around ellipse
-* Transformers of data format
-  * Contours to json
-  * Ellipse to json
-  * Json 2 contours
-  * Json 2 label
-  * Labels 2 contours
-  * Labels 2 lists of points
+- Bounding box fitting (bbox fitting)
+  - Center bounding box fit
+  - Custom location box fit
+- Image helpers
+  - Get image dimensions
+  - Convert color of an image
+- Illumination correction
+  - Brightfield
+  - Fluorescence
+- Contour operations
+  - Get center
+  - Approximate circle by area
+  - Get roundness
+  - Get circularity
+- CytoSMART data format
+  - Tba
+- Json operation
+  - Add circularity property
+  - Scale object
+  - Translate object
+- Make a mask
+  - Ellipse
+  - Polygon
+- Shape fitting
+  - Rect around ellipse
+- Transformers of data format
+  - Contours to json
+  - Ellipse to json
+  - Json 2 contours
+  - Json 2 label
+  - Json 2 bbox
+  - Labels 2 contours
+  - Labels 2 lists of points
+
 
 ## Credits
+
 Sorted alphabetically
 
 - Coenraad Stijne
 - Denisa Daroţi
 - Hristo Atanasov
+- Jan-Niklas Schneider
 - Jelle van Kerkvoorde
 - Kirsten Koopman
 - Manon van Erp
 - Marina Tzenkova
 - Tom de Vries
 - Tom Nijhof
 
+
 # History
+
+2.0.0-b0 (2022-11-29)
+------------------
+- CDF-Main: Implement `filter` to allow filtering of annotations by feature values (aka gating).
+- CDF-Main: Implement `from_contours`.
+- CDF-Main: Implement `to_contours`.
+- CDF-Main: Implement `from_dict`.
+- CDF-Main: Implement `to_dict`. Includes rounding.
+- CDF-Main: Implement `__len__`.
+- CDF-Main: Implement `__iter__` and `__next__`.
+- Add polygon annotation class.
+- CDF-polygon: Implement `__eq__`
+- CDF-polygon: Remove useless point
+- Add ellipse annotation class.
+- CDF-ellipse: Implement `__eq__`
+- CDF-ellipse: Set all rotations between 0 and 90, flip radii if needed
+- Renamed `CytoSmartDataFormat` to `AnnotationManager`
+- Add `is_in_mask` for `Ellipse` and `Polygon`
+- Add `min_overlap`-parameter in `to_dict` to apply masks to filter annotations
+- Add `to_binary_mask` and `to_labeled_mask` for `AnnotationManager`, `Ellipse` and `Polygon`
+- Add init-function `from_binary_mask` and `from_labeled_mask` to `AnnotationManager`
+- Bugfix: Fixed a bug where `simplify_line` returns empty list when passing two points.
+- Add option to to compress polygons in `to_dict()`.
+
+1.15.0 (2022-12-05)
+------------------
+- Add json2bbox for ellipse with angle of rotation
+
+1.14.0 (2022-11-11)
+------------------
+- Add convert to color
+
+1.13.0 (2022-10-24)
+------------------
+- Add json2bbox for polygon and ellipse
+
+1.12.1 (2022-10-06)
+------------------
+- Update Json-circularity with circularity calculation from contour ops.
+
+1.12.0 (2022-04-15)
+------------------
+- BUGFIX: Import approximate_circle_by_area
+- Add roundness
+- Add contour operation circularity
+
+1.11.0 (2022-04-11)
+------------------
+- Add inner contours to labels2contours
+- Add inner contours to mask2json
+
+1.10.0 (2022-02-17)
+------------------
+- Add approximate_circle_by_area to contour operations
+- BUGFIX: Change type np.array to np.ndarray
+- DEPRECATE: Remove simplification so python 3.8+ can be used
+
 1.9.2 (2022-01-03)
 ------------------
-- BUGFIX: Bufferoverflow make_mask_ellipse (again/still) 
+- BUGFIX: Bufferoverflow make_mask_ellipse (again/still)
     remove times 2 for all values in the function
 
 1.9.1 (2021-10-26)
 ------------------
 - add ellipse to json2mask
 - BUGFIX: Bufferoverflow make_mask_ellipse
 - BUGFIX: Make make_mask_ellipse accept floats
@@ -123,15 +194,15 @@
 ------------------
 updated setup file simplification<0.6
 
 1.7.0 (2020-12-03)
 ------------------
 added new functions
 - add_area
-- summary_json 
+- summary_json
 - json2dict
 
 1.6.4 (2020-11-26)
 ------------------
 - add  missing requirements in setup file
 
 1.6.3 (2020-11-25)
@@ -171,15 +242,15 @@
 - add vgg2json
 
 1.3.0
 ------------------
 Updating of relative illumination correction.
 - add (optional) smoothing step
 - add (optional) resize step
-- add (optional) normalization 
+- add (optional) normalization
 
 1.2.0 (2020-07-02)
 ------------------
 - Add translation of json functions
 
 1.1.0 (2020-03-11)
 ------------------
@@ -196,15 +267,15 @@
 1.0.0 (2020-02-28)
 ------------------
 Restructuring of tomni:
 - Migrated Visualization to cytoBoom
 - Migrated validation to manVal
 - Made sure every function followed:
     function_name
-    - __init__.py 
+    - __init__.py
     - main.py
     - test_function_name
 - removed following function:
 -- channel_selecting (was only used for old cell counter)
 -- select_labels (complete replaceable by transformers.labels2listsOfPoints
 - Added docstring to all functions
 - Added typing to all functions
@@ -265,15 +336,15 @@
 similar to the well-known GNU General Public License, yet it retains the
 possibility for LuxConnector authors to financially support the development by
 selling commercial licenses. In fact, if you intend to use LuxConnector in a
 "for-profit" environment, where research is conducted to develop or enhance
 a product, is used in a commercial service offering, or when an entity uses
 LuxConnector to participate in government-funded, EU-funded, military or similar
 research projects, then you need to obtain a commercial license.
-In that case, or if you are unsure, please contact the Author info@cytosmart.com 
+In that case, or if you are unsure, please contact the Author info@cytosmart.com
 to inquire about commercial licenses.
 
   What are the rights given to noncommercial users? Similarly to GPL, you
 have the right to use the software, to distribute copies, to receive source
 code, to change the software and distribute your modifications or the
 modified software. Also similarly to the GPL, if you distribute verbatim or
 modified copies of this software, they must be distributed under this
@@ -484,10 +555,9 @@
 TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
 YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
 PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGES.
 
                      END OF TERMS AND CONDITIONS
 
-Initially written by Andras Varga (public domain) for OMNeT++ https://omnetpp.org/intro/license, 
+Initially written by Andras Varga (public domain) for OMNeT++ https://omnetpp.org/intro/license,
 adapted by CytoSMART TECHNOLOGIES BV. The adaptation is licensed under CC0 1.0 (Public Domain Dedication).
-
```

