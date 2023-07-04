# Comparing `tmp/hotspell-0.1.3.tar.gz` & `tmp/hotspell-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotspell-0.1.3.tar", last modified: Sat Oct 22 18:34:38 2022, max compression
+gzip compressed data, was "hotspell-0.1.4.tar", last modified: Tue Jul  4 11:03:57 2023, max compression
```

## Comparing `hotspell-0.1.3.tar` & `hotspell-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2022-10-22 18:34:38.719414 hotspell-0.1.3/
--rw-r--r--   0 ilias     (1000) ilias     (1000)     1557 2021-05-13 12:57:40.000000 hotspell-0.1.3/LICENSE
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     3468 2022-10-22 18:34:38.719414 hotspell-0.1.3/PKG-INFO
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     2362 2021-09-24 15:19:25.000000 hotspell-0.1.3/README.rst
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2022-10-22 18:34:38.719414 hotspell-0.1.3/hotspell/
--rw-rw-r--   0 ilias     (1000) ilias     (1000)       64 2021-08-13 06:22:04.000000 hotspell-0.1.3/hotspell/__init__.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)    11793 2022-10-22 18:13:48.000000 hotspell-0.1.3/hotspell/heatwaves.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     5692 2022-10-22 18:30:31.000000 hotspell-0.1.3/hotspell/indices.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     3291 2022-10-22 18:20:02.000000 hotspell-0.1.3/hotspell/metrics.py
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     2770 2022-10-22 18:28:35.000000 hotspell-0.1.3/hotspell/utils.py
-drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2022-10-22 18:34:38.719414 hotspell-0.1.3/hotspell.egg-info/
--rw-rw-r--   0 ilias     (1000) ilias     (1000)     3468 2022-10-22 18:34:38.000000 hotspell-0.1.3/hotspell.egg-info/PKG-INFO
--rw-rw-r--   0 ilias     (1000) ilias     (1000)      287 2022-10-22 18:34:38.000000 hotspell-0.1.3/hotspell.egg-info/SOURCES.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)        1 2022-10-22 18:34:38.000000 hotspell-0.1.3/hotspell.egg-info/dependency_links.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)       13 2022-10-22 18:34:38.000000 hotspell-0.1.3/hotspell.egg-info/requires.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)        9 2022-10-22 18:34:38.000000 hotspell-0.1.3/hotspell.egg-info/top_level.txt
--rw-rw-r--   0 ilias     (1000) ilias     (1000)       38 2022-10-22 18:34:38.719414 hotspell-0.1.3/setup.cfg
--rw-r--r--   0 ilias     (1000) ilias     (1000)      623 2022-10-22 18:32:13.000000 hotspell-0.1.3/setup.py
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-07-04 11:03:57.167419 hotspell-0.1.4/
+-rw-r--r--   0 ilias     (1000) ilias     (1000)     1557 2021-05-13 12:57:40.000000 hotspell-0.1.4/LICENSE
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     3468 2023-07-04 11:03:57.167419 hotspell-0.1.4/PKG-INFO
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     2362 2021-09-24 15:19:25.000000 hotspell-0.1.4/README.rst
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-07-04 11:03:57.163419 hotspell-0.1.4/hotspell/
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)       64 2021-08-13 06:22:04.000000 hotspell-0.1.4/hotspell/__init__.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)    11793 2022-10-22 18:13:48.000000 hotspell-0.1.4/hotspell/heatwaves.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     5692 2022-10-22 18:30:31.000000 hotspell-0.1.4/hotspell/indices.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     3291 2022-10-22 18:20:02.000000 hotspell-0.1.4/hotspell/metrics.py
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     2818 2023-07-01 18:42:13.000000 hotspell-0.1.4/hotspell/utils.py
+drwxrwxr-x   0 ilias     (1000) ilias     (1000)        0 2023-07-04 11:03:57.167419 hotspell-0.1.4/hotspell.egg-info/
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)     3468 2023-07-04 11:03:57.000000 hotspell-0.1.4/hotspell.egg-info/PKG-INFO
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)      287 2023-07-04 11:03:57.000000 hotspell-0.1.4/hotspell.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)        1 2023-07-04 11:03:57.000000 hotspell-0.1.4/hotspell.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)       13 2023-07-04 11:03:57.000000 hotspell-0.1.4/hotspell.egg-info/requires.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)        9 2023-07-04 11:03:57.000000 hotspell-0.1.4/hotspell.egg-info/top_level.txt
+-rw-rw-r--   0 ilias     (1000) ilias     (1000)       38 2023-07-04 11:03:57.167419 hotspell-0.1.4/setup.cfg
+-rw-r--r--   0 ilias     (1000) ilias     (1000)      623 2023-07-04 11:00:51.000000 hotspell-0.1.4/setup.py
```

### Comparing `hotspell-0.1.3/LICENSE` & `hotspell-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.3/PKG-INFO` & `hotspell-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotspell
-Version: 0.1.3
+Version: 0.1.4
 Summary: Detect heat waves from weather station data
 Home-page: https://github.com/agathangelidis/hotspell
 Author: Ilias Agathangelidis
 License: UNKNOWN
 Description: """"""""
         hotspell
         """"""""
```

### Comparing `hotspell-0.1.3/README.rst` & `hotspell-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.3/hotspell/heatwaves.py` & `hotspell-0.1.4/hotspell/heatwaves.py`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.3/hotspell/indices.py` & `hotspell-0.1.4/hotspell/indices.py`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.3/hotspell/metrics.py` & `hotspell-0.1.4/hotspell/metrics.py`

 * *Files identical despite different names*

### Comparing `hotspell-0.1.3/hotspell/utils.py` & `hotspell-0.1.4/hotspell/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from calendar import monthrange
 from datetime import date
 
 import numpy as np
 import pandas as pd
 
 
 def _compute_overall_mean(timeseries, summer_months):
@@ -66,18 +67,17 @@
 
 def _percent_of_days_to_days(days_percent, summer_months):
     if summer_months:
         months = list(summer_months)
     else:
         months = [*range(1, 13)]
     if summer_months:
-        days = np.ceil(
-            (days_percent * 0.01)
-            * ((date(2020, months[-1] + 1, 1) - date(2020, months[0], 1)).days)
-        )
+        number_of_summer_days = np.sum(
+            [monthrange(2020, month)[-1] for month in months])
+        days = (days_percent * 0.01) * number_of_summer_days
     else:
         days = (days_percent * 0.01) * 365
     return days
 
 
 def _preprocess_data(df, var, years):
     if var == "tmax":
```

### Comparing `hotspell-0.1.3/hotspell.egg-info/PKG-INFO` & `hotspell-0.1.4/hotspell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotspell
-Version: 0.1.3
+Version: 0.1.4
 Summary: Detect heat waves from weather station data
 Home-page: https://github.com/agathangelidis/hotspell
 Author: Ilias Agathangelidis
 License: UNKNOWN
 Description: """"""""
         hotspell
         """"""""
```

### Comparing `hotspell-0.1.3/setup.py` & `hotspell-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="hotspell",
-    version="0.1.3",
+    version="0.1.4",
     description="Detect heat waves from weather station data",
     author="Ilias Agathangelidis",
     packages=["hotspell"],
     package_data={"hotspell": ["datasets/*.pickle"]},
     install_requires=["numpy", "pandas"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
```

