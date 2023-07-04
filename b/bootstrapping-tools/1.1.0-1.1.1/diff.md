# Comparing `tmp/bootstrapping_tools-1.1.0.tar.gz` & `tmp/bootstrapping_tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrapping_tools-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bootstrapping_tools-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bootstrapping_tools-1.1.0.tar` & `bootstrapping_tools-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      200 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/README.md
--rw-r--r--   0        0        0      137 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/bootstrapping_tools/__init__.py
--rw-r--r--   0        0        0    11784 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/bootstrapping_tools/bootstrapping.py
--rw-r--r--   0        0        0      859 2023-07-03 18:18:07.782256 bootstrapping_tools-1.1.0/bootstrapping_tools/resample_by_blocks.py
--rw-r--r--   0        0        0      516 2023-07-03 18:18:07.786256 bootstrapping_tools-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/README.md
+-rw-r--r--   0        0        0      137 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/bootstrapping_tools/__init__.py
+-rw-r--r--   0        0        0    11811 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/bootstrapping_tools/bootstrapping.py
+-rw-r--r--   0        0        0      859 2023-07-03 19:10:59.600443 bootstrapping_tools-1.1.1/bootstrapping_tools/resample_by_blocks.py
+-rw-r--r--   0        0        0      516 2023-07-03 19:10:59.604443 bootstrapping_tools-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-1.1.1/PKG-INFO
```

### Comparing `bootstrapping_tools-1.1.0/bootstrapping_tools/bootstrapping.py` & `bootstrapping_tools-1.1.1/bootstrapping_tools/bootstrapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,16 +214,16 @@
 def resample_data(dataframe, seed, blocks_length):
     rng = random.Random(seed)
     return random_resample_data_by_blocks(dataframe, blocks_length, rng)
 
 
 def resample_and_shift_data(dataframe, seed, blocks_length):
     resampled_data = resample_data(dataframe, seed, blocks_length)
-    min_season = dataframe.iloc[:, 0].min()
-    resampled_data.iloc[:, 0] = resampled_data.iloc[:, 0] - min_season
+    min_season = dataframe.loc[:, "Temporada"].min()
+    resampled_data.loc[:, "Temporada"] = resampled_data.loc[:, "Temporada"] - min_season
     return resampled_data
 
 
 def calculate_intervals_from_p_values_and_alpha(distribution, p_values, alpha):
     limits = calculate_limits_from_p_values_and_alpha(p_values, alpha)
     return _calculate_intevals(distribution, limits)
```

### Comparing `bootstrapping_tools-1.1.0/bootstrapping_tools/resample_by_blocks.py` & `bootstrapping_tools-1.1.1/bootstrapping_tools/resample_by_blocks.py`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-1.1.0/pyproject.toml` & `bootstrapping_tools-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-1.1.0/PKG-INFO` & `bootstrapping_tools-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapping_tools
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: bootstrapping_tools Version: 1.1.0 Summary: GECI
+Metadata-Version: 2.1 Name: bootstrapping_tools Version: 1.1.1 Summary: GECI
 Tools for bootstrapping Home-page: https://github.com/IslasGECI/
 bootstrapping_tools Author: Ciencia de Datos â¢ GECI Author-email:
 ciencia.datos@islas.org.mx Requires-Python: >=3 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 or later (GPLv3+) Requires-Dist: numpy Requires-Dist: pandas-stubs Requires-
 Dist: pandas Requires-Dist: scipy Requires-Dist: tqdm [https://
 www.islas.org.mx/img/logo.svg] # Bootstrapping tools GECI tools to perform
```

