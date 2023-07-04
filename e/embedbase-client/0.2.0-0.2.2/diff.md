# Comparing `tmp/embedbase_client-0.2.0.tar.gz` & `tmp/embedbase_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.2.0.tar", max compression
+gzip compressed data, was "embedbase_client-0.2.2.tar", max compression
```

## Comparing `embedbase_client-0.2.0.tar` & `embedbase_client-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     1005 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/README.md
--rw-r--r--   0        0        0      389 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/__init__.py
--rw-r--r--   0        0        0    21866 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/base.py
--rw-r--r--   0        0        0     1150 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/errors.py
--rw-r--r--   0        0        0     1645 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/model.py
--rw-r--r--   0        0        0     4525 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/split.py
--rw-r--r--   0        0        0    21767 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     2051 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/utils.py
--rw-r--r--   0        0        0     3535 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1005 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/README.md
+-rw-r--r--   0        0        0      389 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    24965 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/base.py
+-rw-r--r--   0        0        0     1150 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1645 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/model.py
+-rw-r--r--   0        0        0     4525 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/split.py
+-rw-r--r--   0        0        0    24645 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3536 2023-07-04 17:22:48.892766 embedbase_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.2.2/PKG-INFO
```

### Comparing `embedbase_client-0.2.0/LICENSE` & `embedbase_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/README.md` & `embedbase_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/embedbase_client/async_client.py` & `embedbase_client-0.2.2/embedbase_client/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import asyncio
 import itertools
 import json
 from dataclasses import dataclass
 
 import httpx
@@ -180,15 +180,15 @@
             A document.
 
         Example usage:
             result = await dataset.add("Python is a programming language.", {"topic": "programming"})
         """
         return await self.client.add(self.dataset, document, metadata)
 
-    async def batch_add(self, documents: List[Dict[str, Any]]) -> List[Document]:
+    async def batch_add(self, documents: List[AddDocument]) -> List[Document]:
         """
         Add multiple documents to the specified dataset in a single batch asynchronously.
 
         Args:
             documents: A list of documents.
 
         Returns:
@@ -277,14 +277,34 @@
             A string containing the context.
 
         Example usage:
             context = await dataset.create_max_context("What is Python?", max_tokens=100)
         """
         return await self.client.create_max_context(self.dataset, query, max_tokens)
 
+    async def update(self, document: Document) -> Document:
+        """
+        Update the documents in the specified dataset asynchronously.
+
+        Args:
+            dataset: The name of the dataset to update.
+            documents: A list of documents to update.
+
+        Returns:
+            A list of updated documents.
+
+        Example usage:
+            documents = [
+                {"id": "document_id1", "data": "Updated document 1"},
+                {"id": "document_id2", "data": "Updated document 2"},
+            ]
+            results = await dataset.update(documents)
+        """
+        return await self.client.update(self.dataset, document)
+
 
 class EmbedbaseAsyncClient(BaseClient):
     def dataset(self, dataset: str) -> AsyncDataset:
         return AsyncDataset(client=self, dataset=dataset)
 
     async def create_context(
         self, dataset: str, query: str, limit: Optional[int] = None
@@ -575,52 +595,113 @@
             ]
         )
 
         return list(itertools.chain.from_iterable(results))
 
     async def create_max_context(
         self,
-        dataset: str,
+        dataset: Union[str, List[str]],
         query: str,
-        max_tokens: int,
+        max_tokens: Union[int, List[int]],
     ) -> str:
         """
-        Create a context from a query by searching for similar documents and concatenating them up to the specified max tokens.
+        Create a context from a query by searching for similar documents and
+        concatenating them up to the specified max tokens.
 
         Args:
             dataset: The name of the dataset to search.
             query: The query to search for.
             max_tokens: the maximum number of tokens for the context.
 
         Returns:
             A string containing the context.
 
         Example usage:
-            context = create_max_context("Python is a programming language.", max_tokens=30)
+            context = await create_max_context("programming", "Python is a programming language.", 30)
             print(context)
             # Python is a programming language.
             # Python is a high-level, general-purpose programming language.
             # Python is interpreted, dynamically typed and garbage-collected.
             # Python is designed to be highly extensible.
             # Python is a multi-paradig
+            # or
+            context = await create_max_context(["programming", "science"], "Python lives planet earth.", [3, 30])
+            print(context)
+            # Pyt
+            # The earth orbits the sun.
+            # The earth is the third planet from the sun.
+            # The earth is the only planet known to support life.
+            # The earth formed approximately 4.5 billion years ago.
+            # The earth's gravity interacts with other objects in space, especially the sun and the moon.
         """
 
-        # try to build a context until it's big enough by incrementing top_k
-        top_k = 100
-        context = await self.create_context(dataset, query, top_k)
-        merged_context, size = merge_and_return_tokens(context, max_tokens)
-
-        tries = 0
-        max_tries = 3
-        while size < max_tokens and tries < max_tries:
-            top_k *= 3
-            context = await self.create_context(dataset, query, top_k)
+        async def create_context_for_dataset(d, max_tokens):
+            top_k = 100
+            context = await self.create_context(d, query, top_k)
             merged_context, size = merge_and_return_tokens(context, max_tokens)
-            tries += 1
 
-        if size < max_tokens:
-            # warn the user that the context is smaller than the max tokens
-            print(
-                f"Warning: context is smaller than the max tokens ({size} < {max_tokens})"
+            tries = 0
+            max_tries = 3
+            while size < max_tokens and tries < max_tries:
+                top_k *= 3
+                context = await self.create_context(dataset, query, top_k)
+                merged_context, size = merge_and_return_tokens(context, max_tokens)
+                tries += 1
+
+            if size < max_tokens:
+                print(
+                    f"Warning: context for dataset '{dataset}' is smaller than the max tokens ({size} < {max_tokens})"
+                )
+            return merged_context
+
+        if not isinstance(dataset, list):
+            dataset = [dataset]
+
+        if not isinstance(max_tokens, list):
+            max_tokens = [max_tokens for _ in range(len(dataset))]
+
+        if len(dataset) != len(max_tokens):
+            raise ValueError("The number of datasets and max_tokens should be equal.")
+
+        contexts = []
+        for ds, mt in zip(dataset, max_tokens):
+            context = await create_context_for_dataset(ds, mt)
+            contexts.append(context)
+
+        return "\n\n".join(contexts)
+
+    async def update(self, dataset: str, documents: List[Document]) -> List[Document]:
+        """
+        Update the documents in the specified dataset asynchronously.
+
+        Args:
+            dataset: The name of the dataset to update.
+            documents: A list of documents to update.
+
+        Returns:
+            A list of updated documents.
+
+        Example usage:
+            documents = [
+                {"id": "document_id1", "data": "Updated document 1"},
+                {"id": "document_id2", "data": "Updated document 2"},
+            ]
+            results = await embedbase.update("my_dataset", documents)
+        """
+        update_url = f"{self.embedbase_url}/{dataset}"
+        async with httpx.AsyncClient() as client:
+            res = await client.put(
+                update_url,
+                headers=self.headers,
+                json={"documents": [dict(doc) for doc in documents]},
+                timeout=self.timeout,
             )
+            try:
+                data = res.json()
+            except json.JSONDecodeError:
+                # pylint: disable=raise-missing-from
+                raise EmbedbaseAPIException(res.text)
+
+            if res.status_code != 200:
+                raise EmbedbaseAPIException(data.get("error", res.text))
 
-        return merged_context
+            return [Document(**result) for result in data["results"]]
```

### Comparing `embedbase_client-0.2.0/embedbase_client/base.py` & `embedbase_client-0.2.2/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/embedbase_client/errors.py` & `embedbase_client-0.2.2/embedbase_client/errors.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/embedbase_client/model.py` & `embedbase_client-0.2.2/embedbase_client/model.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/embedbase_client/split.py` & `embedbase_client-0.2.2/embedbase_client/split.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/embedbase_client/sync_client.py` & `embedbase_client-0.2.2/embedbase_client/sync_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Generator, List, Optional
+from typing import Any, Dict, Generator, List, Optional, Union
 
 import itertools
 import json
 from dataclasses import dataclass
 from multiprocessing.pool import ThreadPool
 
 import requests
@@ -276,14 +276,33 @@
             A string containing the context.
 
         Example usage:
             context = dataset.create_max_context("What is Python?", max_tokens=100)
         """
         return self.client.create_max_context(self.dataset, query, max_tokens)
 
+    def update(self, documents: List[Document]) -> List[Document]:
+        """
+        Update the documents in the specified dataset.
+
+        Args:
+            documents: A list of documents to update.
+
+        Returns:
+            A list of updated documents.
+
+        Example usage:
+            documents = [
+                Document(id="document_id1", data="Updated document 1"),
+                Document(id="document_id2", data="Updated document 2"),
+            ]
+            results = dataset.update(documents)
+        """
+        return self.client.update(self.dataset, documents)
+
 
 class EmbedbaseClient(BaseClient):
     def __init__(
         self,
         embedbase_url: str = "https://api.embedbase.xyz",
         embedbase_key: Optional[str] = None,
         fastapi_app: Optional[Any] = None,
@@ -596,52 +615,112 @@
         with ThreadPool() as pool:
             pool.map(add_batch, batch_chunks(chunks, parallel_batch_size))
 
         return list(itertools.chain.from_iterable(results))
 
     def create_max_context(
         self,
-        dataset: str,
+        dataset: Union[str, List[str]],
         query: str,
-        max_tokens: int,
+        max_tokens: Union[int, List[int]],
     ) -> str:
         """
-        Create a context from a query by searching for similar documents and concatenating them up to the specified max tokens.
+        Create a context from a query by searching for similar documents and
+        concatenating them up to the specified max tokens.
 
         Args:
             dataset: The name of the dataset to search.
             query: The query to search for.
             max_tokens: the maximum number of tokens for the context.
 
         Returns:
             A string containing the context.
 
         Example usage:
-            context = embedbase.create_max_context("my_dataset", "What is Python?", max_tokens=30)
+            context = create_max_context("programming", "Python is a programming language.", 30)
             print(context)
             # Python is a programming language.
             # Python is a high-level, general-purpose programming language.
             # Python is interpreted, dynamically typed and garbage-collected.
             # Python is designed to be highly extensible.
-            # Python is a multi-paradig...
+            # Python is a multi-paradig
+            # or
+            context = create_max_context(["programming", "science"], "Python lives planet earth.", [3, 30])
+            print(context)
+            # Pyt
+            # The earth orbits the sun.
+            # The earth is the third planet from the sun.
+            # The earth is the only planet known to support life.
+            # The earth formed approximately 4.5 billion years ago.
+            # The earth's gravity interacts with other objects in space, especially the sun and the moon.
         """
 
-        # try to build a context until it's big enough by incrementing top_k
-        top_k = 100
-        context = self.create_context(dataset, query, top_k)
-        merged_context, size = merge_and_return_tokens(context, max_tokens)
-
-        tries = 0
-        max_tries = 3
-        while size < max_tokens and tries < max_tries:
-            top_k *= 3
+        def create_context_for_dataset(dataset, max_tokens):
+            top_k = 100
             context = self.create_context(dataset, query, top_k)
             merged_context, size = merge_and_return_tokens(context, max_tokens)
-            tries += 1
 
-        if size < max_tokens:
-            # warn the user that the context is smaller than the max tokens
-            print(
-                f"Warning: context is smaller than the max tokens ({size} < {max_tokens})"
-            )
+            tries = 0
+            max_tries = 3
+            while size < max_tokens and tries < max_tries:
+                top_k *= 3
+                context = self.create_context(dataset, query, top_k)
+                merged_context, size = merge_and_return_tokens(context, max_tokens)
+                tries += 1
+
+            if size < max_tokens:
+                print(
+                    f"Warning: context for dataset '{dataset}' is smaller than the max tokens ({size} < {max_tokens})"
+                )
+            return merged_context
+
+        if not isinstance(dataset, list):
+            dataset = [dataset]
+
+        if not isinstance(max_tokens, list):
+            max_tokens = [max_tokens for _ in range(len(dataset))]
+
+        if len(dataset) != len(max_tokens):
+            raise ValueError("The number of datasets and max_tokens should be equal.")
+
+        contexts = []
+        for ds, mt in zip(dataset, max_tokens):
+            context = create_context_for_dataset(ds, mt)
+            contexts.append(context)
+
+        return "\n\n".join(contexts)
+
+    def update(self, dataset: str, documents: List[Document]) -> List[Document]:
+        """
+        Update the documents in the specified dataset.
+
+        Args:
+            dataset: The name of the dataset to update.
+            documents: A list of documents to update.
+
+        Returns:
+            A list of updated documents.
+
+        Example usage:
+            documents = [
+                Document(id="document_id1", data="Updated document 1"),
+                Document(id="document_id2", data="Updated document 2"),
+            ]
+            results = embedbase.update("my_dataset", documents)
+        """
+        update_url = f"{self.embedbase_url}/{dataset}"
+        res = requests.put(
+            update_url,
+            headers=self.headers,
+            json={"documents": [doc.dict() for doc in documents]},
+            timeout=self.timeout,
+        )
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
+            raise EmbedbaseAPIException(res.text)
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
 
-        return merged_context
+        return [Document(**result) for result in data["results"]]
```

### Comparing `embedbase_client-0.2.0/embedbase_client/utils.py` & `embedbase_client-0.2.2/embedbase_client/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.2.0/pyproject.toml` & `embedbase_client-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.2.0"
+version = "0.2.2"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 
@@ -139,8 +139,8 @@
 source = "embedbase-client"
 
 [coverage.run]
 branch = true
 
 [coverage.report]
 fail_under = 50
-show_missing = true
+show_missing = true
```

### Comparing `embedbase_client-0.2.0/PKG-INFO` & `embedbase_client-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.2.0
+Version: 0.2.2
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.2.0 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.2.2 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

