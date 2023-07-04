# Comparing `tmp/mini_rec_sys-0.1.0.tar.gz` & `tmp/mini_rec_sys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_rec_sys-0.1.0.tar", max compression
+gzip compressed data, was "mini_rec_sys-0.1.1.tar", max compression
```

## Comparing `mini_rec_sys-0.1.0.tar` & `mini_rec_sys-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.0/LICENSE
--rw-r--r--   0        0        0       80 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-21 01:39:12.515507 mini_rec_sys-0.1.0/mini_rec_sys/__init__.py
--rw-r--r--   0        0        0      107 2023-06-30 08:08:20.124764 mini_rec_sys-0.1.0/mini_rec_sys/constants.py
--rw-r--r--   0        0        0      148 2023-06-28 02:48:13.405018 mini_rec_sys-0.1.0/mini_rec_sys/data/__init__.py
--rw-r--r--   0        0        0    10986 2023-06-30 08:20:28.517286 mini_rec_sys-0.1.0/mini_rec_sys/data/datasets.py
--rw-r--r--   0        0        0     1020 2023-06-28 02:28:53.594015 mini_rec_sys-0.1.0/mini_rec_sys/data/samplers.py
--rw-r--r--   0        0        0     2577 2023-06-26 05:03:49.954321 mini_rec_sys-0.1.0/mini_rec_sys/data/session.py
--rw-r--r--   0        0        0      192 2023-06-19 13:19:40.483582 mini_rec_sys-0.1.0/mini_rec_sys/encoders/__init__.py
--rw-r--r--   0        0        0     3952 2023-06-28 01:47:53.709483 mini_rec_sys-0.1.0/mini_rec_sys/encoders/encoders.py
--rw-r--r--   0        0        0       67 2023-06-21 08:07:03.673242 mini_rec_sys-0.1.0/mini_rec_sys/evaluators/__init__.py
--rw-r--r--   0        0        0     3494 2023-06-30 11:26:55.229027 mini_rec_sys-0.1.0/mini_rec_sys/evaluators/evaluators.py
--rw-r--r--   0        0        0       69 2023-06-30 12:24:35.543985 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/__init__.py
--rw-r--r--   0        0        0       11 2023-06-22 06:56:10.980380 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/.gitignore
--rw-r--r--   0        0        0      598 2023-06-21 06:34:09.426466 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/README.md
--rw-r--r--   0        0        0        0 2023-06-30 12:33:27.541877 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/__init__.py
--rwxr-xr-x   0        0        0      460 2023-06-22 06:59:57.131792 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/download.sh
--rw-r--r--   0        0        0     3494 2023-06-30 12:38:41.845286 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py
--rw-r--r--   0        0        0   190171 2023-06-22 03:15:42.162087 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json
--rw-r--r--   0        0        0    12085 2023-06-22 03:11:30.984882 mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json
--rw-r--r--   0        0        0     6478 2023-06-30 08:29:54.945075 mini_rec_sys-0.1.0/mini_rec_sys/scorers/BM25Scorer.py
--rw-r--r--   0        0        0      816 2023-06-21 07:13:42.549019 mini_rec_sys-0.1.0/mini_rec_sys/scorers/BaseScorer.py
--rw-r--r--   0        0        0     3744 2023-06-30 11:17:28.252552 mini_rec_sys-0.1.0/mini_rec_sys/scorers/DenseScorer.py
--rw-r--r--   0        0        0      107 2023-06-28 08:17:20.287340 mini_rec_sys-0.1.0/mini_rec_sys/scorers/__init__.py
--rw-r--r--   0        0        0     4769 2023-06-30 08:07:38.092499 mini_rec_sys-0.1.0/mini_rec_sys/trainers/DPRModel.py
--rw-r--r--   0        0        0       75 2023-06-28 04:49:24.386866 mini_rec_sys-0.1.0/mini_rec_sys/trainers/__init__.py
--rw-r--r--   0        0        0     2857 2023-06-28 05:24:19.735468 mini_rec_sys-0.1.0/mini_rec_sys/trainers/base_trainers.py
--rw-r--r--   0        0        0     2127 2023-06-28 08:12:43.876534 mini_rec_sys-0.1.0/mini_rec_sys/utils.py
--rw-r--r--   0        0        0      702 2023-06-26 10:53:57.213948 mini_rec_sys-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.0/setup.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.1/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 01:39:12.515507 mini_rec_sys-0.1.1/mini_rec_sys/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-03 06:46:57.470897 mini_rec_sys-0.1.1/mini_rec_sys/constants.py
+-rw-r--r--   0        0        0      172 2023-07-03 06:36:44.571179 mini_rec_sys-0.1.1/mini_rec_sys/data/__init__.py
+-rw-r--r--   0        0        0    12093 2023-07-04 07:45:23.086845 mini_rec_sys-0.1.1/mini_rec_sys/data/datasets.py
+-rw-r--r--   0        0        0     3424 2023-07-03 06:49:46.328910 mini_rec_sys-0.1.1/mini_rec_sys/data/samplers.py
+-rw-r--r--   0        0        0     3014 2023-07-04 05:48:52.583581 mini_rec_sys-0.1.1/mini_rec_sys/data/session.py
+-rw-r--r--   0        0        0      192 2023-06-19 13:19:40.483582 mini_rec_sys-0.1.1/mini_rec_sys/encoders/__init__.py
+-rw-r--r--   0        0        0     3952 2023-06-28 01:47:53.709483 mini_rec_sys-0.1.1/mini_rec_sys/encoders/encoders.py
+-rw-r--r--   0        0        0       67 2023-06-21 08:07:03.673242 mini_rec_sys-0.1.1/mini_rec_sys/evaluators/__init__.py
+-rw-r--r--   0        0        0     3066 2023-07-03 02:04:42.665475 mini_rec_sys-0.1.1/mini_rec_sys/evaluators/evaluators.py
+-rw-r--r--   0        0        0       69 2023-06-30 12:24:35.543985 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/__init__.py
+-rw-r--r--   0        0        0       11 2023-06-22 06:56:10.980380 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/.gitignore
+-rw-r--r--   0        0        0      598 2023-06-21 06:34:09.426466 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 12:33:27.541877 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/__init__.py
+-rwxr-xr-x   0        0        0      460 2023-06-22 06:59:57.131792 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/download.sh
+-rw-r--r--   0        0        0     3494 2023-06-30 12:38:41.845286 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py
+-rw-r--r--   0        0        0   190171 2023-06-22 03:15:42.162087 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json
+-rw-r--r--   0        0        0    12085 2023-06-22 03:11:30.984882 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json
+-rw-r--r--   0        0        0     6478 2023-06-30 08:29:54.945075 mini_rec_sys-0.1.1/mini_rec_sys/scorers/BM25Scorer.py
+-rw-r--r--   0        0        0      816 2023-06-21 07:13:42.549019 mini_rec_sys-0.1.1/mini_rec_sys/scorers/BaseScorer.py
+-rw-r--r--   0        0        0     3778 2023-07-04 07:36:53.986005 mini_rec_sys-0.1.1/mini_rec_sys/scorers/DenseScorer.py
+-rw-r--r--   0        0        0      107 2023-06-28 08:17:20.287340 mini_rec_sys-0.1.1/mini_rec_sys/scorers/__init__.py
+-rw-r--r--   0        0        0     9438 2023-07-04 12:48:12.638160 mini_rec_sys-0.1.1/mini_rec_sys/trainers/DPRModel.py
+-rw-r--r--   0        0        0       75 2023-06-28 04:49:24.386866 mini_rec_sys-0.1.1/mini_rec_sys/trainers/__init__.py
+-rw-r--r--   0        0        0     5316 2023-07-04 12:55:59.211359 mini_rec_sys-0.1.1/mini_rec_sys/trainers/base_trainers.py
+-rw-r--r--   0        0        0     3302 2023-07-04 06:05:52.310608 mini_rec_sys-0.1.1/mini_rec_sys/utils.py
+-rw-r--r--   0        0        0      728 2023-07-04 13:07:58.247063 mini_rec_sys-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.1/PKG-INFO
```

### Comparing `mini_rec_sys-0.1.0/LICENSE` & `mini_rec_sys-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/data/datasets.py` & `mini_rec_sys-0.1.1/mini_rec_sys/data/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from mini_rec_sys.constants import (
     ITEM_ATTRIBUTES_NAME,
     USER_ATTRIBUTES_NAME,
     SESSION_NAME,
 )
 from pdb import set_trace
 
+MAX_DISK_SIZE = int(1e10)
+
 
 class Dataset(torch.utils.data.Dataset):
     """
     A class used to load attributes associated with each user or item.
     At initialization, the attributes are stored in a simple database and retrieved
     during training or evaluation time.
     """
@@ -69,17 +71,17 @@
         else:
             self.subset_ids = subset_ids
 
         if data is not None:
             print(f"Populating database..")
             self.cache = self.populate_db(data)
         else:
-            self.cache = Cache(db_location)
+            self.cache = Cache(db_location, size_limit=MAX_DISK_SIZE, cull_limit=0)
             print(
-                f"Loading / initializing database with {len(self)} entries at {db_location}.."
+                f"Loading / initializing database with {len(self):,} entries at {db_location}.."
             )
 
     def get_files_from_path(self, path: str, suffix="parquet"):
         """Get a list of .suffix files in path."""
         if path.endswith(suffix):
             return [path]
         files = Path(path).glob(f"*.{suffix}")
@@ -107,44 +109,66 @@
             generator = iter(data.items())
 
         else:
             raise ValueError(f"{data} is neither str nor dict.")
 
         if self.db_location is None:
             print("Initializing cache in temp location..")
-            cache = Cache()
+            cache = Cache(size_limit=MAX_DISK_SIZE, cull_limit=0)
             self.db_location = cache.directory
         elif self.db_location.startswith("dbfs:/"):
             print("On databricks, writing to temp location..")
-            cache = Cache()
+            cache = Cache(size_limit=MAX_DISK_SIZE, cull_limit=0)
         else:
-            cache = Cache(self.db_location)
+            cache = Cache(self.db_location, size_limit=MAX_DISK_SIZE, cull_limit=0)
 
         for id, row in tqdm(generator):
-            cache[id] = self.store_fn(id, row)
+            try:
+                res = self.store_fn(id, row)
+            except Exception as e:
+                raise ValueError(
+                    f"Failed to store id: {id} with data: {self.summarize_row(row)}."
+                )
+            if res:
+                cache[id] = res
 
         if self.db_location and self.db_location.startswith("dbfs:/"):
             directory = cache.directory
             copytree(directory, self.db_location)
-            cache = Cache(self.db_location)
+            cache = Cache(self.db_location, size_limit=MAX_DISK_SIZE, cull_limit=0)
         return cache
 
     def json_row_generator(self, files):
         for path in files:
             with open(path) as f:
                 d = json.load(f)
             for id, values in d.items():
                 yield id, values
 
     def parquet_row_generator(self, files):
         for path in files:
             df = pd.read_parquet(path)
-            for _, row in df.iterrows():
-                id = row.pop(self.id_name)
-                yield id, row
+            for row_dict in df.to_dict(orient="records"):
+                try:
+                    id = row_dict[self.id_name]
+                except Exception as e:
+                    raise ValueError(
+                        f"Failed to parse correctly, the row of data loaded was {self.summarize_row(row_dict)}."
+                    )
+                yield id, row_dict
+
+    def summarize_row(self, row_dict: dict):
+        res = {}
+        for k, v in row_dict.items():
+            if isinstance(v, list):
+                v = v[:5]
+            if isinstance(v, str):
+                v = v[:50]
+            res[k] = v
+        return res
 
     def load_object(self, id: int | str):
         """
         Load the raw object for id.
         """
         if self.subset_ids:
             if id not in self.subset_ids:
@@ -180,14 +204,18 @@
 
     def iterkeys(self):
         if self.subset_ids:
             return iter(self.subset_ids)
         else:
             return self.cache.iterkeys()
 
+    def peek(self):
+        key, res = next(iter(self))
+        return {key: res}
+
 
 # For UserDataset and ItemDataset, we just enforce that the load_fn must load
 # a dict object
 class UserItemDataset(Dataset):
     def __init__(
         self,
         db_location: str = None,
@@ -275,14 +303,15 @@
             if self.item_dataset is None
             else self.load_items(session.items)
         )
         user_attributes = (
             session.user if self.user_dataset is None else self.load_users(session.user)
         )
         return {
+            **session.__dict__,
             SESSION_NAME: session,
             USER_ATTRIBUTES_NAME: user_attributes,
             ITEM_ATTRIBUTES_NAME: item_attributes,
         }
 
     def load_item(self, item_id: int | str):
         res = {"item_id": item_id}
```

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/data/session.py` & `mini_rec_sys-0.1.1/mini_rec_sys/data/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,29 @@
     positive_items: list[int | str] = Field(
         ...,
         description="Items that received a positive relevance signal in this session.",
     )
     positive_relevances: list[int | float] = Field(
         ..., description="The relevance scores for each of the `positive_items`."
     )
+    positive_weights: Optional[list[int | float]] = Field(
+        None,
+        description="The weight of each of the `positive_items`, e.g. occurrence probability",
+    )
     user: Optional[int | str] = None
     query: Optional[str] = None
     negative_items: Optional[list[int | str]] = Field(
         None,
         description="Items that are deemed irrelevant in this session, e.g. implicit negatives based on impressions or explicit negatives",
     )
+    negative_weights: Optional[list[int | float]] = Field(
+        None,
+        description="The weight of each of the `negative_items`, e.g. occurrence probability",
+    )
+    session_weight: Optional[int | float] = Field(None, description="Weight of session")
 
     @validator("positive_relevances")
     def at_least_one_relevance(cls, relevances):
         if relevances is None or len(relevances) == 0:
             raise AssertionError("must have at least one relevance!")
         return relevances
```

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/encoders/encoders.py` & `mini_rec_sys-0.1.1/mini_rec_sys/encoders/encoders.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/evaluators/evaluators.py` & `mini_rec_sys-0.1.1/mini_rec_sys/evaluators/evaluators.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,64 +46,53 @@
     # TODO: Currently we only have scorer as a pipeline, but in future will extend
     to a composable pipeline, e.g. retrieval -> scorer.
     """
 
     def __init__(
         self,
         pipeline: BaseScorer,
-        dataset: SessionDataset,
+        dataset: SessionDataset = None,
         batch_size: int = 32,
     ) -> None:
         """ """
         self.pipeline = pipeline
         self.dataset = dataset
         self.batch_size = batch_size
 
     def evaluate(self, k=20, return_raw=False):
         """
         For now we will just evaluate the NDCG, extend in future to take in
         other metrics.
         """
+        assert self.dataset is not None, "Dataset must be provided to evaluate"
         metrics = []
         sampler = BatchedSequentialSampler(
             self.dataset, batch_size=self.batch_size, drop_last=False
         )
         for batch in DataLoader(
             self.dataset, batch_sampler=sampler, collate_fn=lambda x: x
         ):
-            scores: list[list[float]] = self.score_sessions(batch)
-            for i, row in enumerate(batch):
-                row_scores = scores[i]
-                session: Session = row["session"]
-                relevances_reranked = self.rerank(row_scores, session.relevances)
-                metrics.append(ndcg(relevances_reranked, k=k))
+            metrics.extend(self.evaluate_batch(batch, k=k, return_raw=True))
         assert len(metrics) == len(self.dataset)
         if return_raw:
             return metrics
         return mean_with_se(metrics)
 
-    def score_sessions(self, session_dicts: list[dict], k=20):
-        """
-        As scorers might be more efficient computing in batch, we try to stack up
-        user and item attributes as much as possible before passing into the
-        `score` method of the scorer.
-        """
-        data = []
-        for d in session_dicts:
-            session: Session = d[SESSION_NAME]
-            item_attributes = self.dataset.load_items(session.items)
-            user_attributes = self.dataset.load_user(session.user)
-            data.append(
-                {
-                    **session.__dict__,
-                    USER_ATTRIBUTES_NAME: user_attributes,
-                    ITEM_ATTRIBUTES_NAME: item_attributes,
-                }
-            )
-        return self.pipeline(data)
+    def evaluate_batch(self, batch: list[dict], k=20, return_raw=False):
+        metrics = []
+        scores: list[list[float]] = self.pipeline(batch)
+        for i, row in enumerate(batch):
+            row_scores = scores[i]
+            session: Session = row["session"]
+            relevances_reranked = self.rerank(row_scores, session.relevances)
+            metrics.append(ndcg(relevances_reranked, k=k))
+        assert len(metrics) == len(batch)
+        if return_raw:
+            return metrics
+        return mean_with_se(metrics)
 
     def rerank(self, scores: list[float], items: list[object]):
         """
         Rerank items in descending score order.
         """
         sorting = np.argsort(-np.array(scores))
         return np.array(items)[sorting].tolist()
```

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/README.md` & `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/README.md`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py` & `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json` & `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json` & `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/scorers/BM25Scorer.py` & `mini_rec_sys-0.1.1/mini_rec_sys/scorers/BM25Scorer.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/scorers/BaseScorer.py` & `mini_rec_sys-0.1.1/mini_rec_sys/scorers/BaseScorer.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/scorers/DenseScorer.py` & `mini_rec_sys-0.1.1/mini_rec_sys/scorers/DenseScorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         """
         self.q_encoder.eval()
         self.p_encoder.eval()
 
         # Handle single row of data
         if isinstance(test_data, list):
             queries = [d[self.query_key] for d in test_data]
-            item_lists = [d[self.test_documents_key] for d in test_data]
+            item_lists: list[dict] = [d[self.test_documents_key] for d in test_data]
         else:
             queries = [test_data[self.query_key]]
-            item_lists = [test_data[self.test_documents_key]]
+            item_lists: list[dict] = [test_data[self.test_documents_key]]
 
         # Encode queries
         q_embed = []
         for batch in batcher(queries, self.batch_size):
             q_embed.append(self.q_encode(batch))
         q_embed = np.vstack(q_embed)  # n_batch x embed_dim
 
@@ -75,15 +75,15 @@
         idx_list = []
         hash2idx = {}
         item_texts = []
         idx = 0
         for items in item_lists:
             inner_list = []
             for item in items:
-                item_text = item[self.passage_text_key]
+                item_text = item.get(self.passage_text_key, None)
                 if item_text is None:
                     item_text = ""
                 text_hash = hash(item_text)
                 if not text_hash in hash2idx:
                     item_texts.append(item_text)
                     hash2idx[text_hash] = idx
                     idx += 1
```

### Comparing `mini_rec_sys-0.1.0/mini_rec_sys/utils.py` & `mini_rec_sys-0.1.1/mini_rec_sys/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 import os
 import torch
 import pandas as pd
 import re
 import lxml.html
 import lxml.html.clean
+import itertools
+import random
 from pdb import set_trace
 
 
 def get_date():
     date = datetime.datetime.now().date()
     return str(date)
 
@@ -84,7 +86,57 @@
     return text
 
 
 def convert_none_to_empty_string(string):
     if string is None:
         return ""
     return string
+
+
+def flatten_list(l: list[list]):
+    return list(itertools.chain.from_iterable(l))
+
+
+def shuffle(l: list):
+    return random.shuffle(l, len(l))
+
+
+import random
+
+
+class Sampler:
+    def sample(self):
+        raise NotImplementedError()
+
+
+class WeightedSampler:
+    """
+    Class to sample from a dictionary with sample weights.
+    """
+
+    def __init__(self, sample_dict: dict, pop=False) -> None:
+        """
+        sample_dict: dictionary of item to sample probability.
+        pop: Whether we should pop an item after we sample it
+        """
+        self.items = []
+        self.probs = []
+        for k, v in sample_dict.items():
+            if v > 0.0:
+                self.items.append(k)
+                self.probs.append(v)
+        self.pop = pop
+
+    def sample(self):
+        """
+        Return a sample based sample probabilities.
+        """
+        n = len(self.items)
+        idx = random.choices(range(n), self.probs, k=1)[0]
+        selected = self.items[idx]
+        if self.pop:
+            self.items.pop(idx)
+            self.probs.pop(idx)
+        return selected
+
+    def __len__(self):
+        return len(self.items)
```

### Comparing `mini_rec_sys-0.1.0/PKG-INFO` & `mini_rec_sys-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mini-rec-sys
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkit to train and evaluate models for search and recommendations.
 License: MIT
 Author: Charles Low
 Author-email: charleslow88@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
+Requires-Dist: fastparquet (>=2023.4.0,<2024.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.16.5,<1.23.0)
 Requires-Dist: pandas (>=1.0.5)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pysos (>=1.3.0,<2.0.0)
 Requires-Dist: pytorch-lightning (>=2.0.4,<3.0.0)
```

