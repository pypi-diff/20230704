# Comparing `tmp/quik-ai-1.3.0.tar.gz` & `tmp/quik-ai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik-ai-1.3.0.tar", last modified: Sun Jun 25 20:29:58 2023, max compression
+gzip compressed data, was "quik-ai-1.3.1.tar", last modified: Tue Jul  4 16:29:19 2023, max compression
```

## Comparing `quik-ai-1.3.0.tar` & `quik-ai-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 20:29:58.497736 quik-ai-1.3.0/
--rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     2235 2023-06-25 20:29:58.497736 quik-ai-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1697 2023-06-11 13:33:07.000000 quik-ai-1.3.0/README.md
--rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      768 2023-06-25 20:29:58.507712 quik-ai-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:29:58.361446 quik-ai-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 20:29:58.459839 quik-ai-1.3.0/src/quik_ai/
--rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.3.0/src/quik_ai/__init__.py
--rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.3.0/src/quik_ai/backend.py
--rw-rw-rw-   0        0        0    13147 2023-06-24 13:52:15.000000 quik-ai-1.3.0/src/quik_ai/engine.py
--rw-rw-rw-   0        0        0     5387 2023-06-25 15:49:39.000000 quik-ai-1.3.0/src/quik_ai/heads.py
--rw-rw-rw-   0        0        0    20012 2023-06-25 19:52:41.000000 quik-ai-1.3.0/src/quik_ai/layers.py
--rw-rw-rw-   0        0        0      941 2023-06-24 18:02:43.000000 quik-ai-1.3.0/src/quik_ai/losses.py
--rw-rw-rw-   0        0        0     2750 2023-06-24 19:15:10.000000 quik-ai-1.3.0/src/quik_ai/metrics.py
--rw-rw-rw-   0        0        0    29967 2023-06-25 14:37:54.000000 quik-ai-1.3.0/src/quik_ai/models.py
--rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.3.0/src/quik_ai/optimizers.py
--rw-rw-rw-   0        0        0    12821 2023-06-25 14:51:52.000000 quik-ai-1.3.0/src/quik_ai/predictors.py
--rw-rw-rw-   0        0        0     9426 2023-06-24 00:56:24.000000 quik-ai-1.3.0/src/quik_ai/tuners.py
--rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.3.0/src/quik_ai/tuning.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:29:58.495743 quik-ai-1.3.0/src/quik_ai.egg-info/
--rw-rw-rw-   0        0        0     2235 2023-06-25 20:29:58.000000 quik-ai-1.3.0/src/quik_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-25 20:29:58.000000 quik-ai-1.3.0/src/quik_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 20:29:58.000000 quik-ai-1.3.0/src/quik_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-06-25 20:29:58.000000 quik-ai-1.3.0/src/quik_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 20:29:58.000000 quik-ai-1.3.0/src/quik_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.203240 quik-ai-1.3.1/
+-rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2270 2023-07-04 16:29:19.203240 quik-ai-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-06-25 22:06:12.000000 quik-ai-1.3.1/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      768 2023-07-04 16:29:19.210744 quik-ai-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.142415 quik-ai-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.175006 quik-ai-1.3.1/src/quik_ai/
+-rw-rw-rw-   0        0        0      445 2023-07-04 15:16:34.000000 quik-ai-1.3.1/src/quik_ai/__init__.py
+-rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.3.1/src/quik_ai/backend.py
+-rw-rw-rw-   0        0        0    13361 2023-06-27 22:06:46.000000 quik-ai-1.3.1/src/quik_ai/engine.py
+-rw-rw-rw-   0        0        0     5511 2023-07-04 15:19:01.000000 quik-ai-1.3.1/src/quik_ai/heads.py
+-rw-rw-rw-   0        0        0    20052 2023-06-28 21:09:36.000000 quik-ai-1.3.1/src/quik_ai/layers.py
+-rw-rw-rw-   0        0        0      941 2023-06-24 18:02:43.000000 quik-ai-1.3.1/src/quik_ai/losses.py
+-rw-rw-rw-   0        0        0     3868 2023-06-28 22:37:12.000000 quik-ai-1.3.1/src/quik_ai/metrics.py
+-rw-rw-rw-   0        0        0    30799 2023-07-04 15:17:15.000000 quik-ai-1.3.1/src/quik_ai/models.py
+-rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.3.1/src/quik_ai/optimizers.py
+-rw-rw-rw-   0        0        0    12821 2023-06-25 14:51:52.000000 quik-ai-1.3.1/src/quik_ai/predictors.py
+-rw-rw-rw-   0        0        0     9426 2023-06-24 00:56:24.000000 quik-ai-1.3.1/src/quik_ai/tuners.py
+-rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.3.1/src/quik_ai/tuning.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:29:19.202219 quik-ai-1.3.1/src/quik_ai.egg-info/
+-rw-rw-rw-   0        0        0     2270 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 16:29:19.000000 quik-ai-1.3.1/src/quik_ai.egg-info/top_level.txt
```

### Comparing `quik-ai-1.3.0/LICENSE` & `quik-ai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/PKG-INFO` & `quik-ai-1.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.1.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,14 +35,15 @@
 3. Specify the predictors used for model fitting.
 ```python
 # All the predictors for the model.
 predictors = [
     qa.predictors.Numerical('numerical'),
     qa.predictors.Categorical('categorical'),
     qa.predictors.Periodic('periodic', 24.0),
+    qa.predictors.Image('image'),
 ]
 ```
 
 4. Select the model architecture.
 ```python
 # Select the architecture and feed the response column, and other
 # necessary data for training, testing the model.
```

### Comparing `quik-ai-1.3.0/README.md` & `quik-ai-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 3. Specify the predictors used for model fitting.
 ```python
 # All the predictors for the model.
 predictors = [
     qa.predictors.Numerical('numerical'),
     qa.predictors.Categorical('categorical'),
     qa.predictors.Periodic('periodic', 24.0),
+    qa.predictors.Image('image'),
 ]
 ```
 
 4. Select the model architecture.
 ```python
 # Select the architecture and feed the response column, and other
 # necessary data for training, testing the model.
```

### Comparing `quik-ai-1.3.0/setup.cfg` & `quik-ai-1.3.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7569 6b2d 6169 0d0a 7665 7273   = quik-ai..vers
-00000020: 696f 6e20 3d20 312e 332e 300d 0a61 7574  ion = 1.3.0..aut
+00000020: 696f 6e20 3d20 312e 332e 310d 0a61 7574  ion = 1.3.1..aut
 00000030: 686f 7220 3d20 416c 656b 7361 6e64 7220  hor = Aleksandr 
 00000040: 546f 757a 6f76 0d0a 6465 7363 7269 7074  Touzov..descript
 00000050: 696f 6e20 3d20 5175 6963 6b20 556e 6966  ion = Quick Unif
 00000060: 7969 6e67 2049 6e66 7261 7374 7275 6374  ying Infrastruct
 00000070: 7572 6520 4b69 7420 666f 7220 4d61 6368  ure Kit for Mach
 00000080: 696e 6520 4c65 6172 6e69 6e67 2061 6e64  ine Learning and
 00000090: 2041 490d 0a6c 6f6e 675f 6465 7363 7269   AI..long_descri
@@ -16,15 +16,15 @@
 000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000100: 2f74 6f75 7a6f 7631 3031 322f 7175 696b  /touzov1012/quik
 00000110: 2d61 690d 0a64 6f77 6e6c 6f61 645f 7572  -ai..download_ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f74 6f75 7a6f 7631 3031  ub.com/touzov101
 00000140: 322f 7175 696b 2d61 692f 6172 6368 6976  2/quik-ai/archiv
 00000150: 652f 7265 6673 2f74 6167 732f 7631 2e33  e/refs/tags/v1.3
-00000160: 2e30 2e74 6172 2e67 7a0d 0a63 6c61 7373  .0.tar.gz..class
+00000160: 2e31 2e74 6172 2e67 7a0d 0a63 6c61 7373  .1.tar.gz..class
 00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
 00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
 000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001b0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
 000001c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
 000001d0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
```

### Comparing `quik-ai-1.3.0/src/quik_ai/backend.py` & `quik-ai-1.3.1/src/quik_ai/backend.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/src/quik_ai/engine.py` & `quik-ai-1.3.1/src/quik_ai/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,22 @@
 
         # then, we stack the 2D arrays along new dimensions
         result = np.stack(arr_reshaped)
 
         # reshape the result back to the desired shape
         entry_shape = arr[0,0].shape if not isinstance(arr[0,0], str) else ()
         result = result.reshape(*arr.shape, *entry_shape)
-
+        
+        # cast to correct dtype
+        if self.get_input_dtype(columns[0]) == tf.string:
+            result = result.astype(str)
+        else:
+            result = result.astype(np.float32)
+        
+        # return the result
         return result
     
     def get_input_dtype(self, column):
         cell = self.training_data[column].iloc[0]
         if isinstance(cell, str):
             return tf.string
         return tf.float32 if cell.flatten()[0].dtype.kind in 'iufcb' else tf.string
@@ -229,25 +236,25 @@
                         group_id = cache['group_order'][end]
                         for key, value in cache['tensor_map'].items():
                             sliced_tensors[key] = value[end-group_id:end+1]
 
                     # different fetch for time series and flat array, we may need to pad
                     # the time series if it there is not enough history
                     for key in sliced_tensors.keys():
-                        fill_type = '[UNK]' if key[0] == tf.string else 0
+                        fill_type = '[UNK]' if key[0] == tf.string else np.float32(0.0)
                         sliced_tensors[key] = backend.get_k_from_end(sliced_tensors[key], time_window, fill=fill_type)
 
                     # combine the predictor vectors
                     x_values = []
                     for key, value in sliced_tensors.items():
                         splits = np.split(value, value.shape[1], axis=1)
                         for split in splits:
                             squeezed = np.squeeze(split, axis=(0,1)) if time_window <= 1 else np.squeeze(split, axis=1)
                             squeezed = np.reshape(squeezed, key[1])
-                            x_values.append(tf.convert_to_tensor(squeezed, dtype=key[0]))
+                            x_values.append(squeezed)
 
                     if cache['y'] is None:
                         example = self.__serialize_example(dict(zip(x_keys, x_values)))
                     elif cache['w'] is None:
                         example = self.__serialize_example(dict(zip(x_keys, x_values)), cache['y'][end])
                     else:
                         example = self.__serialize_example(dict(zip(x_keys, x_values)), cache['y'][end], cache['w'][end])
```

### Comparing `quik-ai-1.3.0/src/quik_ai/heads.py` & `quik-ai-1.3.1/src/quik_ai/heads.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from quik_ai import metrics
 
 import numpy as np
 import tensorflow as tf
 import tensorflow_probability as tfp
 
 losses_dictionary = {
+    'mean_absolute_error' : tf.keras.losses.MeanAbsoluteError,
     'mean_squared_error' : tf.keras.losses.MeanSquaredError,
     'log_prob' : losses.LogProbLoss,
 }
 
 metrics_dictionary = {
+    'mean_absolute_error' : metrics.MeanAbsoluteErrorMetric,
     'mean_squared_error' : metrics.MeanSquaredErrorMetric,
     'log_prob' : metrics.LogProbMetric,
 }
 
 class Head(tuning.Tunable):
     def __init__(
         self,
```

### Comparing `quik-ai-1.3.0/src/quik_ai/layers.py` & `quik-ai-1.3.1/src/quik_ai/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,18 @@
 
 @tf.keras.utils.register_keras_serializable(package="quik_ai")
 class GaussianMixtureLayer(tf.keras.layers.Layer):
     def __init__(self, num_components, event_shape, **kwargs):
         super().__init__(**kwargs)
         self.num_components = num_components
         self.event_shape = event_shape
+        self.tfp_layer = tfp.layers.MixtureNormal(self.num_components, self.event_shape)
 
     def call(self, inputs):
-        return tfp.layers.MixtureNormal(self.num_components, self.event_shape)(inputs)
+        return self.tfp_layer(inputs)
 
     def get_config(self):
         config = super().get_config()
         config.update({
             'num_components' : self.num_components,
             'event_shape' : self.event_shape
         })
```

### Comparing `quik-ai-1.3.0/src/quik_ai/losses.py` & `quik-ai-1.3.1/src/quik_ai/losses.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/src/quik_ai/metrics.py` & `quik-ai-1.3.1/src/quik_ai/metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 import tensorflow as tf
 
 @tf.keras.utils.register_keras_serializable(package="quik_ai")
+class MeanAbsoluteErrorMetric(tf.keras.metrics.Metric):
+    def __init__(self, name='mean_absolute_error', **kwargs):
+        super().__init__(name=name, **kwargs)
+        self.total = self.add_weight(name='total', initializer='zeros')
+        self.count = self.add_weight(name='count', initializer='zeros')
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        y_true = tf.reshape(y_true, tf.shape(y_pred))
+        abs_error = tf.math.abs(y_true - y_pred)
+        if sample_weight is not None:
+            sample_weight = tf.cast(sample_weight, y_true.dtype)
+            abs_error = tf.multiply(abs_error, sample_weight)
+        num_values = tf.cast(tf.size(y_true), self.dtype)
+        
+        self.total.assign_add(tf.reduce_sum(abs_error))
+        self.count.assign_add(num_values)
+
+    def result(self):
+        return tf.math.divide_no_nan(self.total, self.count)
+
+    def reset_state(self):
+        # The state of the metric will be reset at the start of each epoch.
+        self.total.assign(0.)
+        self.count.assign(0.)
+
+@tf.keras.utils.register_keras_serializable(package="quik_ai")
 class MeanSquaredErrorMetric(tf.keras.metrics.Metric):
     def __init__(self, name='mean_squared_error', **kwargs):
         super().__init__(name=name, **kwargs)
         self.total = self.add_weight(name='total', initializer='zeros')
         self.count = self.add_weight(name='count', initializer='zeros')
 
     def update_state(self, y_true, y_pred, sample_weight=None):
```

### Comparing `quik-ai-1.3.0/src/quik_ai/models.py` & `quik-ai-1.3.1/src/quik_ai/models.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,833 +1,833 @@
-from quik_ai import tuning
-from quik_ai import layers
-from quik_ai import backend
-from quik_ai import tuners
-
-try:
-    import mlflow
-except ImportError:  # pragma: no cover
-    mlflow = None  # pragma: no cover
-
-import os
-import cloudpickle
-import tensorflow as tf
-import tensorflow_probability as tfp
-import keras_tuner as kt
-import numpy as np
-import pandas as pd
-
-class HyperModel(kt.HyperModel, tuning.Tunable):
-    
-    def __init__(
-        self, 
-        name, 
-        response,
-        head,
-        predictors,
-        driver,
-        instance=None,
-        time_window=1,
-        time_dropout=0.05,
-        seed=None,
-        run_eagerly=None,
-        working_dir='./tmp', 
-        **kwargs
-    ):
-        kt.HyperModel.__init__(self, name, **kwargs)
-        tuning.Tunable.__init__(self, name, **kwargs)
-        
-        self.response = response
-        self.head = head
-        self.predictors = predictors
-        self.driver = driver
-        self.instance = instance
-        
-        self.time_window = time_window
-        self.time_dropout = time_dropout
-        self.seed = seed
-        self.run_eagerly = run_eagerly
-        self.working_dir = working_dir
-    
-    @classmethod
-    def load(cls, filepath='./model'):
-        # load tensorflow model, if it was saved
-        model = None
-        tf_model_path = backend.join_path(filepath, 'tf_model')
-        if os.path.exists(tf_model_path):
-            model = tf.keras.models.load_model(tf_model_path)
-
-        # load other attributes
-        with open(backend.join_path(filepath, 'model.pkl'), 'rb') as f:
-            data = cloudpickle.load(f)
-
-        attrs = data['attrs']
-        class_name = data['class_name']
-        attrs['instance'] = model
-
-        # get the class
-        actual_class = globals()[class_name]
-
-        # create a new instance of the class
-        instance = actual_class(**attrs)
-
-        return instance
-    
-    def save(self, filepath='./model'):
-        # make sure the directory exists
-        os.makedirs(filepath, exist_ok=True)
-
-        # save model in a subfolder, if it exists
-        if self.instance is not None:
-            self.instance.save(backend.join_path(filepath, 'tf_model'))
-
-        # save other attributes with cloudpickle
-        attrs = {name: attr for name, attr in self.__dict__.items() if name != 'instance' and not callable(attr) and not name.startswith('_')}
-        data = {
-            'class_name': self.__class__.__name__,
-            'attrs': attrs,
-        }
-        
-        with open(backend.join_path(filepath, 'model.pkl'), 'wb') as f:
-            cloudpickle.dump(data, f)
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        config.update({
-            'time_window' : self._get_hp(None, 'time_window', hp),
-            'time_dropout' : self._get_hp(None, 'time_dropout', hp),
-            'seed' : self._get_hp(None, 'seed', hp),
-        })
-        return config
-    
-    def get_dependent_tunables(self):
-        tunables = super().get_dependent_tunables()
-        tunables.extend(self.driver.get_dependent_tunables())
-        tunables.extend(self.head.get_dependent_tunables())
-        for predictor in self.predictors:
-            tunables.extend(predictor.get_dependent_tunables())
-        return tunables
-    
-    def get_input_names(self):
-        names = []
-        uniques = set()
-        for predictor in self.predictors:
-            for name in predictor.names:
-                if name not in uniques:
-                    uniques.add(name)
-                    names.append(name)
-        return names
-    
-    def __build_input_layers(self, time_window, **kwargs):
-        input_layers = {}
-        
-        input_names = self.get_input_names()
-        
-        for name in input_names:
-            dtype = self.driver.get_input_dtype(name)
-            shape = self.driver.get_input_shape(name, time_window)
-
-            input_layers[name] = tf.keras.Input(name=name, dtype=dtype, shape=shape)
-        
-        return input_layers
-    
-    def __build_input_tensor(self, hp, input_layers, time_window, time_dropout, seed, **kwargs):
-        
-        # if we have time, we need to apply history dropout
-        if time_window > 1:
-            dropped_inputs = layers.HistoryDropout(time_dropout, seed)(input_layers.values())
-            input_layers = {k: v for k, v in zip(input_layers, dropped_inputs)}
-        
-        # process each predictor transform
-        inputs = []
-        for predictor in self.predictors:
-            inputs.append(predictor.transform(input_layers, self.driver, time_window, hp))
-        
-        # remove dropped inputs
-        inputs = [x for x in inputs if x is not None]
-        
-        # if we do not have a time dimension, then we either flatten and concat all inputs
-        # or we leave the singular input in its desired form. If we do have a time dimension
-        # then we time flatten all inputs
-        if time_window <= 1 and len(inputs) > 1:
-            inputs = [tf.keras.layers.Flatten()(x) for x in inputs]
-        elif time_window > 1 and len(inputs) > 0:
-            # we have a time component, so we need to time flatten everything
-            inputs = [layers.TimeFlatten()(x) for x in inputs]
-        
-        # if all inputs are dropped, we replace with a constant
-        if not inputs:
-            inputs = []
-            for x in input_layers.values():
-                inputs.append(tf.ones_like(tf.keras.layers.Flatten()(x), dtype=tf.float32))
-            inputs = [tf.keras.layers.GlobalAveragePooling1D()(tf.expand_dims(tf.concat(inputs, -1), -1))]
-        
-        # will be either shape (batch, time, features) or (batch, features)
-        return tf.concat(inputs, axis=-1)
-    
-    def __build_mlflow_callback(self, metric_name, run_id, objective_direction, verbose):
-        class MlflowCallback(tf.keras.callbacks.Callback):
-            def on_epoch_end(self, epoch, logs=None):
-                if logs is None or run_id is None:
-                    return
-
-                if metric_name not in logs or np.isnan(logs[metric_name]):
-                    backend.info('Terminated epoch with NaN result ...', verbose)
-                    return
-
-                # get stored metrics
-                logged_metrics = mlflow.MlflowClient().get_run(run_id).data.metrics
-
-                # we need to post a new update
-                if metric_name not in logged_metrics:
-                    mlflow.MlflowClient().log_metric(run_id, metric_name, logs[metric_name])
-                    return
-                
-                if objective_direction == 'min' and logs[metric_name] < logged_metrics[metric_name]:
-                    mlflow.MlflowClient().log_metric(run_id, metric_name, logs[metric_name])
-                    return
-                
-                if objective_direction == 'max' and logs[metric_name] > logged_metrics[metric_name]:
-                    mlflow.MlflowClient().log_metric(run_id, metric_name, logs[metric_name])
-                    return
-        
-        # return the callback
-        return MlflowCallback()
-    
-    def build(self, hp):
-        
-        # if we want to build without tuning fill out a
-        # dummy instance of hp so we can sample some params
-        if hp is None:
-            hp = kt.HyperParameters()
-        
-        # cache parameters of driver
-        self.driver.get_parameters(hp)
-        
-        # get parameters
-        config = self.get_parameters(hp)
-        
-        # get input layers as a dict
-        inputs = self.__build_input_layers(**config)
-        
-        # build the input tensor from all input layers
-        outputs = self.__build_input_tensor(hp, inputs, **config)
-        
-        # apply the model body
-        outputs = self.body(outputs, **config)
-        
-        # transform using output head
-        outputs = self.head.transform(hp, outputs)
-        
-        # construct the model
-        model = tf.keras.Model(
-            inputs=list(inputs.values()), 
-            outputs=outputs,
-        )
-        
-        # compile
-        model.compile(
-            loss=self.head.loss(), 
-            optimizer=self.driver.get_optimizer(hp), 
-            weighted_metrics=self.head.metrics(),
-            run_eagerly=self.run_eagerly,
-        )
-        
-        return model
-    
-    def fit(self, hp, model, *args, **kwargs):
-        # if we want to build without tuning fill out a
-        # dummy instance of hp so we can sample some params
-        if hp is None:
-            hp = kt.HyperParameters()
-        
-        config = self.get_parameters(hp)
-        input_names = self.get_input_names()
-        
-        # cache the args to the fit function
-        fit_args = [
-            self.driver.get_training_tensorflow_dataset(input_names, self.response, config['time_window'], hp),
-            *args, 
-        ]
-        
-        # cache the kwargs to the fit function
-        fit_kwargs = dict(
-            steps_per_epoch=self.driver.get_training_steps_per_epoch(hp), 
-            validation_data=self.driver.get_validation_tensorflow_dataset(input_names, self.response, config['time_window'], hp), 
-        )
-        
-        # check if we have mlflow active
-        active_run = mlflow.active_run() if mlflow is not None else None
-        
-        # if we have an active mlflow run
-        if active_run is not None:
-            with mlflow.start_run(nested=True):
-                mlflow.log_params(hp.values)
-                mlflow.tensorflow.autolog()
-                return model.fit(*fit_args, **fit_kwargs, **kwargs)
-        
-        # no mlflow run, return as normal
-        return model.fit(*fit_args, **fit_kwargs, **kwargs)
-    
-    def train(
-        self,
-        tuner=tuners.BOHB,
-        early_stopping_tune=10, 
-        early_stopping_full=10,
-        full_rounds=1,
-        tuner_params={},
-        verbose=1
-    ):
-        
-        # create working directory for the build
-        build_dir = backend.create_unique_dir(working_dir=self.working_dir)
-
-        backend.info('Checking for hyper-parameters to tune ...', verbose)
-
-        # set up the keras tuner parameters
-        checkpoint_monitor = 'val_' + self.head.monitor()
-
-        # create the tuner
-        tuner_epochs = tuner_params.pop('epochs', 1)
-        tuner = tuner(
-            self, 
-            objective=kt.Objective(checkpoint_monitor, direction=self.head.objective_direction),
-            directory=backend.join_path(build_dir, 'tuner'),
-            project_name='kt_tuner', 
-            **tuner_params
-        )
-
-        # early stopping
-        early_stopping = tf.keras.callbacks.EarlyStopping(
-            monitor=checkpoint_monitor, 
-            patience=early_stopping_tune,
-            mode=self.head.objective_direction
-        )
-        
-        # mlflow callback
-        active_run = mlflow.active_run() if mlflow is not None else None
-        run_id = active_run.info.run_id if active_run is not None else None
-        
-        # if we have a mlflow job, create a child job
-        if run_id is not None:
-            mlflow.start_run(run_name='hyperparameter-search', nested=True)
-
-        # search the space
-        tuner.search(
-            epochs=tuner_epochs, 
-            callbacks=[
-                tf.keras.callbacks.TerminateOnNaN(), 
-                early_stopping,
-                self.__build_mlflow_callback(checkpoint_monitor, run_id, self.head.objective_direction, verbose),
-            ], 
-            verbose=backend.clamp(verbose)
-        )
-        
-        # terminate the mlflow child job
-        if run_id is not None:
-            mlflow.end_run()
-
-        # get the best hyperparameters
-        best_hps = tuner.get_best_hyperparameters(num_trials=1)
-        if best_hps is not None and len(best_hps) > 0:
-            best_hps = best_hps[0].values
-
-            # apply to all parameters tuned through model
-            tunables = self.get_dependent_tunables()
-            for tunable in tunables:
-                tunable._apply_hp(best_hps)
-
-        # early stopping
-        early_stopping = tf.keras.callbacks.EarlyStopping(
-            monitor=checkpoint_monitor, 
-            patience=early_stopping_full,
-            mode=self.head.objective_direction
-        )
-
-        # checkpoint to catch best validation
-        checkpoint_filepath = backend.join_path(build_dir, 'cp')
-        model_checkpoint_callback = tf.keras.callbacks.ModelCheckpoint(
-            filepath=checkpoint_filepath,
-            save_weights_only=True,
-            monitor=checkpoint_monitor,
-            mode=self.head.objective_direction,
-            save_best_only=True,
-            verbose=backend.clamp(verbose-1)
-        )
-        
-        # if we have mlflow create the child job for the full training
-        if run_id is not None:
-            mlflow.start_run(run_name='full-training', nested=True)
-
-        # full training
-        for i in range(full_rounds):
-
-            # clean up last model
-            if i > 0:
-                del model
-                backend.clean_tensorflow()
-
-            # re-initialize the model
-            model = self.build(None)
-
-            # for each full training run, create a sub job
-            if run_id is not None:
-                mlflow.start_run(run_name='full-model-%s' % i, nested=True)
-                mlflow.tensorflow.autolog()
-            
-            # fit the model
-            history = self.fit(
-                None, 
-                model, 
-                epochs=1_000_000, 
-                callbacks=[
-                    tf.keras.callbacks.TerminateOnNaN(), 
-                    model_checkpoint_callback, 
-                    early_stopping,
-                    self.__build_mlflow_callback(checkpoint_monitor, run_id, self.head.objective_direction, verbose),
-                ], 
-                verbose=backend.clamp(verbose-2)
-            )
-            
-            # end the mlflow run
-            if run_id is not None:
-                mlflow.end_run()
-
-            # process history to get extrema score
-            scores = history.history[checkpoint_monitor]
-            curr_score = min(scores) if self.head.objective_direction == 'min' else max(scores)
-
-            # log the current run
-            backend.info('Round %s best score: %.4f' % (i+1, curr_score), verbose)
-
-        # end the full training job
-        if run_id is not None:
-            mlflow.end_run()
-            
-        # load the best weights
-        model.load_weights(checkpoint_filepath)
-        
-        # store the model instance
-        self.instance = model
-    
-    def predict(self, data, verbose=1):
-        
-        if self.instance is None:
-            backend.error('Cannot predict for a NULL instance. Make sure you train the model before invoking.')
-            return None
-        
-        # build the input dataset from the numpy array
-        tdf = self.driver.get_tensorflow_dataset(
-            data, 
-            input_names=self.get_input_names(), 
-            response=None, 
-            time_window=self.time_window, 
-            hp=None, 
-            shuffle=False,
-        )
-        
-        return self.instance.predict(tdf, verbose=verbose)
-    
-    def predict_distribution(self, data, samples):
-        
-        if self.instance is None:
-            backend.error('Cannot predict for a NULL instance. Make sure you train the model before invoking.')
-            return None
-        
-        # build the input dataset from the numpy array
-        tdf = self.driver.get_tensorflow_dataset(
-            data, 
-            input_names=self.get_input_names(), 
-            response=None, 
-            time_window=self.time_window, 
-            hp=None, 
-            shuffle=False,
-        )
-        
-        # get outputs for each data point
-        outputs = []
-        for x in tdf:
-            outputs.append(self.instance(x))
-        
-        # if we do not have a distribution layer
-        if not isinstance(outputs[0], tfp.distributions.Distribution):
-            backend.error('Cannot predict distribution for a non-density model. Make sure you choose the right model head.')
-            return None
-        
-        # get array for final results
-        results = []
-
-        # for each value in the samples, calculate the prob of the distribution
-        for value in samples:
-            batch = []
-            for output in outputs:
-                batch.append(tf.exp(output.log_prob(value)))
-            results.append(tf.concat(batch, 0))
-
-        # concat results along the second axis
-        return tf.stack(results, axis=-1)
-    
-    def evaluate(self, data=None, verbose=1):
-        
-        if self.instance is None:
-            backend.error('Cannot evaluate for a NULL instance. Make sure you train the model before invoking.')
-            return None
-        
-        # default to the test set
-        if data is None:
-            data = self.driver.testing_data
-        
-        # build the input dataset from the numpy array
-        tdf = self.driver.get_tensorflow_dataset(
-            data, 
-            input_names=self.get_input_names(), 
-            response=self.response, 
-            time_window=self.time_window, 
-            hp=None, 
-            shuffle=False,
-        )
-        
-        # evalute the results
-        evals = self.instance.evaluate(tdf, verbose=verbose)
-        
-        # pair each result with the metric name
-        res = {}
-        for i in range(len(evals)):
-            res[self.instance.metrics[i].name.strip('_')] = evals[i]
-        
-        return res
-    
-    def report(self, filepath='./model', verbose=0):
-        
-        if self.instance is None:
-            backend.error('Cannot report for a NULL instance. Make sure you train the model before invoking.')
-            return
-        
-        # make sure the directory exists
-        os.makedirs(filepath, exist_ok=True)
-            
-        # readme
-        predictors = []
-        for lyr in self.instance.layers:
-            if lyr.__class__.__name__ == 'InputLayer':
-                predictors.append(lyr.name)
-
-        # check if we have mlflow active
-        active_run = mlflow.active_run() if mlflow is not None else None
-
-        # header and file name
-        fname = backend.join_path(filepath, 'README.md')
-        lines = []
-        lines.append('## Model\n\n')
-        lines.append('This README.md file outlines the parameters and predictors used by the model.\n\n')
-        lines.append('#### Input layers:\n\n')
-        lines.append('* %s\n\n' % '\n* '.join(predictors))
-
-        # save parameters table
-        parameters = self.get_instance_parameters()
-        if len(parameters) > 0:
-            parameters = {k: v for k, v in parameters.items() if not isinstance(v, tuning.HyperVariable)}
-            parameters = pd.DataFrame(list(parameters.items()), columns=['Parameter', 'Value'])
-            lines.append('#### Model parameters:\n\n')
-            lines.append('%s\n\n' % parameters.to_markdown(index=False))
-
-        # save full model scores
-        if self.driver is not None and self.driver.testing_data is not None:
-            scores = self.evaluate(self.driver.testing_data, verbose=verbose)
-            scores = pd.DataFrame(list(scores.items()), columns=['Metric', 'Value'])
-            lines.append('#### Test performance:\n\n')
-            lines.append('%s\n\n' % scores.to_markdown(index=False))
-
-        if active_run is not None:
-            mlflow.log_text(''.join(lines), fname)
-        else:
-            readme = open(fname, "w")
-            readme.write(''.join(lines))
-            readme.close()
-    
-    def get_instance_parameters(self):
-        
-        if self.instance is None:
-            backend.error('Cannot fetch instance parameters for a NULL instance. Make sure you train the model before invoking.')
-            return None
-        
-        tunables = self.get_dependent_tunables()
-        
-        all_params = {}
-        
-        # iterate over each tunable in our dependent stack
-        for tunable in tunables:
-            params = tunable.get_parameters(None)
-            
-            # iterate over all params in the tunable
-            for key, value in params.items():
-                all_params['%s/%s' % (tunable.name, key)] = value
-        
-        return all_params
-
-class ResNet(HyperModel):
-    
-    def __init__(
-        self,
-        response,
-        head,
-        predictors,
-        driver,
-        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
-        blocks=tuning.HyperInt(min_value=0, max_value=6),
-        activation=tuning.HyperChoice(['relu','gelu']),
-        dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        projection_scale=tuning.HyperInt(min_value=1, max_value=4),
-        name='ResNet',
-        **kwargs
-    ):
-        super().__init__(name, response, head, predictors, driver, **kwargs)
-        
-        self.model_dim = model_dim
-        self.blocks = blocks
-        self.activation = activation
-        self.dropout = dropout
-        self.projection_scale = projection_scale
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        config.update({
-            'model_dim' : self._get_hp(None, 'model_dim', hp),
-            'blocks' : self._get_hp(None, 'blocks', hp),
-            'activation' : self._get_hp(None, 'activation', hp),
-            'dropout' : self._get_hp(None, 'dropout', hp),
-            'projection_scale' : self._get_hp(None, 'projection_scale', hp),
-        })
-        return config
-    
-    def body(self, inputs, model_dim, blocks, activation, dropout, projection_scale, **kwargs):
-        
-        # flatten dimensions
-        if len(inputs.shape) > 2:
-            inputs = tf.keras.layers.Flatten()(inputs)
-        
-        # project into model dimension
-        inputs = tf.keras.layers.Dense(model_dim)(inputs)
-        
-        # apply resnet blocks
-        for _ in range(blocks):
-            inputs = layers.ResNetBlock(
-                activation=activation, 
-                dropout=dropout, 
-                projection_scale=projection_scale,
-            )(inputs)
-        
-        # return this body output
-        return inputs
-
-class RNN(HyperModel):
-    
-    def __init__(
-        self,
-        response,
-        head,
-        predictors,
-        driver,
-        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
-        dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        recurrent_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        recurrent_func=tuning.HyperChoice(['SimpleRNN','LSTM','GRU']),
-        name='RNN',
-        **kwargs
-    ):
-        super().__init__(name, response, head, predictors, driver, **kwargs)
-        
-        self.model_dim = model_dim
-        self.dropout = dropout
-        self.recurrent_dropout = recurrent_dropout
-        self.recurrent_func = recurrent_func
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        config.update({
-            'model_dim' : self._get_hp(None, 'model_dim', hp),
-            'dropout' : self._get_hp(None, 'dropout', hp),
-            'recurrent_dropout' : self._get_hp(None, 'recurrent_dropout', hp),
-            'recurrent_func' : self._get_hp(None, 'recurrent_func', hp),
-        })
-        return config
-    
-    def body(self, inputs, model_dim, dropout, recurrent_dropout, recurrent_func, **kwargs):
-        
-        # rnn needs second dimension to be time
-        if len(inputs.shape) <= 2:
-            inputs = tf.expand_dims(inputs, 1)
-            
-        if recurrent_func == 'SimpleRNN':
-            inputs = tf.keras.layers.SimpleRNN(model_dim, dropout=dropout, recurrent_dropout=recurrent_dropout)(inputs)
-        elif recurrent_func == 'LSTM':
-            inputs = tf.keras.layers.LSTM(model_dim, dropout=dropout, recurrent_dropout=recurrent_dropout)(inputs)
-        elif recurrent_func == 'GRU':
-            inputs = tf.keras.layers.GRU(model_dim, dropout=dropout, recurrent_dropout=recurrent_dropout)(inputs)
-        else:
-            backend.error('Recurrent function %s is not known!' % recurrent_func)
-        
-        # return this body output
-        return inputs
-    
-class Transformer(HyperModel):
-    
-    def __init__(
-        self,
-        response,
-        head,
-        predictors,
-        driver,
-        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
-        num_layers=tuning.HyperInt(min_value=1, max_value=6),
-        ffn_activation=tuning.HyperChoice(['relu','gelu']),
-        ffn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        ffn_projection_scale=tuning.HyperInt(min_value=1, max_value=4),
-        num_heads=tuning.HyperInt(min_value=1, max_value=5),
-        attn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        name='Transformer',
-        **kwargs
-    ):
-        super().__init__(name, response, head, predictors, driver, **kwargs)
-        
-        self.model_dim = model_dim
-        self.num_layers = num_layers
-        self.ffn_activation = ffn_activation
-        self.ffn_dropout = ffn_dropout
-        self.ffn_projection_scale = ffn_projection_scale
-        self.num_heads = num_heads
-        self.attn_dropout = attn_dropout
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        config.update({
-            'model_dim' : self._get_hp(None, 'model_dim', hp),
-            'num_layers' : self._get_hp(None, 'num_layers', hp),
-            'ffn_activation' : self._get_hp(None, 'ffn_activation', hp),
-            'ffn_dropout' : self._get_hp(None, 'ffn_dropout', hp),
-            'ffn_projection_scale' : self._get_hp(None, 'ffn_projection_scale', hp),
-            'num_heads' : self._get_hp(None, 'num_heads', hp),
-            'attn_dropout' : self._get_hp(None, 'attn_dropout', hp),
-        })
-        return config
-    
-    def body(
-        self, 
-        inputs, 
-        model_dim, 
-        num_layers, 
-        ffn_activation, 
-        ffn_dropout, 
-        ffn_projection_scale, 
-        num_heads, 
-        attn_dropout, 
-        **kwargs
-    ):
-        
-        # transformer needs data with at least 3 dimensions
-        if len(inputs.shape) <= 2:
-            inputs = tf.expand_dims(inputs, -1)
-            
-        # linear projection and positional encoding
-        inputs = layers.ChunkEmbedding(model_dim)(inputs)
-
-        # transformer layer
-        inputs = layers.Transformer(
-            num_layers=num_layers,
-            ffn_activation=ffn_activation,
-            ffn_dropout=ffn_dropout,
-            ffn_projection_scale=ffn_projection_scale,
-            num_heads=num_heads,
-            attn_dropout=attn_dropout,
-        )(inputs)
-        
-        # global average pool results
-        inputs = tf.keras.layers.GlobalAveragePooling1D()(inputs)
-        
-        # return this body output
-        return inputs
-
-class TransformerLong(HyperModel):
-    
-    def __init__(
-        self,
-        response,
-        head,
-        predictors,
-        driver,
-        chunk_size,
-        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
-        xattn_rate=tuning.HyperInt(min_value=2, max_value=4),
-        num_layers=tuning.HyperInt(min_value=1, max_value=6),
-        ffn_activation=tuning.HyperChoice(['relu','gelu']),
-        ffn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        ffn_projection_scale=tuning.HyperInt(min_value=1, max_value=4),
-        num_heads=tuning.HyperInt(min_value=1, max_value=5),
-        attn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
-        name='TransformerLong',
-        **kwargs
-    ):
-        super().__init__(name, response, head, predictors, driver, **kwargs)
-        
-        self.chunk_size = chunk_size
-        self.model_dim = model_dim
-        self.xattn_rate = xattn_rate
-        self.num_layers = num_layers
-        self.ffn_activation = ffn_activation
-        self.ffn_dropout = ffn_dropout
-        self.ffn_projection_scale = ffn_projection_scale
-        self.num_heads = num_heads
-        self.attn_dropout = attn_dropout
-    
-    def get_parameters(self, hp):
-        config = super().get_parameters(hp)
-        config.update({
-            'model_dim' : self._get_hp(None, 'model_dim', hp),
-            'xattn_rate' : self._get_hp(None, 'xattn_rate', hp),
-            'num_layers' : self._get_hp(None, 'num_layers', hp),
-            'ffn_activation' : self._get_hp(None, 'ffn_activation', hp),
-            'ffn_dropout' : self._get_hp(None, 'ffn_dropout', hp),
-            'ffn_projection_scale' : self._get_hp(None, 'ffn_projection_scale', hp),
-            'num_heads' : self._get_hp(None, 'num_heads', hp),
-            'attn_dropout' : self._get_hp(None, 'attn_dropout', hp),
-        })
-        return config
-    
-    def body(
-        self, 
-        inputs, 
-        model_dim, 
-        xattn_rate,
-        num_layers, 
-        ffn_activation, 
-        ffn_dropout, 
-        ffn_projection_scale, 
-        num_heads, 
-        attn_dropout, 
-        **kwargs
-    ):
-        
-        # transformer needs data with at least 3 dimensions
-        if len(inputs.shape) <= 2:
-            inputs = tf.expand_dims(inputs, -1)
-            
-        # linear projection and positional encoding
-        inputs = layers.ChunkEmbedding(model_dim, self.chunk_size)(inputs)
-
-        # transformer layer
-        inputs = tf.keras.layers.RNN(layers.TransformerRecurrentCell(
-            chunk_size=self.chunk_size,
-            model_dim=model_dim,
-            xattn_rate=xattn_rate,
-            num_layers=num_layers,
-            ffn_activation=ffn_activation,
-            ffn_dropout=ffn_dropout,
-            ffn_projection_scale=ffn_projection_scale,
-            num_heads=num_heads,
-            attn_dropout=attn_dropout,
-        ))(inputs)
-        
-        # global average pool results
-        inputs = tf.keras.layers.GlobalAveragePooling1D()(inputs)
-        
-        # return this body output
+from quik_ai import tuning
+from quik_ai import layers
+from quik_ai import backend
+from quik_ai import tuners
+
+try:
+    import mlflow
+except ImportError:  # pragma: no cover
+    mlflow = None  # pragma: no cover
+
+import os
+import cloudpickle
+import tensorflow as tf
+import tensorflow_probability as tfp
+import keras_tuner as kt
+import numpy as np
+import pandas as pd
+
+class HyperModel(kt.HyperModel, tuning.Tunable):
+    
+    def __init__(
+        self, 
+        name, 
+        response,
+        head,
+        predictors,
+        driver,
+        instance=None,
+        time_window=1,
+        time_dropout=0.05,
+        seed=None,
+        run_eagerly=None,
+        working_dir='./tmp', 
+        **kwargs
+    ):
+        kt.HyperModel.__init__(self, name, **kwargs)
+        tuning.Tunable.__init__(self, name, **kwargs)
+        
+        self.response = response
+        self.head = head
+        self.predictors = predictors
+        self.driver = driver
+        self.instance = instance
+        
+        self.time_window = time_window
+        self.time_dropout = time_dropout
+        self.seed = seed
+        self.run_eagerly = run_eagerly
+        self.working_dir = working_dir
+    
+    @classmethod
+    def load(cls, filepath='./model'):
+        # load tensorflow model, if it was saved
+        model = None
+        tf_model_path = backend.join_path(filepath, 'tf_model')
+        if os.path.exists(tf_model_path):
+            model = tf.keras.models.load_model(tf_model_path)
+
+        # load other attributes
+        with open(backend.join_path(filepath, 'model.pkl'), 'rb') as f:
+            data = cloudpickle.load(f)
+
+        attrs = data['attrs']
+        class_name = data['class_name']
+        attrs['instance'] = model
+
+        # get the class
+        actual_class = globals()[class_name]
+
+        # create a new instance of the class
+        instance = actual_class(**attrs)
+
+        return instance
+    
+    def save(self, filepath='./model'):
+        # make sure the directory exists
+        os.makedirs(filepath, exist_ok=True)
+
+        # save model in a subfolder, if it exists
+        if self.instance is not None:
+            self.instance.save(backend.join_path(filepath, 'tf_model'))
+
+        # save other attributes with cloudpickle
+        attrs = {name: attr for name, attr in self.__dict__.items() if name != 'instance' and not callable(attr) and not name.startswith('_')}
+        data = {
+            'class_name': self.__class__.__name__,
+            'attrs': attrs,
+        }
+        
+        with open(backend.join_path(filepath, 'model.pkl'), 'wb') as f:
+            cloudpickle.dump(data, f)
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        config.update({
+            'time_window' : self._get_hp(None, 'time_window', hp),
+            'time_dropout' : self._get_hp(None, 'time_dropout', hp),
+            'seed' : self._get_hp(None, 'seed', hp),
+        })
+        return config
+    
+    def get_dependent_tunables(self):
+        tunables = super().get_dependent_tunables()
+        tunables.extend(self.driver.get_dependent_tunables())
+        tunables.extend(self.head.get_dependent_tunables())
+        for predictor in self.predictors:
+            tunables.extend(predictor.get_dependent_tunables())
+        return tunables
+    
+    def get_input_names(self):
+        names = []
+        uniques = set()
+        for predictor in self.predictors:
+            for name in predictor.names:
+                if name not in uniques:
+                    uniques.add(name)
+                    names.append(name)
+        return names
+    
+    def __build_input_layers(self, time_window, **kwargs):
+        input_layers = {}
+        
+        input_names = self.get_input_names()
+        
+        for name in input_names:
+            dtype = self.driver.get_input_dtype(name)
+            shape = self.driver.get_input_shape(name, time_window)
+
+            input_layers[name] = tf.keras.Input(name=name, dtype=dtype, shape=shape)
+        
+        return input_layers
+    
+    def __build_input_tensor(self, hp, input_layers, time_window, time_dropout, seed, **kwargs):
+        
+        # if we have time, we need to apply history dropout
+        if time_window > 1:
+            dropped_inputs = layers.HistoryDropout(time_dropout, seed)(input_layers.values())
+            input_layers = {k: v for k, v in zip(input_layers, dropped_inputs)}
+        
+        # process each predictor transform
+        inputs = []
+        for predictor in self.predictors:
+            inputs.append(predictor.transform(input_layers, self.driver, time_window, hp))
+        
+        # remove dropped inputs
+        inputs = [x for x in inputs if x is not None]
+        
+        # if we do not have a time dimension, then we either flatten and concat all inputs
+        # or we leave the singular input in its desired form. If we do have a time dimension
+        # then we time flatten all inputs
+        if time_window <= 1 and len(inputs) > 1:
+            inputs = [tf.keras.layers.Flatten()(x) for x in inputs]
+        elif time_window > 1 and len(inputs) > 0:
+            # we have a time component, so we need to time flatten everything
+            inputs = [layers.TimeFlatten()(x) for x in inputs]
+        
+        # if all inputs are dropped, we replace with a constant
+        if not inputs:
+            inputs = []
+            for x in input_layers.values():
+                inputs.append(tf.ones_like(tf.keras.layers.Flatten()(x), dtype=tf.float32))
+            inputs = [tf.keras.layers.GlobalAveragePooling1D()(tf.expand_dims(tf.concat(inputs, -1), -1))]
+        
+        # will be either shape (batch, time, features) or (batch, features)
+        return tf.concat(inputs, axis=-1)
+    
+    def __build_mlflow_callback(self, metric_name, run_id, objective_direction, verbose):
+        class MlflowCallback(tf.keras.callbacks.Callback):
+            def on_epoch_end(self, epoch, logs=None):
+                if logs is None or run_id is None:
+                    return
+
+                if metric_name not in logs or np.isnan(logs[metric_name]):
+                    backend.info('Terminated epoch with NaN result ...', verbose)
+                    return
+
+                # get stored metrics
+                logged_metrics = mlflow.MlflowClient().get_run(run_id).data.metrics
+
+                # we need to post a new update
+                if metric_name not in logged_metrics:
+                    mlflow.MlflowClient().log_metric(run_id, metric_name, logs[metric_name])
+                    return
+                
+                if objective_direction == 'min' and logs[metric_name] < logged_metrics[metric_name]:
+                    mlflow.MlflowClient().log_metric(run_id, metric_name, logs[metric_name])
+                    return
+                
+                if objective_direction == 'max' and logs[metric_name] > logged_metrics[metric_name]:
+                    mlflow.MlflowClient().log_metric(run_id, metric_name, logs[metric_name])
+                    return
+        
+        # return the callback
+        return MlflowCallback()
+    
+    def build(self, hp):
+        
+        # if we want to build without tuning fill out a
+        # dummy instance of hp so we can sample some params
+        if hp is None:
+            hp = kt.HyperParameters()
+        
+        # cache parameters of driver
+        self.driver.get_parameters(hp)
+        
+        # get parameters
+        config = self.get_parameters(hp)
+        
+        # get input layers as a dict
+        inputs = self.__build_input_layers(**config)
+        
+        # build the input tensor from all input layers
+        outputs = self.__build_input_tensor(hp, inputs, **config)
+        
+        # apply the model body
+        outputs = self.body(outputs, **config)
+        
+        # transform using output head
+        outputs = self.head.transform(hp, outputs)
+        
+        # construct the model
+        model = tf.keras.Model(
+            inputs=list(inputs.values()), 
+            outputs=outputs,
+        )
+        
+        # compile
+        model.compile(
+            loss=self.head.loss(), 
+            optimizer=self.driver.get_optimizer(hp), 
+            weighted_metrics=self.head.metrics(),
+            run_eagerly=self.run_eagerly,
+        )
+        
+        return model
+    
+    def fit(self, hp, model, *args, **kwargs):
+        # if we want to build without tuning fill out a
+        # dummy instance of hp so we can sample some params
+        if hp is None:
+            hp = kt.HyperParameters()
+        
+        config = self.get_parameters(hp)
+        input_names = self.get_input_names()
+        
+        # cache the args to the fit function
+        fit_args = [
+            self.driver.get_training_tensorflow_dataset(input_names, self.response, config['time_window'], hp),
+            *args, 
+        ]
+        
+        # cache the kwargs to the fit function
+        fit_kwargs = dict(
+            steps_per_epoch=self.driver.get_training_steps_per_epoch(hp), 
+            validation_data=self.driver.get_validation_tensorflow_dataset(input_names, self.response, config['time_window'], hp), 
+        )
+        
+        # check if we have mlflow active
+        active_run = mlflow.active_run() if mlflow is not None else None
+        
+        # if we have an active mlflow run
+        if active_run is not None:
+            with mlflow.start_run(nested=True):
+                mlflow.log_params(hp.values)
+                mlflow.tensorflow.autolog()
+                return model.fit(*fit_args, **fit_kwargs, **kwargs)
+        
+        # no mlflow run, return as normal
+        return model.fit(*fit_args, **fit_kwargs, **kwargs)
+    
+    def train(
+        self,
+        tuner=tuners.BOHB,
+        early_stopping_tune=10, 
+        early_stopping_full=10,
+        full_rounds=1,
+        tuner_params={},
+        verbose=1
+    ):
+        
+        # create working directory for the build
+        build_dir = backend.create_unique_dir(working_dir=self.working_dir)
+
+        backend.info('Checking for hyper-parameters to tune ...', verbose)
+
+        # set up the keras tuner parameters
+        checkpoint_monitor = 'val_' + self.head.monitor()
+
+        # create the tuner
+        tuner_epochs = tuner_params.pop('epochs', 1)
+        tuner = tuner(
+            self, 
+            objective=kt.Objective(checkpoint_monitor, direction=self.head.objective_direction),
+            directory=backend.join_path(build_dir, 'tuner'),
+            project_name='kt_tuner', 
+            **tuner_params
+        )
+
+        # early stopping
+        early_stopping = tf.keras.callbacks.EarlyStopping(
+            monitor=checkpoint_monitor, 
+            patience=early_stopping_tune,
+            mode=self.head.objective_direction
+        )
+        
+        # mlflow callback
+        active_run = mlflow.active_run() if mlflow is not None else None
+        run_id = active_run.info.run_id if active_run is not None else None
+        
+        # if we have a mlflow job, create a child job
+        if run_id is not None:
+            mlflow.start_run(run_name='hyperparameter-search', nested=True)
+
+        # search the space
+        tuner.search(
+            epochs=tuner_epochs, 
+            callbacks=[
+                tf.keras.callbacks.TerminateOnNaN(), 
+                early_stopping,
+                self.__build_mlflow_callback(checkpoint_monitor, run_id, self.head.objective_direction, verbose),
+            ], 
+            verbose=backend.clamp(verbose)
+        )
+        
+        # terminate the mlflow child job
+        if run_id is not None:
+            mlflow.end_run()
+
+        # get the best hyperparameters
+        best_hps = tuner.get_best_hyperparameters(num_trials=1)
+        if best_hps is not None and len(best_hps) > 0:
+            best_hps = best_hps[0].values
+
+            # apply to all parameters tuned through model
+            tunables = self.get_dependent_tunables()
+            for tunable in tunables:
+                tunable._apply_hp(best_hps)
+
+        # early stopping
+        early_stopping = tf.keras.callbacks.EarlyStopping(
+            monitor=checkpoint_monitor, 
+            patience=early_stopping_full,
+            mode=self.head.objective_direction
+        )
+
+        # checkpoint to catch best validation
+        checkpoint_filepath = backend.join_path(build_dir, 'cp')
+        model_checkpoint_callback = tf.keras.callbacks.ModelCheckpoint(
+            filepath=checkpoint_filepath,
+            save_weights_only=True,
+            monitor=checkpoint_monitor,
+            mode=self.head.objective_direction,
+            save_best_only=True,
+            verbose=backend.clamp(verbose-1)
+        )
+        
+        # if we have mlflow create the child job for the full training
+        if run_id is not None:
+            mlflow.start_run(run_name='full-training', nested=True)
+
+        # full training
+        for i in range(full_rounds):
+
+            # clean up last model
+            if i > 0:
+                del model
+                backend.clean_tensorflow()
+
+            # re-initialize the model
+            model = self.build(None)
+
+            # for each full training run, create a sub job
+            if run_id is not None:
+                mlflow.start_run(run_name='full-model-%s' % i, nested=True)
+                mlflow.tensorflow.autolog()
+            
+            # fit the model
+            history = self.fit(
+                None, 
+                model, 
+                epochs=1_000_000, 
+                callbacks=[
+                    tf.keras.callbacks.TerminateOnNaN(), 
+                    model_checkpoint_callback, 
+                    early_stopping,
+                    self.__build_mlflow_callback(checkpoint_monitor, run_id, self.head.objective_direction, verbose),
+                ], 
+                verbose=backend.clamp(verbose-2)
+            )
+            
+            # end the mlflow run
+            if run_id is not None:
+                mlflow.end_run()
+
+            # process history to get extrema score
+            scores = history.history[checkpoint_monitor]
+            curr_score = min(scores) if self.head.objective_direction == 'min' else max(scores)
+
+            # log the current run
+            backend.info('Round %s best score: %.4f' % (i+1, curr_score), verbose)
+
+        # end the full training job
+        if run_id is not None:
+            mlflow.end_run()
+            
+        # load the best weights
+        model.load_weights(checkpoint_filepath)
+        
+        # store the model instance
+        self.instance = model
+    
+    def predict(self, data, verbose=1):
+        
+        if self.instance is None:
+            backend.error('Cannot predict for a NULL instance. Make sure you train the model before invoking.')
+            return None
+        
+        # build the input dataset from the numpy array
+        tdf = self.driver.get_tensorflow_dataset(
+            data, 
+            input_names=self.get_input_names(), 
+            response=None, 
+            time_window=self.time_window, 
+            hp=None, 
+            shuffle=False,
+        )
+        
+        return self.instance.predict(tdf, verbose=verbose)
+    
+    def predict_distribution(self, data, samples):
+        
+        if self.instance is None:
+            backend.error('Cannot predict for a NULL instance. Make sure you train the model before invoking.')
+            return None
+        
+        # build the input dataset from the numpy array
+        tdf = self.driver.get_tensorflow_dataset(
+            data, 
+            input_names=self.get_input_names(), 
+            response=None, 
+            time_window=self.time_window, 
+            hp=None, 
+            shuffle=False,
+        )
+        
+        # get outputs for each data point
+        outputs = []
+        for x in tdf:
+            outputs.append(self.instance(x))
+        
+        # if we do not have a distribution layer
+        if not isinstance(outputs[0], tfp.distributions.Distribution):
+            backend.error('Cannot predict distribution for a non-density model. Make sure you choose the right model head.')
+            return None
+        
+        # get array for final results
+        results = []
+
+        # for each value in the samples, calculate the prob of the distribution
+        for value in samples:
+            batch = []
+            for output in outputs:
+                batch.append(tf.exp(output.log_prob(value)))
+            results.append(tf.concat(batch, 0))
+
+        # concat results along the second axis
+        return tf.stack(results, axis=-1)
+    
+    def evaluate(self, data=None, verbose=1):
+        
+        if self.instance is None:
+            backend.error('Cannot evaluate for a NULL instance. Make sure you train the model before invoking.')
+            return None
+        
+        # default to the test set
+        if data is None:
+            data = self.driver.testing_data
+        
+        # build the input dataset from the numpy array
+        tdf = self.driver.get_tensorflow_dataset(
+            data, 
+            input_names=self.get_input_names(), 
+            response=self.response, 
+            time_window=self.time_window, 
+            hp=None, 
+            shuffle=False,
+        )
+        
+        # evalute the results
+        evals = self.instance.evaluate(tdf, verbose=verbose)
+        
+        # pair each result with the metric name
+        res = {}
+        for i in range(len(evals)):
+            res[self.instance.metrics[i].name.strip('_')] = evals[i]
+        
+        return res
+    
+    def report(self, filepath='./model', verbose=0):
+        
+        if self.instance is None:
+            backend.error('Cannot report for a NULL instance. Make sure you train the model before invoking.')
+            return
+        
+        # make sure the directory exists
+        os.makedirs(filepath, exist_ok=True)
+            
+        # readme
+        predictors = []
+        for lyr in self.instance.layers:
+            if lyr.__class__.__name__ == 'InputLayer':
+                predictors.append(lyr.name)
+
+        # check if we have mlflow active
+        active_run = mlflow.active_run() if mlflow is not None else None
+
+        # header and file name
+        fname = backend.join_path(filepath, 'README.md')
+        lines = []
+        lines.append('## Model\n\n')
+        lines.append('This README.md file outlines the parameters and predictors used by the model.\n\n')
+        lines.append('#### Input layers:\n\n')
+        lines.append('* %s\n\n' % '\n* '.join(predictors))
+
+        # save parameters table
+        parameters = self.get_instance_parameters()
+        if len(parameters) > 0:
+            parameters = {k: v for k, v in parameters.items() if not isinstance(v, tuning.HyperVariable)}
+            parameters = pd.DataFrame(list(parameters.items()), columns=['Parameter', 'Value'])
+            lines.append('#### Model parameters:\n\n')
+            lines.append('%s\n\n' % parameters.to_markdown(index=False))
+
+        # save full model scores
+        if self.driver is not None and self.driver.testing_data is not None:
+            scores = self.evaluate(self.driver.testing_data, verbose=verbose)
+            scores = pd.DataFrame(list(scores.items()), columns=['Metric', 'Value'])
+            lines.append('#### Test performance:\n\n')
+            lines.append('%s\n\n' % scores.to_markdown(index=False))
+
+        if active_run is not None:
+            mlflow.log_text(''.join(lines), fname)
+        else:
+            readme = open(fname, "w")
+            readme.write(''.join(lines))
+            readme.close()
+    
+    def get_instance_parameters(self):
+        
+        if self.instance is None:
+            backend.error('Cannot fetch instance parameters for a NULL instance. Make sure you train the model before invoking.')
+            return None
+        
+        tunables = self.get_dependent_tunables()
+        
+        all_params = {}
+        
+        # iterate over each tunable in our dependent stack
+        for tunable in tunables:
+            params = tunable.get_parameters(None)
+            
+            # iterate over all params in the tunable
+            for key, value in params.items():
+                all_params['%s/%s' % (tunable.name, key)] = value
+        
+        return all_params
+
+class ResNet(HyperModel):
+    
+    def __init__(
+        self,
+        response,
+        head,
+        predictors,
+        driver,
+        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
+        blocks=tuning.HyperInt(min_value=0, max_value=6),
+        activation=tuning.HyperChoice(['relu','gelu']),
+        dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        projection_scale=tuning.HyperInt(min_value=1, max_value=4),
+        name='ResNet',
+        **kwargs
+    ):
+        super().__init__(name, response, head, predictors, driver, **kwargs)
+        
+        self.model_dim = model_dim
+        self.blocks = blocks
+        self.activation = activation
+        self.dropout = dropout
+        self.projection_scale = projection_scale
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        config.update({
+            'model_dim' : self._get_hp(None, 'model_dim', hp),
+            'blocks' : self._get_hp(None, 'blocks', hp),
+            'activation' : self._get_hp(None, 'activation', hp),
+            'dropout' : self._get_hp(None, 'dropout', hp),
+            'projection_scale' : self._get_hp(None, 'projection_scale', hp),
+        })
+        return config
+    
+    def body(self, inputs, model_dim, blocks, activation, dropout, projection_scale, **kwargs):
+        
+        # flatten dimensions
+        if len(inputs.shape) > 2:
+            inputs = tf.keras.layers.Flatten()(inputs)
+        
+        # project into model dimension
+        inputs = tf.keras.layers.Dense(model_dim)(inputs)
+        
+        # apply resnet blocks
+        for _ in range(blocks):
+            inputs = layers.ResNetBlock(
+                activation=activation, 
+                dropout=dropout, 
+                projection_scale=projection_scale,
+            )(inputs)
+        
+        # return this body output
+        return inputs
+
+class RNN(HyperModel):
+    
+    def __init__(
+        self,
+        response,
+        head,
+        predictors,
+        driver,
+        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
+        dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        recurrent_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        recurrent_func=tuning.HyperChoice(['SimpleRNN','LSTM','GRU']),
+        name='RNN',
+        **kwargs
+    ):
+        super().__init__(name, response, head, predictors, driver, **kwargs)
+        
+        self.model_dim = model_dim
+        self.dropout = dropout
+        self.recurrent_dropout = recurrent_dropout
+        self.recurrent_func = recurrent_func
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        config.update({
+            'model_dim' : self._get_hp(None, 'model_dim', hp),
+            'dropout' : self._get_hp(None, 'dropout', hp),
+            'recurrent_dropout' : self._get_hp(None, 'recurrent_dropout', hp),
+            'recurrent_func' : self._get_hp(None, 'recurrent_func', hp),
+        })
+        return config
+    
+    def body(self, inputs, model_dim, dropout, recurrent_dropout, recurrent_func, **kwargs):
+        
+        # rnn needs second dimension to be time
+        if len(inputs.shape) <= 2:
+            inputs = tf.expand_dims(inputs, 1)
+            
+        if recurrent_func == 'SimpleRNN':
+            inputs = tf.keras.layers.SimpleRNN(model_dim, dropout=dropout, recurrent_dropout=recurrent_dropout)(inputs)
+        elif recurrent_func == 'LSTM':
+            inputs = tf.keras.layers.LSTM(model_dim, dropout=dropout, recurrent_dropout=recurrent_dropout)(inputs)
+        elif recurrent_func == 'GRU':
+            inputs = tf.keras.layers.GRU(model_dim, dropout=dropout, recurrent_dropout=recurrent_dropout)(inputs)
+        else:
+            backend.error('Recurrent function %s is not known!' % recurrent_func)
+        
+        # return this body output
+        return inputs
+    
+class Transformer(HyperModel):
+    
+    def __init__(
+        self,
+        response,
+        head,
+        predictors,
+        driver,
+        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
+        num_layers=tuning.HyperInt(min_value=1, max_value=6),
+        ffn_activation=tuning.HyperChoice(['relu','gelu']),
+        ffn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        ffn_projection_scale=tuning.HyperInt(min_value=1, max_value=4),
+        num_heads=tuning.HyperInt(min_value=1, max_value=5),
+        attn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        name='Transformer',
+        **kwargs
+    ):
+        super().__init__(name, response, head, predictors, driver, **kwargs)
+        
+        self.model_dim = model_dim
+        self.num_layers = num_layers
+        self.ffn_activation = ffn_activation
+        self.ffn_dropout = ffn_dropout
+        self.ffn_projection_scale = ffn_projection_scale
+        self.num_heads = num_heads
+        self.attn_dropout = attn_dropout
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        config.update({
+            'model_dim' : self._get_hp(None, 'model_dim', hp),
+            'num_layers' : self._get_hp(None, 'num_layers', hp),
+            'ffn_activation' : self._get_hp(None, 'ffn_activation', hp),
+            'ffn_dropout' : self._get_hp(None, 'ffn_dropout', hp),
+            'ffn_projection_scale' : self._get_hp(None, 'ffn_projection_scale', hp),
+            'num_heads' : self._get_hp(None, 'num_heads', hp),
+            'attn_dropout' : self._get_hp(None, 'attn_dropout', hp),
+        })
+        return config
+    
+    def body(
+        self, 
+        inputs, 
+        model_dim, 
+        num_layers, 
+        ffn_activation, 
+        ffn_dropout, 
+        ffn_projection_scale, 
+        num_heads, 
+        attn_dropout, 
+        **kwargs
+    ):
+        
+        # transformer needs data with at least 3 dimensions
+        if len(inputs.shape) <= 2:
+            inputs = tf.expand_dims(inputs, -1)
+            
+        # linear projection and positional encoding
+        inputs = layers.ChunkEmbedding(model_dim)(inputs)
+
+        # transformer layer
+        inputs = layers.Transformer(
+            num_layers=num_layers,
+            ffn_activation=ffn_activation,
+            ffn_dropout=ffn_dropout,
+            ffn_projection_scale=ffn_projection_scale,
+            num_heads=num_heads,
+            attn_dropout=attn_dropout,
+        )(inputs)
+        
+        # global average pool results
+        inputs = tf.keras.layers.GlobalAveragePooling1D()(inputs)
+        
+        # return this body output
+        return inputs
+
+class TransformerLong(HyperModel):
+    
+    def __init__(
+        self,
+        response,
+        head,
+        predictors,
+        driver,
+        chunk_size,
+        model_dim=tuning.HyperChoice([4, 8, 16, 32, 64, 128, 256, 512]),
+        xattn_rate=tuning.HyperInt(min_value=2, max_value=4),
+        num_layers=tuning.HyperInt(min_value=1, max_value=6),
+        ffn_activation=tuning.HyperChoice(['relu','gelu']),
+        ffn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        ffn_projection_scale=tuning.HyperInt(min_value=1, max_value=4),
+        num_heads=tuning.HyperInt(min_value=1, max_value=5),
+        attn_dropout=tuning.HyperFloat(min_value=0.0, max_value=0.4, step=0.1),
+        name='TransformerLong',
+        **kwargs
+    ):
+        super().__init__(name, response, head, predictors, driver, **kwargs)
+        
+        self.chunk_size = chunk_size
+        self.model_dim = model_dim
+        self.xattn_rate = xattn_rate
+        self.num_layers = num_layers
+        self.ffn_activation = ffn_activation
+        self.ffn_dropout = ffn_dropout
+        self.ffn_projection_scale = ffn_projection_scale
+        self.num_heads = num_heads
+        self.attn_dropout = attn_dropout
+    
+    def get_parameters(self, hp):
+        config = super().get_parameters(hp)
+        config.update({
+            'model_dim' : self._get_hp(None, 'model_dim', hp),
+            'xattn_rate' : self._get_hp(None, 'xattn_rate', hp),
+            'num_layers' : self._get_hp(None, 'num_layers', hp),
+            'ffn_activation' : self._get_hp(None, 'ffn_activation', hp),
+            'ffn_dropout' : self._get_hp(None, 'ffn_dropout', hp),
+            'ffn_projection_scale' : self._get_hp(None, 'ffn_projection_scale', hp),
+            'num_heads' : self._get_hp(None, 'num_heads', hp),
+            'attn_dropout' : self._get_hp(None, 'attn_dropout', hp),
+        })
+        return config
+    
+    def body(
+        self, 
+        inputs, 
+        model_dim, 
+        xattn_rate,
+        num_layers, 
+        ffn_activation, 
+        ffn_dropout, 
+        ffn_projection_scale, 
+        num_heads, 
+        attn_dropout, 
+        **kwargs
+    ):
+        
+        # transformer needs data with at least 3 dimensions
+        if len(inputs.shape) <= 2:
+            inputs = tf.expand_dims(inputs, -1)
+            
+        # linear projection and positional encoding
+        inputs = layers.ChunkEmbedding(model_dim, self.chunk_size)(inputs)
+
+        # transformer layer
+        inputs = tf.keras.layers.RNN(layers.TransformerRecurrentCell(
+            chunk_size=self.chunk_size,
+            model_dim=model_dim,
+            xattn_rate=xattn_rate,
+            num_layers=num_layers,
+            ffn_activation=ffn_activation,
+            ffn_dropout=ffn_dropout,
+            ffn_projection_scale=ffn_projection_scale,
+            num_heads=num_heads,
+            attn_dropout=attn_dropout,
+        ))(inputs)
+        
+        # global average pool results
+        inputs = tf.keras.layers.GlobalAveragePooling1D()(inputs)
+        
+        # return this body output
         return inputs
```

### Comparing `quik-ai-1.3.0/src/quik_ai/optimizers.py` & `quik-ai-1.3.1/src/quik_ai/optimizers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/src/quik_ai/predictors.py` & `quik-ai-1.3.1/src/quik_ai/predictors.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/src/quik_ai/tuners.py` & `quik-ai-1.3.1/src/quik_ai/tuners.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/src/quik_ai/tuning.py` & `quik-ai-1.3.1/src/quik_ai/tuning.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.3.0/src/quik_ai.egg-info/PKG-INFO` & `quik-ai-1.3.1/src/quik_ai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.3.1.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,14 +35,15 @@
 3. Specify the predictors used for model fitting.
 ```python
 # All the predictors for the model.
 predictors = [
     qa.predictors.Numerical('numerical'),
     qa.predictors.Categorical('categorical'),
     qa.predictors.Periodic('periodic', 24.0),
+    qa.predictors.Image('image'),
 ]
 ```
 
 4. Select the model architecture.
 ```python
 # Select the architecture and feed the response column, and other
 # necessary data for training, testing the model.
```

