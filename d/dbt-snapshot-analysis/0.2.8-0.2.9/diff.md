# Comparing `tmp/dbt_snapshot_analysis-0.2.8.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.2.8.tar", last modified: Fri Jun 30 10:42:35 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.9.tar", last modified: Mon Jul  3 12:30:10 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.2.8.tar` & `dbt_snapshot_analysis-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-30 10:42:35.122973 dbt_snapshot_analysis-0.2.8/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-30 10:42:35.122832 dbt_snapshot_analysis-0.2.8/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      936 2023-06-26 08:26:25.000000 dbt_snapshot_analysis-0.2.8/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-30 10:42:35.121715 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/data_validation.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)    14423 2023-06-30 10:41:14.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/dbt_snapshot_analysis.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2025 2023-06-26 15:24:40.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/snapshot_utils.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/streamlit_entry_point.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-30 10:42:35.122606 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-30 10:42:35.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-30 10:42:35.123030 dbt_snapshot_analysis-0.2.8/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-06-30 10:41:39.000000 dbt_snapshot_analysis-0.2.8/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 12:30:10.071115 dbt_snapshot_analysis-0.2.9/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1654 2023-07-03 12:30:10.070954 dbt_snapshot_analysis-0.2.9/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1235 2023-07-03 12:29:32.000000 dbt_snapshot_analysis-0.2.9/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 12:30:10.069233 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)    14423 2023-07-03 12:29:32.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2025 2023-06-26 15:24:40.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 12:30:10.070672 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1654 2023-07-03 12:30:09.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-07-03 12:30:09.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 12:30:09.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-07-03 12:30:09.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-07-03 12:30:09.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-07-03 12:30:09.000000 dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 12:30:10.071182 dbt_snapshot_analysis-0.2.9/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-07-03 12:29:46.000000 dbt_snapshot_analysis-0.2.9/setup.py
```

### Comparing `dbt_snapshot_analysis-0.2.8/PKG-INFO` & `dbt_snapshot_analysis-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_snapshot_analysis
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,33 +13,48 @@
 </br>
 <p align="center">
   <a href="https://www.data-drift.io">
     <img src="https://github.com/data-drift/data-drift/blob/main/datadrift-logo.png?raw=true" width="100px" alt="DataDrift logo" />
   </a>
 </p>
 
-<h2 align="center" >A Changelog for Data</h3>
-<p align="center">Git-Based. Data-Consumer-Friendly.</p>
+<h2 align="center" >dbt Snapshot Analysis</h3>
 
 <p align="center"><a href="https://data-drift.io">Website</a> · <a href="https://www.data-drift.io/blog">Blog</a></p>
+</br>
 
-# DBT Snapshot Analysis
+# dbt Snapshot Analysis
 
 [![PyPI version](https://badge.fury.io/py/dbt-snapshot-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis)
 
-This project is developped by the DataDrift team.
+**Analyse the stability of your key metrics**
+</br>
+Changes of a metric’s historical value harms data consumers’ trust.
 
-DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
+dbt Snapshot Analysis is Python package to get insight on the quality and stability of the metrics your report.
 
+</br>
+<p align="center">
+  <a href="https://pypi.org/project/dbt-snapshot-analysis">
+    <img src="dbt-snapshot-analysis.gif" alt="Dat" />
+  </a>
+</p>
+
+
+# 🚀 Quickstart
 ## Installation
 
 You can install DBT Snapshot Analysis using `pip`:
 
 ```sh
 pip install dbt-snapshot-analysis
 ```
 
 ## Usage
 
 ```sh
 dbt_snapshot_analysis
 ```
+
+</br>
+
+This project is developped by the DataDrift team with 💚. Check out our [main repository](https://github.com/data-drift/data-drift).
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_xgr1lo3d_/tmpnitw2ydq_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_xgr1lo3d_/tmpnitw2ydq_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.8 Summary: A
+Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.9 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
-                       ***** A Changelog for Data *****
-                      Git-Based. Data-Consumer-Friendly.
+                       ***** dbt Snapshot Analysis *****
                                 Website Â· Blog
-# DBT Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-snapshot-
-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis) This project is
-developped by the DataDrift team. DBT Snapshot Analysis is a Python package for
-analyzing snapshots. It provides a set of tools for visualizing and exploring
-data in a variety of ways. ## Installation You can install DBT Snapshot
-Analysis using `pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage
-```sh dbt_snapshot_analysis ```
+ # dbt Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-
+snapshot-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis)
+**Analyse the stability of your key metrics**  Changes of a metricâs
+historical value harms data consumersâ trust. dbt Snapshot Analysis is Python
+package to get insight on the quality and stability of the metrics your report.
+                                     [Dat]
+# ð Quickstart ## Installation You can install DBT Snapshot Analysis using
+`pip`: ```sh pip install dbt-snapshot-analysis ``` ## Usage ```sh
+dbt_snapshot_analysis ```  This project is developped by the DataDrift team
+with ð. Check out our [main repository](https://github.com/data-drift/data-
+drift).
```

### Comparing `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/data_validation.py` & `dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/data_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/dbt_snapshot_analysis.py` & `dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/dbt_snapshot_analysis.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/snapshot_utils.py` & `dbt_snapshot_analysis-0.2.9/dbt_snapshot_analysis/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.8/setup.py` & `dbt_snapshot_analysis-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.2.8",
+    version="0.2.9",
     packages=find_packages(),
     py_modules=["dbt_snapshot_analysis"],
     install_requires=["pandas", "plotly", "streamlit"],
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
```

