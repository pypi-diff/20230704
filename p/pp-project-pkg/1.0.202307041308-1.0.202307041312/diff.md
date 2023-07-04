# Comparing `tmp/pp_project_pkg-1.0.202307041308-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307041312-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 14455 bytes, number of entries: 20
+Zip file size: 14447 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 14:49 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     4343 b- defN 23-Jul-04 12:51 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     7679 b- defN 23-Jul-04 13:08 pp_project_pkg/train_loop.py
+-rw-rw-r--  2.0 unx     7440 b- defN 23-Jul-04 13:12 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7448 b- defN 23-Jul-04 10:39 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 13:08 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 13:12 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 10:39 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041308.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 13:08 pp_project_pkg-1.0.202307041308.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 13:08 pp_project_pkg-1.0.202307041308.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 13:08 pp_project_pkg-1.0.202307041308.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 13:08 pp_project_pkg-1.0.202307041308.dist-info/RECORD
-20 files, 39384 bytes uncompressed, 11431 bytes compressed:  71.0%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/RECORD
+20 files, 39145 bytes uncompressed, 11423 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041308.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041308.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307041312.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041308.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307041312.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041308.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307041312.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041308.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307041312.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/train_loop.py

```diff
@@ -62,26 +62,21 @@
     r2 = r2_score(y_test, y_pred)
 
     if logger:
         logger.info('Mean squared error: {}'.format(mse))
         logger.info('Mean absolute error: {}'.format(mae))
         logger.info('R2 score: {}'.format(r2))   
 
-    # Check feature importances
-    importances = model.feature_importances_ 
-    feature_df = pd.DataFrame({'Feature': list(X), 'Importance': importances})
-    feature_df = feature_df.sort_values('Importance', ascending=False)
-
     # perform inference to predict actual_production based on no_of_covers
     if test_case:
         input_data = [test_case]
         predicted_output = model.predict(input_data)
         if logger:
             logger.info("Predicted output for a test case: {}".format(predicted_output))
-    return model,feature_df
+    return model,
 
 
 
 def train_model(data,logger=None):
     """
     Trains a linear model on the data and upload the model to the cloud with parameters
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('04')
 VERSION_HOUR = int('13')
-VERSION_MINUTE = int('08')
+VERSION_MINUTE = int('12')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307041308
-version_date = '2023/07/04 13:08'
+PATCH_VERSION = 202307041312
+version_date = '2023/07/04 13:12'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307041308.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

