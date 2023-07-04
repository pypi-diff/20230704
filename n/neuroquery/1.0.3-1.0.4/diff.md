# Comparing `tmp/neuroquery-1.0.3.tar.gz` & `tmp/neuroquery-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroquery-1.0.3.tar", last modified: Thu Dec 15 11:18:03 2022, max compression
+gzip compressed data, was "neuroquery-1.0.4.tar", last modified: Tue Jul  4 13:46:32 2023, max compression
```

## Comparing `neuroquery-1.0.3.tar` & `neuroquery-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2022-12-15 11:18:03.690735 neuroquery-1.0.3/
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     1524 2020-05-14 16:20:37.000000 neuroquery-1.0.3/LICENSE
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     4622 2022-12-15 11:18:03.690735 neuroquery-1.0.3/PKG-INFO
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     2575 2022-07-28 19:32:12.000000 neuroquery-1.0.3/README.md
--rw-rw-r--   0 jerome    (1000) jerome    (1000)       89 2022-07-28 19:31:34.000000 neuroquery-1.0.3/pyproject.toml
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      852 2022-12-15 11:18:03.690735 neuroquery-1.0.3/setup.cfg
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      326 2022-07-28 19:31:34.000000 neuroquery-1.0.3/setup.py
-drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2022-12-15 11:18:03.686735 neuroquery-1.0.3/src/
-drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2022-12-15 11:18:03.690735 neuroquery-1.0.3/src/neuroquery/
--rw-rw-r--   0 jerome    (1000) jerome    (1000)        6 2022-12-15 11:11:06.000000 neuroquery-1.0.3/src/neuroquery/VERSION.txt
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      581 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/__init__.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      295 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/_compat.py
-drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2022-12-15 11:18:03.690735 neuroquery-1.0.3/src/neuroquery/data/
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      599 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/data/highlight.xsl
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      743 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/data/nltk_stop_words.txt
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     3256 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/datasets.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)    13047 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/encoding.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     2973 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/img_utils.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     2260 2022-12-14 23:51:49.000000 neuroquery-1.0.3/src/neuroquery/nmf.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)    11574 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/ridge.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     2435 2022-07-28 19:31:34.000000 neuroquery-1.0.3/src/neuroquery/smoothed_regression.py
--rw-rw-r--   0 jerome    (1000) jerome    (1000)    24717 2022-12-15 10:59:24.000000 neuroquery-1.0.3/src/neuroquery/tokenization.py
-drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2022-12-15 11:18:03.690735 neuroquery-1.0.3/src/neuroquery.egg-info/
--rw-rw-r--   0 jerome    (1000) jerome    (1000)     4622 2022-12-15 11:18:03.000000 neuroquery-1.0.3/src/neuroquery.egg-info/PKG-INFO
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      628 2022-12-15 11:18:03.000000 neuroquery-1.0.3/src/neuroquery.egg-info/SOURCES.txt
--rw-rw-r--   0 jerome    (1000) jerome    (1000)        1 2022-12-15 11:18:03.000000 neuroquery-1.0.3/src/neuroquery.egg-info/dependency_links.txt
--rw-rw-r--   0 jerome    (1000) jerome    (1000)        1 2022-07-28 19:21:49.000000 neuroquery-1.0.3/src/neuroquery.egg-info/not-zip-safe
--rw-rw-r--   0 jerome    (1000) jerome    (1000)      159 2022-12-15 11:18:03.000000 neuroquery-1.0.3/src/neuroquery.egg-info/requires.txt
--rw-rw-r--   0 jerome    (1000) jerome    (1000)       11 2022-12-15 11:18:03.000000 neuroquery-1.0.3/src/neuroquery.egg-info/top_level.txt
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2023-07-04 13:46:32.778148 neuroquery-1.0.4/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1524 2023-07-04 13:45:05.000000 neuroquery-1.0.4/LICENSE
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     4622 2023-07-04 13:46:32.778148 neuroquery-1.0.4/PKG-INFO
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2575 2022-07-28 19:32:12.000000 neuroquery-1.0.4/README.md
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)       89 2022-07-28 19:31:34.000000 neuroquery-1.0.4/pyproject.toml
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      852 2023-07-04 13:46:32.782148 neuroquery-1.0.4/setup.cfg
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      326 2022-07-28 19:31:34.000000 neuroquery-1.0.4/setup.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2023-07-04 13:46:32.774148 neuroquery-1.0.4/src/
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2023-07-04 13:46:32.774148 neuroquery-1.0.4/src/neuroquery/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        6 2023-07-04 13:44:34.000000 neuroquery-1.0.4/src/neuroquery/VERSION.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      581 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      295 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/_compat.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2023-07-04 13:46:32.778148 neuroquery-1.0.4/src/neuroquery/data/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      599 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/data/highlight.xsl
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      743 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/data/nltk_stop_words.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3256 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/datasets.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    13047 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/encoding.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2973 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/img_utils.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2260 2022-12-14 23:51:49.000000 neuroquery-1.0.4/src/neuroquery/nmf.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    11574 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/ridge.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2435 2022-07-28 19:31:34.000000 neuroquery-1.0.4/src/neuroquery/smoothed_regression.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    24719 2023-07-04 13:40:41.000000 neuroquery-1.0.4/src/neuroquery/tokenization.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2023-07-04 13:46:32.778148 neuroquery-1.0.4/src/neuroquery.egg-info/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     4622 2023-07-04 13:46:32.000000 neuroquery-1.0.4/src/neuroquery.egg-info/PKG-INFO
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      797 2023-07-04 13:46:32.000000 neuroquery-1.0.4/src/neuroquery.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        1 2023-07-04 13:46:32.000000 neuroquery-1.0.4/src/neuroquery.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        1 2022-07-28 19:21:49.000000 neuroquery-1.0.4/src/neuroquery.egg-info/not-zip-safe
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      159 2023-07-04 13:46:32.000000 neuroquery-1.0.4/src/neuroquery.egg-info/requires.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)       11 2023-07-04 13:46:32.000000 neuroquery-1.0.4/src/neuroquery.egg-info/top_level.txt
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2023-07-04 13:46:32.778148 neuroquery-1.0.4/tests/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2680 2022-07-28 19:31:34.000000 neuroquery-1.0.4/tests/test_datasets.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3640 2022-07-28 19:31:34.000000 neuroquery-1.0.4/tests/test_encoding.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2676 2022-07-28 19:31:34.000000 neuroquery-1.0.4/tests/test_img_utils.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1222 2022-12-15 00:33:06.000000 neuroquery-1.0.4/tests/test_nmf.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     4187 2022-07-28 19:31:34.000000 neuroquery-1.0.4/tests/test_ridge.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1638 2022-07-28 19:31:34.000000 neuroquery-1.0.4/tests/test_smoothed_regression.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    12808 2022-12-15 00:25:08.000000 neuroquery-1.0.4/tests/test_tokenization.py
```

### Comparing `neuroquery-1.0.3/LICENSE` & `neuroquery-1.0.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2019, Jérôme Dockès
+Copyright (c) 2023, Jérôme Dockès
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `neuroquery-1.0.3/PKG-INFO` & `neuroquery-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroquery
-Version: 1.0.3
+Version: 1.0.4
 Summary: Meta-analysis of neuroimaging studies.
 Home-page: https://github.com/neuroquery/neuroquery
 Author: Jérôme Dockès
 Author-email: jerome@dockes.org
 Maintainer: Jérôme Dockès
 Maintainer-email: jerome@dockes.org
 License: BSD 3-Clause License
@@ -83,15 +83,15 @@
 publications' text and stereotactic peak activation coordinates (see
 [`training_neuroquery.ipynb`](https://nbviewer.jupyter.org/github/neuroquery/neuroquery/blob/main/examples/training_neuroquery.ipynb)
 in the examples).
 
 
 BSD 3-Clause License
 
-Copyright (c) 2019, Jérôme Dockès
+Copyright (c) 2023, Jérôme Dockès
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `neuroquery-1.0.3/README.md` & `neuroquery-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/setup.cfg` & `neuroquery-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/__init__.py` & `neuroquery-1.0.4/src/neuroquery/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/data/highlight.xsl` & `neuroquery-1.0.4/src/neuroquery/data/highlight.xsl`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/data/nltk_stop_words.txt` & `neuroquery-1.0.4/src/neuroquery/data/nltk_stop_words.txt`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/datasets.py` & `neuroquery-1.0.4/src/neuroquery/datasets.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/encoding.py` & `neuroquery-1.0.4/src/neuroquery/encoding.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/img_utils.py` & `neuroquery-1.0.4/src/neuroquery/img_utils.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/nmf.py` & `neuroquery-1.0.4/src/neuroquery/nmf.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/ridge.py` & `neuroquery-1.0.4/src/neuroquery/ridge.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/smoothed_regression.py` & `neuroquery-1.0.4/src/neuroquery/smoothed_regression.py`

 * *Files identical despite different names*

### Comparing `neuroquery-1.0.3/src/neuroquery/tokenization.py` & `neuroquery-1.0.4/src/neuroquery/tokenization.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,15 +727,15 @@
     def to_vocabulary_file(self, voc_file):
         return self.tokenizer.to_vocabulary_file(voc_file)
 
     def fit(self, *args, **kwargs):
         self.counter_ = CountVectorizer(
             analyzer=self.tokenizer,
             vocabulary=self.tokenizer.get_vocabulary(),
-            min_df=0,
+            min_df=0.0,
         ).fit([])
         if self.use_idf:
             self.idf_ = -np.log(self.tokenizer.get_frequencies()) + 1
             self._idf_diag = sparse.spdiags(
                 self.idf_,
                 diags=0,
                 m=self.idf_.shape[0],
```

### Comparing `neuroquery-1.0.3/src/neuroquery.egg-info/PKG-INFO` & `neuroquery-1.0.4/src/neuroquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroquery
-Version: 1.0.3
+Version: 1.0.4
 Summary: Meta-analysis of neuroimaging studies.
 Home-page: https://github.com/neuroquery/neuroquery
 Author: Jérôme Dockès
 Author-email: jerome@dockes.org
 Maintainer: Jérôme Dockès
 Maintainer-email: jerome@dockes.org
 License: BSD 3-Clause License
@@ -83,15 +83,15 @@
 publications' text and stereotactic peak activation coordinates (see
 [`training_neuroquery.ipynb`](https://nbviewer.jupyter.org/github/neuroquery/neuroquery/blob/main/examples/training_neuroquery.ipynb)
 in the examples).
 
 
 BSD 3-Clause License
 
-Copyright (c) 2019, Jérôme Dockès
+Copyright (c) 2023, Jérôme Dockès
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

