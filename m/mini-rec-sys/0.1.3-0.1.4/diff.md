# Comparing `tmp/mini_rec_sys-0.1.3.tar.gz` & `tmp/mini_rec_sys-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_rec_sys-0.1.3.tar", max compression
+gzip compressed data, was "mini_rec_sys-0.1.4.tar", max compression
```

## Comparing `mini_rec_sys-0.1.3.tar` & `mini_rec_sys-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.3/LICENSE
--rw-r--r--   0        0        0       80 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.3/README.md
--rw-r--r--   0        0        0       34 2023-07-04 13:26:00.281003 mini_rec_sys-0.1.3/mini_rec_sys/__init__.py
--rw-r--r--   0        0        0      307 2023-07-03 06:46:57.470897 mini_rec_sys-0.1.3/mini_rec_sys/constants.py
--rw-r--r--   0        0        0      207 2023-07-04 13:32:02.158793 mini_rec_sys-0.1.3/mini_rec_sys/data/__init__.py
--rw-r--r--   0        0        0    12158 2023-07-04 13:57:02.362213 mini_rec_sys-0.1.3/mini_rec_sys/data/datasets.py
--rw-r--r--   0        0        0     3459 2023-07-04 13:35:58.865909 mini_rec_sys-0.1.3/mini_rec_sys/data/samplers.py
--rw-r--r--   0        0        0     3118 2023-07-04 13:40:47.185166 mini_rec_sys-0.1.3/mini_rec_sys/data/session.py
--rw-r--r--   0        0        0      192 2023-06-19 13:19:40.483582 mini_rec_sys-0.1.3/mini_rec_sys/encoders/__init__.py
--rw-r--r--   0        0        0     3988 2023-07-04 13:36:13.637863 mini_rec_sys-0.1.3/mini_rec_sys/encoders/encoders.py
--rw-r--r--   0        0        0       67 2023-06-21 08:07:03.673242 mini_rec_sys-0.1.3/mini_rec_sys/evaluators/__init__.py
--rw-r--r--   0        0        0     3101 2023-07-04 13:36:21.709839 mini_rec_sys-0.1.3/mini_rec_sys/evaluators/evaluators.py
--rw-r--r--   0        0        0      104 2023-07-04 13:36:34.717800 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/__init__.py
--rw-r--r--   0        0        0       11 2023-06-22 06:56:10.980380 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/.gitignore
--rw-r--r--   0        0        0      598 2023-06-21 06:34:09.426466 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/README.md
--rw-r--r--   0        0        0        0 2023-06-30 12:33:27.541877 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/__init__.py
--rwxr-xr-x   0        0        0      460 2023-06-22 06:59:57.131792 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/download.sh
--rw-r--r--   0        0        0     3494 2023-06-30 12:38:41.845286 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py
--rw-r--r--   0        0        0   190171 2023-06-22 03:15:42.162087 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json
--rw-r--r--   0        0        0    12085 2023-06-22 03:11:30.984882 mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json
--rw-r--r--   0        0        0     6544 2023-07-04 13:41:57.749021 mini_rec_sys-0.1.3/mini_rec_sys/scorers/BM25Scorer.py
--rw-r--r--   0        0        0      816 2023-06-21 07:13:42.549019 mini_rec_sys-0.1.3/mini_rec_sys/scorers/BaseScorer.py
--rw-r--r--   0        0        0     3813 2023-07-04 13:42:09.044999 mini_rec_sys-0.1.3/mini_rec_sys/scorers/DenseScorer.py
--rw-r--r--   0        0        0      107 2023-06-28 08:17:20.287340 mini_rec_sys-0.1.3/mini_rec_sys/scorers/__init__.py
--rw-r--r--   0        0        0     9473 2023-07-04 13:42:55.113376 mini_rec_sys-0.1.3/mini_rec_sys/trainers/DPRModel.py
--rw-r--r--   0        0        0       75 2023-06-28 04:49:24.386866 mini_rec_sys-0.1.3/mini_rec_sys/trainers/__init__.py
--rw-r--r--   0        0        0     5384 2023-07-04 13:42:44.465071 mini_rec_sys-0.1.3/mini_rec_sys/trainers/base_trainers.py
--rw-r--r--   0        0        0     3337 2023-07-04 13:43:08.685757 mini_rec_sys-0.1.3/mini_rec_sys/utils.py
--rw-r--r--   0        0        0      727 2023-07-04 13:57:22.714362 mini_rec_sys-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.4/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.4/README.md
+-rw-r--r--   0        0        0       34 2023-07-04 13:26:00.281003 mini_rec_sys-0.1.4/mini_rec_sys/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-03 06:46:57.470897 mini_rec_sys-0.1.4/mini_rec_sys/constants.py
+-rw-r--r--   0        0        0      207 2023-07-04 13:32:02.158793 mini_rec_sys-0.1.4/mini_rec_sys/data/__init__.py
+-rw-r--r--   0        0        0    12157 2023-07-04 14:10:59.870343 mini_rec_sys-0.1.4/mini_rec_sys/data/datasets.py
+-rw-r--r--   0        0        0     3459 2023-07-04 13:35:58.865909 mini_rec_sys-0.1.4/mini_rec_sys/data/samplers.py
+-rw-r--r--   0        0        0     3118 2023-07-04 13:40:47.185166 mini_rec_sys-0.1.4/mini_rec_sys/data/session.py
+-rw-r--r--   0        0        0      192 2023-06-19 13:19:40.483582 mini_rec_sys-0.1.4/mini_rec_sys/encoders/__init__.py
+-rw-r--r--   0        0        0     3988 2023-07-04 13:36:13.637863 mini_rec_sys-0.1.4/mini_rec_sys/encoders/encoders.py
+-rw-r--r--   0        0        0       67 2023-06-21 08:07:03.673242 mini_rec_sys-0.1.4/mini_rec_sys/evaluators/__init__.py
+-rw-r--r--   0        0        0     3101 2023-07-04 13:36:21.709839 mini_rec_sys-0.1.4/mini_rec_sys/evaluators/evaluators.py
+-rw-r--r--   0        0        0      104 2023-07-04 13:36:34.717800 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/__init__.py
+-rw-r--r--   0        0        0       11 2023-06-22 06:56:10.980380 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/.gitignore
+-rw-r--r--   0        0        0      598 2023-06-21 06:34:09.426466 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 12:33:27.541877 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/__init__.py
+-rwxr-xr-x   0        0        0      460 2023-06-22 06:59:57.131792 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/download.sh
+-rw-r--r--   0        0        0     3494 2023-06-30 12:38:41.845286 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py
+-rw-r--r--   0        0        0   190171 2023-06-22 03:15:42.162087 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json
+-rw-r--r--   0        0        0    12085 2023-06-22 03:11:30.984882 mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json
+-rw-r--r--   0        0        0     6544 2023-07-04 13:41:57.749021 mini_rec_sys-0.1.4/mini_rec_sys/scorers/BM25Scorer.py
+-rw-r--r--   0        0        0      816 2023-06-21 07:13:42.549019 mini_rec_sys-0.1.4/mini_rec_sys/scorers/BaseScorer.py
+-rw-r--r--   0        0        0     3813 2023-07-04 13:42:09.044999 mini_rec_sys-0.1.4/mini_rec_sys/scorers/DenseScorer.py
+-rw-r--r--   0        0        0      107 2023-06-28 08:17:20.287340 mini_rec_sys-0.1.4/mini_rec_sys/scorers/__init__.py
+-rw-r--r--   0        0        0     9473 2023-07-04 13:42:55.113376 mini_rec_sys-0.1.4/mini_rec_sys/trainers/DPRModel.py
+-rw-r--r--   0        0        0       75 2023-06-28 04:49:24.386866 mini_rec_sys-0.1.4/mini_rec_sys/trainers/__init__.py
+-rw-r--r--   0        0        0     5384 2023-07-04 13:42:44.465071 mini_rec_sys-0.1.4/mini_rec_sys/trainers/base_trainers.py
+-rw-r--r--   0        0        0     3337 2023-07-04 13:43:08.685757 mini_rec_sys-0.1.4/mini_rec_sys/utils.py
+-rw-r--r--   0        0        0      727 2023-07-04 14:11:12.766387 mini_rec_sys-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.4/PKG-INFO
```

### Comparing `mini_rec_sys-0.1.3/LICENSE` & `mini_rec_sys-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/data/datasets.py` & `mini_rec_sys-0.1.4/mini_rec_sys/data/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         else:
             raise ValueError(f"{data} is neither str nor dict.")
 
         if self.db_location is None:
             print("Initializing cache in temp location..")
             cache = Cache(size_limit=MAX_DISK_SIZE, cull_limit=0)
             self.db_location = cache.directory
-        elif self.db_location.startswith("dbfs:/"):
+        elif self.db_location.startswith("/dbfs"):
             print("On databricks, writing to temp location..")
             cache = Cache(size_limit=MAX_DISK_SIZE, cull_limit=0)
         else:
             cache = Cache(self.db_location, size_limit=MAX_DISK_SIZE, cull_limit=0)
 
         for id, row in tqdm(generator):
             try:
```

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/data/samplers.py` & `mini_rec_sys-0.1.4/mini_rec_sys/data/samplers.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/data/session.py` & `mini_rec_sys-0.1.4/mini_rec_sys/data/session.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/encoders/encoders.py` & `mini_rec_sys-0.1.4/mini_rec_sys/encoders/encoders.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/evaluators/evaluators.py` & `mini_rec_sys-0.1.4/mini_rec_sys/evaluators/evaluators.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/README.md` & `mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/README.md`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py` & `mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json` & `mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json` & `mini_rec_sys-0.1.4/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/scorers/BM25Scorer.py` & `mini_rec_sys-0.1.4/mini_rec_sys/scorers/BM25Scorer.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/scorers/BaseScorer.py` & `mini_rec_sys-0.1.4/mini_rec_sys/scorers/BaseScorer.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/scorers/DenseScorer.py` & `mini_rec_sys-0.1.4/mini_rec_sys/scorers/DenseScorer.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/trainers/DPRModel.py` & `mini_rec_sys-0.1.4/mini_rec_sys/trainers/DPRModel.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/trainers/base_trainers.py` & `mini_rec_sys-0.1.4/mini_rec_sys/trainers/base_trainers.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/mini_rec_sys/utils.py` & `mini_rec_sys-0.1.4/mini_rec_sys/utils.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.3/pyproject.toml` & `mini_rec_sys-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mini-rec-sys"
-version = "0.1.3"
+version = "0.1.4"
 description = "Toolkit to train and evaluate models for search and recommendations."
 authors = ["Charles Low <charleslow88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mini_rec_sys"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mini_rec_sys-0.1.3/PKG-INFO` & `mini_rec_sys-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-rec-sys
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkit to train and evaluate models for search and recommendations.
 License: MIT
 Author: Charles Low
 Author-email: charleslow88@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

