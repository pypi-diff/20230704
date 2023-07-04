# Comparing `tmp/pyhard-2.1.6.tar.gz` & `tmp/pyhard-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhard-2.1.6.tar", last modified: Sat Jun 10 14:23:10 2023, max compression
+gzip compressed data, was "pyhard-2.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyhard-2.1.6.tar` & `pyhard-2.1.7.tar`

### file list

```diff
@@ -1,132 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.619742 pyhard-2.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-10 14:23:02.000000 pyhard-2.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9423 2023-06-10 14:23:10.619742 pyhard-2.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8692 2023-06-10 14:23:02.000000 pyhard-2.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.597741 pyhard-2.1.6/pyhard/
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    37751 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/app.py
--rw-rw-rw-   0 root         (0) root         (0)    19119 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/base.py
--rw-rw-rw-   0 root         (0) root         (0)    12128 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    20574 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.598742 pyhard-2.1.6/pyhard/conf/
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/conf/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    12210 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.594741 pyhard-2.1.6/pyhard/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.599742 pyhard-2.1.6/pyhard/data/2normals/
--rw-rw-rw-   0 root         (0) root         (0)    39390 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39209 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   242683 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   168248 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   328455 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normals/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.601742 pyhard-2.1.6/pyhard/data/2normalsSd030/
--rw-rw-rw-   0 root         (0) root         (0)    39624 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    38990 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   130100 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)    94130 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   284473 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd030/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.602742 pyhard-2.1.6/pyhard/data/2normalsSd045/
--rw-rw-rw-   0 root         (0) root         (0)    39780 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39157 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   178828 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   131886 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   318453 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/2normalsSd045/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.604742 pyhard-2.1.6/pyhard/data/circle/
--rw-rw-rw-   0 root         (0) root         (0)    39346 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40231 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   226405 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   145447 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   320526 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/circle/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.605742 pyhard-2.1.6/pyhard/data/easy/
--rw-rw-rw-   0 root         (0) root         (0)    40190 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40952 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   147238 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)    54473 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/feature_raw_color.csv
--rw-rw-rw-   0 root         (0) root         (0)   282881 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.606742 pyhard-2.1.6/pyhard/data/easy2/
--rw-rw-rw-   0 root         (0) root         (0)    39957 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40817 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   285261 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/easy2/projection_matrix.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.607742 pyhard-2.1.6/pyhard/data/iris/
--rw-rw-rw-   0 root         (0) root         (0)     5787 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/iris/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)     3877 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/iris/data.csv
--rw-rw-rw-   0 root         (0) root         (0)    42802 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/iris/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.608742 pyhard-2.1.6/pyhard/data/mix/
--rw-rw-rw-   0 root         (0) root         (0)    39716 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40903 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   193499 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   144369 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   296920 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/mix/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.609742 pyhard-2.1.6/pyhard/data/overlap/
--rw-rw-rw-   0 root         (0) root         (0)    39233 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/overlap/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39752 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/overlap/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   321095 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/overlap/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.610742 pyhard-2.1.6/pyhard/data/separate/
--rw-rw-rw-   0 root         (0) root         (0)    39995 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    42167 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   177556 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   113525 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   287283 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/separate/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.617742 pyhard-2.1.6/pyhard/data/wine/
--rw-rw-rw-   0 root         (0) root         (0)    29361 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/algorithm_bin.csv
--rw-rw-rw-   0 root         (0) root         (0)   226327 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/algorithm_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   218520 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/algorithm_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)    10101 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/beta_easy.csv
--rw-rw-rw-   0 root         (0) root         (0)    69563 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)   100951 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   163688 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   163380 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_bagging_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_bagging_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_gradient_boosting_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_gradient_boosting_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_instance_easiness_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_logistic_regression_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_logistic_regression_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_mlp_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_mlp_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_performance.csv
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_linear_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_linear_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_rbf_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/footprint_svc_rbf_good.csv
--rw-rw-rw-   0 root         (0) root         (0)    10103 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/good_algos.csv
--rw-rw-rw-   0 root         (0) root         (0)    37458 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/ih.csv
--rw-rw-rw-   0 root         (0) root         (0)   317680 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)   522841 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/metadata_full.csv
--rw-rw-rw-   0 root         (0) root         (0)    10105 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/portfolio.csv
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/wine/projection_matrix.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.618742 pyhard-2.1.6/pyhard/data/xor/
--rw-rw-rw-   0 root         (0) root         (0)    40143 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40214 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   272866 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/data/xor/projection_matrix.csv
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/feature_selection.py
--rw-rw-rw-   0 root         (0) root         (0)    10144 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/hpo.py
--rw-rw-rw-   0 root         (0) root         (0)    10847 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/integrator.py
--rw-rw-rw-   0 root         (0) root         (0)    43027 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/measures.py
--rw-rw-rw-   0 root         (0) root         (0)     3787 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.618742 pyhard-2.1.6/pyhard/midia/
--rw-rw-rw-   0 root         (0) root         (0)   157445 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/midia/blobs.svg
--rw-rw-rw-   0 root         (0) root         (0)    11042 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.618742 pyhard-2.1.6/pyhard/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10787 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/entropy_estimators.py
--rw-rw-rw-   0 root         (0) root         (0)     4948 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/rank_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)    21966 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/thirdparty/skfeature.py
--rw-rw-rw-   0 root         (0) root         (0)     5221 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/validator.py
--rw-rw-rw-   0 root         (0) root         (0)    38600 2023-06-10 14:23:02.000000 pyhard-2.1.6/pyhard/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 14:23:10.598742 pyhard-2.1.6/pyhard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9423 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3654 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 14:23:10.000000 pyhard-2.1.6/pyhard.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-10 14:23:10.619742 pyhard-2.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-06-10 14:23:02.000000 pyhard-2.1.6/setup.py
+-rw-r--r--   0        0        0      293 2022-09-10 19:42:26.675132 pyhard-2.1.7/.gitignore
+-rw-r--r--   0        0        0      993 2023-07-03 18:46:39.481967 pyhard-2.1.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1068 2022-09-10 19:43:10.726287 pyhard-2.1.7/LICENSE
+-rw-r--r--   0        0        0     8692 2022-09-10 19:43:10.728487 pyhard-2.1.7/README.md
+-rw-r--r--   0        0        0      511 2023-01-06 02:35:24.340268 pyhard-2.1.7/environment.yml
+-rw-r--r--   0        0        0     1297 2023-07-04 01:54:20.998863 pyhard-2.1.7/pyhard/__init__.py
+-rw-r--r--   0        0        0       66 2022-07-07 15:19:14.354365 pyhard-2.1.7/pyhard/__main__.py
+-rw-r--r--   0        0        0    37751 2023-05-02 01:19:20.837594 pyhard-2.1.7/pyhard/app.py
+-rw-r--r--   0        0        0    19119 2022-09-10 19:42:26.716734 pyhard-2.1.7/pyhard/base.py
+-rw-r--r--   0        0        0    12128 2022-09-10 19:42:26.718773 pyhard-2.1.7/pyhard/classification.py
+-rw-r--r--   0        0        0    20574 2023-05-02 01:19:20.839160 pyhard-2.1.7/pyhard/cli.py
+-rw-r--r--   0        0        0     5199 2022-09-10 19:43:10.738044 pyhard-2.1.7/pyhard/conf/config.yaml
+-rw-r--r--   0        0        0     3469 2022-07-07 15:19:14.382687 pyhard-2.1.7/pyhard/conf/config_old.yaml
+-rw-r--r--   0        0        0      703 2022-07-07 15:19:14.386390 pyhard-2.1.7/pyhard/conf/options.json
+-rw-r--r--   0        0        0    12210 2022-07-07 15:19:14.389540 pyhard-2.1.7/pyhard/context.py
+-rw-r--r--   0        0        0    64554 2022-07-07 15:19:16.307400 pyhard-2.1.7/pyhard/data/2normals/2normals.pdf
+-rw-r--r--   0        0        0    39390 2022-07-07 15:19:16.300124 pyhard-2.1.7/pyhard/data/2normals/coordinates.csv
+-rw-r--r--   0        0        0    39209 2022-07-07 15:19:16.291739 pyhard-2.1.7/pyhard/data/2normals/data.csv
+-rw-r--r--   0        0        0   242683 2022-07-07 15:19:16.286839 pyhard-2.1.7/pyhard/data/2normals/feature_process.csv
+-rw-r--r--   0        0        0   168248 2022-07-07 15:19:16.282477 pyhard-2.1.7/pyhard/data/2normals/feature_raw.csv
+-rw-r--r--   0        0        0   328455 2022-07-07 15:19:16.276723 pyhard-2.1.7/pyhard/data/2normals/metadata.csv
+-rw-r--r--   0        0        0      598 2022-07-07 15:19:16.273004 pyhard-2.1.7/pyhard/data/2normals/options.json
+-rw-r--r--   0        0        0    64659 2022-07-07 15:19:16.270651 pyhard-2.1.7/pyhard/data/2normalsSd030/2normals030.pdf
+-rw-r--r--   0        0        0    39624 2022-07-07 15:19:16.260253 pyhard-2.1.7/pyhard/data/2normalsSd030/coordinates.csv
+-rw-r--r--   0        0        0    38990 2022-07-07 15:19:16.253252 pyhard-2.1.7/pyhard/data/2normalsSd030/data.csv
+-rw-r--r--   0        0        0   130100 2022-07-07 15:19:16.246955 pyhard-2.1.7/pyhard/data/2normalsSd030/feature_process.csv
+-rw-r--r--   0        0        0    94130 2022-07-07 15:19:16.242926 pyhard-2.1.7/pyhard/data/2normalsSd030/feature_raw.csv
+-rw-r--r--   0        0        0   284473 2022-07-07 15:19:16.238366 pyhard-2.1.7/pyhard/data/2normalsSd030/metadata.csv
+-rw-r--r--   0        0        0      597 2022-07-07 15:19:16.235376 pyhard-2.1.7/pyhard/data/2normalsSd030/options.json
+-rw-r--r--   0        0        0    64807 2022-07-07 15:19:16.233118 pyhard-2.1.7/pyhard/data/2normalsSd045/2normals045.pdf
+-rw-r--r--   0        0        0    39780 2022-07-07 15:19:16.230124 pyhard-2.1.7/pyhard/data/2normalsSd045/coordinates.csv
+-rw-r--r--   0        0        0    39157 2022-07-07 15:19:16.225448 pyhard-2.1.7/pyhard/data/2normalsSd045/data.csv
+-rw-r--r--   0        0        0   178828 2022-07-07 15:19:16.221671 pyhard-2.1.7/pyhard/data/2normalsSd045/feature_process.csv
+-rw-r--r--   0        0        0   131886 2022-07-07 15:19:16.217522 pyhard-2.1.7/pyhard/data/2normalsSd045/feature_raw.csv
+-rw-r--r--   0        0        0   318453 2022-07-07 15:19:16.212124 pyhard-2.1.7/pyhard/data/2normalsSd045/metadata.csv
+-rw-r--r--   0        0        0      597 2022-07-07 15:19:16.208428 pyhard-2.1.7/pyhard/data/2normalsSd045/options.json
+-rw-r--r--   0        0        0    15846 2022-07-07 15:19:16.206370 pyhard-2.1.7/pyhard/data/circle/circle.png
+-rw-r--r--   0        0        0    39346 2022-07-07 15:19:16.203183 pyhard-2.1.7/pyhard/data/circle/coordinates.csv
+-rw-r--r--   0        0        0    40231 2022-07-07 15:19:16.197629 pyhard-2.1.7/pyhard/data/circle/data.csv
+-rw-r--r--   0        0        0   226405 2022-07-07 15:19:16.193013 pyhard-2.1.7/pyhard/data/circle/feature_process.csv
+-rw-r--r--   0        0        0   145447 2022-07-07 15:19:16.188686 pyhard-2.1.7/pyhard/data/circle/feature_raw.csv
+-rw-r--r--   0        0        0   320526 2022-07-07 15:19:16.183158 pyhard-2.1.7/pyhard/data/circle/metadata.csv
+-rw-r--r--   0        0        0      595 2022-07-07 15:19:16.179901 pyhard-2.1.7/pyhard/data/circle/options.json
+-rw-r--r--   0        0        0    40190 2022-07-07 15:19:16.177325 pyhard-2.1.7/pyhard/data/easy/coordinates.csv
+-rw-r--r--   0        0        0    40952 2022-07-07 15:19:16.172903 pyhard-2.1.7/pyhard/data/easy/data.csv
+-rw-r--r--   0        0        0   147238 2022-07-07 15:19:16.169378 pyhard-2.1.7/pyhard/data/easy/feature_process.csv
+-rw-r--r--   0        0        0    54473 2022-07-07 15:19:16.160755 pyhard-2.1.7/pyhard/data/easy/feature_raw_color.csv
+-rw-r--r--   0        0        0   282881 2022-07-07 15:19:16.154575 pyhard-2.1.7/pyhard/data/easy/metadata.csv
+-rw-r--r--   0        0        0      595 2022-07-07 15:19:16.148835 pyhard-2.1.7/pyhard/data/easy/options.json
+-rw-r--r--   0        0        0    39957 2022-07-07 15:19:16.145667 pyhard-2.1.7/pyhard/data/easy2/coordinates.csv
+-rw-r--r--   0        0        0    40817 2022-07-07 15:19:16.140618 pyhard-2.1.7/pyhard/data/easy2/data.csv
+-rw-r--r--   0        0        0    42676 2022-07-07 15:19:16.137758 pyhard-2.1.7/pyhard/data/easy2/easy2.png
+-rw-r--r--   0        0        0   285261 2022-07-07 15:19:16.133038 pyhard-2.1.7/pyhard/data/easy2/metadata.csv
+-rw-r--r--   0        0        0      597 2022-07-07 15:19:16.129112 pyhard-2.1.7/pyhard/data/easy2/options.json
+-rw-r--r--   0        0        0      190 2022-07-07 15:19:16.127011 pyhard-2.1.7/pyhard/data/easy2/projection_matrix.csv
+-rw-r--r--   0        0        0     5787 2022-07-07 15:19:16.124315 pyhard-2.1.7/pyhard/data/iris/coordinates.csv
+-rw-r--r--   0        0        0     3877 2022-07-07 15:19:16.122174 pyhard-2.1.7/pyhard/data/iris/data.csv
+-rw-r--r--   0        0        0    42802 2022-07-07 15:19:16.119524 pyhard-2.1.7/pyhard/data/iris/metadata.csv
+-rw-r--r--   0        0        0      597 2022-07-07 15:19:16.117220 pyhard-2.1.7/pyhard/data/iris/options.json
+-rw-r--r--   0        0        0    39716 2022-07-07 15:19:16.114954 pyhard-2.1.7/pyhard/data/mix/coordinates.csv
+-rw-r--r--   0        0        0    40903 2022-07-07 15:19:16.108341 pyhard-2.1.7/pyhard/data/mix/data.csv
+-rw-r--r--   0        0        0   193499 2022-07-07 15:19:16.103631 pyhard-2.1.7/pyhard/data/mix/feature_process.csv
+-rw-r--r--   0        0        0   144369 2022-07-07 15:19:16.098375 pyhard-2.1.7/pyhard/data/mix/feature_raw.csv
+-rw-r--r--   0        0        0   296920 2022-07-07 15:19:16.092083 pyhard-2.1.7/pyhard/data/mix/metadata.csv
+-rw-r--r--   0        0        0    66400 2022-07-07 15:19:16.088401 pyhard-2.1.7/pyhard/data/mix/mix.png
+-rw-r--r--   0        0        0      597 2022-07-07 15:19:16.085879 pyhard-2.1.7/pyhard/data/mix/options.json
+-rw-r--r--   0        0        0    39233 2022-07-07 15:19:16.083741 pyhard-2.1.7/pyhard/data/overlap/coordinates.csv
+-rw-r--r--   0        0        0    39752 2022-07-07 15:19:16.077624 pyhard-2.1.7/pyhard/data/overlap/data.csv
+-rw-r--r--   0        0        0   321095 2022-07-07 15:19:16.072075 pyhard-2.1.7/pyhard/data/overlap/metadata.csv
+-rw-r--r--   0        0        0      598 2022-07-07 15:19:16.068655 pyhard-2.1.7/pyhard/data/overlap/options.json
+-rw-r--r--   0        0        0    13099 2022-07-07 15:19:16.059158 pyhard-2.1.7/pyhard/data/overlap/overlap.png
+-rw-r--r--   0        0        0    39995 2022-07-07 15:19:16.056246 pyhard-2.1.7/pyhard/data/separate/coordinates.csv
+-rw-r--r--   0        0        0    42167 2022-07-07 15:19:16.052710 pyhard-2.1.7/pyhard/data/separate/data.csv
+-rw-r--r--   0        0        0   177556 2022-07-07 15:19:16.048070 pyhard-2.1.7/pyhard/data/separate/feature_process.csv
+-rw-r--r--   0        0        0   113525 2022-07-07 15:19:16.043411 pyhard-2.1.7/pyhard/data/separate/feature_raw.csv
+-rw-r--r--   0        0        0   287283 2022-07-07 15:19:16.038511 pyhard-2.1.7/pyhard/data/separate/metadata.csv
+-rw-r--r--   0        0        0      597 2022-07-07 15:19:16.035108 pyhard-2.1.7/pyhard/data/separate/options.json
+-rw-r--r--   0        0        0    29361 2022-09-10 19:43:10.739591 pyhard-2.1.7/pyhard/data/wine/algorithm_bin.csv
+-rw-r--r--   0        0        0   226327 2022-09-10 19:43:10.769935 pyhard-2.1.7/pyhard/data/wine/algorithm_process.csv
+-rw-r--r--   0        0        0   218520 2022-09-10 19:43:10.812172 pyhard-2.1.7/pyhard/data/wine/algorithm_raw.csv
+-rw-r--r--   0        0        0    10101 2022-09-10 19:43:10.847127 pyhard-2.1.7/pyhard/data/wine/beta_easy.csv
+-rw-r--r--   0        0        0     4375 2022-09-10 19:43:10.848659 pyhard-2.1.7/pyhard/data/wine/config.yaml
+-rw-r--r--   0        0        0    69563 2022-09-10 19:43:10.890677 pyhard-2.1.7/pyhard/data/wine/coordinates.csv
+-rw-r--r--   0        0        0   100951 2022-09-10 19:43:10.930692 pyhard-2.1.7/pyhard/data/wine/data.csv
+-rw-r--r--   0        0        0   163688 2022-09-10 19:43:10.971386 pyhard-2.1.7/pyhard/data/wine/feature_process.csv
+-rw-r--r--   0        0        0   163380 2022-09-10 19:43:11.012771 pyhard-2.1.7/pyhard/data/wine/feature_raw.csv
+-rw-r--r--   0        0        0       12 2022-09-10 19:43:11.050969 pyhard-2.1.7/pyhard/data/wine/footprint_bagging_best.csv
+-rw-r--r--   0        0        0     1634 2022-09-10 19:43:11.091983 pyhard-2.1.7/pyhard/data/wine/footprint_bagging_good.csv
+-rw-r--r--   0        0        0      174 2022-09-10 19:43:11.094778 pyhard-2.1.7/pyhard/data/wine/footprint_gradient_boosting_best.csv
+-rw-r--r--   0        0        0     1726 2022-09-10 19:43:11.095902 pyhard-2.1.7/pyhard/data/wine/footprint_gradient_boosting_good.csv
+-rw-r--r--   0        0        0      720 2022-09-10 19:43:11.097050 pyhard-2.1.7/pyhard/data/wine/footprint_instance_easiness_good.csv
+-rw-r--r--   0        0        0       12 2022-09-10 19:43:11.097447 pyhard-2.1.7/pyhard/data/wine/footprint_logistic_regression_best.csv
+-rw-r--r--   0        0        0     1696 2022-09-10 19:43:11.135864 pyhard-2.1.7/pyhard/data/wine/footprint_logistic_regression_good.csv
+-rw-r--r--   0        0        0       12 2022-09-10 19:43:11.136263 pyhard-2.1.7/pyhard/data/wine/footprint_mlp_best.csv
+-rw-r--r--   0        0        0     1663 2022-09-10 19:43:11.175857 pyhard-2.1.7/pyhard/data/wine/footprint_mlp_good.csv
+-rw-r--r--   0        0        0      893 2022-09-10 19:43:11.216534 pyhard-2.1.7/pyhard/data/wine/footprint_performance.csv
+-rw-r--r--   0        0        0     2760 2022-09-10 19:43:11.259939 pyhard-2.1.7/pyhard/data/wine/footprint_random_forest_best.csv
+-rw-r--r--   0        0        0     1903 2022-09-10 19:43:11.299116 pyhard-2.1.7/pyhard/data/wine/footprint_random_forest_good.csv
+-rw-r--r--   0        0        0      259 2022-09-10 19:43:11.300838 pyhard-2.1.7/pyhard/data/wine/footprint_svc_linear_best.csv
+-rw-r--r--   0        0        0     1434 2022-09-10 19:43:11.339621 pyhard-2.1.7/pyhard/data/wine/footprint_svc_linear_good.csv
+-rw-r--r--   0        0        0       12 2022-09-10 19:43:11.340258 pyhard-2.1.7/pyhard/data/wine/footprint_svc_rbf_best.csv
+-rw-r--r--   0        0        0     1516 2022-09-10 19:43:11.379434 pyhard-2.1.7/pyhard/data/wine/footprint_svc_rbf_good.csv
+-rw-r--r--   0        0        0    10103 2022-09-10 19:43:11.420636 pyhard-2.1.7/pyhard/data/wine/good_algos.csv
+-rw-r--r--   0        0        0    37458 2022-09-10 19:43:11.461424 pyhard-2.1.7/pyhard/data/wine/ih.csv
+-rw-r--r--   0        0        0   317680 2022-09-10 19:43:11.468933 pyhard-2.1.7/pyhard/data/wine/metadata.csv
+-rw-r--r--   0        0        0   522841 2022-09-10 19:43:11.517736 pyhard-2.1.7/pyhard/data/wine/metadata_full.csv
+-rw-r--r--   0        0        0   409402 2022-09-10 19:43:11.526763 pyhard-2.1.7/pyhard/data/wine/model.pkl
+-rw-r--r--   0        0        0      790 2022-09-10 19:43:11.538518 pyhard-2.1.7/pyhard/data/wine/options.json
+-rw-r--r--   0        0        0    10105 2022-09-10 19:43:11.561872 pyhard-2.1.7/pyhard/data/wine/portfolio.csv
+-rw-r--r--   0        0        0      231 2022-09-10 19:43:11.601312 pyhard-2.1.7/pyhard/data/wine/projection_matrix.csv
+-rw-r--r--   0        0        0    40143 2022-07-07 15:19:16.031394 pyhard-2.1.7/pyhard/data/xor/coordinates.csv
+-rw-r--r--   0        0        0    40214 2022-07-07 15:19:16.025912 pyhard-2.1.7/pyhard/data/xor/data.csv
+-rw-r--r--   0        0        0   272866 2022-07-07 15:19:16.021272 pyhard-2.1.7/pyhard/data/xor/metadata.csv
+-rw-r--r--   0        0        0      598 2022-07-07 15:19:16.017615 pyhard-2.1.7/pyhard/data/xor/options.json
+-rw-r--r--   0        0        0      196 2022-07-07 15:19:16.015426 pyhard-2.1.7/pyhard/data/xor/projection_matrix.csv
+-rw-r--r--   0        0        0    65163 2022-07-07 15:19:16.012466 pyhard-2.1.7/pyhard/data/xor/xor.pdf
+-rw-r--r--   0        0        0     7659 2022-07-07 15:19:14.699086 pyhard-2.1.7/pyhard/feature_selection.py
+-rw-r--r--   0        0        0    10144 2022-09-10 19:43:11.618770 pyhard-2.1.7/pyhard/hpo.py
+-rw-r--r--   0        0        0    10847 2022-09-10 19:42:26.837873 pyhard-2.1.7/pyhard/integrator.py
+-rw-r--r--   0        0        0    43027 2023-07-03 12:51:43.657686 pyhard-2.1.7/pyhard/measures.py
+-rw-r--r--   0        0        0     3787 2022-09-10 19:43:11.621488 pyhard-2.1.7/pyhard/metrics.py
+-rw-r--r--   0        0        0   157445 2022-09-10 19:43:11.623636 pyhard-2.1.7/pyhard/midia/blobs.svg
+-rw-r--r--   0        0        0    11042 2022-09-10 19:43:11.625070 pyhard-2.1.7/pyhard/regression.py
+-rw-r--r--   0        0        0     4123 2022-09-10 19:43:11.626431 pyhard-2.1.7/pyhard/structures.py
+-rw-r--r--   0        0        0        0 2020-07-14 12:56:01.000000 pyhard-2.1.7/pyhard/thirdparty/__init__.py
+-rwxr-xr-x   0        0        0    10787 2022-07-07 15:19:14.943411 pyhard-2.1.7/pyhard/thirdparty/entropy_estimators.py
+-rw-r--r--   0        0        0     4948 2022-07-07 15:19:14.949316 pyhard-2.1.7/pyhard/thirdparty/rank_aggregation.py
+-rw-r--r--   0        0        0    21966 2022-07-07 15:19:14.952426 pyhard-2.1.7/pyhard/thirdparty/skfeature.py
+-rw-r--r--   0        0        0     5221 2022-09-10 19:43:11.627963 pyhard-2.1.7/pyhard/utils.py
+-rw-r--r--   0        0        0     2359 2023-03-21 01:42:05.849790 pyhard-2.1.7/pyhard/validator.py
+-rw-r--r--   0        0        0    38600 2022-09-10 19:42:27.086092 pyhard-2.1.7/pyhard/visualization.py
+-rw-r--r--   0        0        0     1574 2023-07-03 21:28:17.308921 pyhard-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0       62 2022-09-10 19:43:11.691599 pyhard-2.1.7/setup.cfg
+-rw-r--r--   0        0        0     1794 2023-07-03 21:15:36.990332 pyhard-2.1.7/setup.py
+-rw-r--r--   0        0        0    10244 1970-01-01 00:00:00.000000 pyhard-2.1.7/PKG-INFO
```

### Comparing `pyhard-2.1.6/LICENSE` & `pyhard-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/PKG-INFO` & `pyhard-2.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pyhard
-Version: 2.1.6
-Summary: Analyze, explore and visualize instance hardness within datasets
-Home-page: https://gitlab.com/ita-ml/pyhard
-Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.6/pyhard-v2.1.6.tar.gz
-Author: Pedro Paiva
-Author-email: paiva@ita.br
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 <!--
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
 -->
 
 # PyHard
```

### Comparing `pyhard-2.1.6/README.md` & `pyhard-2.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,50 @@
+Metadata-Version: 2.1
+Name: pyhard
+Version: 2.1.7
+Summary: Analyze, explore and visualize instance hardness within datasets
+Author-email: Pedro Paiva <paiva@ita.br>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Requires-Dist: pandas>=1.3.0
+Requires-Dist: scikit-learn>=1.0.1
+Requires-Dist: numpy>=1.18.4
+Requires-Dist: PyYAML>=5.3
+Requires-Dist: scipy>=1.4.1
+Requires-Dist: panel~=0.14.1
+Requires-Dist: param>=1.12.2
+Requires-Dist: bokeh>=2.4.3
+Requires-Dist: holoviews>=1.15.0
+Requires-Dist: matplotlib>=3.2.2
+Requires-Dist: plotly>=5.9.0
+Requires-Dist: plotting>=0.0.7
+Requires-Dist: shapely~=1.8.0
+Requires-Dist: hyperopt>=0.2.4
+Requires-Dist: pyispace>=0.3.4
+Requires-Dist: deprecation>=2.1.0
+Requires-Dist: joblib>=1.0.0
+Requires-Dist: ncafs>=0.2
+Requires-Dist: typer>=0.4.1
+Requires-Dist: packaging>=21.0
+Requires-Dist: requests>=2.27.0
+Requires-Dist: plotly>=5.6 ; extra == "dev"
+Requires-Dist: sphinx ; extra == "dev"
+Requires-Dist: sphinx_rtd_theme ; extra == "dev"
+Requires-Dist: notebook>=6.4 ; extra == "dev"
+Requires-Dist: jupyterlab>=3.5.3 ; extra == "dev"
+Project-URL: Documentation, https://ita-ml.gitlab.io/pyhard/
+Project-URL: Repository, https://gitlab.com/ita-ml/pyhard
+Provides-Extra: dev
+
 <!--
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
 -->
 
 # PyHard
@@ -159,7 +202,8 @@
 
 11. James Bergstra, Rémi Bardenet, Yoshua Bengio, and Balázs Kégl. 2011. __Algorithms for hyper-parameter optimization__. In Proceedings of the 24th International Conference on Neural Information Processing Systems (NIPS’11). Curran Associates Inc., Red Hook, NY, USA, 2546–2554.
 
 12. Jasper Snoek, Hugo Larochelle, and Ryan P. Adams. 2012. __Practical Bayesian optimization of machine learning algorithms__. In Proceedings of the 25th International Conference on Neural Information Processing Systems - Volume 2 (NIPS’12). Curran Associates Inc., Red Hook, NY, USA, 2951–2959.
   
 13. J. Bergstra, D. Yamins, and D. D. Cox. 2013. __Making a science of model search: hyperparameter optimization in hundreds of dimensions for vision architectures__. In Proceedings of the 30th International Conference on International Conference on Machine Learning - Volume 28 (ICML’13). JMLR.org, I–115–I–123.
   
+
```

### Comparing `pyhard-2.1.6/pyhard/__init__.py` & `pyhard-2.1.7/pyhard/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union
 
 
-__version__ = "2.1.6"
+__version__ = "2.1.7"
 
 
 def get_seed() -> Union[int, None]:
     seed = os.environ.get("PYHARD_SEED")
     if seed is None:
         return seed
     else:
```

### Comparing `pyhard-2.1.6/pyhard/app.py` & `pyhard-2.1.7/pyhard/app.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/base.py` & `pyhard-2.1.7/pyhard/base.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/classification.py` & `pyhard-2.1.7/pyhard/classification.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/cli.py` & `pyhard-2.1.7/pyhard/cli.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/conf/config.yaml` & `pyhard-2.1.7/pyhard/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/context.py` & `pyhard-2.1.7/pyhard/context.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normals/coordinates.csv` & `pyhard-2.1.7/pyhard/data/2normals/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normals/data.csv` & `pyhard-2.1.7/pyhard/data/2normals/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normals/feature_process.csv` & `pyhard-2.1.7/pyhard/data/2normals/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normals/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/2normals/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normals/metadata.csv` & `pyhard-2.1.7/pyhard/data/2normals/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd030/coordinates.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd030/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd030/data.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd030/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd030/feature_process.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd030/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd030/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd030/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd030/metadata.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd030/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd045/coordinates.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd045/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd045/data.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd045/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd045/feature_process.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd045/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd045/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd045/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/2normalsSd045/metadata.csv` & `pyhard-2.1.7/pyhard/data/2normalsSd045/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/circle/coordinates.csv` & `pyhard-2.1.7/pyhard/data/circle/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/circle/data.csv` & `pyhard-2.1.7/pyhard/data/circle/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/circle/feature_process.csv` & `pyhard-2.1.7/pyhard/data/circle/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/circle/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/circle/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/circle/metadata.csv` & `pyhard-2.1.7/pyhard/data/circle/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy/coordinates.csv` & `pyhard-2.1.7/pyhard/data/easy/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy/data.csv` & `pyhard-2.1.7/pyhard/data/easy/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy/feature_process.csv` & `pyhard-2.1.7/pyhard/data/easy/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy/feature_raw_color.csv` & `pyhard-2.1.7/pyhard/data/easy/feature_raw_color.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy/metadata.csv` & `pyhard-2.1.7/pyhard/data/easy/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy2/coordinates.csv` & `pyhard-2.1.7/pyhard/data/easy2/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy2/data.csv` & `pyhard-2.1.7/pyhard/data/easy2/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/easy2/metadata.csv` & `pyhard-2.1.7/pyhard/data/easy2/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/iris/coordinates.csv` & `pyhard-2.1.7/pyhard/data/iris/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/iris/data.csv` & `pyhard-2.1.7/pyhard/data/iris/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/iris/metadata.csv` & `pyhard-2.1.7/pyhard/data/iris/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/mix/coordinates.csv` & `pyhard-2.1.7/pyhard/data/mix/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/mix/data.csv` & `pyhard-2.1.7/pyhard/data/mix/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/mix/feature_process.csv` & `pyhard-2.1.7/pyhard/data/mix/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/mix/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/mix/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/mix/metadata.csv` & `pyhard-2.1.7/pyhard/data/mix/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/overlap/coordinates.csv` & `pyhard-2.1.7/pyhard/data/overlap/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/overlap/data.csv` & `pyhard-2.1.7/pyhard/data/overlap/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/overlap/metadata.csv` & `pyhard-2.1.7/pyhard/data/overlap/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/separate/coordinates.csv` & `pyhard-2.1.7/pyhard/data/separate/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/separate/data.csv` & `pyhard-2.1.7/pyhard/data/separate/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/separate/feature_process.csv` & `pyhard-2.1.7/pyhard/data/separate/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/separate/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/separate/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/separate/metadata.csv` & `pyhard-2.1.7/pyhard/data/separate/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/algorithm_bin.csv` & `pyhard-2.1.7/pyhard/data/wine/algorithm_bin.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/algorithm_process.csv` & `pyhard-2.1.7/pyhard/data/wine/algorithm_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/algorithm_raw.csv` & `pyhard-2.1.7/pyhard/data/wine/algorithm_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/beta_easy.csv` & `pyhard-2.1.7/pyhard/data/wine/beta_easy.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/coordinates.csv` & `pyhard-2.1.7/pyhard/data/wine/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/data.csv` & `pyhard-2.1.7/pyhard/data/wine/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/feature_process.csv` & `pyhard-2.1.7/pyhard/data/wine/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/feature_raw.csv` & `pyhard-2.1.7/pyhard/data/wine/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_bagging_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_bagging_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_gradient_boosting_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_gradient_boosting_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_instance_easiness_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_instance_easiness_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_logistic_regression_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_logistic_regression_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_mlp_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_mlp_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_performance.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_performance.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_best.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_random_forest_best.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_random_forest_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_random_forest_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_svc_linear_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_svc_linear_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/footprint_svc_rbf_good.csv` & `pyhard-2.1.7/pyhard/data/wine/footprint_svc_rbf_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/good_algos.csv` & `pyhard-2.1.7/pyhard/data/wine/good_algos.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/ih.csv` & `pyhard-2.1.7/pyhard/data/wine/ih.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/metadata.csv` & `pyhard-2.1.7/pyhard/data/wine/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/metadata_full.csv` & `pyhard-2.1.7/pyhard/data/wine/metadata_full.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/wine/portfolio.csv` & `pyhard-2.1.7/pyhard/data/wine/portfolio.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/xor/coordinates.csv` & `pyhard-2.1.7/pyhard/data/xor/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/xor/data.csv` & `pyhard-2.1.7/pyhard/data/xor/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/data/xor/metadata.csv` & `pyhard-2.1.7/pyhard/data/xor/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/feature_selection.py` & `pyhard-2.1.7/pyhard/feature_selection.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/hpo.py` & `pyhard-2.1.7/pyhard/hpo.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/integrator.py` & `pyhard-2.1.7/pyhard/integrator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/measures.py` & `pyhard-2.1.7/pyhard/measures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/metrics.py` & `pyhard-2.1.7/pyhard/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/midia/blobs.svg` & `pyhard-2.1.7/pyhard/midia/blobs.svg`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/regression.py` & `pyhard-2.1.7/pyhard/regression.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/structures.py` & `pyhard-2.1.7/pyhard/structures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/thirdparty/entropy_estimators.py` & `pyhard-2.1.7/pyhard/thirdparty/entropy_estimators.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/thirdparty/rank_aggregation.py` & `pyhard-2.1.7/pyhard/thirdparty/rank_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/thirdparty/skfeature.py` & `pyhard-2.1.7/pyhard/thirdparty/skfeature.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/utils.py` & `pyhard-2.1.7/pyhard/utils.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/validator.py` & `pyhard-2.1.7/pyhard/validator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/pyhard/visualization.py` & `pyhard-2.1.7/pyhard/visualization.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.6/setup.py` & `pyhard-2.1.7/setup.py`

 * *Files identical despite different names*

