# Comparing `tmp/InterpretME-1.3.1.tar.gz` & `tmp/InterpretME-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InterpretME-1.3.1.tar", last modified: Mon Jul  3 13:36:49 2023, max compression
+gzip compressed data, was "InterpretME-1.3.2.tar", last modified: Tue Jul  4 08:30:26 2023, max compression
```

## Comparing `InterpretME-1.3.1.tar` & `InterpretME-1.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:36:49.377261 InterpretME-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:36:49.373261 InterpretME-1.3.1/InterpretME/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/dtreeviz_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/federated_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:36:49.377261 InterpretME-1.3.1/InterpretME/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/classes.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/cross_validation.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/definition_feature.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/endpoint.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/entity_alignment.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/imp_features.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/lime_features.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/model_details.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/precision_recall.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/prediction_probabilities.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/sampling_strategy.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/mappings/shacl_validation_results.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/preprocessing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/sampling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/semantification.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/shacl_api_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 13:36:37.000000 InterpretME-1.3.1/InterpretME/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:36:49.373261 InterpretME-1.3.1/InterpretME.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-03 13:36:49.000000 InterpretME-1.3.1/InterpretME.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 13:36:49.000000 InterpretME-1.3.1/InterpretME.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:36:49.000000 InterpretME-1.3.1/InterpretME.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-03 13:36:49.000000 InterpretME-1.3.1/InterpretME.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 13:36:49.000000 InterpretME-1.3.1/InterpretME.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-03 13:36:37.000000 InterpretME-1.3.1/LIBRARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 13:36:37.000000 InterpretME-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 13:36:37.000000 InterpretME-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-03 13:36:49.377261 InterpretME-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-03 13:36:37.000000 InterpretME-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:36:49.377261 InterpretME-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-03 13:36:37.000000 InterpretME-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:30:26.108497 InterpretME-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:30:26.104498 InterpretME-1.3.2/InterpretME/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/dtreeviz_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/federated_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:30:26.108497 InterpretME-1.3.2/InterpretME/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/classes.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/cross_validation.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/definition_feature.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/endpoint.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/entity_alignment.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/imp_features.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/lime_features.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/model_details.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/precision_recall.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/prediction_probabilities.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/sampling_strategy.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/mappings/shacl_validation_results.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/preprocessing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/sampling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/semantification.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/shacl_api_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-04 08:30:15.000000 InterpretME-1.3.2/InterpretME/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:30:26.104498 InterpretME-1.3.2/InterpretME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-04 08:30:26.000000 InterpretME-1.3.2/InterpretME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-04 08:30:26.000000 InterpretME-1.3.2/InterpretME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:30:26.000000 InterpretME-1.3.2/InterpretME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-04 08:30:26.000000 InterpretME-1.3.2/InterpretME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 08:30:26.000000 InterpretME-1.3.2/InterpretME.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-04 08:30:15.000000 InterpretME-1.3.2/LIBRARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-04 08:30:15.000000 InterpretME-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-04 08:30:15.000000 InterpretME-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-04 08:30:26.108497 InterpretME-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-04 08:30:15.000000 InterpretME-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:30:26.108497 InterpretME-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 08:30:15.000000 InterpretME-1.3.2/setup.py
```

### Comparing `InterpretME-1.3.1/InterpretME/classification.py` & `InterpretME-1.3.2/InterpretME/classification.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/dtreeviz_lib.py` & `InterpretME-1.3.2/InterpretME/dtreeviz_lib.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/federated_query_engine.py` & `InterpretME-1.3.2/InterpretME/federated_query_engine.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/classes.ttl` & `InterpretME-1.3.2/InterpretME/mappings/classes.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/cross_validation.ttl` & `InterpretME-1.3.2/InterpretME/mappings/cross_validation.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/definition_feature.ttl` & `InterpretME-1.3.2/InterpretME/mappings/definition_feature.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/endpoint.ttl` & `InterpretME-1.3.2/InterpretME/mappings/endpoint.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/entity_alignment.ttl` & `InterpretME-1.3.2/InterpretME/mappings/entity_alignment.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/imp_features.ttl` & `InterpretME-1.3.2/InterpretME/mappings/imp_features.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/lime_features.ttl` & `InterpretME-1.3.2/InterpretME/mappings/lime_features.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/model_details.ttl` & `InterpretME-1.3.2/InterpretME/mappings/model_details.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/precision_recall.ttl` & `InterpretME-1.3.2/InterpretME/mappings/precision_recall.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/prediction_probabilities.ttl` & `InterpretME-1.3.2/InterpretME/mappings/prediction_probabilities.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/sampling_strategy.ttl` & `InterpretME-1.3.2/InterpretME/mappings/sampling_strategy.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/mappings/shacl_validation_results.ttl` & `InterpretME-1.3.2/InterpretME/mappings/shacl_validation_results.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/pipeline.py` & `InterpretME-1.3.2/InterpretME/pipeline.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/plots.py` & `InterpretME-1.3.2/InterpretME/plots.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/preprocessing_data.py` & `InterpretME-1.3.2/InterpretME/preprocessing_data.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/sampling_strategy.py` & `InterpretME-1.3.2/InterpretME/sampling_strategy.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/semantification.py` & `InterpretME-1.3.2/InterpretME/semantification.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/upload.py` & `InterpretME-1.3.2/InterpretME/upload.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME/utils.py` & `InterpretME-1.3.2/InterpretME/utils.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/InterpretME.egg-info/PKG-INFO` & `InterpretME-1.3.2/InterpretME.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: InterpretME
-Version: 1.3.1
+Version: 1.3.2
 Summary: An interpretable machine learning pipeline over knowledge graphs
 Home-page: https://github.com/SDM-TIB/InterpretME
-Download-URL: https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v1.3.1.tar.gz
+Download-URL: https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v1.3.2.tar.gz
 Author: Yashraj Chudasama, Disha Purohit, Philipp Rohde, Julian Gercke
 Author-email: yashraj.chudasama@tib.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
```

### Comparing `InterpretME-1.3.1/InterpretME.egg-info/SOURCES.txt` & `InterpretME-1.3.2/InterpretME.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/LIBRARY.md` & `InterpretME-1.3.2/LIBRARY.md`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/LICENSE` & `InterpretME-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/PKG-INFO` & `InterpretME-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: InterpretME
-Version: 1.3.1
+Version: 1.3.2
 Summary: An interpretable machine learning pipeline over knowledge graphs
 Home-page: https://github.com/SDM-TIB/InterpretME
-Download-URL: https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v1.3.1.tar.gz
+Download-URL: https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v1.3.2.tar.gz
 Author: Yashraj Chudasama, Disha Purohit, Philipp Rohde, Julian Gercke
 Author-email: yashraj.chudasama@tib.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
```

### Comparing `InterpretME-1.3.1/README.md` & `InterpretME-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `InterpretME-1.3.1/setup.py` & `InterpretME-1.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("LIBRARY.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
-VERSION = '1.3.1'
+VERSION = '1.3.2'
 
 setup(
     name='InterpretME',
     packages=['InterpretME'],
     version=VERSION,
     description='An interpretable machine learning pipeline over knowledge graphs',
     long_description=long_description,
@@ -43,10 +43,10 @@
         'dtreeviz>=2.2.0',
         'python-slugify>=6.0.0',
         'requests>=2.31.0',
         'rdfizer>=4.5.5',
         'DeTrusty>=0.12.3',
         'validating-models>=0.9.5',
         'optuna>=3.2.0',
-        'scikit-learn>=1.2.0'
+        'scikit-learn>=1.2.0,<1.3.0'
     ]
 )
```

