# Comparing `tmp/pp_project_pkg-1.0.202307041312-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307041314-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 14447 bytes, number of entries: 20
+Zip file size: 14443 bytes, number of entries: 20
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
--rw-rw-r--  2.0 unx     7440 b- defN 23-Jul-04 13:12 pp_project_pkg/train_loop.py
+-rw-rw-r--  2.0 unx     7439 b- defN 23-Jul-04 13:14 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7448 b- defN 23-Jul-04 10:39 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 13:12 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 13:14 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 10:39 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 13:13 pp_project_pkg-1.0.202307041312.dist-info/RECORD
-20 files, 39145 bytes uncompressed, 11423 bytes compressed:  70.8%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041314.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 13:14 pp_project_pkg-1.0.202307041314.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 13:14 pp_project_pkg-1.0.202307041314.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 13:14 pp_project_pkg-1.0.202307041314.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 13:14 pp_project_pkg-1.0.202307041314.dist-info/RECORD
+20 files, 39144 bytes uncompressed, 11419 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307041314.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041312.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307041314.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041312.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307041314.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041312.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307041314.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041312.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307041314.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/train_loop.py

```diff
@@ -68,15 +68,15 @@
 
     # perform inference to predict actual_production based on no_of_covers
     if test_case:
         input_data = [test_case]
         predicted_output = model.predict(input_data)
         if logger:
             logger.info("Predicted output for a test case: {}".format(predicted_output))
-    return model,
+    return model
 
 
 
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
-VERSION_MINUTE = int('12')
+VERSION_MINUTE = int('14')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307041312
-version_date = '2023/07/04 13:12'
+PATCH_VERSION = 202307041314
+version_date = '2023/07/04 13:14'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307041314.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307041312.dist-info/RECORD` & `pp_project_pkg-1.0.202307041314.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/extra.py,sha256=cCFm5vQVbDt1Oebpe8HJI8LpjrxfELdcNrirRBLCFjo,4343
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
-pp_project_pkg/train_loop.py,sha256=MQ18cU5Il6IzJ-0vPavOsKDk37MN15jBTjZCDPXJeEQ,7440
+pp_project_pkg/train_loop.py,sha256=aIpXH21zjnMbWMMe-ylQ4Wmq866bHhDdh8Em-cGS1-w,7439
 pp_project_pkg/utils.py,sha256=KmLqDW3F66lo5e4oQFNCMrUZGVtFkHbqgxjyODeeVY8,7448
-pp_project_pkg/version.py,sha256=AVr6D15ptEokF-H1ydIfnx7wNf50GzJMEVEd_t52RIU,396
+pp_project_pkg/version.py,sha256=hqJy7HQ81RfAOAeScWNV_6rnzVEJMYCYfMHXF4pPwLo,396
 pp_project_pkg/wrangling.py,sha256=g9y6mJXvtV-C1YNel_fLRjhtqpPtXcL131Mc1NdVv8s,5301
-pp_project_pkg-1.0.202307041312.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307041312.dist-info/METADATA,sha256=Y0iigu9jb1fknK9nD0uv6fNX2rE9hbbiTi7CaGuXdcI,191
-pp_project_pkg-1.0.202307041312.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202307041312.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307041312.dist-info/RECORD,,
+pp_project_pkg-1.0.202307041314.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307041314.dist-info/METADATA,sha256=u1Z_pvx1JC6PfKtz72zxbOL9Tl8z_8rPmJ7ElAO5mQo,191
+pp_project_pkg-1.0.202307041314.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202307041314.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307041314.dist-info/RECORD,,
```

