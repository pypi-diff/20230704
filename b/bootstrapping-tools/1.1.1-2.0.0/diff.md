# Comparing `tmp/bootstrapping_tools-1.1.1.tar.gz` & `tmp/bootstrapping_tools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrapping_tools-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bootstrapping_tools-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bootstrapping_tools-1.1.1.tar` & `bootstrapping_tools-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      200 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/README.md
--rw-r--r--   0        0        0      137 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/bootstrapping_tools/__init__.py
--rw-r--r--   0        0        0    11811 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/bootstrapping_tools/bootstrapping.py
--rw-r--r--   0        0        0      859 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/bootstrapping_tools/resample_by_blocks.py
--rw-r--r--   0        0        0      516 2023-07-03 19:10:59.604443 bootstrapping_tools-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/README.md
+-rw-r--r--   0        0        0      185 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/__init__.py
+-rw-r--r--   0        0        0    11721 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/bootstrapping.py
+-rw-r--r--   0        0        0      293 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/n0_and_lambdas_intervals.py
+-rw-r--r--   0        0        0      859 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/resample_by_blocks.py
+-rw-r--r--   0        0        0      516 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-2.0.0/PKG-INFO
```

### Comparing `bootstrapping_tools-1.1.1/bootstrapping_tools/bootstrapping.py` & `bootstrapping_tools-2.0.0/bootstrapping_tools/bootstrapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 import random
 
+from .n0_and_lambdas_intervals import get_percentile
 from .resample_by_blocks import random_resample_data_by_blocks
 from scipy.optimize import curve_fit
 from tqdm import tqdm
 
 
 def power_law(time_interval, population_growth_rate, initial_population_size):
     """This function represent a simple power law of the type: f(y) = a*x^y
@@ -143,16 +144,16 @@
     print("Calculating samples per season:")
     for season in tqdm(seasons):
         data_per_season = dataframe[dataframe.Temporada == season]
         bootstraped_data[season] = boostrapping_feature(data_per_season[column_name], N)
     lambdas_bootstraps = lambdas_from_bootstrap_table(bootstraped_data)
     limits = _return_central_limits_from_alpha(alpha)
     if return_distribution:
-        return lambdas_bootstraps, _calculate_intevals(lambdas_bootstraps, limits)
-    return _calculate_intevals(lambdas_bootstraps, limits)
+        return lambdas_bootstraps, get_percentile(lambdas_bootstraps, limits)
+    return get_percentile(lambdas_bootstraps, limits)
 
 
 def get_bootstrap_deltas(bootstrap_distribution, **kwargs):
     """Generate bootstrap interval differences for reports from 95% bootstrap interval array (2.5, 50 and 97.5 percentiles).
 
     Args:
         bootstrap_distribution (ndarray): 95% bootstrap interval array.
@@ -181,38 +182,34 @@
         column_name (string): Name of the column in the DataFrame to fit the model.
         N (int, optional): Number of bootstrap samples you want. Defaults to 2000.
         return_distribution (bool, optional): True if you want the bootstrap distribution. Defaults to False.
     Returns:
         [ndarray]: 95% bootstrap interval for lambda coefficient. The interval is conformed by 2.5, 50 and 97.5 percentiles in an Numpy array.
         If `return_distribution` is True, returns the distribution too.
     """
-    lambdas_bootstraps = []
+    bootstrap_tuples = []
     cont = 0
     rand = 0
     print("Calculating bootstrap growth rates distribution:")
     while cont < N:
         resampled_data = resample_and_shift_data(dataframe, rand, blocks_length)
         try:
             fitting_result = lambda_calculator_from_resampled_data(
                 resampled_data["Temporada"], resampled_data[column_name]
             )
         except RuntimeError:
             rand += 1
             continue
-        lambdas_bootstraps.append(fitting_result[0])
+        bootstrap_tuples.append(tuple(fitting_result))
         cont += 1
         rand += 1
     limits = _return_central_limits_from_alpha(alpha)
     if return_distribution:
-        return lambdas_bootstraps, _calculate_intevals(lambdas_bootstraps, limits)
-    return _calculate_intevals(lambdas_bootstraps, limits)
-
-
-def _calculate_intevals(lambdas_distribution, limits):
-    return np.percentile(lambdas_distribution, limits)
+        return bootstrap_tuples, get_percentile(bootstrap_tuples, limits)
+    return get_percentile(bootstrap_tuples, limits)
 
 
 def resample_data(dataframe, seed, blocks_length):
     rng = random.Random(seed)
     return random_resample_data_by_blocks(dataframe, blocks_length, rng)
 
 
@@ -221,15 +218,15 @@
     min_season = dataframe.loc[:, "Temporada"].min()
     resampled_data.loc[:, "Temporada"] = resampled_data.loc[:, "Temporada"] - min_season
     return resampled_data
 
 
 def calculate_intervals_from_p_values_and_alpha(distribution, p_values, alpha):
     limits = calculate_limits_from_p_values_and_alpha(p_values, alpha)
-    return _calculate_intevals(distribution, limits)
+    return get_percentile(distribution, limits)
 
 
 def calculate_limits_from_p_values_and_alpha(p_values, alpha):
     type_of_limit = choose_type_of_limits_from_p_values(p_values, alpha)
     return _LIMITS_FROM_ALPHA[type_of_limit](alpha=alpha)
```

### Comparing `bootstrapping_tools-1.1.1/bootstrapping_tools/resample_by_blocks.py` & `bootstrapping_tools-2.0.0/bootstrapping_tools/resample_by_blocks.py`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-1.1.1/pyproject.toml` & `bootstrapping_tools-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-1.1.1/PKG-INFO` & `bootstrapping_tools-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapping_tools
-Version: 1.1.1
+Version: 2.0.0
 Summary: GECI Tools for bootstrapping
 Home-page: https://github.com/IslasGECI/bootstrapping_tools
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bootstrapping_tools Version: 1.1.1 Summary: GECI
+Metadata-Version: 2.1 Name: bootstrapping_tools Version: 2.0.0 Summary: GECI
 Tools for bootstrapping Home-page: https://github.com/IslasGECI/
 bootstrapping_tools Author: Ciencia de Datos â¢ GECI Author-email:
 ciencia.datos@islas.org.mx Requires-Python: >=3 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 or later (GPLv3+) Requires-Dist: numpy Requires-Dist: pandas-stubs Requires-
 Dist: pandas Requires-Dist: scipy Requires-Dist: tqdm [https://
 www.islas.org.mx/img/logo.svg] # Bootstrapping tools GECI tools to perform
```

