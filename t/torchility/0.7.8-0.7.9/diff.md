# Comparing `tmp/torchility-0.7.8.tar.gz` & `tmp/torchility-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.7.8.tar", last modified: Tue Jul  4 01:31:45 2023, max compression
+gzip compressed data, was "torchility-0.7.9.tar", last modified: Tue Jul  4 14:49:50 2023, max compression
```

## Comparing `torchility-0.7.8.tar` & `torchility-0.7.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.987336 torchility-0.7.8/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.8/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-04 01:31:45.986777 torchility-0.7.8/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1716 2023-06-02 07:34:33.000000 torchility-0.7.8/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.968061 torchility-0.7.8/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.8/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.8/examples/10-model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.8/examples/11-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2608 2023-07-02 14:13:43.000000 torchility-0.7.8/examples/2-metrics_basic.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.8/examples/3-metrics_more.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.8/examples/4-callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.8/examples/5-lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.8/examples/6-optimizer.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.8/examples/7-interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.8/examples/8-multi_dataloaders.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.8/examples/9-reset_train_dataloader.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.968884 torchility-0.7.8/imgs/
--rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.8/imgs/data_flow.png
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-07-04 01:31:45.987594 torchility-0.7.8/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.8/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.975731 torchility-0.7.8/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-07-04 01:31:17.000000 torchility-0.7.8/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.982735 torchility-0.7.8/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.8/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.8/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.8/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.8/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-07-04 01:31:05.000000 torchility-0.7.8/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.8/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.8/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.8/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.8/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5811 2023-06-27 04:58:49.000000 torchility-0.7.8/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.8/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.986019 torchility-0.7.8/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       97 2023-05-28 01:59:22.000000 torchility-0.7.8/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2645 2023-06-27 06:54:19.000000 torchility-0.7.8/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.8/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.8/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3160 2023-07-03 13:23:54.000000 torchility-0.7.8/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 01:31:45.979666 torchility-0.7.8/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-04 01:31:45.000000 torchility-0.7.8/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      998 2023-07-04 01:31:45.000000 torchility-0.7.8/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-07-04 01:31:45.000000 torchility-0.7.8/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-07-04 01:31:45.000000 torchility-0.7.8/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-07-04 01:31:45.000000 torchility-0.7.8/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.046904 torchility-0.7.9/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.9/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-04 14:49:50.045899 torchility-0.7.9/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1716 2023-06-02 07:34:33.000000 torchility-0.7.9/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.018840 torchility-0.7.9/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.9/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.9/examples/10-model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.9/examples/11-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2608 2023-07-02 14:13:43.000000 torchility-0.7.9/examples/2-metrics_basic.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.9/examples/3-metrics_more.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.9/examples/4-callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.9/examples/5-lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.9/examples/6-optimizer.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.9/examples/7-interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.9/examples/8-multi_dataloaders.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.9/examples/9-reset_train_dataloader.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.020612 torchility-0.7.9/imgs/
+-rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.9/imgs/data_flow.png
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-07-04 14:49:50.047348 torchility-0.7.9/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.9/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.030368 torchility-0.7.9/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-07-04 14:49:23.000000 torchility-0.7.9/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.038704 torchility-0.7.9/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.9/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.9/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.9/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.9/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-07-04 01:31:05.000000 torchility-0.7.9/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.9/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.9/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.9/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.9/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5811 2023-06-27 04:58:49.000000 torchility-0.7.9/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    12817 2023-07-04 14:49:12.000000 torchility-0.7.9/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.043934 torchility-0.7.9/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)      121 2023-07-04 14:44:26.000000 torchility-0.7.9/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2645 2023-06-27 06:54:19.000000 torchility-0.7.9/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      769 2023-07-04 14:44:57.000000 torchility-0.7.9/torchility/utils/model_io.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.9/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.9/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3160 2023-07-03 13:23:54.000000 torchility-0.7.9/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-04 14:49:50.033861 torchility-0.7.9/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-04 14:49:49.000000 torchility-0.7.9/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1027 2023-07-04 14:49:49.000000 torchility-0.7.9/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-07-04 14:49:49.000000 torchility-0.7.9/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-07-04 14:49:49.000000 torchility-0.7.9/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-07-04 14:49:49.000000 torchility-0.7.9/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.7.8/LICENSE` & `torchility-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/PKG-INFO` & `torchility-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.8
+Version: 0.7.9
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.7.8/README.md` & `torchility-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/1-mnist.py` & `torchility-0.7.9/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/10-model_analysis.py` & `torchility-0.7.9/examples/10-model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/11-graph_node_clasification_DGL.py` & `torchility-0.7.9/examples/11-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/2-metrics_basic.py` & `torchility-0.7.9/examples/2-metrics_basic.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/3-metrics_more.py` & `torchility-0.7.9/examples/3-metrics_more.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/4-callbacks.py` & `torchility-0.7.9/examples/4-callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/5-lr_find.py` & `torchility-0.7.9/examples/5-lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/6-optimizer.py` & `torchility-0.7.9/examples/6-optimizer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/7-interpreter.py` & `torchility-0.7.9/examples/7-interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/8-multi_dataloaders.py` & `torchility-0.7.9/examples/8-multi_dataloaders.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/examples/9-reset_train_dataloader.py` & `torchility-0.7.9/examples/9-reset_train_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/imgs/data_flow.png` & `torchility-0.7.9/imgs/data_flow.png`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/setup.py` & `torchility-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/callbacks/common.py` & `torchility-0.7.9/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/callbacks/interpreters.py` & `torchility-0.7.9/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/callbacks/performances.py` & `torchility-0.7.9/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/callbacks/progress.py` & `torchility-0.7.9/torchility/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/datamodule.py` & `torchility-0.7.9/torchility/datamodule.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/hooks.py` & `torchility-0.7.9/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/losses.py` & `torchility-0.7.9/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/metrics.py` & `torchility-0.7.9/torchility/metrics.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/tasks.py` & `torchility-0.7.9/torchility/tasks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/trainer.py` & `torchility-0.7.9/torchility/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pytorch_lightning.callbacks import ProgressBar
 
 from torchmetrics import Metric
 
 from .callbacks import ResetMetrics, SimpleBar
 from .tasks import GeneralTaskModule
 from .callbacks import Progress
-from .utils import batches, set_metric_attr
+from .utils import batches, set_metric_attr, load_state_dict
 from .datamodule import GeneralDataModule
 
 def default_args(func):
     signature = inspect.signature(func)
     return {
         k: v.default
         for k, v in signature.parameters.items()
@@ -241,15 +241,15 @@
         opt = self.task_module.opt
         model =self.task_module.model
         for ckp_path in best_ckp_paths:
             self.task_module.load_from_checkpoint(ckp_path, model=model, loss=loss, optimizer=opt)
             best_models.append(deepcopy(self.task_module.model))
         return best_models
 
-    def save_state_dict(self, path='best_model.pth', mode='best'):
+    def save_torch_state_dict(self, path='best_model.pth', mode='best'):
         """
         Save state_dict of pytorch model.
         Args:
             path: path and filename of the state_dict file.
             mode: 'best' for the best model and others for current model.
         """
         if mode == 'best':
@@ -258,15 +258,25 @@
             opt = self.task_module.opt
             task = self.task_module.load_from_checkpoint(self.checkpoint_callback.best_model_path,
                                                             model=model, loss=loss, optimizer=opt)
             torch.save(task.model.state_dict(), path)
         else:
             torch.save(self.task_module.model.state_dict(), path)
 
-    def load_state_dict(self, path='best_model.pth', model=None):
+    def load_torch_state_dict(self, path='best_model.pth', model=None):
         """load state_dict for pytorch model"""
         if model:
             model.load_state_dict(torch.load(path))
         else:
             self.task_module.model.load_state_dict(torch.load(path))
             model = self.task_module.model
         return model
+
+    @staticmethod
+    def load_state_dict(model, ckpt_path):
+        """
+        load state_dict for pytorch model from pytorch_lightning checkpoint.
+        Args:
+            model: pytorch model
+            ckpt_path: path of pytorch_lightning checkpoint
+        """
+        return load_state_dict(model, ckpt_path)
```

### Comparing `torchility-0.7.8/torchility/utils/metric_utils.py` & `torchility-0.7.9/torchility/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/utils/plots.py` & `torchility-0.7.9/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/utils/utils.py` & `torchility-0.7.9/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility/utils/yaml_config.py` & `torchility-0.7.9/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.8/torchility.egg-info/PKG-INFO` & `torchility-0.7.9/torchility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.8
+Version: 0.7.9
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.7.8/torchility.egg-info/SOURCES.txt` & `torchility-0.7.9/torchility.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 torchility/callbacks/__init__.py
 torchility/callbacks/common.py
 torchility/callbacks/interpreters.py
 torchility/callbacks/performances.py
 torchility/callbacks/progress.py
 torchility/utils/__init__.py
 torchility/utils/metric_utils.py
+torchility/utils/model_io.py
 torchility/utils/plots.py
 torchility/utils/utils.py
 torchility/utils/yaml_config.py
```

