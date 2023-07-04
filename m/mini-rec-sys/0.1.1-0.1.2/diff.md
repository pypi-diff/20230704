# Comparing `tmp/mini_rec_sys-0.1.1.tar.gz` & `tmp/mini_rec_sys-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_rec_sys-0.1.1.tar", max compression
+gzip compressed data, was "mini_rec_sys-0.1.2.tar", max compression
```

## Comparing `mini_rec_sys-0.1.1.tar` & `mini_rec_sys-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.1/LICENSE
--rw-r--r--   0        0        0       80 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-21 01:39:12.515507 mini_rec_sys-0.1.1/mini_rec_sys/__init__.py
--rw-r--r--   0        0        0      307 2023-07-03 06:46:57.470897 mini_rec_sys-0.1.1/mini_rec_sys/constants.py
--rw-r--r--   0        0        0      172 2023-07-03 06:36:44.571179 mini_rec_sys-0.1.1/mini_rec_sys/data/__init__.py
--rw-r--r--   0        0        0    12093 2023-07-04 07:45:23.086845 mini_rec_sys-0.1.1/mini_rec_sys/data/datasets.py
--rw-r--r--   0        0        0     3424 2023-07-03 06:49:46.328910 mini_rec_sys-0.1.1/mini_rec_sys/data/samplers.py
--rw-r--r--   0        0        0     3014 2023-07-04 05:48:52.583581 mini_rec_sys-0.1.1/mini_rec_sys/data/session.py
--rw-r--r--   0        0        0      192 2023-06-19 13:19:40.483582 mini_rec_sys-0.1.1/mini_rec_sys/encoders/__init__.py
--rw-r--r--   0        0        0     3952 2023-06-28 01:47:53.709483 mini_rec_sys-0.1.1/mini_rec_sys/encoders/encoders.py
--rw-r--r--   0        0        0       67 2023-06-21 08:07:03.673242 mini_rec_sys-0.1.1/mini_rec_sys/evaluators/__init__.py
--rw-r--r--   0        0        0     3066 2023-07-03 02:04:42.665475 mini_rec_sys-0.1.1/mini_rec_sys/evaluators/evaluators.py
--rw-r--r--   0        0        0       69 2023-06-30 12:24:35.543985 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/__init__.py
--rw-r--r--   0        0        0       11 2023-06-22 06:56:10.980380 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/.gitignore
--rw-r--r--   0        0        0      598 2023-06-21 06:34:09.426466 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/README.md
--rw-r--r--   0        0        0        0 2023-06-30 12:33:27.541877 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/__init__.py
--rwxr-xr-x   0        0        0      460 2023-06-22 06:59:57.131792 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/download.sh
--rw-r--r--   0        0        0     3494 2023-06-30 12:38:41.845286 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py
--rw-r--r--   0        0        0   190171 2023-06-22 03:15:42.162087 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json
--rw-r--r--   0        0        0    12085 2023-06-22 03:11:30.984882 mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json
--rw-r--r--   0        0        0     6478 2023-06-30 08:29:54.945075 mini_rec_sys-0.1.1/mini_rec_sys/scorers/BM25Scorer.py
--rw-r--r--   0        0        0      816 2023-06-21 07:13:42.549019 mini_rec_sys-0.1.1/mini_rec_sys/scorers/BaseScorer.py
--rw-r--r--   0        0        0     3778 2023-07-04 07:36:53.986005 mini_rec_sys-0.1.1/mini_rec_sys/scorers/DenseScorer.py
--rw-r--r--   0        0        0      107 2023-06-28 08:17:20.287340 mini_rec_sys-0.1.1/mini_rec_sys/scorers/__init__.py
--rw-r--r--   0        0        0     9438 2023-07-04 12:48:12.638160 mini_rec_sys-0.1.1/mini_rec_sys/trainers/DPRModel.py
--rw-r--r--   0        0        0       75 2023-06-28 04:49:24.386866 mini_rec_sys-0.1.1/mini_rec_sys/trainers/__init__.py
--rw-r--r--   0        0        0     5316 2023-07-04 12:55:59.211359 mini_rec_sys-0.1.1/mini_rec_sys/trainers/base_trainers.py
--rw-r--r--   0        0        0     3302 2023-07-04 06:05:52.310608 mini_rec_sys-0.1.1/mini_rec_sys/utils.py
--rw-r--r--   0        0        0      728 2023-07-04 13:07:58.247063 mini_rec_sys-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.2/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-13 07:20:33.869967 mini_rec_sys-0.1.2/README.md
+-rw-r--r--   0        0        0       34 2023-07-04 13:26:00.281003 mini_rec_sys-0.1.2/mini_rec_sys/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-03 06:46:57.470897 mini_rec_sys-0.1.2/mini_rec_sys/constants.py
+-rw-r--r--   0        0        0      207 2023-07-04 13:32:02.158793 mini_rec_sys-0.1.2/mini_rec_sys/data/__init__.py
+-rw-r--r--   0        0        0    12128 2023-07-04 13:35:50.949934 mini_rec_sys-0.1.2/mini_rec_sys/data/datasets.py
+-rw-r--r--   0        0        0     3459 2023-07-04 13:35:58.865909 mini_rec_sys-0.1.2/mini_rec_sys/data/samplers.py
+-rw-r--r--   0        0        0     3118 2023-07-04 13:40:47.185166 mini_rec_sys-0.1.2/mini_rec_sys/data/session.py
+-rw-r--r--   0        0        0      192 2023-06-19 13:19:40.483582 mini_rec_sys-0.1.2/mini_rec_sys/encoders/__init__.py
+-rw-r--r--   0        0        0     3988 2023-07-04 13:36:13.637863 mini_rec_sys-0.1.2/mini_rec_sys/encoders/encoders.py
+-rw-r--r--   0        0        0       67 2023-06-21 08:07:03.673242 mini_rec_sys-0.1.2/mini_rec_sys/evaluators/__init__.py
+-rw-r--r--   0        0        0     3101 2023-07-04 13:36:21.709839 mini_rec_sys-0.1.2/mini_rec_sys/evaluators/evaluators.py
+-rw-r--r--   0        0        0      104 2023-07-04 13:36:34.717800 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/__init__.py
+-rw-r--r--   0        0        0       11 2023-06-22 06:56:10.980380 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/.gitignore
+-rw-r--r--   0        0        0      598 2023-06-21 06:34:09.426466 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 12:33:27.541877 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/__init__.py
+-rwxr-xr-x   0        0        0      460 2023-06-22 06:59:57.131792 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/download.sh
+-rw-r--r--   0        0        0     3494 2023-06-30 12:38:41.845286 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py
+-rw-r--r--   0        0        0   190171 2023-06-22 03:15:42.162087 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json
+-rw-r--r--   0        0        0    12085 2023-06-22 03:11:30.984882 mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json
+-rw-r--r--   0        0        0     6544 2023-07-04 13:41:57.749021 mini_rec_sys-0.1.2/mini_rec_sys/scorers/BM25Scorer.py
+-rw-r--r--   0        0        0      816 2023-06-21 07:13:42.549019 mini_rec_sys-0.1.2/mini_rec_sys/scorers/BaseScorer.py
+-rw-r--r--   0        0        0     3813 2023-07-04 13:42:09.044999 mini_rec_sys-0.1.2/mini_rec_sys/scorers/DenseScorer.py
+-rw-r--r--   0        0        0      107 2023-06-28 08:17:20.287340 mini_rec_sys-0.1.2/mini_rec_sys/scorers/__init__.py
+-rw-r--r--   0        0        0     9473 2023-07-04 13:42:55.113376 mini_rec_sys-0.1.2/mini_rec_sys/trainers/DPRModel.py
+-rw-r--r--   0        0        0       75 2023-06-28 04:49:24.386866 mini_rec_sys-0.1.2/mini_rec_sys/trainers/__init__.py
+-rw-r--r--   0        0        0     5384 2023-07-04 13:42:44.465071 mini_rec_sys-0.1.2/mini_rec_sys/trainers/base_trainers.py
+-rw-r--r--   0        0        0     3337 2023-07-04 13:43:08.685757 mini_rec_sys-0.1.2/mini_rec_sys/utils.py
+-rw-r--r--   0        0        0      727 2023-07-04 13:44:16.795535 mini_rec_sys-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 mini_rec_sys-0.1.2/PKG-INFO
```

### Comparing `mini_rec_sys-0.1.1/LICENSE` & `mini_rec_sys-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/data/datasets.py` & `mini_rec_sys-0.1.2/mini_rec_sys/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from diskcache import Cache
 from pathlib import Path
 from tqdm import tqdm
 import pandas as pd
 import json
 from shutil import copytree
 import torch
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/data/samplers.py` & `mini_rec_sys-0.1.2/mini_rec_sys/data/samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Besides the default samplers, one can also subclass Sampler and define custom sampling logic.
 """
+from __future__ import annotations
 from typing import Optional, Sized
 import torch
 import random
 import math
 from mini_rec_sys.data.datasets import Dataset, SessionDataset
 from mini_rec_sys.utils import flatten_list
 from mini_rec_sys.constants import SESSION_WEIGHT_NAME
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/data/session.py` & `mini_rec_sys-0.1.2/mini_rec_sys/data/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+from __future__ import annotations
 from pydantic import Field, validator
 from pydantic.dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Union
 
 
 @dataclass
 class Session:
     """Session is a generalized concept to store relevance judgments for training and evaluation.
 
     Some examples of how we might define a session:
     - One user query and items that the user clicked on.
     - A triplet of (query, positive_item, negative_item)
     """
 
-    session_id: int | str
-    positive_items: list[int | str] = Field(
+    session_id: Union[int, str]
+    positive_items: list[Union[int, str]] = Field(
         ...,
         description="Items that received a positive relevance signal in this session.",
     )
-    positive_relevances: list[int | float] = Field(
+    positive_relevances: list[Union[int, float]] = Field(
         ..., description="The relevance scores for each of the `positive_items`."
     )
-    positive_weights: Optional[list[int | float]] = Field(
+    positive_weights: Optional[list[Union[int, float]]] = Field(
         None,
         description="The weight of each of the `positive_items`, e.g. occurrence probability",
     )
-    user: Optional[int | str] = None
+    user: Optional[Union[int, str]] = None
     query: Optional[str] = None
-    negative_items: Optional[list[int | str]] = Field(
+    negative_items: Optional[list[Union[int, str]]] = Field(
         None,
         description="Items that are deemed irrelevant in this session, e.g. implicit negatives based on impressions or explicit negatives",
     )
-    negative_weights: Optional[list[int | float]] = Field(
+    negative_weights: Optional[list[Union[int, float]]] = Field(
         None,
         description="The weight of each of the `negative_items`, e.g. occurrence probability",
     )
-    session_weight: Optional[int | float] = Field(None, description="Weight of session")
+    session_weight: Optional[Union[int, float]] = Field(
+        None, description="Weight of session"
+    )
 
     @validator("positive_relevances")
     def at_least_one_relevance(cls, relevances):
         if relevances is None or len(relevances) == 0:
             raise AssertionError("must have at least one relevance!")
         return relevances
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/encoders/encoders.py` & `mini_rec_sys-0.1.2/mini_rec_sys/encoders/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 """
 Wrappers around various transformer models to define a consistent interface
 for encoding texts and using for search.
 """
 from transformers import AutoModel, AutoTokenizer, AutoConfig
 import torch
 from torch import nn
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/evaluators/evaluators.py` & `mini_rec_sys-0.1.2/mini_rec_sys/evaluators/evaluators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import pandas as pd
 import numpy as np
 import math
 from torch.utils.data import DataLoader
 from mini_rec_sys.scorers import BaseScorer
 from mini_rec_sys.data import Session, SessionDataset, BatchedSequentialSampler
 from mini_rec_sys.constants import (
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/README.md` & `mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/README.md`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py` & `mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/generate_data.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json` & `mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_items.json`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json` & `mini_rec_sys-0.1.2/mini_rec_sys/sample_data/msmarco_reranking/msmarco_sample_sessions.json`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/scorers/BM25Scorer.py` & `mini_rec_sys-0.1.2/mini_rec_sys/scorers/BM25Scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
 import math
 import re
 import numpy as np
 from collections import Counter
 from mini_rec_sys.scorers import BaseScorer
+from typing import Union
 from pdb import set_trace
 
 STOP_WORDS = [
     "i",
     "am",
     "stop",
     "the",
@@ -62,15 +64,15 @@
         self.stop_words = set(STOP_WORDS)
 
         # Initialize empty dicts for training
         self.df = {}  # Document frequency of a term
         self.field_doclens = {field: 0.0 for field in fields}
         self.train(train_documents)
 
-    def score(self, input_data: dict | list[dict]):
+    def score(self, input_data: Union[dict, list[dict]]):
         if input_data is None:
             return None
         if isinstance(input_data, dict):
             return self.score_single(input_data)
         return [self.score_single(row) for row in input_data]
 
     def score_single(self, row: dict):
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/scorers/BaseScorer.py` & `mini_rec_sys-0.1.2/mini_rec_sys/scorers/BaseScorer.py`

 * *Files identical despite different names*

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/scorers/DenseScorer.py` & `mini_rec_sys-0.1.2/mini_rec_sys/scorers/DenseScorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import List, Tuple
 import torch
 import numpy as np
 from tqdm import tqdm
 
 from mini_rec_sys.encoders import BaseBertEncoder
 from mini_rec_sys.scorers import BaseScorer
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/trainers/DPRModel.py` & `mini_rec_sys-0.1.2/mini_rec_sys/trainers/DPRModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module for training a query and passage encoder based on Karpukhin 2020 -
 Dense Passage Retrieval for Open-Domain Question Answering.
 """
+from __future__ import annotations
 from torch.optim import Optimizer, Adam
 import random
 
 from mini_rec_sys.data import Session, ItemDataset, SessionDataset, Sampler
 from mini_rec_sys.trainers.base_trainers import BaseModel
 from mini_rec_sys.encoders import BaseBertEncoder
 from mini_rec_sys.scorers import DenseScorer
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/trainers/base_trainers.py` & `mini_rec_sys-0.1.2/mini_rec_sys/trainers/base_trainers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
 from torch.optim import Optimizer, Adam
 from torch.utils.data import DataLoader, Sampler
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import ModelCheckpoint
 import numpy as np
+from typing import Union
 
 from mini_rec_sys.data import Session, SessionDataset, BatchedSequentialSampler
 from mini_rec_sys.evaluators import mean_with_se
 from mini_rec_sys.constants import (
     VAL_METRIC_NAME,
     TRAIN_METRIC_NAME,
     TEST_METRIC_NAME,
@@ -101,18 +103,18 @@
 def train(
     model: BaseModel,
     max_epochs: int = 20,
     limit_train_batches: int = 100,
     limit_val_batches: int = 20,
     log_every_n_steps: int = 50,
     limit_test_batches: int = 20,
-    precision: int | str = 32,
+    precision: Union[int, str] = 32,
     checkpoint_metric: str = None,
     checkpoint_behaviour: str = "min",
-    **kwargs
+    **kwargs,
 ):
     """
     Additional arguments / keyword arguments are passed into pl.Trainer.
     """
     train_loader = DataLoader(
         model.train_dataset, batch_sampler=model.sampler, collate_fn=lambda x: x
     )
@@ -150,15 +152,15 @@
         max_epochs=max_epochs,
         limit_train_batches=limit_train_batches,
         limit_val_batches=limit_val_batches,
         log_every_n_steps=log_every_n_steps,
         limit_test_batches=limit_test_batches,
         precision=precision,
         callbacks=callbacks,
-        **kwargs
+        **kwargs,
     )
     trainer.fit(
         model=model,
         train_dataloaders=train_loader,
         val_dataloaders=val_loader,
     )
     if test_loader is not None:
```

### Comparing `mini_rec_sys-0.1.1/mini_rec_sys/utils.py` & `mini_rec_sys-0.1.2/mini_rec_sys/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import datetime
 import os
 import torch
 import pandas as pd
 import re
 import lxml.html
 import lxml.html.clean
```

### Comparing `mini_rec_sys-0.1.1/pyproject.toml` & `mini_rec_sys-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "mini-rec-sys"
-version = "0.1.1"
+version = "0.1.2"
 description = "Toolkit to train and evaluate models for search and recommendations."
 authors = ["Charles Low <charleslow88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mini_rec_sys"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 transformers = "^4.26.1"
 numpy = ">=1.16.5,<1.23.0"
 pandas = ">=1.0.5"
 pysos = "^1.3.0"
 nltk = "^3.8.1"
 lxml = "^4.9.2"
 torch = "<2.0.0"
```

### Comparing `mini_rec_sys-0.1.1/PKG-INFO` & `mini_rec_sys-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mini-rec-sys
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolkit to train and evaluate models for search and recommendations.
 License: MIT
 Author: Charles Low
 Author-email: charleslow88@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fastparquet (>=2023.4.0,<2024.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
```

