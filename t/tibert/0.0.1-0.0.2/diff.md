# Comparing `tmp/tibert-0.0.1.tar.gz` & `tmp/tibert-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibert-0.0.1.tar", max compression
+gzip compressed data, was "tibert-0.0.2.tar", max compression
```

## Comparing `tibert-0.0.1.tar` & `tibert-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-04 10:22:09.254266 tibert-0.0.1/LICENSE
--rw-r--r--   0        0        0     5929 2023-07-04 12:51:01.410790 tibert-0.0.1/README.md
--rw-r--r--   0        0        0      600 2023-07-04 10:26:11.153299 tibert-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      141 2023-07-04 12:15:55.862129 tibert-0.0.1/tibert/__init__.py
--rw-r--r--   0        0        0    49687 2023-07-04 12:38:28.504506 tibert-0.0.1/tibert/bertcoref.py
--rw-r--r--   0        0        0     3176 2023-07-04 12:16:01.266205 tibert-0.0.1/tibert/predict.py
--rw-r--r--   0        0        0     2298 2023-07-04 10:26:10.637292 tibert-0.0.1/tibert/run_train.py
--rw-r--r--   0        0        0     4530 2023-07-04 12:16:20.738479 tibert-0.0.1/tibert/score.py
--rw-r--r--   0        0        0     5792 2023-07-04 10:26:09.773280 tibert-0.0.1/tibert/train.py
--rw-r--r--   0        0        0     4417 2023-07-04 12:40:38.986271 tibert-0.0.1/tibert/utils.py
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 tibert-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 10:22:09.254266 tibert-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5929 2023-07-04 12:51:01.410790 tibert-0.0.2/README.md
+-rw-r--r--   0        0        0      600 2023-07-04 14:21:39.083284 tibert-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-07-04 12:15:55.862129 tibert-0.0.2/tibert/__init__.py
+-rw-r--r--   0        0        0    49687 2023-07-04 13:15:45.925452 tibert-0.0.2/tibert/bertcoref.py
+-rw-r--r--   0        0        0     3176 2023-07-04 12:16:01.266205 tibert-0.0.2/tibert/predict.py
+-rw-r--r--   0        0        0     2298 2023-07-04 10:26:10.637292 tibert-0.0.2/tibert/run_train.py
+-rw-r--r--   0        0        0     4530 2023-07-04 12:16:20.738479 tibert-0.0.2/tibert/score.py
+-rw-r--r--   0        0        0     5792 2023-07-04 10:26:09.773280 tibert-0.0.2/tibert/train.py
+-rw-r--r--   0        0        0     4417 2023-07-04 12:40:38.986271 tibert-0.0.2/tibert/utils.py
+-rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 tibert-0.0.2/PKG-INFO
```

### Comparing `tibert-0.0.1/LICENSE` & `tibert-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/README.md` & `tibert-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/pyproject.toml` & `tibert-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibert"
-version = "0.0.1"
+version = "0.0.2"
 description = "BERT for Coreference Resolution"
 authors = ["Arthur Amalvy <arthur.amalvy@univ-avignon.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "tibert" }
 ]
```

### Comparing `tibert-0.0.1/tibert/bertcoref.py` & `tibert-0.0.2/tibert/bertcoref.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         ]
 
         new_chains = []
         for chain in self.coref_chains:
             new_chain = []
             for mention in chain:
                 new_start_idx = wp_to_token[mention.start_idx]
-                new_end_idx = wp_to_token[mention.end_idx]
+                new_end_idx = wp_to_token[mention.end_idx - 1] + 1
                 new_chain.append(
                     Mention(
                         tokens[new_start_idx:new_end_idx],
                         new_start_idx,
                         new_end_idx,
                     )
                 )
@@ -653,15 +653,15 @@
 
                 span_idx = int(self.top_mentions_index[b_i][m_j].item())
                 span_coords = spans_idx[span_idx]
 
                 top_antecedent_idx = int(antecedents_idx[b_i][m_j].item())
 
                 span_mention = Mention(
-                    tokens[b_i][span_coords[0] : span_coords[1] + 1],
+                    tokens[b_i][span_coords[0] : span_coords[1]],
                     span_coords[0],
                     span_coords[1],
                 )
 
                 # the antecedent is the dummy mention : maybe we have
                 # a one-mention chain ?
                 if top_antecedent_idx == antecedents_nb - 1:
@@ -672,15 +672,15 @@
                 antecedent_idx = int(
                     self.top_antecedents_index[b_i][m_j][top_antecedent_idx].item()
                 )
 
                 antecedent_coords = spans_idx[antecedent_idx]
 
                 antecedent_mention = Mention(
-                    tokens[b_i][antecedent_coords[0] : antecedent_coords[1] + 1],
+                    tokens[b_i][antecedent_coords[0] : antecedent_coords[1]],
                     antecedent_coords[0],
                     antecedent_coords[1],
                 )
 
                 G.add_node(antecedent_mention)
                 G.add_node(span_mention)
                 G.add_edge(antecedent_mention, span_mention)
```

### Comparing `tibert-0.0.1/tibert/predict.py` & `tibert-0.0.2/tibert/predict.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/tibert/run_train.py` & `tibert-0.0.2/tibert/run_train.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/tibert/score.py` & `tibert-0.0.2/tibert/score.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/tibert/train.py` & `tibert-0.0.2/tibert/train.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/tibert/utils.py` & `tibert-0.0.2/tibert/utils.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.1/PKG-INFO` & `tibert-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibert
-Version: 0.0.1
+Version: 0.0.2
 Summary: BERT for Coreference Resolution
 License: GPL-3.0-only
 Author: Arthur Amalvy
 Author-email: arthur.amalvy@univ-avignon.fr
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

