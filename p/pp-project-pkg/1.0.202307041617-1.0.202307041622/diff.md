# Comparing `tmp/pp_project_pkg-1.0.202307041617-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307041622-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 14678 bytes, number of entries: 20
+Zip file size: 14680 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 14:49 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:35 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 10:34 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5130 b- defN 23-Jul-04 16:04 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 13:59 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7418 b- defN 23-Jul-04 15:47 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7847 b- defN 23-Jul-04 16:17 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 16:17 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 10:39 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041617.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 16:17 pp_project_pkg-1.0.202307041617.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 16:17 pp_project_pkg-1.0.202307041617.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 16:17 pp_project_pkg-1.0.202307041617.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 16:17 pp_project_pkg-1.0.202307041617.dist-info/RECORD
-20 files, 40309 bytes uncompressed, 11654 bytes compressed:  71.1%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-04 16:22 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-04 16:21 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202307041622.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-04 16:23 pp_project_pkg-1.0.202307041622.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 16:23 pp_project_pkg-1.0.202307041622.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-04 16:23 pp_project_pkg-1.0.202307041622.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1799 b- defN 23-Jul-04 16:23 pp_project_pkg-1.0.202307041622.dist-info/RECORD
+20 files, 40309 bytes uncompressed, 11656 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041617.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307041622.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041617.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307041622.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041617.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307041622.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041617.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307041622.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307041617.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307041622.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('04')
 VERSION_HOUR = int('16')
-VERSION_MINUTE = int('17')
+VERSION_MINUTE = int('22')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307041617
-version_date = '2023/07/04 16:17'
+PATCH_VERSION = 202307041622
+version_date = '2023/07/04 16:22'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -37,15 +37,15 @@
     else:
         cover_count = covers.values[0]
     
     pp_rework = pp_rework.drop(columns=['meal_service_id']).reset_index(drop=True)
     pp_production_rework = pd.merge(pp_production, pp_rework, on=['taxonomy_code'])
     name_pd = pd.read_csv('./taxcode_name_mapping.csv')
     name_pd = name_pd.drop(columns=['Unnamed: 0']).reset_index(drop=True)
-    name_pd = name_pd.rename(columns={name_pd.columns[0]:'taxonomy_code',name_pd.columns[1]:'name'})
+    name_pd = name_pd.rename(columns={name_pd.columns[1]:'taxonomy_code',name_pd.columns[0]:'name'})
     pp_production_rework = pd.merge(pp_production_rework, name_pd, on=['taxonomy_code'])
 
     actual_production_and_rework = pp_production_rework.copy()
     actual_production_and_rework['quantity_g'] = actual_production_and_rework['actual_production_kg']*1000
     actual_production_and_rework['rework_g'] = actual_production_and_rework['rework_kg']*1000
     
     joined_df = waste_data_for_site.join(hub_custom_breakdown.set_index('id'), on='reason_guid', how='inner')
```

## Comparing `pp_project_pkg-1.0.202307041617.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307041622.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307041617.dist-info/RECORD` & `pp_project_pkg-1.0.202307041622.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/extra.py,sha256=ChMXzpCfCPpkvfhTC4NQcCnNqHQKY59zr7NF_Gw1KlY,5130
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/train_loop.py,sha256=ozHLyx6fdFnywjKqAdJsLwkyTDZjX1Cjftum1umZRE4,7418
 pp_project_pkg/utils.py,sha256=4qIYSi8u7uO2HujXvkYnV4FQ8tyOUbH3Cri8N_aJsY4,7847
-pp_project_pkg/version.py,sha256=--jWdXMG6pxwWxrT4TD2Sasp3YYateCAIgHmLRyxONs,396
-pp_project_pkg/wrangling.py,sha256=g9y6mJXvtV-C1YNel_fLRjhtqpPtXcL131Mc1NdVv8s,5301
-pp_project_pkg-1.0.202307041617.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307041617.dist-info/METADATA,sha256=NGBAhxwrekhlmlMOczMh9Q_t0HPSfU0ea6_Fl6yQ0RI,191
-pp_project_pkg-1.0.202307041617.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202307041617.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307041617.dist-info/RECORD,,
+pp_project_pkg/version.py,sha256=929cKdKPTVFerEo_pZomEStVb_dnGfa6m2MJMqADnZI,396
+pp_project_pkg/wrangling.py,sha256=0l0_MMgUEyjNlwOmrYrEj7pNtvCT_LyZFXOiKSko3PM,5301
+pp_project_pkg-1.0.202307041622.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307041622.dist-info/METADATA,sha256=sSIpsYC_-dyZz6BqUJqsbE_uwE2wcYTsXs9r-0u_9Dg,191
+pp_project_pkg-1.0.202307041622.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202307041622.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307041622.dist-info/RECORD,,
```

