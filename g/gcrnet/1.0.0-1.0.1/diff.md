# Comparing `tmp/gcrnet-1.0.0.tar.gz` & `tmp/gcrnet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gcrnet-1.0.0.tar", last modified: Mon Jul  3 14:59:01 2023, max compression
+gzip compressed data, was "dist\gcrnet-1.0.1.tar", last modified: Tue Jul  4 14:33:28 2023, max compression
```

## Comparing `gcrnet-1.0.0.tar` & `gcrnet-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:01.331373 gcrnet-1.0.0/
--rw-rw-rw-   0        0        0     1084 2023-06-26 18:33:53.000000 gcrnet-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       88 2023-07-03 12:42:46.000000 gcrnet-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1271 2023-07-03 14:59:01.330403 gcrnet-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      948 2023-07-03 12:42:46.000000 gcrnet-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:01.245564 gcrnet-1.0.0/gcrnet/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:19:54.000000 gcrnet-1.0.0/gcrnet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:01.322385 gcrnet-1.0.0/gcrnet/__pycache__/
--rw-rw-rw-   0        0        0      169 2023-06-17 13:50:00.000000 gcrnet-1.0.0/gcrnet/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1647 2023-06-22 12:49:09.000000 gcrnet-1.0.0/gcrnet/__pycache__/base.cpython-38.pyc
--rw-rw-rw-   0        0        0    17271 2023-06-19 19:48:00.000000 gcrnet-1.0.0/gcrnet/__pycache__/crsdnn.cpython-38.pyc
--rw-rw-rw-   0        0        0    12839 2023-07-02 13:48:38.000000 gcrnet-1.0.0/gcrnet/__pycache__/gcrnet.cpython-38.pyc
--rw-rw-rw-   0        0        0    12820 2023-06-26 17:14:55.000000 gcrnet-1.0.0/gcrnet/__pycache__/gcrnn.cpython-38.pyc
--rw-rw-rw-   0        0        0     3014 2023-06-17 13:50:02.000000 gcrnet-1.0.0/gcrnet/__pycache__/io.cpython-38.pyc
--rw-rw-rw-   0        0        0     2226 2023-06-19 20:02:12.000000 gcrnet-1.0.0/gcrnet/__pycache__/layers.cpython-38.pyc
--rw-rw-rw-   0        0        0     1555 2023-06-22 14:49:35.000000 gcrnet-1.0.0/gcrnet/__pycache__/losses.cpython-38.pyc
--rw-rw-rw-   0        0        0     4911 2023-06-17 13:50:02.000000 gcrnet-1.0.0/gcrnet/__pycache__/matching.cpython-38.pyc
--rw-rw-rw-   0        0        0     1442 2023-06-22 15:45:30.000000 gcrnet-1.0.0/gcrnet/__pycache__/meter.cpython-38.pyc
--rw-rw-rw-   0        0        0     1418 2023-06-22 15:52:03.000000 gcrnet-1.0.0/gcrnet/__pycache__/meters.cpython-38.pyc
--rw-rw-rw-   0        0        0     1627 2023-07-02 13:48:40.000000 gcrnet-1.0.0/gcrnet/__pycache__/mlp.cpython-38.pyc
--rw-rw-rw-   0        0        0     5659 2023-07-02 13:48:40.000000 gcrnet-1.0.0/gcrnet/__pycache__/models.cpython-38.pyc
--rw-rw-rw-   0        0        0     3803 2023-06-22 14:49:36.000000 gcrnet-1.0.0/gcrnet/__pycache__/penalty.cpython-38.pyc
--rw-rw-rw-   0        0        0     1109 2023-06-06 16:19:54.000000 gcrnet-1.0.0/gcrnet/__pycache__/simulate_data.cpython-38.pyc
--rw-rw-rw-   0        0        0    10789 2023-06-22 17:09:25.000000 gcrnet-1.0.0/gcrnet/__pycache__/utils.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:01.327395 gcrnet-1.0.0/gcrnet/datasets/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:19:54.000000 gcrnet-1.0.0/gcrnet/datasets/__init__.py
--rw-rw-rw-   0        0        0    21643 2023-07-03 14:51:59.000000 gcrnet-1.0.0/gcrnet/gcrnet.py
--rw-rw-rw-   0        0        0     1697 2023-06-22 14:44:51.000000 gcrnet-1.0.0/gcrnet/losses.py
--rw-rw-rw-   0        0        0     1347 2023-07-02 13:47:35.000000 gcrnet-1.0.0/gcrnet/mlp.py
--rw-rw-rw-   0        0        0     6649 2023-07-02 13:47:35.000000 gcrnet-1.0.0/gcrnet/models.py
--rw-rw-rw-   0        0        0     3759 2023-06-22 14:48:49.000000 gcrnet-1.0.0/gcrnet/penalty.py
--rw-rw-rw-   0        0        0     9631 2023-06-22 17:09:16.000000 gcrnet-1.0.0/gcrnet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:01.259944 gcrnet-1.0.0/gcrnet.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-07-03 14:59:00.000000 gcrnet-1.0.0/gcrnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2023-07-03 14:59:01.000000 gcrnet-1.0.0/gcrnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:59:00.000000 gcrnet-1.0.0/gcrnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-03 14:59:00.000000 gcrnet-1.0.0/gcrnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 14:59:00.000000 gcrnet-1.0.0/gcrnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       77 2023-07-03 12:42:46.000000 gcrnet-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:59:01.332370 gcrnet-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-07-03 12:52:45.000000 gcrnet-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:33:28.557397 gcrnet-1.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-06-26 18:33:53.000000 gcrnet-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:42:46.000000 gcrnet-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1532 2023-07-04 14:33:28.556261 gcrnet-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2023-07-04 14:25:43.000000 gcrnet-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 14:33:28.497398 gcrnet-1.0.1/gcrnet/
+-rw-rw-rw-   0        0        0       26 2023-07-04 14:12:17.000000 gcrnet-1.0.1/gcrnet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:33:28.551256 gcrnet-1.0.1/gcrnet/__pycache__/
+-rw-rw-rw-   0        0        0      169 2023-06-17 13:50:00.000000 gcrnet-1.0.1/gcrnet/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1647 2023-06-22 12:49:09.000000 gcrnet-1.0.1/gcrnet/__pycache__/base.cpython-38.pyc
+-rw-rw-rw-   0        0        0    17271 2023-06-19 19:48:00.000000 gcrnet-1.0.1/gcrnet/__pycache__/crsdnn.cpython-38.pyc
+-rw-rw-rw-   0        0        0    12839 2023-07-02 13:48:38.000000 gcrnet-1.0.1/gcrnet/__pycache__/gcrnet.cpython-38.pyc
+-rw-rw-rw-   0        0        0    12820 2023-06-26 17:14:55.000000 gcrnet-1.0.1/gcrnet/__pycache__/gcrnn.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3014 2023-06-17 13:50:02.000000 gcrnet-1.0.1/gcrnet/__pycache__/io.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2226 2023-06-19 20:02:12.000000 gcrnet-1.0.1/gcrnet/__pycache__/layers.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1555 2023-06-22 14:49:35.000000 gcrnet-1.0.1/gcrnet/__pycache__/losses.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4911 2023-06-17 13:50:02.000000 gcrnet-1.0.1/gcrnet/__pycache__/matching.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1442 2023-06-22 15:45:30.000000 gcrnet-1.0.1/gcrnet/__pycache__/meter.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1418 2023-06-22 15:52:03.000000 gcrnet-1.0.1/gcrnet/__pycache__/meters.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1627 2023-07-02 13:48:40.000000 gcrnet-1.0.1/gcrnet/__pycache__/mlp.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5659 2023-07-02 13:48:40.000000 gcrnet-1.0.1/gcrnet/__pycache__/models.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3803 2023-06-22 14:49:36.000000 gcrnet-1.0.1/gcrnet/__pycache__/penalty.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1109 2023-06-06 16:19:54.000000 gcrnet-1.0.1/gcrnet/__pycache__/simulate_data.cpython-38.pyc
+-rw-rw-rw-   0        0        0    10789 2023-06-22 17:09:25.000000 gcrnet-1.0.1/gcrnet/__pycache__/utils.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-07-04 14:33:28.553554 gcrnet-1.0.1/gcrnet/datasets/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:19:54.000000 gcrnet-1.0.1/gcrnet/datasets/__init__.py
+-rw-rw-rw-   0        0        0    21643 2023-07-03 14:51:59.000000 gcrnet-1.0.1/gcrnet/gcrnet.py
+-rw-rw-rw-   0        0        0     1697 2023-06-22 14:44:51.000000 gcrnet-1.0.1/gcrnet/losses.py
+-rw-rw-rw-   0        0        0     1347 2023-07-02 13:47:35.000000 gcrnet-1.0.1/gcrnet/mlp.py
+-rw-rw-rw-   0        0        0     6649 2023-07-02 13:47:35.000000 gcrnet-1.0.1/gcrnet/models.py
+-rw-rw-rw-   0        0        0     3759 2023-06-22 14:48:49.000000 gcrnet-1.0.1/gcrnet/penalty.py
+-rw-rw-rw-   0        0        0     9631 2023-06-22 17:09:16.000000 gcrnet-1.0.1/gcrnet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:33:28.508371 gcrnet-1.0.1/gcrnet.egg-info/
+-rw-rw-rw-   0        0        0     1532 2023-07-04 14:33:28.000000 gcrnet-1.0.1/gcrnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2023-07-04 14:33:28.000000 gcrnet-1.0.1/gcrnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:33:28.000000 gcrnet-1.0.1/gcrnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-04 14:33:28.000000 gcrnet-1.0.1/gcrnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 14:33:28.000000 gcrnet-1.0.1/gcrnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       77 2023-07-03 12:42:46.000000 gcrnet-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 14:33:28.558237 gcrnet-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-07-04 14:33:22.000000 gcrnet-1.0.1/setup.py
```

### Comparing `gcrnet-1.0.0/LICENSE` & `gcrnet-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/PKG-INFO` & `gcrnet-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 Metadata-Version: 2.1
 Name: gcrnet
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for sparse-input neural networks using group concave regularization
-Home-page: UNKNOWN
 Author: Bin Luo
 Author-email: bin.luo2@duke.edu
 License: MIT
-Description: # GCRNet: Sparse-Input Neural Networks with Group Concave Regularization
-        
-        GCRNet is a Python library that implements a novel framework for sparse-input neural networks using group concave regularization. Leveraging the power of concave penalties, specifically MCP and SCAD, GCRNet provides a comprehensive approach for simultaneous feature selection and non-linear function estimation. The proposed framework considers all outgoing connections from a single input neuron as a group and applies an appropriate concave penalty to the $l_2$ norm of weights within each group. By selectively shrinking the weights of certain groups to exact zeros, GCRNet constructs a neural network that utilizes only a small subset of variables, enhancing both the accuracy and interpretability of the feature selection process. GCRNet offers versatile functionality, supporting regression or classification tasks with continuous, binary, or time-to-event outcomes.
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GCRNet: Sparse-Input Neural Networks with Group Concave Regularization
+
+GCRNet is a Python library that implements a novel framework for sparse-input neural networks using group concave regularization. Leveraging the power of concave penalties, specifically MCP and SCAD, GCRNet provides a comprehensive approach for simultaneous feature selection and non-linear function estimation. The proposed framework considers all outgoing connections from a single input neuron as a group and applies an appropriate concave penalty to the $l_2$ norm of weights within each group. By selectively shrinking the weights of certain groups to exact zeros, GCRNet constructs a neural network that utilizes only a small subset of variables, enhancing both the accuracy and interpretability of the feature selection process. GCRNet offers versatile functionality, supporting regression or classification tasks with continuous, binary, or time-to-event outcomes.
+
+### Installation
+
+#### Installation with pip
+
+To install with `pip`, run the following command:
+```
+pip install --user gcrnet
+```
+
+#### Installation from GitHub
+
+You can also clone the repository and install manually:
+```
+git clone 
+cd gcrnet/python
+python setup.py install --user
+```
```

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/base.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/crsdnn.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/crsdnn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/gcrnet.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/gcrnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/gcrnn.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/gcrnn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/io.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/io.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/layers.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/layers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/losses.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/losses.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/matching.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/matching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/meter.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/meter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/meters.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/meters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/mlp.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/mlp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/models.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/penalty.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/penalty.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/simulate_data.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/simulate_data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/__pycache__/utils.cpython-38.pyc` & `gcrnet-1.0.1/gcrnet/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/gcrnet.py` & `gcrnet-1.0.1/gcrnet/gcrnet.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/losses.py` & `gcrnet-1.0.1/gcrnet/losses.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/mlp.py` & `gcrnet-1.0.1/gcrnet/mlp.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/models.py` & `gcrnet-1.0.1/gcrnet/models.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/penalty.py` & `gcrnet-1.0.1/gcrnet/penalty.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet/utils.py` & `gcrnet-1.0.1/gcrnet/utils.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/gcrnet.egg-info/PKG-INFO` & `gcrnet-1.0.1/gcrnet.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 Metadata-Version: 2.1
 Name: gcrnet
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for sparse-input neural networks using group concave regularization
-Home-page: UNKNOWN
 Author: Bin Luo
 Author-email: bin.luo2@duke.edu
 License: MIT
-Description: # GCRNet: Sparse-Input Neural Networks with Group Concave Regularization
-        
-        GCRNet is a Python library that implements a novel framework for sparse-input neural networks using group concave regularization. Leveraging the power of concave penalties, specifically MCP and SCAD, GCRNet provides a comprehensive approach for simultaneous feature selection and non-linear function estimation. The proposed framework considers all outgoing connections from a single input neuron as a group and applies an appropriate concave penalty to the $l_2$ norm of weights within each group. By selectively shrinking the weights of certain groups to exact zeros, GCRNet constructs a neural network that utilizes only a small subset of variables, enhancing both the accuracy and interpretability of the feature selection process. GCRNet offers versatile functionality, supporting regression or classification tasks with continuous, binary, or time-to-event outcomes.
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GCRNet: Sparse-Input Neural Networks with Group Concave Regularization
+
+GCRNet is a Python library that implements a novel framework for sparse-input neural networks using group concave regularization. Leveraging the power of concave penalties, specifically MCP and SCAD, GCRNet provides a comprehensive approach for simultaneous feature selection and non-linear function estimation. The proposed framework considers all outgoing connections from a single input neuron as a group and applies an appropriate concave penalty to the $l_2$ norm of weights within each group. By selectively shrinking the weights of certain groups to exact zeros, GCRNet constructs a neural network that utilizes only a small subset of variables, enhancing both the accuracy and interpretability of the feature selection process. GCRNet offers versatile functionality, supporting regression or classification tasks with continuous, binary, or time-to-event outcomes.
+
+### Installation
+
+#### Installation with pip
+
+To install with `pip`, run the following command:
+```
+pip install --user gcrnet
+```
+
+#### Installation from GitHub
+
+You can also clone the repository and install manually:
+```
+git clone 
+cd gcrnet/python
+python setup.py install --user
+```
```

### Comparing `gcrnet-1.0.0/gcrnet.egg-info/SOURCES.txt` & `gcrnet-1.0.1/gcrnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.0/setup.py` & `gcrnet-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='gcrnet',
-      version='1.0.0',
+      version='1.0.1',
       author="Bin Luo",
       author_email="bin.luo2@duke.edu",
       description="A Python library for sparse-input neural networks using group concave regularization",
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='MIT',
       packages=['gcrnet'],
```

