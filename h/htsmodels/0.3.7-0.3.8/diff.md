# Comparing `tmp/htsmodels-0.3.7.tar.gz` & `tmp/htsmodels-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htsmodels-0.3.7.tar", last modified: Thu Dec 29 10:50:40 2022, max compression
+gzip compressed data, was "htsmodels-0.3.8.tar", last modified: Thu Dec 29 11:58:08 2022, max compression
```

## Comparing `htsmodels-0.3.7.tar` & `htsmodels-0.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-29 10:50:40.643211 htsmodels-0.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/htsmodels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/htsmodels/Tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/Tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/Tests/test_deepar_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/Tests/test_mint_results_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/Tests/test_mint_results_store_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/Tests/test_mint_results_tourism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/Tests/test_standard_gp_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/htsmodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/models/deepar.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/models/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/models/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11264 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/models/mint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/models/standard_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/htsmodels/results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14837 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/results/calculate_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/htsmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2022-12-29 10:50:31.000000 htsmodels-0.3.7/htsmodels/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 10:50:40.643211 htsmodels-0.3.7/htsmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-29 10:50:40.000000 htsmodels-0.3.7/htsmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-29 10:50:40.000000 htsmodels-0.3.7/htsmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 10:50:40.000000 htsmodels-0.3.7/htsmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-29 10:50:40.000000 htsmodels-0.3.7/htsmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-29 10:50:40.000000 htsmodels-0.3.7/htsmodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 10:50:40.643211 htsmodels-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2022-12-29 10:50:31.000000 htsmodels-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.315189 htsmodels-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-29 11:58:08.311188 htsmodels-0.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.311188 htsmodels-0.3.8/htsmodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.311188 htsmodels-0.3.8/htsmodels/Tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/Tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/Tests/test_deepar_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/Tests/test_deepar_results_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/Tests/test_mint_results_store_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/Tests/test_mint_results_tourism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/Tests/test_standard_gp_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.311188 htsmodels-0.3.8/htsmodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/models/deepar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/models/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/models/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/models/mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/models/standard_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.311188 htsmodels-0.3.8/htsmodels/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14837 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/results/calculate_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.311188 htsmodels-0.3.8/htsmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2022-12-29 11:57:55.000000 htsmodels-0.3.8/htsmodels/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 11:58:08.311188 htsmodels-0.3.8/htsmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-29 11:58:08.000000 htsmodels-0.3.8/htsmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-29 11:58:08.000000 htsmodels-0.3.8/htsmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 11:58:08.000000 htsmodels-0.3.8/htsmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-29 11:58:08.000000 htsmodels-0.3.8/htsmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-29 11:58:08.000000 htsmodels-0.3.8/htsmodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 11:58:08.315189 htsmodels-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2022-12-29 11:57:55.000000 htsmodels-0.3.8/setup.py
```

### Comparing `htsmodels-0.3.7/PKG-INFO` & `htsmodels-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htsmodels
-Version: 0.3.7
+Version: 0.3.8
 Summary: Forecasting algorithms for hierarchical time series
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 Keywords: python,time series,hierarchical,forecasting,htsmodels,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `htsmodels-0.3.7/htsmodels/Tests/test_deepar_results.py` & `htsmodels-0.3.8/htsmodels/Tests/test_deepar_results.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/Tests/test_mint_results_police.py` & `htsmodels-0.3.8/htsmodels/Tests/test_deepar_results_police.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/Tests/test_mint_results_store_prison.py` & `htsmodels-0.3.8/htsmodels/Tests/test_mint_results_store_prison.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/Tests/test_mint_results_tourism.py` & `htsmodels-0.3.8/htsmodels/Tests/test_mint_results_tourism.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/Tests/test_standard_gp_prison.py` & `htsmodels-0.3.8/htsmodels/Tests/test_standard_gp_prison.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/models/deepar.py` & `htsmodels-0.3.8/htsmodels/models/deepar.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             )
 
         self.wall_time_predict = time.time() - timer_start
         return pred_mean, pred_std
 
     def store_metrics(self, res, track_mem=True):
         with open(
-            f"{self.input_dir}results/results_gp_cov_{self.dataset}.pickle", "wb"
+            f"{self.input_dir}results_gp_cov_{self.dataset}.pickle", "wb"
         ) as handle:
             if track_mem:
                 process = psutil.Process(os.getpid())
                 mem = process.memory_info().rss / (1024**3)
                 self.logger_metrics.info(
                     f"Storing error metrics used {mem:.3f} GB of RAM"
                 )
```

### Comparing `htsmodels-0.3.7/htsmodels/models/mean_functions.py` & `htsmodels-0.3.8/htsmodels/models/mean_functions.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/models/mint.py` & `htsmodels-0.3.8/htsmodels/models/mint.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 
         # Filter only the predictions
         pred_mint = pred_mint[pred_mint['Date'] > self.last_train_date]
 
         return pred_mint
 
     def store_metrics(self, res, track_mem=True):
-        with open(f'{self.input_dir}results/results_gp_cov_{self.dataset}.pickle', 'wb') as handle:
+        with open(f"{self.input_dir}results_gp_cov_{self.dataset}.pickle", 'wb') as handle:
             if track_mem:
                 process = psutil.Process(os.getpid())
                 mem = process.memory_info().rss / (1024**3)
                 self.logger_metrics.info(
                     f"Storing error metrics used {mem:.3f} GB of RAM"
                 )
             pickle.dump(res, handle, pickle.HIGHEST_PROTOCOL)
```

### Comparing `htsmodels-0.3.7/htsmodels/models/standard_gp.py` & `htsmodels-0.3.8/htsmodels/models/standard_gp.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
     def store_metrics(
         self,
         res: Dict[str, Dict[str, Union[float, np.ndarray]]],
         track_mem: bool = True,
     ):
         with open(
-            f"{self.input_dir}results/results_gp_cov_{self.dataset}_{self.model_version}.pickle",
+            f"{self.input_dir}results_gp_cov_{self.dataset}_{self.model_version}.pickle",
             "wb",
         ) as handle:
             if track_mem:
                 process = psutil.Process(os.getpid())
                 mem = process.memory_info().rss / (1024**3)
                 self.logger_metrics.info(
                     f"Storing error metrics used {mem:.3f} GB of RAM"
```

### Comparing `htsmodels-0.3.7/htsmodels/results/calculate_metrics.py` & `htsmodels-0.3.8/htsmodels/results/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels/utils/logger.py` & `htsmodels-0.3.8/htsmodels/utils/logger.py`

 * *Files identical despite different names*

### Comparing `htsmodels-0.3.7/htsmodels.egg-info/PKG-INFO` & `htsmodels-0.3.8/htsmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htsmodels
-Version: 0.3.7
+Version: 0.3.8
 Summary: Forecasting algorithms for hierarchical time series
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 Keywords: python,time series,hierarchical,forecasting,htsmodels,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `htsmodels-0.3.7/htsmodels.egg-info/SOURCES.txt` & `htsmodels-0.3.8/htsmodels.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 htsmodels.egg-info/PKG-INFO
 htsmodels.egg-info/SOURCES.txt
 htsmodels.egg-info/dependency_links.txt
 htsmodels.egg-info/requires.txt
 htsmodels.egg-info/top_level.txt
 htsmodels/Tests/__init__.py
 htsmodels/Tests/test_deepar_results.py
-htsmodels/Tests/test_mint_results_police.py
+htsmodels/Tests/test_deepar_results_police.py
 htsmodels/Tests/test_mint_results_store_prison.py
 htsmodels/Tests/test_mint_results_tourism.py
 htsmodels/Tests/test_standard_gp_prison.py
 htsmodels/models/__init__.py
 htsmodels/models/deepar.py
 htsmodels/models/gp.py
 htsmodels/models/mean_functions.py
```

### Comparing `htsmodels-0.3.7/setup.py` & `htsmodels-0.3.8/setup.py`

 * *Files identical despite different names*

