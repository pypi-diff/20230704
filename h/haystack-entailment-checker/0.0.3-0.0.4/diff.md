# Comparing `tmp/haystack_entailment_checker-0.0.3.tar.gz` & `tmp/haystack_entailment_checker-0.0.4.tar.gz`

## Comparing `haystack_entailment_checker-0.0.3.tar` & `haystack_entailment_checker-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/haystack_entailment_checker/__init__.py
--rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/haystack_entailment_checker/entailment_checker.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/.gitignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/README.md
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/haystack_entailment_checker/__init__.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/haystack_entailment_checker/entailment_checker.py
+-rw-r--r--   0        0        0   208223 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/images/entailment_checker_node.png
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/.gitignore
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/README.md
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 haystack_entailment_checker-0.0.4/PKG-INFO
```

### Comparing `haystack_entailment_checker-0.0.3/haystack_entailment_checker/entailment_checker.py` & `haystack_entailment_checker-0.0.4/haystack_entailment_checker/entailment_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         self.model.to(str(self.devices[0]))
 
         id2label = AutoConfig.from_pretrained(model_name_or_path).id2label
         self.labels = [id2label[k].lower() for k in sorted(id2label)]
         if "entailment" not in self.labels:
             raise ValueError("The model config must contain entailment value in the id2label dict.")
 
-    def run(self, statement_to_check: str, documents: List[Document]):
+    def run(self, query: str, documents: List[Document]):
         scores, agg_con, agg_neu, agg_ent = 0, 0, 0, 0
         premise_batch = [doc.content for doc in documents]
-        hypothesis_batch = [statement_to_check] * len(documents)
+        hypothesis_batch = [query] * len(documents)
         entailment_info_batch = self.get_entailment_batch(
             premise_batch=premise_batch, hypothesis_batch=hypothesis_batch
         )
         for i, (doc, entailment_info) in enumerate(zip(documents, entailment_info_batch)):
             doc.meta["entailment_info"] = entailment_info
 
             con, neu, ent = (
@@ -94,17 +94,17 @@
         entailment_checker_result = {
             "documents": documents[: i + 1],
             "aggregate_entailment_info": aggregate_entailment_info,
         }
 
         return entailment_checker_result, "output_1"
 
-    def run_batch(self, statements_to_check: List[str], documents: List[Document]):
+    def run_batch(self, queries: List[str], documents: List[Document]):
         entailment_checker_result_batch = []
-        entailment_info_batch = self.get_entailment_batch(premise_batch=documents, hypothesis_batch=statements_to_check)
+        entailment_info_batch = self.get_entailment_batch(premise_batch=documents, hypothesis_batch=queries)
         for doc, entailment_info in zip(documents, entailment_info_batch):
             doc.meta["entailment_info"] = entailment_info
             aggregate_entailment_info = {
                 "contradiction": round(entailment_info["contradiction"] / doc.score),
                 "neutral": round(entailment_info["neutral"] / doc.score),
                 "entailment": round(entailment_info["entailment"] / doc.score),
             }
```

### Comparing `haystack_entailment_checker-0.0.3/.gitignore` & `haystack_entailment_checker-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_entailment_checker-0.0.3/pyproject.toml` & `haystack_entailment_checker-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "haystack-entailment-checker"
 description = 'Haystack node for checking the entailment between a statement and a list of Documents'
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "anakin87", email = "stefanofiorucci@gmail.com" },
 ]
```

