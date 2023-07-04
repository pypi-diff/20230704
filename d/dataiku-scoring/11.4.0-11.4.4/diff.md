# Comparing `tmp/dataiku-scoring-11.4.0.tar.gz` & `tmp/dataiku-scoring-11.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataiku-scoring-11.4.0.tar", last modified: Thu Mar 16 17:26:56 2023, max compression
+gzip compressed data, was "dist/dataiku-scoring-11.4.4.tar", last modified: Tue Jul  4 10:44:01 2023, max compression
```

## Comparing `dataiku-scoring-11.4.0.tar` & `dataiku-scoring-11.4.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.605542 dataiku-scoring-11.4.0/
--rw-r--r--   0 clement    (502) staff       (20)      168 2023-03-16 17:23:42.000000 dataiku-scoring-11.4.0/HISTORY.txt
--rw-r--r--   0 clement    (502) staff       (20)      524 2022-10-18 17:37:21.000000 dataiku-scoring-11.4.0/LICENSE.txt
--rw-r--r--   0 clement    (502) staff       (20)       65 2022-10-18 17:38:57.000000 dataiku-scoring-11.4.0/MANIFEST.in
--rw-r--r--   0 clement    (502) staff       (20)       27 2022-10-18 17:38:15.000000 dataiku-scoring-11.4.0/NOTICE.txt
--rw-r--r--   0 clement    (502) staff       (20)      965 2023-03-16 17:26:56.605238 dataiku-scoring-11.4.0/PKG-INFO
--rw-r--r--   0 clement    (502) staff       (20)      214 2022-10-18 07:49:17.000000 dataiku-scoring-11.4.0/README.md
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.567349 dataiku-scoring-11.4.0/dataiku_scoring.egg-info/
--rw-r--r--   0 clement    (502) staff       (20)      965 2023-03-16 17:26:56.000000 dataiku-scoring-11.4.0/dataiku_scoring.egg-info/PKG-INFO
--rw-r--r--   0 clement    (502) staff       (20)     2506 2023-03-16 17:26:56.000000 dataiku-scoring-11.4.0/dataiku_scoring.egg-info/SOURCES.txt
--rw-r--r--   0 clement    (502) staff       (20)        1 2023-03-16 17:26:56.000000 dataiku-scoring-11.4.0/dataiku_scoring.egg-info/dependency_links.txt
--rw-r--r--   0 clement    (502) staff       (20)        6 2023-03-16 17:26:56.000000 dataiku-scoring-11.4.0/dataiku_scoring.egg-info/requires.txt
--rw-r--r--   0 clement    (502) staff       (20)       15 2023-03-16 17:26:56.000000 dataiku-scoring-11.4.0/dataiku_scoring.egg-info/top_level.txt
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.568558 dataiku-scoring-11.4.0/dataikuscoring/
--rw-r--r--   0 clement    (502) staff       (20)       61 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/__init__.py
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.576494 dataiku-scoring-11.4.0/dataikuscoring/algorithms/
--rw-r--r--   0 clement    (502) staff       (20)      903 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/__init__.py
--rw-r--r--   0 clement    (502) staff       (20)      576 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/common.py
--rw-r--r--   0 clement    (502) staff       (20)     4771 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/decision_tree_model.py
--rw-r--r--   0 clement    (502) staff       (20)      708 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/forest_classifier.py
--rw-r--r--   0 clement    (502) staff       (20)      672 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/forest_regressor.py
--rw-r--r--   0 clement    (502) staff       (20)     1157 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/generic_mlp.py
--rw-r--r--   0 clement    (502) staff       (20)     1581 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/gradient_boosting_classifier.py
--rw-r--r--   0 clement    (502) staff       (20)     1103 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/gradient_boosting_regressor.py
--rw-r--r--   0 clement    (502) staff       (20)      429 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/linear_regression.py
--rw-r--r--   0 clement    (502) staff       (20)     1597 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/logistic.py
--rw-r--r--   0 clement    (502) staff       (20)      848 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/mlp_classifier.py
--rw-r--r--   0 clement    (502) staff       (20)      258 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/algorithms/mlp_regressor.py
--rw-r--r--   0 clement    (502) staff       (20)     9455 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/load.py
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.579503 dataiku-scoring-11.4.0/dataikuscoring/mlflow/
--rw-r--r--   0 clement    (502) staff       (20)      681 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/mlflow/__init__.py
--rw-r--r--   0 clement    (502) staff       (20)    10732 2023-03-03 14:00:38.000000 dataiku-scoring-11.4.0/dataikuscoring/mlflow/classification.py
--rw-r--r--   0 clement    (502) staff       (20)     6912 2023-03-03 14:00:38.000000 dataiku-scoring-11.4.0/dataikuscoring/mlflow/common.py
--rw-r--r--   0 clement    (502) staff       (20)    11000 2023-03-03 14:00:38.000000 dataiku-scoring-11.4.0/dataikuscoring/mlflow/dss_flavor.py
--rw-r--r--   0 clement    (502) staff       (20)     2357 2023-03-03 14:00:38.000000 dataiku-scoring-11.4.0/dataikuscoring/mlflow/regression.py
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.584838 dataiku-scoring-11.4.0/dataikuscoring/models/
--rw-r--r--   0 clement    (502) staff       (20)      635 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/__init__.py
--rw-r--r--   0 clement    (502) staff       (20)      880 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/binary.py
--rw-r--r--   0 clement    (502) staff       (20)     2409 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/common.py
--rw-r--r--   0 clement    (502) staff       (20)     2457 2023-02-03 09:43:28.000000 dataiku-scoring-11.4.0/dataikuscoring/models/mlflow.py
--rw-r--r--   0 clement    (502) staff       (20)     3964 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/model.py
--rw-r--r--   0 clement    (502) staff       (20)      334 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/multiclass.py
--rw-r--r--   0 clement    (502) staff       (20)     6240 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/partitioned.py
--rw-r--r--   0 clement    (502) staff       (20)      205 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/models/regression.py
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.598513 dataiku-scoring-11.4.0/dataikuscoring/processors/
--rw-r--r--   0 clement    (502) staff       (20)     1241 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/__init__.py
--rw-r--r--   0 clement    (502) staff       (20)      711 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/binarize.py
--rw-r--r--   0 clement    (502) staff       (20)     2863 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/calibration.py
--rw-r--r--   0 clement    (502) staff       (20)     1047 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/cat_cat_interaction.py
--rw-r--r--   0 clement    (502) staff       (20)     1399 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/categorical_encode.py
--rw-r--r--   0 clement    (502) staff       (20)     2098 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/datetime_cyclical.py
--rw-r--r--   0 clement    (502) staff       (20)     1290 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/derive.py
--rw-r--r--   0 clement    (502) staff       (20)     2080 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/derive_rescale.py
--rw-r--r--   0 clement    (502) staff       (20)      995 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/drop_rows.py
--rw-r--r--   0 clement    (502) staff       (20)     1131 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/dummify.py
--rw-r--r--   0 clement    (502) staff       (20)      759 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/flag.py
--rw-r--r--   0 clement    (502) staff       (20)     1205 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/impute.py
--rw-r--r--   0 clement    (502) staff       (20)     1423 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/normalize.py
--rw-r--r--   0 clement    (502) staff       (20)      864 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/num_cat_interaction.py
--rw-r--r--   0 clement    (502) staff       (20)     1023 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/num_num_interaction.py
--rw-r--r--   0 clement    (502) staff       (20)     5038 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/prepare_input.py
--rw-r--r--   0 clement    (502) staff       (20)     1302 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/preprocessings.py
--rw-r--r--   0 clement    (502) staff       (20)      996 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/preprocessor.py
--rw-r--r--   0 clement    (502) staff       (20)      928 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/rescale.py
--rw-r--r--   0 clement    (502) staff       (20)     1679 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/selection.py
--rw-r--r--   0 clement    (502) staff       (20)     2471 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/vectorize_tfidf.py
--rw-r--r--   0 clement    (502) staff       (20)     1246 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/vectorize_word_count.py
--rw-r--r--   0 clement    (502) staff       (20)      783 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/processors/vectors_unfold.py
-drwxr-xr-x   0 clement    (502) staff       (20)        0 2023-03-16 17:26:56.604635 dataiku-scoring-11.4.0/dataikuscoring/utils/
--rw-r--r--   0 clement    (502) staff       (20)      559 2023-03-03 14:00:38.000000 dataiku-scoring-11.4.0/dataikuscoring/utils/__init__.py
--rw-r--r--   0 clement    (502) staff       (20)     2323 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/utils/indexed_matrix.py
--rw-r--r--   0 clement    (502) staff       (20)      239 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/utils/math_utils.py
--rw-r--r--   0 clement    (502) staff       (20)     5298 2023-03-16 17:14:53.000000 dataiku-scoring-11.4.0/dataikuscoring/utils/prediction_result.py
--rw-r--r--   0 clement    (502) staff       (20)     1272 2023-03-16 17:14:53.000000 dataiku-scoring-11.4.0/dataikuscoring/utils/scoring_data.py
--rw-r--r--   0 clement    (502) staff       (20)     1413 2023-01-27 13:34:30.000000 dataiku-scoring-11.4.0/dataikuscoring/utils/tokenizer.py
--rw-r--r--   0 clement    (502) staff       (20)        6 2022-10-18 17:42:02.000000 dataiku-scoring-11.4.0/requirements.txt
--rw-r--r--   0 clement    (502) staff       (20)       38 2023-03-16 17:26:56.605599 dataiku-scoring-11.4.0/setup.cfg
--rw-r--r--   0 clement    (502) staff       (20)      876 2023-03-16 17:23:46.000000 dataiku-scoring-11.4.0/setup.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1098 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/PKG-INFO
+-rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/requirements.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)       65 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/MANIFEST.in
+-rw-r--r--   0 kevinremy   (502) staff       (20)      214 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/README.md
+-rw-r--r--   0 kevinremy   (502) staff       (20)       27 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/NOTICE.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)      876 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/setup.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)       38 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/setup.cfg
+-rw-r--r--   0 kevinremy   (502) staff       (20)      169 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/HISTORY.txt
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1098 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/PKG-INFO
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2506 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/requires.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)       15 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/top_level.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)        1 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)      524 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/LICENSE.txt
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1103 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     4771 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/decision_tree_model.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1157 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/generic_mlp.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1597 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/logistic.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      672 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      903 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      848 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/mlp_classifier.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1581 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_classifier.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      576 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/common.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      429 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/linear_regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      258 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/mlp_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      708 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_classifier.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2357 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)    10732 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/classification.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)    11000 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/dss_flavor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      681 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     6912 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/common.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1069 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/__init__.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      239 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/math_utils.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      242 2023-06-15 08:28:03.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     5406 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/prediction_result.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1413 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/tokenizer.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1380 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/scoring_data.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2323 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/indexed_matrix.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/models/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      880 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/binary.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      205 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2457 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/models/mlflow.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      334 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/multiclass.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      635 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     6240 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/models/partitioned.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     3964 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/model.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2409 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/common.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      928 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/rescale.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2080 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/derive_rescale.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      759 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/flag.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2471 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_tfidf.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      783 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/vectors_unfold.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1399 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/categorical_encode.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1423 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/normalize.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1047 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/cat_cat_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1290 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/derive.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1241 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1205 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/impute.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      996 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1023 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/num_num_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1131 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/dummify.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      711 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/binarize.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1679 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/selection.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      864 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/num_cat_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2098 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/datetime_cyclical.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1302 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessings.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      995 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/drop_rows.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     5038 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/prepare_input.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2863 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/calibration.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1246 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_word_count.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     9455 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/load.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dataiku-scoring-11.4.0/LICENSE.txt` & `dataiku-scoring-11.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/PKG-INFO` & `dataiku-scoring-11.4.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: dataiku-scoring
-Version: 11.4.0
+Version: 11.4.4
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
+Description: # Dataiku ML Scoring Python library
+        
+        This repository contains the Python library to run exported Dataiku models outside of Dataiku.
+        
+        To use this library, you need to first export your model to Python from Dataiku.
+        
+        
+        Changelog
+        ==========
+        
+        11.4.4 (2023-07-04)
+        -------------------
+        
+        * Initial release for DSS 11.4.4
+        
+        11.1.0 (2022-10-20)
+        -------------------
+        
+        * Initial release for DSS 11.1
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-License-File: LICENSE.txt
-License-File: NOTICE.txt
-
-# Dataiku ML Scoring Python library
-
-This repository contains the Python library to run exported Dataiku models outside of Dataiku.
-
-To use this library, you need to first export your model to Python from Dataiku.
-
-
-Changelog
-==========
-
-11.4.0 (2023-03-16)
--------------------
-
-* Initial release for DSS 11.4
-
-
-11.1.0 (2022-10-20)
--------------------
-
-* Initial release for DSS 11.1
```

### Comparing `dataiku-scoring-11.4.0/dataiku_scoring.egg-info/PKG-INFO` & `dataiku-scoring-11.4.4/dataiku_scoring.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: dataiku-scoring
-Version: 11.4.0
+Version: 11.4.4
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
+Description: # Dataiku ML Scoring Python library
+        
+        This repository contains the Python library to run exported Dataiku models outside of Dataiku.
+        
+        To use this library, you need to first export your model to Python from Dataiku.
+        
+        
+        Changelog
+        ==========
+        
+        11.4.4 (2023-07-04)
+        -------------------
+        
+        * Initial release for DSS 11.4.4
+        
+        11.1.0 (2022-10-20)
+        -------------------
+        
+        * Initial release for DSS 11.1
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-License-File: LICENSE.txt
-License-File: NOTICE.txt
-
-# Dataiku ML Scoring Python library
-
-This repository contains the Python library to run exported Dataiku models outside of Dataiku.
-
-To use this library, you need to first export your model to Python from Dataiku.
-
-
-Changelog
-==========
-
-11.4.0 (2023-03-16)
--------------------
-
-* Initial release for DSS 11.4
-
-
-11.1.0 (2022-10-20)
--------------------
-
-* Initial release for DSS 11.1
```

### Comparing `dataiku-scoring-11.4.0/dataiku_scoring.egg-info/SOURCES.txt` & `dataiku-scoring-11.4.4/dataiku_scoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/__init__.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/common.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/decision_tree_model.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/forest_classifier.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/forest_regressor.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/generic_mlp.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/generic_mlp.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/gradient_boosting_classifier.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/gradient_boosting_regressor.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/logistic.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/logistic.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/algorithms/mlp_classifier.py` & `dataiku-scoring-11.4.4/dataikuscoring/algorithms/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/load.py` & `dataiku-scoring-11.4.4/dataikuscoring/load.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/mlflow/__init__.py` & `dataiku-scoring-11.4.4/dataikuscoring/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/mlflow/classification.py` & `dataiku-scoring-11.4.4/dataikuscoring/mlflow/classification.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/mlflow/common.py` & `dataiku-scoring-11.4.4/dataikuscoring/mlflow/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/mlflow/dss_flavor.py` & `dataiku-scoring-11.4.4/dataikuscoring/mlflow/dss_flavor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/mlflow/regression.py` & `dataiku-scoring-11.4.4/dataikuscoring/mlflow/regression.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/models/__init__.py` & `dataiku-scoring-11.4.4/dataikuscoring/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/models/binary.py` & `dataiku-scoring-11.4.4/dataikuscoring/models/binary.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/models/common.py` & `dataiku-scoring-11.4.4/dataikuscoring/models/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/models/mlflow.py` & `dataiku-scoring-11.4.4/dataikuscoring/models/mlflow.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/models/model.py` & `dataiku-scoring-11.4.4/dataikuscoring/models/model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/models/partitioned.py` & `dataiku-scoring-11.4.4/dataikuscoring/models/partitioned.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/__init__.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/binarize.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/binarize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/calibration.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/calibration.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/cat_cat_interaction.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/cat_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/categorical_encode.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/categorical_encode.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/datetime_cyclical.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/datetime_cyclical.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/derive.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/derive.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/derive_rescale.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/derive_rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/drop_rows.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/drop_rows.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/dummify.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/dummify.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/flag.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/flag.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/impute.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/impute.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/normalize.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/normalize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/num_cat_interaction.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/num_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/num_num_interaction.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/num_num_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/prepare_input.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/prepare_input.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/preprocessings.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessings.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/preprocessor.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/rescale.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/selection.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/selection.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/vectorize_tfidf.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_tfidf.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/vectorize_word_count.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_word_count.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/processors/vectors_unfold.py` & `dataiku-scoring-11.4.4/dataikuscoring/processors/vectors_unfold.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/utils/indexed_matrix.py` & `dataiku-scoring-11.4.4/dataikuscoring/utils/indexed_matrix.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/utils/prediction_result.py` & `dataiku-scoring-11.4.4/dataikuscoring/utils/prediction_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Warning: This module MUST NOT be imported in any common area of the package as it relies on pandas
+"""
+
 import numpy as np
 import pandas as pd
 import six
 from abc import abstractmethod
 from abc import ABCMeta
```

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/utils/scoring_data.py` & `dataiku-scoring-11.4.4/dataikuscoring/utils/scoring_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Warning: This module MUST NOT be imported in any common area of the package as it relies on pandas
+"""
+
 import pandas as pd
 
 
 class ScoringData(object):
     def __init__(self, is_empty=False, prediction_result=None, valid_y=None, valid_sample_weights=None, preds_df=None,
                  probas_df=None, decisions_and_cuts=None, reason=None, valid_unprocessed=None):
         """
```

### Comparing `dataiku-scoring-11.4.0/dataikuscoring/utils/tokenizer.py` & `dataiku-scoring-11.4.4/dataikuscoring/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.0/setup.py` & `dataiku-scoring-11.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 
 long_description = (open('README.md').read() + '\n\n' +
                     open('HISTORY.txt').read())
 
-VERSION = "11.4.0"
+VERSION = "11.4.4"
 
 setuptools.setup(
     name='dataiku-scoring',
     version=VERSION,
     license="Apache Software License",
     packages=setuptools.find_packages(),
     description="Dataiku ML Scoring Python library",
```

