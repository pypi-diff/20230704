# Comparing `tmp/torchility-0.7.6.tar.gz` & `tmp/torchility-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.7.6.tar", last modified: Sun Jul  2 14:17:44 2023, max compression
+gzip compressed data, was "torchility-0.7.7.tar", last modified: Mon Jul  3 13:25:23 2023, max compression
```

## Comparing `torchility-0.7.6.tar` & `torchility-0.7.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.282322 torchility-0.7.6/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.6/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-02 14:17:44.281961 torchility-0.7.6/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1716 2023-06-02 07:34:33.000000 torchility-0.7.6/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.256166 torchility-0.7.6/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.6/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.6/examples/10-model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.6/examples/11-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2608 2023-07-02 14:13:43.000000 torchility-0.7.6/examples/2-metrics_basic.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.6/examples/3-metrics_more.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.6/examples/4-callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.6/examples/5-lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.6/examples/6-optimizer.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.6/examples/7-interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.6/examples/8-multi_dataloaders.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.6/examples/9-reset_train_dataloader.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.257313 torchility-0.7.6/imgs/
--rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.6/imgs/data_flow.png
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-07-02 14:17:44.282531 torchility-0.7.6/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.6/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.270276 torchility-0.7.6/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-07-02 14:16:15.000000 torchility-0.7.6/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.274424 torchility-0.7.6/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.6/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.6/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.6/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.6/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9798 2023-07-02 14:11:37.000000 torchility-0.7.6/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.6/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.6/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.6/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.6/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5811 2023-06-27 04:58:49.000000 torchility-0.7.6/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.6/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.281012 torchility-0.7.6/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       97 2023-05-28 01:59:22.000000 torchility-0.7.6/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2645 2023-06-27 06:54:19.000000 torchility-0.7.6/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.6/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.6/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.6/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 14:17:44.272295 torchility-0.7.6/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-02 14:17:43.000000 torchility-0.7.6/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      998 2023-07-02 14:17:44.000000 torchility-0.7.6/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-07-02 14:17:43.000000 torchility-0.7.6/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-07-02 14:17:43.000000 torchility-0.7.6/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-07-02 14:17:43.000000 torchility-0.7.6/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.667205 torchility-0.7.7/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.7/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-03 13:25:23.666645 torchility-0.7.7/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1716 2023-06-02 07:34:33.000000 torchility-0.7.7/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.643580 torchility-0.7.7/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.7/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.7/examples/10-model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.7/examples/11-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2608 2023-07-02 14:13:43.000000 torchility-0.7.7/examples/2-metrics_basic.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.7/examples/3-metrics_more.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.7/examples/4-callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.7/examples/5-lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.7/examples/6-optimizer.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.7/examples/7-interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.7/examples/8-multi_dataloaders.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.7/examples/9-reset_train_dataloader.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.645018 torchility-0.7.7/imgs/
+-rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.7/imgs/data_flow.png
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-07-03 13:25:23.667406 torchility-0.7.7/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.7/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.654836 torchility-0.7.7/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-07-03 13:24:50.000000 torchility-0.7.7/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.662160 torchility-0.7.7/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.7/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.7/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.7/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.7/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9798 2023-07-02 14:11:37.000000 torchility-0.7.7/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.7/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.7/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.7/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.7/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5811 2023-06-27 04:58:49.000000 torchility-0.7.7/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.7/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.665855 torchility-0.7.7/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       97 2023-05-28 01:59:22.000000 torchility-0.7.7/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2645 2023-06-27 06:54:19.000000 torchility-0.7.7/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.7/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.7/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3160 2023-07-03 13:23:54.000000 torchility-0.7.7/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-03 13:25:23.657391 torchility-0.7.7/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-03 13:25:23.000000 torchility-0.7.7/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      998 2023-07-03 13:25:23.000000 torchility-0.7.7/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-07-03 13:25:23.000000 torchility-0.7.7/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-07-03 13:25:23.000000 torchility-0.7.7/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-07-03 13:25:23.000000 torchility-0.7.7/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.7.6/LICENSE` & `torchility-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/PKG-INFO` & `torchility-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.6
+Version: 0.7.7
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.7.6/README.md` & `torchility-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/1-mnist.py` & `torchility-0.7.7/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/10-model_analysis.py` & `torchility-0.7.7/examples/10-model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/11-graph_node_clasification_DGL.py` & `torchility-0.7.7/examples/11-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/2-metrics_basic.py` & `torchility-0.7.7/examples/2-metrics_basic.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/3-metrics_more.py` & `torchility-0.7.7/examples/3-metrics_more.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/4-callbacks.py` & `torchility-0.7.7/examples/4-callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/5-lr_find.py` & `torchility-0.7.7/examples/5-lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/6-optimizer.py` & `torchility-0.7.7/examples/6-optimizer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/7-interpreter.py` & `torchility-0.7.7/examples/7-interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/8-multi_dataloaders.py` & `torchility-0.7.7/examples/8-multi_dataloaders.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/examples/9-reset_train_dataloader.py` & `torchility-0.7.7/examples/9-reset_train_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/imgs/data_flow.png` & `torchility-0.7.7/imgs/data_flow.png`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/setup.py` & `torchility-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/callbacks/common.py` & `torchility-0.7.7/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/callbacks/interpreters.py` & `torchility-0.7.7/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/callbacks/performances.py` & `torchility-0.7.7/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/callbacks/progress.py` & `torchility-0.7.7/torchility/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/datamodule.py` & `torchility-0.7.7/torchility/datamodule.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/hooks.py` & `torchility-0.7.7/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/losses.py` & `torchility-0.7.7/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/metrics.py` & `torchility-0.7.7/torchility/metrics.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/tasks.py` & `torchility-0.7.7/torchility/tasks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/trainer.py` & `torchility-0.7.7/torchility/trainer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/utils/metric_utils.py` & `torchility-0.7.7/torchility/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/utils/plots.py` & `torchility-0.7.7/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/utils/utils.py` & `torchility-0.7.7/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.6/torchility/utils/yaml_config.py` & `torchility-0.7.7/torchility/utils/yaml_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,20 +35,25 @@
     def str_fn(loader, node):
         items = loader.construct_sequence(node)
         return ''.join([str(item) for item in items])
     
     def echo_fn(loader, node):
         seq = loader.construct_sequence(node)
         return seq[0]
+    
+    def sum_fn(loader, node):
+        seq = loader.construct_sequence(node)
+        return sum(seq)
 
     yaml.add_constructor('!path', path_fn)
     yaml.add_constructor('!join', path_fn)  # forward compatible
     yaml.add_constructor('!str', str_fn)
     yaml.add_constructor('!cat', str_fn)    # forward compatible
     yaml.add_constructor('!echo', echo_fn)
+    yaml.add_constructor('!sum', sum_fn)
 
     with open(yaml_path, 'r', encoding=encoding) as f:
         cfg = yaml.load(f, Loader=yaml.FullLoader)
 
     return ddict(cfg)
```

### Comparing `torchility-0.7.6/torchility.egg-info/PKG-INFO` & `torchility-0.7.7/torchility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.6
+Version: 0.7.7
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.7.6/torchility.egg-info/SOURCES.txt` & `torchility-0.7.7/torchility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

