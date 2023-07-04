# Comparing `tmp/spectralnet-0.0.6.tar.gz` & `tmp/spectralnet-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.0.6.tar", last modified: Thu Jun 29 19:01:27 2023, max compression
+gzip compressed data, was "spectralnet-0.0.7.tar", last modified: Tue Jul  4 19:55:36 2023, max compression
```

## Comparing `spectralnet-0.0.6.tar` & `spectralnet-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.995085 spectralnet-0.0.6/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-29 14:40:19.000000 spectralnet-0.0.6/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)     2266 2023-06-29 19:01:27.995193 spectralnet-0.0.6/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-29 14:42:02.000000 spectralnet-0.0.6/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-29 14:42:18.000000 spectralnet-0.0.6/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      615 2023-06-29 19:01:27.995505 spectralnet-0.0.6/setup.cfg
--rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-29 14:42:12.000000 spectralnet-0.0.6/setup.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.987843 spectralnet-0.0.6/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.990848 spectralnet-0.0.6/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/__init__.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.992757 spectralnet-0.0.6/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.993615 spectralnet-0.0.6/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_spectral.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.994753 spectralnet-0.0.6/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-06-29 18:46:31.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.992062 spectralnet-0.0.6/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)     2266 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      845 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       18 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/top_level.txt
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.994962 spectralnet-0.0.6/src/tests/
--rw-r--r--   0 amitai     (501) staff       (20)        0 2023-06-29 18:58:30.000000 spectralnet-0.0.6/src/tests/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.091422 spectralnet-0.0.7/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-29 14:40:19.000000 spectralnet-0.0.7/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     2262 2023-07-04 19:55:36.091535 spectralnet-0.0.7/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     1768 2023-07-04 19:51:11.000000 spectralnet-0.0.7/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-29 14:42:18.000000 spectralnet-0.0.7/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      615 2023-07-04 19:55:36.091822 spectralnet-0.0.7/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-29 14:42:12.000000 spectralnet-0.0.7/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.085194 spectralnet-0.0.7/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.087241 spectralnet-0.0.7/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.088620 spectralnet-0.0.7/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.089454 spectralnet-0.0.7/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_spectral.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.091124 spectralnet-0.0.7/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-06-29 18:46:31.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-29 14:41:56.000000 spectralnet-0.0.7/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.088034 spectralnet-0.0.7/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     2262 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      845 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       18 2023-07-04 19:55:36.000000 spectralnet-0.0.7/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-07-04 19:55:36.091315 spectralnet-0.0.7/src/tests/
+-rw-r--r--   0 amitai     (501) staff       (20)        0 2023-06-29 18:58:30.000000 spectralnet-0.0.7/src/tests/__init__.py
```

### Comparing `spectralnet-0.0.6/LICENSE.md` & `spectralnet-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/PKG-INFO` & `spectralnet-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # SpectralNet
 
 <p align="center">
-    <img src="https://github.com/AmitaiYacobi/SpectralNet01/blob/main/figures/twomoons.png">
+    <img src="https://github.com/shaham-lab/SpectralNet/blob/main/figures/twomoons.png">
 
 SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
 This package is based on the following paper - [SpectralNet](https://openreview.net/pdf?id=HJ_aoCyRZ)
 
 ## Installation
 
 You can install the latest package version via
```

### Comparing `spectralnet-0.0.6/README.md` & `spectralnet-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SpectralNet
 
 <p align="center">
-    <img src="https://github.com/AmitaiYacobi/SpectralNet01/blob/main/figures/twomoons.png">
+    <img src="https://github.com/shaham-lab/SpectralNet/blob/main/figures/twomoons.png">
 
 SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
 This package is based on the following paper - [SpectralNet](https://openreview.net/pdf?id=HJ_aoCyRZ)
 
 ## Installation
 
 You can install the latest package version via
```

### Comparing `spectralnet-0.0.6/setup.cfg` & `spectralnet-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spectralnet
-version = 0.0.6
+version = 0.0.7
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shaham-lab/SpectralNet.git
 project_urls = 
 	Bug Tracker = https://github.com/shaham-lab/SpectralNet/issues
```

### Comparing `spectralnet-0.0.6/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.0.7/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.0.7/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_metrics.py` & `spectralnet-0.0.7/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.0.7/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.0.7/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.0.7/src/spectralnet/_models/_spectralnet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_spectral.py` & `spectralnet-0.0.7/src/spectralnet/_spectral.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.0.7/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.0.7/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.0.7/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet/_utils.py` & `spectralnet-0.0.7/src/spectralnet/_utils.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.6/src/spectralnet.egg-info/PKG-INFO` & `spectralnet-0.0.7/src/spectralnet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # SpectralNet
 
 <p align="center">
-    <img src="https://github.com/AmitaiYacobi/SpectralNet01/blob/main/figures/twomoons.png">
+    <img src="https://github.com/shaham-lab/SpectralNet/blob/main/figures/twomoons.png">
 
 SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
 This package is based on the following paper - [SpectralNet](https://openreview.net/pdf?id=HJ_aoCyRZ)
 
 ## Installation
 
 You can install the latest package version via
```

### Comparing `spectralnet-0.0.6/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.0.7/src/spectralnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

