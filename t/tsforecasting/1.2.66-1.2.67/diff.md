# Comparing `tmp/tsforecasting-1.2.66-py3-none-any.whl.zip` & `tmp/tsforecasting-1.2.67-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18592 bytes, number of entries: 12
+Zip file size: 18580 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      393 b- defN 23-Feb-21 11:35 tsforecasting/__init__.py
 -rw-rw-rw-  2.0 fat    10033 b- defN 23-Apr-17 15:36 tsforecasting/tsf_data_eng.py
 -rw-rw-rw-  2.0 fat    10138 b- defN 23-Jun-20 17:28 tsforecasting/tsf_expanding_window.py
--rw-rw-rw-  2.0 fat     1684 b- defN 23-Mar-02 11:05 tsforecasting/tsf_model_configs.py
+-rw-rw-rw-  2.0 fat     1640 b- defN 23-Jul-04 20:46 tsforecasting/tsf_model_configs.py
 -rw-rw-rw-  2.0 fat     4009 b- defN 23-Apr-17 15:43 tsforecasting/tsf_model_selection.py
 -rw-rw-rw-  2.0 fat     7891 b- defN 23-Apr-17 15:44 tsforecasting/tsf_performance.py
 -rw-rw-rw-  2.0 fat     8385 b- defN 23-May-27 21:19 tsforecasting/tsf_predictions.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11121 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/RECORD
-12 files, 55885 bytes uncompressed, 16820 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-Jul-04 20:53 tsforecasting-1.2.67.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11121 b- defN 23-Jul-04 20:53 tsforecasting-1.2.67.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 20:53 tsforecasting-1.2.67.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-04 20:53 tsforecasting-1.2.67.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1047 b- defN 23-Jul-04 20:53 tsforecasting-1.2.67.dist-info/RECORD
+12 files, 55841 bytes uncompressed, 16808 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tsforecasting/tsf_performance.py
 Comment: 
 
 Filename: tsforecasting/tsf_predictions.py
 Comment: 
 
-Filename: tsforecasting-1.2.66.dist-info/LICENSE
+Filename: tsforecasting-1.2.67.dist-info/LICENSE
 Comment: 
 
-Filename: tsforecasting-1.2.66.dist-info/METADATA
+Filename: tsforecasting-1.2.67.dist-info/METADATA
 Comment: 
 
-Filename: tsforecasting-1.2.66.dist-info/WHEEL
+Filename: tsforecasting-1.2.67.dist-info/WHEEL
 Comment: 
 
-Filename: tsforecasting-1.2.66.dist-info/top_level.txt
+Filename: tsforecasting-1.2.67.dist-info/top_level.txt
 Comment: 
 
-Filename: tsforecasting-1.2.66.dist-info/RECORD
+Filename: tsforecasting-1.2.67.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsforecasting/tsf_model_configs.py

```diff
@@ -1,13 +1,13 @@
 def model_configurations():
     
     model_configs ={'RandomForest':{'n_estimators':250,'random_state':42,'criterion':"squared_error",
-                       'max_depth':None,'max_features':"auto"},
+                       'max_depth':None},
                    'ExtraTrees':{'n_estimators':250,'random_state':42,'criterion':"squared_error",
-                       'max_depth':None,'max_features':"auto"}, 
+                       'max_depth':None}, 
                    'GBR':{'n_estimators':250,'learning_rate':0.1,'criterion':"friedman_mse",
                         'max_depth':3,'min_samples_split':5,'learning_rate':0.01,'loss':'squared_error'},
                    'KNN':{'n_neighbors': 3,'weights':"uniform",'algorithm':"auto",'metric_params':None},
                    'GeneralizedLR':{'power':1,'alpha':0.5,'link':'log','fit_intercept':True,
                         'max_iter':100,'warm_start':False,'verbose':0},
                    'XGBoost':{'objective':'reg:squarederror','n_estimators':1000,'nthread':24},
                    'H2O_AutoML':{'max_models':50,'nfolds':0,'seed':1,'max_runtime_secs':30,
```

## Comparing `tsforecasting-1.2.66.dist-info/LICENSE` & `tsforecasting-1.2.67.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.66.dist-info/METADATA` & `tsforecasting-1.2.67.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.66
+Version: 1.2.67
 Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
```

## Comparing `tsforecasting-1.2.66.dist-info/RECORD` & `tsforecasting-1.2.67.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tsforecasting/__init__.py,sha256=RIdya5qTwjBffBeeNTSBTSaeSGma5i4XGXmiFzswJQs,393
 tsforecasting/tsf_data_eng.py,sha256=83glbKi5r3xLavkck2ssz5W1Pp1KyhQDhvfzAD_c_9Y,10033
 tsforecasting/tsf_expanding_window.py,sha256=nKC3GpKr1-NRVizUlNEeHE5Ijo5cS1Wa77X9RfiVDrg,10138
-tsforecasting/tsf_model_configs.py,sha256=vSsZuNQkmcrie_HEpsg1PCT565BPAUjlgj2w3IkhlD4,1684
+tsforecasting/tsf_model_configs.py,sha256=h-5FahWqMI6zfsW5iiIOBiiFXURHhS5ogwcpkO03JCY,1640
 tsforecasting/tsf_model_selection.py,sha256=3fI9tXKw5XA-YEn3cycOKQeLMj5Dq4ICNpJj8dEnmxQ,4009
 tsforecasting/tsf_performance.py,sha256=Wru_7VWLO1NDieeVm8AcA2P3Kd3yEhI8wz0yNUH6gQE,7891
 tsforecasting/tsf_predictions.py,sha256=QW1hxediVFV3hvChvOcjl6YGC0PjPHI_OifApmb-Rw8,8385
-tsforecasting-1.2.66.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-tsforecasting-1.2.66.dist-info/METADATA,sha256=9ycGibeUNVR9gmvUW7Hp4f3xfNhI94A3FaRj3qgZ2CM,11121
-tsforecasting-1.2.66.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tsforecasting-1.2.66.dist-info/top_level.txt,sha256=oKWWwpca0QkvqhgDcYBoVWqcFDLNSkSOuCvuEcZFABY,14
-tsforecasting-1.2.66.dist-info/RECORD,,
+tsforecasting-1.2.67.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+tsforecasting-1.2.67.dist-info/METADATA,sha256=qHLEE8lF-cYs2uQ8vuJMUwlRj76Hzt_rA3NusfmMRHw,11121
+tsforecasting-1.2.67.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+tsforecasting-1.2.67.dist-info/top_level.txt,sha256=oKWWwpca0QkvqhgDcYBoVWqcFDLNSkSOuCvuEcZFABY,14
+tsforecasting-1.2.67.dist-info/RECORD,,
```

