# Comparing `tmp/pp_project_pkg-1.0.202307041559-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307041609-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 14589 bytes, number of entries: 20
+Zip file size: 14610 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 14:49 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
--rw-rw-r--  2.0 unx     5027 b- defN 23-Jul-04 15:54 pp_project_pkg/extra.py
+-rw-rw-r--  2.0 unx     5130 b- defN 23-Jul-04 16:04 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7418 b- defN 23-Jul-04 15:47 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7448 b- defN 23-Jul-04 10:39 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 15:59 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 16:09 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 10:39 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041559.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 15:59 pp_project_pkg-1.0.202307041559.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 15:59 pp_project_pkg-1.0.202307041559.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 15:59 pp_project_pkg-1.0.202307041559.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 15:59 pp_project_pkg-1.0.202307041559.dist-info/RECORD
-20 files, 39807 bytes uncompressed, 11565 bytes compressed:  70.9%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041609.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 16:09 pp_project_pkg-1.0.202307041609.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 16:09 pp_project_pkg-1.0.202307041609.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 16:09 pp_project_pkg-1.0.202307041609.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 16:09 pp_project_pkg-1.0.202307041609.dist-info/RECORD
+20 files, 39910 bytes uncompressed, 11586 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041559.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307041609.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041559.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307041609.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041559.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307041609.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041559.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307041609.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041559.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307041609.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/extra.py

```diff
@@ -17,19 +17,21 @@
 
     d1 =datetime.datetime.strptime(start_date,'%Y-%m-%d').date()
     #d2 =datetime.datetime.strptime(d2,'%Y-%m-%d').date()
 
     dates_to_add = [d1,d1]
     #dates_closing = [d2,d2]
     
-    tx = pd.DataFrame(data=dates_to_add,columns=['date','closed'])
+    tx = pd.DataFrame(data=[dates_to_add],columns=['date','closed'])
     if logger:
         logger.info(tx.head())
     tx.to_sql(name='waldorf_report_closed_data_latest',con=wv.ml_engine,schema='pp_tables' ,if_exists='replace',index=False)
     tx.to_sql(name='waldorf_report_closed_data_all',con=wv.ml_engine,schema='pp_tables' ,if_exists='replace',index=False)
+    if logger:
+        logger.info("Tables resetted to initial config date : {}".format(start_date))
 
     
     
     
 def convert_tables_to_data(logger=None):
     """
     Function to convert the tables to data
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('04')
-VERSION_HOUR = int('15')
-VERSION_MINUTE = int('59')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('09')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307041559
-version_date = '2023/07/04 15:59'
+PATCH_VERSION = 202307041609
+version_date = '2023/07/04 16:09'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307041559.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307041609.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307041559.dist-info/RECORD` & `pp_project_pkg-1.0.202307041609.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 mlflow_pipelines/fetch_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/fetch_data/get_data.py,sha256=OCoL8C6L0H-tKN5p5eSxo6l6elnrXU21EPB5Tk-IgY8,887
 mlflow_pipelines/train_model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
-pp_project_pkg/extra.py,sha256=-xLC3wpsXXFDYZJR96bixQqK4V1yn6XIWZe6-73asxo,5027
+pp_project_pkg/extra.py,sha256=ChMXzpCfCPpkvfhTC4NQcCnNqHQKY59zr7NF_Gw1KlY,5130
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/train_loop.py,sha256=ozHLyx6fdFnywjKqAdJsLwkyTDZjX1Cjftum1umZRE4,7418
 pp_project_pkg/utils.py,sha256=KmLqDW3F66lo5e4oQFNCMrUZGVtFkHbqgxjyODeeVY8,7448
-pp_project_pkg/version.py,sha256=i4oV4JvSFoB2lDb-tLvG-9IrmCXwX7jLryB5lMnagiQ,396
+pp_project_pkg/version.py,sha256=aZOwQt3PzPpPCspuepPR8bLSf27MVmLzYzImFHjhokQ,396
 pp_project_pkg/wrangling.py,sha256=g9y6mJXvtV-C1YNel_fLRjhtqpPtXcL131Mc1NdVv8s,5301
-pp_project_pkg-1.0.202307041559.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307041559.dist-info/METADATA,sha256=oj7r9p6bVgc8WfKVsezoKFebRXel79hew0sAP98CcQE,191
-pp_project_pkg-1.0.202307041559.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202307041559.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307041559.dist-info/RECORD,,
+pp_project_pkg-1.0.202307041609.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307041609.dist-info/METADATA,sha256=FvTPld3hGtm4aj9le6Gbst9kfh6BH71REmY6mfELT2Y,191
+pp_project_pkg-1.0.202307041609.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202307041609.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307041609.dist-info/RECORD,,
```

