# Comparing `tmp/libmultilabel-0.3.1.tar.gz` & `tmp/libmultilabel-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmultilabel-0.3.1.tar", last modified: Mon Jun 12 14:02:48 2023, max compression
+gzip compressed data, was "libmultilabel-0.3.2.tar", last modified: Tue Jul  4 05:25:37 2023, max compression
```

## Comparing `libmultilabel-0.3.1.tar` & `libmultilabel-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/nn/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/bert_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/caml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/kim_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/labelwise_attention_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/xml_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/nn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 14:02:48.533157 libmultilabel-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:37.365084 libmultilabel-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 05:25:37.365084 libmultilabel-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:37.361084 libmultilabel-0.3.2/libmultilabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:37.361084 libmultilabel-0.3.2/libmultilabel/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/linear/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:37.361084 libmultilabel-0.3.2/libmultilabel/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:37.365084 libmultilabel-0.3.2/libmultilabel/nn/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/bert_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/caml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/kim_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/labelwise_attention_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/networks/xml_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/libmultilabel/nn/nn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:25:37.361084 libmultilabel-0.3.2/libmultilabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 05:25:37.000000 libmultilabel-0.3.2/libmultilabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-04 05:25:37.000000 libmultilabel-0.3.2/libmultilabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:25:37.000000 libmultilabel-0.3.2/libmultilabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 05:25:37.000000 libmultilabel-0.3.2/libmultilabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 05:25:37.000000 libmultilabel-0.3.2/libmultilabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 05:25:26.000000 libmultilabel-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-04 05:25:37.365084 libmultilabel-0.3.2/setup.cfg
```

### Comparing `libmultilabel-0.3.1/LICENSE` & `libmultilabel-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/PKG-INFO` & `libmultilabel-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.3.1/README.md` & `libmultilabel-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/common_utils.py` & `libmultilabel-0.3.2/libmultilabel/common_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/linear/data_utils.py` & `libmultilabel-0.3.2/libmultilabel/linear/data_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/linear/linear.py` & `libmultilabel-0.3.2/libmultilabel/linear/linear.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/linear/metrics.py` & `libmultilabel-0.3.2/libmultilabel/linear/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/linear/preprocessor.py` & `libmultilabel-0.3.2/libmultilabel/linear/preprocessor.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/linear/tree.py` & `libmultilabel-0.3.2/libmultilabel/linear/tree.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/linear/utils.py` & `libmultilabel-0.3.2/libmultilabel/linear/utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/logging.py` & `libmultilabel-0.3.2/libmultilabel/logging.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/data_utils.py` & `libmultilabel-0.3.2/libmultilabel/nn/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,15 +375,24 @@
         logging.info(f"Load pretrained embedding from torchtext.")
         # Adapted from https://pytorch.org/text/0.9.0/_modules/torchtext/vocab.html#Vocab.load_vectors.
         if embed_file not in pretrained_aliases:
             raise ValueError(
                 "Got embed_file {}, but allowed pretrained "
                 "vectors are {}".format(embed_file, list(pretrained_aliases.keys()))
             )
-        vector_dict = pretrained_aliases[embed_file](cache=cache)
+
+        # Hotfix: Glove URLs are outdated in Torchtext
+        # (https://github.com/pytorch/text/blob/main/torchtext/vocab/vectors.py#L213-L217)
+        pretrained_cls = pretrained_aliases[embed_file]
+        if embed_file.startswith("glove"):
+            for name, url in pretrained_cls.func.url.items():
+                file_name = url.split("/")[-1]
+                pretrained_cls.func.url[name] = f"https://huggingface.co/stanfordnlp/glove/resolve/main/{file_name}"
+
+        vector_dict = pretrained_cls(cache=cache)
         embed_size = vector_dict.dim
 
     embedding_weights = torch.zeros(len(word_dict), embed_size)
 
     if load_embedding_from_file:
         # Add UNK embedding
         # AttentionXML: np.random.uniform(-1.0, 1.0, embed_size)
```

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/metrics.py` & `libmultilabel-0.3.2/libmultilabel/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/model.py` & `libmultilabel-0.3.2/libmultilabel/nn/model.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/__init__.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/bert.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/bert.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/bert_attention.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/bert_attention.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/caml.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/caml.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/kim_cnn.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/kim_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/labelwise_attention_networks.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/labelwise_attention_networks.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/modules.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/modules.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/networks/xml_cnn.py` & `libmultilabel-0.3.2/libmultilabel/nn/networks/xml_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel/nn/nn_utils.py` & `libmultilabel-0.3.2/libmultilabel/nn/nn_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/libmultilabel.egg-info/PKG-INFO` & `libmultilabel-0.3.2/libmultilabel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.3.1/libmultilabel.egg-info/SOURCES.txt` & `libmultilabel-0.3.2/libmultilabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.1/setup.cfg` & `libmultilabel-0.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libmultilabel
-version = 0.3.1
+version = 0.3.2
 author = LibMultiLabel Team
 license = MIT License
 license_file = LICENSE
 description = A library for multi-label text classification
 long_description = See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 url = https://github.com/ASUS-AICS/LibMultiLabel
 project_urls =
```

