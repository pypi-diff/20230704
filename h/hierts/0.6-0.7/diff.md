# Comparing `tmp/hierts-0.6.tar.gz` & `tmp/hierts-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierts-0.6.tar", last modified: Thu Jun 15 06:52:29 2023, max compression
+gzip compressed data, was "hierts-0.7.tar", last modified: Tue Jul  4 14:37:28 2023, max compression
```

## Comparing `hierts-0.6.tar` & `hierts-0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.404559 hierts-0.6/
--rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.6/LICENSE
--rw-rw-rw-   0        0        0    14643 2023-06-15 06:52:29.403559 hierts-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.6/README.md
--rw-rw-rw-   0        0        0      793 2023-06-15 06:50:31.000000 hierts-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 06:52:29.404559 hierts-0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.374559 hierts-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.380559 hierts-0.6/src/hierts/
--rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.6/src/hierts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.402559 hierts-0.6/src/hierts/_old/
--rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.6/src/hierts/_old/reconciliation.py
--rw-rw-rw-   0        0        0    20417 2023-06-15 06:48:19.000000 hierts-0.6/src/hierts/reconciliation.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.400561 hierts-0.6/src/hierts.egg-info/
--rw-rw-rw-   0        0        0    14643 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 14:37:28.318714 hierts-0.7/
+-rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.7/LICENSE
+-rw-rw-rw-   0        0        0    14643 2023-07-04 14:37:28.318714 hierts-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.7/README.md
+-rw-rw-rw-   0        0        0      793 2023-07-04 14:36:35.000000 hierts-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 14:37:28.319713 hierts-0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 14:37:28.272198 hierts-0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 14:37:28.285200 hierts-0.7/src/hierts/
+-rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.7/src/hierts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:37:28.316714 hierts-0.7/src/hierts/_old/
+-rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.7/src/hierts/_old/reconciliation.py
+-rw-rw-rw-   0        0        0    25043 2023-07-04 13:22:52.000000 hierts-0.7/src/hierts/reconciliation.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:37:28.305713 hierts-0.7/src/hierts.egg-info/
+-rw-rw-rw-   0        0        0    14643 2023-07-04 14:37:28.000000 hierts-0.7/src/hierts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-04 14:37:28.000000 hierts-0.7/src/hierts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:37:28.000000 hierts-0.7/src/hierts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-04 14:37:28.000000 hierts-0.7/src/hierts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 14:37:28.000000 hierts-0.7/src/hierts.egg-info/top_level.txt
```

### Comparing `hierts-0.6/LICENSE` & `hierts-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hierts-0.6/PKG-INFO` & `hierts-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.6
+Version: 0.7
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hierts-0.6/README.md` & `hierts-0.7/README.md`

 * *Files identical despite different names*

### Comparing `hierts-0.6/pyproject.toml` & `hierts-0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hierts"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Olivier Sprangers", email="o.r.sprangers@uva.nl" },
 ]
 description = "Hierarchical time series reconciliation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hierts-0.6/src/hierts/_old/reconciliation.py` & `hierts-0.7/src/hierts/_old/reconciliation.py`

 * *Files identical despite different names*

### Comparing `hierts-0.6/src/hierts/reconciliation.py` & `hierts-0.7/src/hierts/reconciliation.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import numpy as np 
 import pandas as pd
 import time
 from numba import njit, prange
 from typing import List, Tuple
 from scipy.sparse import coo_matrix, csc_matrix
 from sklearn.linear_model import LassoCV, Lasso
+from pandas.api.types import is_datetime64_any_dtype as is_datetime
 #%% Functions to perform forecast reconciliation
 def reconcile_forecasts(yhat: np.ndarray, S: np.ndarray, y_train: np.ndarray=None, yhat_train: np.ndarray=None, method: str='ols', positive: bool=False) -> np.ndarray:
     """Optimal reconciliation of hierarchical forecasts using various approaches.
     
         Based on approaches from:
     
         ['ols', 'wls_var', 'wls_struct', 'mint_cov', 'mint_shrink']
@@ -184,53 +185,71 @@
     # Fill diagonal with original empirical covariance diagonal
     np.fill_diagonal(W, emp_cov_diag)
 
     return W
 
 def calc_summing_matrix(df: pd.DataFrame, aggregation_cols: List[str], aggregations: List[List[str]] = None, 
                         sparse: bool = False, name_bottom_timeseries: str = 'bottom_timeseries') -> pd.DataFrame:
-    """Given a dataframe of timeseries and columns indicating their groupings, this function calculates a summing matrix according to a set of specified aggregations for the time series. 
+    """Given a dataframe of timeseries and columns indicating their groupings, this function calculates a cross-sectional hierarchy according to a set of specified aggregations for the time series. This function is deprecated, please use 'hierarchy_cross_sectional' instead. 
 
         :param df: DataFrame containing information about time series and their groupings
         :type df: pd.DataFrame
         :param aggregation_cols: List containing all the columns that contain categorization of the timeseries. 
-        :type df: List[str]
+        :type aggregation_cols: List[str]
         :param aggregations: List of Lists containing the aggregations required, defaults to None. In case of None, the summing matrix will only contain (i) the summation vector for the total series (i.e. a row vector of ones of length n_bottom_series), and (ii) the summation matrix for the bottom level series (i.e. the identity matrix for the amount of bottom level time series). Hence, in the case of None, the output df_S will have shape [n_bottom_series + 1, n_bottom_series]
-        :type df: List[List[str]]
+        :type aggregations: List[List[str]]
         :param sparse: Boolean to indicate whether the returned summing matrix should be backed by a SparseArray (True) or a regular Numpy array (False), defaults to False.
         :type sparse: bool
         :param name_bottom_timeseries: name for the bottom level time series in the hierarchy, defaults to 'bottom_timeseries'.
         :type name_bottom_timeseries: str
         
         :return: df_S, output dataframe containing the summing matrix of shape [(n_bottom_timeseries + n_aggregate_timeseries) x n_bottom_timeseries]. The number of aggregate time series is the result of applying all the required aggregations.
         :rtype: pd.DataFrame filled with np.float32
     
     """
-    # Set aggregations to empty list in case it is not provided
-    if aggregations is None:
-        aggregations = []
-    # Check whether aggregations are in the aggregation_cols
-    aggregation_cols_in_aggregations = list(set([col for cols in aggregations for col in cols]))
+    print("'calc_summing_matrix' is deprecated. Please use hierarchy_cross_sectional to compute cross-sectional hierarchies")
+
+    return None
+
+def hierarchy_cross_sectional(df: pd.DataFrame, aggregations: List[List[str]], 
+                        sparse: bool = False, name_bottom_timeseries: str = 'bottom_timeseries') -> pd.DataFrame:
+    """Given a dataframe of timeseries and columns indicating their groupings, this function calculates a cross-sectional hierarchy according to a set of specified aggregations for the time series.
+
+        :param df: DataFrame containing information about time series and their groupings
+        :type df: pd.DataFrame
+        :param aggregations: List of Lists containing the aggregations required. 
+        :type aggregations: List[List[str]]
+        :param sparse: Boolean to indicate whether the returned summing matrix should be backed by a SparseArray (True) or a regular Numpy array (False), defaults to False.
+        :type sparse: bool
+        :param name_bottom_timeseries: name for the bottom level time series in the hierarchy, defaults to 'bottom_timeseries'.
+        :type name_bottom_timeseries: str
+        
+        :return: df_S, output dataframe containing the summing matrix of shape [(n_bottom_timeseries + n_aggregate_timeseries) x n_bottom_timeseries]. The number of aggregate time series is the result of applying all the required aggregations.
+        :rtype: pd.DataFrame filled with np.float32
+    
+    """
+    # Check whether aggregations are in the df
+    aggregation_cols_in_aggregations = list(dict.fromkeys([col for cols in aggregations for col in cols]))
     for col in aggregation_cols_in_aggregations:
-        assert col in aggregation_cols, f"Column {col} in aggregations not present in aggregation_cols"
+        assert col in df.columns, f"Column {col} in aggregations not present in df"
     # Find the unique aggregation columns from the given set of aggregations
-    levels = df[aggregation_cols].drop_duplicates()
-    levels[name_bottom_timeseries] = levels[aggregation_cols].astype(str).agg('-'.join, axis=1)
+    levels = df[aggregation_cols_in_aggregations].drop_duplicates()
+    levels[name_bottom_timeseries] = levels[aggregation_cols_in_aggregations].astype(str).agg('-'.join, axis=1)
     levels = levels.sort_values(by=name_bottom_timeseries).reset_index(drop=True)
     n_bottom_timeseries = len(levels)
-    aggregations += [[name_bottom_timeseries]]
+    aggregations_total = aggregations + [[name_bottom_timeseries]]
     # Create summing matrix for all aggregation levels
     ones = np.ones(n_bottom_timeseries, dtype=np.float32)
     idx_range = np.arange(n_bottom_timeseries)
     df_S_aggs = []
     # Create summing matrix (=row vector) for top level (=total) series
     df_S_top = pd.DataFrame(ones[None, :], index=['Total'])
     df_S_top = pd.concat({'Total': df_S_top}, names=['Aggregation', 'Value'])
     df_S_aggs.append(df_S_top)
-    for aggregation in aggregations:
+    for aggregation in aggregations_total:
         aggregation_name = '-'.join(aggregation)
         agg = pd.Categorical(levels[aggregation].astype(str).agg('-'.join, axis=1))
         S_agg_sp = coo_matrix((ones, (agg.codes, idx_range)))        
         if sparse:
             S_agg = pd.DataFrame.sparse.from_spmatrix(S_agg_sp, index=agg.categories)    
         else:
             S_agg = pd.DataFrame(S_agg_sp.todense(), index=agg.categories)
@@ -239,14 +258,62 @@
     
     # Stack all summing matrices: top, aggregations, bottom
     df_S = pd.concat(df_S_aggs)
     df_S.columns = levels[name_bottom_timeseries]
 
     return df_S
 
+def hierarchy_temporal(df: pd.DataFrame, time_column: str, aggregations: List[List[str]], sparse: bool = False) -> pd.DataFrame:
+    """Given a dataframe of timeseries and a time_column indicating the timestamp of each series, this function calculates a temporal hierarchy according to a set of specified aggregations for the time series.
+
+        :param df: DataFrame containing information about time series and their groupings
+        :type df: pd.DataFrame
+        :param time_column: String containing the column name that contains the time column of the timeseries 
+        :type time_column: str
+        :param aggregations: List of Lists containing the aggregations required. 
+        :type aggregations: List[List[str]]
+        :param sparse: Boolean to indicate whether the returned summing matrix should be backed by a SparseArray (True) or a regular Numpy array (False), defaults to False.
+        :type sparse: bool
+        
+        :return: df_S, output dataframe containing a summing matrix of shape [n_timesteps x (n_timesteps + n_aggregate_timesteps)]. The number of aggregate timesteps is the result of applying all the required temporal aggregations.
+        :rtype: pd.DataFrame filled with np.float32
+    
+    """
+    assert time_column in df.columns, "The time_column is not a column in the dataframe"
+    assert is_datetime(df[time_column]), "The time_column should be a datetime64-dtype. Use `pd.to_datetime` to convert objects to the correct datetime format."
+    # Check whether aggregations are in the df
+    aggregation_cols_in_aggregations = list(dict.fromkeys([col for cols in aggregations for col in cols]))
+    for col in aggregation_cols_in_aggregations:
+        assert col in df.columns, f"Column {col} in aggregations not present in df"
+    # Find the unique aggregation columns from the given set of aggregations
+    levels = df[aggregation_cols_in_aggregations + [time_column]].drop_duplicates()
+    levels = levels.sort_values(by=time_column).reset_index(drop=True)
+    n_bottom_timestamps = len(levels)
+    aggregations_total = aggregations + [[time_column]]
+    # Create summing matrix for all aggregation levels
+    ones = np.ones(n_bottom_timestamps, dtype=np.float32)
+    idx_range = np.arange(n_bottom_timestamps)
+    df_S_aggs = []
+    for aggregation in aggregations_total:
+        aggregation_name = '-'.join(aggregation)
+        agg = pd.Categorical(levels[aggregation].astype(str).agg('-'.join, axis=1))
+        S_agg_sp = coo_matrix((ones, (agg.codes, idx_range)))        
+        if sparse:
+            S_agg = pd.DataFrame.sparse.from_spmatrix(S_agg_sp, index=agg.categories)    
+        else:
+            S_agg = pd.DataFrame(S_agg_sp.todense(), index=agg.categories)
+        S_agg = pd.concat({f'{aggregation_name}': S_agg}, names=['Aggregation', 'Value'])
+        df_S_aggs.append(S_agg)
+    
+    # Stack all summing matrices: aggregations, bottom
+    df_S = pd.concat(df_S_aggs)
+    df_S.columns = levels[time_column]
+
+    return df_S
+
 def apply_reconciliation_methods(forecasts: pd.DataFrame, df_S: pd.DataFrame, y_train: pd.DataFrame,
                                 yhat_train: pd.DataFrame, methods: List[str] = None, 
                                 positive: bool = False, return_timing: bool = False) -> pd.DataFrame:
     """Apply all hierarchical forecasting reconciliation methods to a set of forecasts.
 
         :param forecasts: dataframe containing forecasts for all aggregations
         :type forecasts: pd.DataFrame
```

### Comparing `hierts-0.6/src/hierts.egg-info/PKG-INFO` & `hierts-0.7/src/hierts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.6
+Version: 0.7
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

