# Comparing `tmp/mlimputer-1.0.5-py3-none-any.whl.zip` & `tmp/mlimputer-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9285 bytes, number of entries: 9
+Zip file size: 9246 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 mlimputer/__init__.py
 -rw-rw-rw-  2.0 fat     4834 b- defN 23-May-06 15:58 mlimputer/mli_imputation.py
--rw-rw-rw-  2.0 fat     6325 b- defN 23-May-06 16:00 mlimputer/mli_model_selection.py
--rw-rw-rw-  2.0 fat     1402 b- defN 23-Apr-17 14:19 mlimputer/mli_parameters.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6952 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      730 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/RECORD
-9 files, 21824 bytes uncompressed, 8027 bytes compressed:  63.2%
+-rw-rw-rw-  2.0 fat     6293 b- defN 23-Jul-04 20:19 mlimputer/mli_model_selection.py
+-rw-rw-rw-  2.0 fat     1358 b- defN 23-Jul-04 20:20 mlimputer/mli_parameters.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      730 b- defN 23-Jul-04 20:22 mlimputer-1.0.6.dist-info/RECORD
+9 files, 21692 bytes uncompressed, 7988 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mlimputer/mli_model_selection.py
 Comment: 
 
 Filename: mlimputer/mli_parameters.py
 Comment: 
 
-Filename: mlimputer-1.0.5.dist-info/LICENSE
+Filename: mlimputer-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: mlimputer-1.0.5.dist-info/METADATA
+Filename: mlimputer-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: mlimputer-1.0.5.dist-info/WHEEL
+Filename: mlimputer-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: mlimputer-1.0.5.dist-info/top_level.txt
+Filename: mlimputer-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mlimputer-1.0.5.dist-info/RECORD
+Filename: mlimputer-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlimputer/mli_model_selection.py

```diff
@@ -92,17 +92,17 @@
     for each numerical column in the input dataset. 
     Sorted by the percentage of missing values in ascending order. <-***********
     """
     
     df=dataset.copy()
     
     num_cols=df.select_dtypes(include=['int','float']).columns.tolist()
-    df_md = pd.DataFrame(df[num_cols].isna().sum().loc[df[num_cols].isna().sum() > 0], columns=['missing_data_count'])
-    df_md['missing_data_percentage'] = df_md['missing_data_count'] / len(df)
-    df_md = df_md.sort_values(by='missing_data_percentage', ascending=True)
+    df_md = pd.DataFrame(df[num_cols].isna().sum().loc[df[num_cols].isna().sum() > 0], columns=['null_count'])
+    df_md['null_percentage'] = df_md['null_count'] / len(df)
+    df_md = df_md.sort_values(by='null_percentage', ascending=True)
     df_md['columns']=df_md.index
     df_md=df_md.reset_index(drop=True)
     
     return df_md
 
 def cross_validation(dataset:pd.DataFrame, target:str, test_size:float=0.2, n_splits:int=5,models:list=[]):
     """
```

## mlimputer/mli_parameters.py

```diff
@@ -1,12 +1,12 @@
 def imputer_parameters():
     parameters ={'RandomForest':{'n_estimators':50,'random_state':42,'criterion':"squared_error",
-                                 'max_depth':None,'max_features':"auto"},
+                                 'max_depth':None},
                  'ExtraTrees':{'n_estimators':50,'random_state':42,'criterion':"squared_error",
-                               'max_depth':None,'max_features':"auto"}, 
+                               'max_depth':None}, 
                  'GBR':{'n_estimators':50,'learning_rate':0.1,'criterion':"friedman_mse",
                         'max_depth':3,'min_samples_split':5,'learning_rate':0.01,'loss':'squared_error'},
                  'KNN':{'n_neighbors': 3,'weights':"uniform",
                         'algorithm':"auto",'metric_params':None},
                  'XGBoost':{'objective':'reg:squarederror','n_estimators':1000,'nthread':24},
                  "Lightgbm": {'boosting_type': 'gbdt','objective':'regression','metric': 'mse',
                               'num_leaves': 31,'learning_rate': 0.05,'feature_fraction': 0.9,
```

## Comparing `mlimputer-1.0.5.dist-info/LICENSE` & `mlimputer-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlimputer-1.0.5.dist-info/METADATA` & `mlimputer-1.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlimputer
-Version: 1.0.5
+Version: 1.0.6
 Summary: MLimputer - Null Imputation Framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/MLimputer
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data preprecessing,null imputation,predictive null imputation,multiple null imputation,automated machine learning
 Classifier: Intended Audience :: Education
@@ -149,9 +149,7 @@
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
 
 ## Contact 
  
 Luis Santos - [LinkedIn](https://www.linkedin.com/in/lu%C3%ADsfssantos/)
-    
-Feel free to contact me and share your feedback.
```

## Comparing `mlimputer-1.0.5.dist-info/RECORD` & `mlimputer-1.0.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlimputer/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
 mlimputer/mli_imputation.py,sha256=clFXtMhBr304RllNvIZ_McnCrHndlF9OfiBiZj3spOM,4834
-mlimputer/mli_model_selection.py,sha256=tEt55AYa4JSBm_zezov_2Or30w4Flj_56VjgKP1-a5U,6325
-mlimputer/mli_parameters.py,sha256=G6x291YIhf--4jdv4gaBNsaxknTKjnqBdl73KEmTPfU,1402
-mlimputer-1.0.5.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
-mlimputer-1.0.5.dist-info/METADATA,sha256=8f611ydtMyAZT9ykZxT4mZfP-Wja94v4VOkUmqPSYHE,6952
-mlimputer-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mlimputer-1.0.5.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
-mlimputer-1.0.5.dist-info/RECORD,,
+mlimputer/mli_model_selection.py,sha256=ACnlqoQi584ucOfVL8xVpea90OEsIvpBQ0HTxfzR5Hc,6293
+mlimputer/mli_parameters.py,sha256=ihhlZZUL9DQ_tECwuwvPJqY7_3lDuoE58kVmEp2-bHk,1358
+mlimputer-1.0.6.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
+mlimputer-1.0.6.dist-info/METADATA,sha256=QEMPJHlVYH76yul5HpY8MEjESpd0s4P_tdC7ZzZfIj0,6896
+mlimputer-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mlimputer-1.0.6.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
+mlimputer-1.0.6.dist-info/RECORD,,
```

