# Comparing `tmp/tibert-0.0.2.tar.gz` & `tmp/tibert-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibert-0.0.2.tar", max compression
+gzip compressed data, was "tibert-0.0.3.tar", max compression
```

## Comparing `tibert-0.0.2.tar` & `tibert-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-04 10:22:09.254266 tibert-0.0.2/LICENSE
--rw-r--r--   0        0        0     5929 2023-07-04 12:51:01.410790 tibert-0.0.2/README.md
--rw-r--r--   0        0        0      600 2023-07-04 14:21:39.083284 tibert-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      141 2023-07-04 12:15:55.862129 tibert-0.0.2/tibert/__init__.py
--rw-r--r--   0        0        0    49687 2023-07-04 13:15:45.925452 tibert-0.0.2/tibert/bertcoref.py
--rw-r--r--   0        0        0     3176 2023-07-04 12:16:01.266205 tibert-0.0.2/tibert/predict.py
--rw-r--r--   0        0        0     2298 2023-07-04 10:26:10.637292 tibert-0.0.2/tibert/run_train.py
--rw-r--r--   0        0        0     4530 2023-07-04 12:16:20.738479 tibert-0.0.2/tibert/score.py
--rw-r--r--   0        0        0     5792 2023-07-04 10:26:09.773280 tibert-0.0.2/tibert/train.py
--rw-r--r--   0        0        0     4417 2023-07-04 12:40:38.986271 tibert-0.0.2/tibert/utils.py
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 tibert-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 10:22:09.254266 tibert-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5929 2023-07-04 12:51:01.410790 tibert-0.0.3/README.md
+-rw-r--r--   0        0        0      600 2023-07-04 15:09:36.658247 tibert-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-07-04 12:15:55.862129 tibert-0.0.3/tibert/__init__.py
+-rw-r--r--   0        0        0    50015 2023-07-04 15:08:45.449549 tibert-0.0.3/tibert/bertcoref.py
+-rw-r--r--   0        0        0     3176 2023-07-04 12:16:01.266205 tibert-0.0.3/tibert/predict.py
+-rw-r--r--   0        0        0     2298 2023-07-04 10:26:10.637292 tibert-0.0.3/tibert/run_train.py
+-rw-r--r--   0        0        0     4530 2023-07-04 12:16:20.738479 tibert-0.0.3/tibert/score.py
+-rw-r--r--   0        0        0     5792 2023-07-04 10:26:09.773280 tibert-0.0.3/tibert/train.py
+-rw-r--r--   0        0        0     4417 2023-07-04 12:40:38.986271 tibert-0.0.3/tibert/utils.py
+-rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 tibert-0.0.3/PKG-INFO
```

### Comparing `tibert-0.0.2/LICENSE` & `tibert-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/README.md` & `tibert-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/pyproject.toml` & `tibert-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibert"
-version = "0.0.2"
+version = "0.0.3"
 description = "BERT for Coreference Resolution"
 authors = ["Arthur Amalvy <arthur.amalvy@univ-avignon.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "tibert" }
 ]
```

### Comparing `tibert-0.0.2/tibert/bertcoref.py` & `tibert-0.0.3/tibert/bertcoref.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,22 +282,29 @@
             if "mention_labels" in features[0].keys()
             else None
         )
         assert (coref_labels is None and mention_labels is None) or (
             coref_labels and mention_labels
         )
 
+        warning_state = self.tokenizer.deprecation_warnings.get(
+            "Asking-to-pad-a-fast-tokenizer", False
+        )
+        self.tokenizer.deprecation_warnings["Asking-to-pad-a-fast-tokenizer"] = True
         batch = self.tokenizer.pad(
             features,
             padding=self.padding,
             max_length=self.max_length,
             # Conversion to tensors will fail if we have labels as
             # they are not of the same length yet.
             return_tensors="pt" if coref_labels is None else None,
         )
+        self.tokenizer.deprecation_warnings[
+            "Asking-to-pad-a-fast-tokenizer"
+        ] = warning_state
 
         # keep encoding info
         batch._encodings = [f.encodings[0] for f in features]
 
         if coref_labels is None:
             return batch
```

### Comparing `tibert-0.0.2/tibert/predict.py` & `tibert-0.0.3/tibert/predict.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/tibert/run_train.py` & `tibert-0.0.3/tibert/run_train.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/tibert/score.py` & `tibert-0.0.3/tibert/score.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/tibert/train.py` & `tibert-0.0.3/tibert/train.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/tibert/utils.py` & `tibert-0.0.3/tibert/utils.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.2/PKG-INFO` & `tibert-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibert
-Version: 0.0.2
+Version: 0.0.3
 Summary: BERT for Coreference Resolution
 License: GPL-3.0-only
 Author: Arthur Amalvy
 Author-email: arthur.amalvy@univ-avignon.fr
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

