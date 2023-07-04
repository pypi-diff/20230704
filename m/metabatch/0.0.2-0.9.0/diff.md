# Comparing `tmp/metabatch-0.0.2.tar.gz` & `tmp/metabatch-0.9.0.tar.gz`

## Comparing `metabatch-0.0.2.tar` & `metabatch-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 metabatch-0.0.2/src/metabatch/__init__.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 metabatch-0.0.2/src/metabatch/dataloader.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 metabatch-0.0.2/src/metabatch/dataset.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 metabatch-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metabatch-0.0.2/LICENSE
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 metabatch-0.0.2/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 metabatch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 metabatch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 metabatch-0.9.0/examples/maml-omniglot.py
+-rw-r--r--   0        0        0    20267 2020-02-02 00:00:00.000000 metabatch-0.9.0/examples/maml.py
+-rwxr-xr-x   0        0        0     9613 2020-02-02 00:00:00.000000 metabatch-0.9.0/examples/neural_process.py
+-rw-r--r--   0        0        0    18904 2020-02-02 00:00:00.000000 metabatch-0.9.0/examples/omniglot_loaders.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 metabatch-0.9.0/src/metabatch/__init__.py
+-rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 metabatch-0.9.0/src/metabatch/dataloader.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 metabatch-0.9.0/src/metabatch/dataset.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 metabatch-0.9.0/tests/utils.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 metabatch-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metabatch-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 metabatch-0.9.0/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 metabatch-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 metabatch-0.9.0/PKG-INFO
```

### Comparing `metabatch-0.0.2/src/metabatch/dataloader.py` & `metabatch-0.9.0/src/metabatch/dataloader.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,15 +41,22 @@
     Args:
         dataset (Dataset): Dataset.
         batch_size (int): Size of mini-batch.
         drop_last (bool): If ``True``, the sampler will drop the last batch if
             its size would be less than ``batch_size``
     """
 
-    def __init__(self, dataset, batch_size, drop_last, shuffle: bool = False):
+    def __init__(
+        self,
+        dataset,
+        batch_size,
+        drop_last,
+        shuffle: bool = False,
+        iterations: Optional[int] = None,
+    ):
         if (
             not isinstance(batch_size, int)
             or isinstance(batch_size, bool)
             or batch_size <= 0
         ):
             raise ValueError(
                 "batch_size should be a positive integer value, "
@@ -62,29 +69,48 @@
             )
         if not isinstance(shuffle, bool):
             raise ValueError(
                 "shuffle should be a boolean value, but got "
                 "shuffle={}".format(shuffle)
             )
         self.batch_size = batch_size
-        self.drop_last = drop_last
+        self.drop_last = drop_last if iterations is None else False
+        self.n_batches = iterations
         self._sampling_inst = Manager().dict()
         dataset.register_sampling_inst(
             self._sampling_inst
         )  # Will modify every copy assigned to all workers, so they all get the same sampling_inst reference
         self.dataset = dataset
-        self.sampler = RandomSampler(dataset) if shuffle else SequentialSampler(dataset)
+        if iterations is not None and iterations <= 0:
+            raise ValueError(
+                "Number of iterations should be a positive integer value, "
+                "but got num_iterations={}".format(iterations)
+            )
+        if iterations is not None and not shuffle:
+            raise ValueError(
+                "shuffle should be True when num_iterations is not None, "
+                "but got shuffle={}".format(shuffle)
+            )
+        self.sampler = (
+            RandomSampler(
+                dataset,
+                replacement=iterations is not None,
+                num_samples=iterations * batch_size if iterations is not None else None,
+            )
+            if shuffle
+            else SequentialSampler(dataset)
+        )
 
     def new_batch(self):
         n_context = random.randint(self.dataset.min_pts, self.dataset.max_ctx_pts)
         n_targets = (
             (
                 self.dataset.total_tgt_pts - n_context
-                if self.dataset.eval
-                else random.randint(self.dataset.min_pts, self.dataset.max_tgt_pts)
+                if self.dataset.eval and self.dataset.predict_full_target_during_eval
+                else random.randint(n_context, self.dataset.max_tgt_pts)
             )
             if not self.dataset.predict_full_target
             else self.dataset.total_tgt_pts
         )
         return n_context, n_targets
 
     def __iter__(self) -> Iterator[List[int]]:
@@ -105,39 +131,70 @@
                     yield batch
                     ctx_pts, tgt_pts = self.new_batch()
                 except StopIteration:
                     break
         else:
             batch = [0] * self.batch_size
             idx_in_batch = 0
-            for idx in self.sampler:
-                self._sampling_inst[idx] = (ctx_pts, tgt_pts)
-                batch[idx_in_batch] = idx
-                idx_in_batch += 1
-                if idx_in_batch == self.batch_size:
-                    yield batch
-                    idx_in_batch = 0
-                    batch = [0] * self.batch_size
-                    ctx_pts, tgt_pts = self.new_batch()
+            n_batches = 0
+            if self.n_batches is not None:
+                while n_batches < self.n_batches:  # type: ignore
+                    for idx in self.sampler:
+                        if n_batches >= self.n_batches:  # type: ignore
+                            break
+                        # Because I'm using a dict, I can't have duplicate indices in
+                        # the batch. However, I'm setting replacement=True in the RandomSampler, so I can
+                        # have duplicate indices. A quick hack is to skip the duplicate indices:
+                        if idx in self._sampling_inst.keys():
+                            # This effectively prevents the batch from having duplicate elements, while
+                            # allowing to resample previously seen elements in future batches. This way, we
+                            # can continue to train on the same dataset indefinitely or for an arbitrary
+                            # number of iterations.
+                            # We also need to update the number of samples in the sampler because it is not
+                            # aware that we skipped some samples.
+                            self.sampler._num_samples += 1  # type: ignore
+                            continue
+                        self._sampling_inst[idx] = (ctx_pts, tgt_pts)
+                        batch[idx_in_batch] = idx
+                        idx_in_batch += 1
+                        if idx_in_batch == self.batch_size:
+                            n_batches += 1
+                            yield batch
+                            idx_in_batch = 0
+                            batch = [0] * self.batch_size
+                            ctx_pts, tgt_pts = self.new_batch()
+            else:
+                for idx in self.sampler:
+                    self._sampling_inst[idx] = (ctx_pts, tgt_pts)
+                    batch[idx_in_batch] = idx
+                    idx_in_batch += 1
+                    if idx_in_batch == self.batch_size:
+                        yield batch
+                        idx_in_batch = 0
+                        batch = [0] * self.batch_size
+                        ctx_pts, tgt_pts = self.new_batch()
             if idx_in_batch > 0:
                 yield batch[:idx_in_batch]
 
     def __len__(self):
-        if self.drop_last:
+        if self.n_batches is not None:
+            return self.n_batches
+        elif self.drop_last:
             return len(self.sampler) // self.batch_size
         else:
             return (len(self.sampler) + self.batch_size - 1) // self.batch_size
 
 
 class TaskLoader(DataLoader):
     def __init__(
         self,
         dataset: Dataset,
         batch_size: Optional[int] = 1,
         shuffle: bool = False,
+        n_batches: Optional[int] = None,
         num_workers: int = 0,
         collate_fn: Optional[Callable] = None,
         pin_memory: bool = False,
         drop_last: bool = False,
         timeout: float = 0,
         worker_init_fn: Optional[Callable] = None,
         multiprocessing_context=None,
@@ -145,16 +202,17 @@
         *,
         prefetch_factor: int = 2,
         persistent_workers: bool = False,
         pin_memory_device: str = ""
     ):
         super().__init__(
             dataset,
-            batch_size=batch_size,
-            batch_sampler=SeededBatchSampler(dataset, batch_size, drop_last, shuffle),
+            batch_sampler=SeededBatchSampler(
+                dataset, batch_size, drop_last, shuffle, n_batches
+            ),
             num_workers=num_workers,
             collate_fn=collate_fn,
             pin_memory=pin_memory,
             timeout=timeout,
             worker_init_fn=worker_init_fn,
             multiprocessing_context=multiprocessing_context,
             generator=generator,
```

### Comparing `metabatch-0.0.2/src/metabatch/dataset.py` & `metabatch-0.9.0/src/metabatch/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,34 +21,37 @@
         self,
         min_pts: int,
         max_ctx_pts: int,
         max_tgt_pts: int,
         total_tgt_pts: int,
         eval: bool,
         predict_full_target: bool,
+        predict_full_target_during_eval: bool,
     ):
+        assert max_ctx_pts >= min_pts, "max_ctx_pts must be greater than min_pts"
+        assert max_ctx_pts < max_tgt_pts, "max_ctx_pts must be smaller than max_tgt_pts"
         self.max_ctx_pts = max_ctx_pts
         self.max_tgt_pts = max_tgt_pts
         self.min_pts = min_pts
         self.total_tgt_pts = total_tgt_pts
         self.eval = eval
         self.predict_full_target = predict_full_target
+        self.predict_full_target_during_eval = predict_full_target_during_eval
         self._sampling_instructor = None
 
     def register_sampling_inst(self, sampling_inst: DictProxy):
         self._sampling_instructor = sampling_inst
 
     def __getitem__(self, index: Union[int, List[int]]) -> Tuple:
         assert self._sampling_instructor is not None, "sampling_inst attribute not set!"
         try:
-            n_context, n_targets = self._sampling_instructor.pop(index)
+            n_context, n_target = self._sampling_instructor.pop(index)
         except KeyError as e:
             print(
                 f"Could not get key {e} from sampling_inst -- make sure you are using the SeededBatchSampler as the batch_sampler argument of the DataLoader!"
             )
             raise e
-        self.__gettask__(index, n_context, n_targets)
-
+        return self.__gettask__(index, n_context, n_target)
 
     @abc.abstractmethod
-    def __gettask__(self, index, n_context, n_targets):
+    def __gettask__(self, index, n_context, n_target):
         raise NotImplementedError
```

### Comparing `metabatch-0.0.2/LICENSE` & `metabatch-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metabatch-0.0.2/README.md` & `metabatch-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Introduction
 
 MetaBatch is a micro-framework for meta-learning in PyTorch. It provides convenient `Taskset` and
-`TaskLoader` classes for efficient batching and fast meta-training in a few-shot learning context.
+`TaskLoader` classes for **batch-aware online task creation for meta-learning**.
 
 ## Efficient batching
 
 Training meta-learning models efficiently can be a challenge, especially when it comes to creating
 random tasks of a consistent shape in one batch. The task creation process can be time-consuming
-and typically requires all tasks to have the same amount of context and target points. This can be
-a bottleneck during training:
+and typically requires all tasks in the batch to have the same amount of context and target points.
+This can be a bottleneck during training:
 
 ```python
 # Sample code for creating a batch of tasks with traditional approach
 class MyTaskDataset(Dataset):
     ...
     def __getitem__(self, idx):
         task = self.task_data[idx]
@@ -45,16 +45,15 @@
     model(tasks)
     ...
 ```
 
 ### Multiprocessing
 Wouldn't it be better to offload the task creation to the dataloader, so that it can be done in
 parallel on multiple cores?
-With **MetaBatch**, we simplify the process by allowing you to do just
-that.
+With **MetaBatch**, we simplify the process by allowing you to do just that.
 We provide a `TaskSet` wrapper, where you can implement the `__gettask__(self, index, n_context,
 n_target)__` method instead of PyTorch's `__getitem(self, index)__`. Our `TaskLoader` and
 custom sampler take care of synchronizing `n_context` and `n_target` for each batch element
 dispatched to all workers. With **MetaBatch**, the training bottleneck can be removed from the
 above example:
 ```python
 # Sample code for creating a batch of tasks with MetaBatch
@@ -88,21 +87,37 @@
     ...
     # Simply access the batch of constructed tasks (no bottleneck!)
     model(batch)
     ...
 
 ```
 
-## Advantages
+## Installation & usage
+
+Install it: `pip install metabatch`
+
+Requirements:
+- `pytorch`
 
-- MetaBatch allows for efficient task creation and batching during training, resulting in faster training times.
-- Our approach provides more task diversity and allows for easy customization of task creation.
+Look at the example above for an idea or how to use `TaskLoader` with `TaskSet`, or go through the
+examples in `examples/` (**TODO**).
 
 
+
+## Advantages
+
+- MetaBatch allows for efficient task creation and batching during training, resulting in more task
+    variations since you are no longer limited to precomputed tasks.
+- Reduces boilerplate needed to precompute and load tasks.
+
 MetaBatch is a micro-framework for meta-learning in PyTorch that provides convenient tools for
-faster meta-training. It simplifies the task creation process and allows for efficient batching,
+(potentially faster) meta-training. It simplifies the task creation process and allows for efficient batching,
 making it a useful tool for researchers and engineers working on meta-learning projects.
 
+## How much faster?
+
+**TODO**: benchmark MAML and CNP examples with typical implementation and other repos.
+
 
 ## License
 
 MetaBatch is released under the MIT License. See the LICENSE file for more information.
```

### Comparing `metabatch-0.0.2/PKG-INFO` & `metabatch-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: metabatch
-Version: 0.0.2
+Version: 0.9.0
 Summary: MetaBatch: A micro-framework for efficient batching of tasks in PyTorch.
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/DubiousCactus/metabatch
+Project-URL: Bug Tracker, https://github.com/DubiousCactus/metabatch/issues
 Author-email: Théo Morales <moralest@tcd.ie>
 License-File: LICENSE
 Keywords: MAML,dataset,deep,few-shot,learning,meta,meta-learning,pytorch,task,taskset
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Introduction
 
 MetaBatch is a micro-framework for meta-learning in PyTorch. It provides convenient `Taskset` and
-`TaskLoader` classes for efficient batching and fast meta-training in a few-shot learning context.
+`TaskLoader` classes for **batch-aware online task creation for meta-learning**.
 
 ## Efficient batching
 
 Training meta-learning models efficiently can be a challenge, especially when it comes to creating
 random tasks of a consistent shape in one batch. The task creation process can be time-consuming
-and typically requires all tasks to have the same amount of context and target points. This can be
-a bottleneck during training:
+and typically requires all tasks in the batch to have the same amount of context and target points.
+This can be a bottleneck during training:
 
 ```python
 # Sample code for creating a batch of tasks with traditional approach
 class MyTaskDataset(Dataset):
     ...
     def __getitem__(self, idx):
         task = self.task_data[idx]
@@ -63,16 +63,15 @@
     model(tasks)
     ...
 ```
 
 ### Multiprocessing
 Wouldn't it be better to offload the task creation to the dataloader, so that it can be done in
 parallel on multiple cores?
-With **MetaBatch**, we simplify the process by allowing you to do just
-that.
+With **MetaBatch**, we simplify the process by allowing you to do just that.
 We provide a `TaskSet` wrapper, where you can implement the `__gettask__(self, index, n_context,
 n_target)__` method instead of PyTorch's `__getitem(self, index)__`. Our `TaskLoader` and
 custom sampler take care of synchronizing `n_context` and `n_target` for each batch element
 dispatched to all workers. With **MetaBatch**, the training bottleneck can be removed from the
 above example:
 ```python
 # Sample code for creating a batch of tasks with MetaBatch
@@ -106,21 +105,37 @@
     ...
     # Simply access the batch of constructed tasks (no bottleneck!)
     model(batch)
     ...
 
 ```
 
-## Advantages
+## Installation & usage
+
+Install it: `pip install metabatch`
+
+Requirements:
+- `pytorch`
 
-- MetaBatch allows for efficient task creation and batching during training, resulting in faster training times.
-- Our approach provides more task diversity and allows for easy customization of task creation.
+Look at the example above for an idea or how to use `TaskLoader` with `TaskSet`, or go through the
+examples in `examples/` (**TODO**).
 
 
+
+## Advantages
+
+- MetaBatch allows for efficient task creation and batching during training, resulting in more task
+    variations since you are no longer limited to precomputed tasks.
+- Reduces boilerplate needed to precompute and load tasks.
+
 MetaBatch is a micro-framework for meta-learning in PyTorch that provides convenient tools for
-faster meta-training. It simplifies the task creation process and allows for efficient batching,
+(potentially faster) meta-training. It simplifies the task creation process and allows for efficient batching,
 making it a useful tool for researchers and engineers working on meta-learning projects.
 
+## How much faster?
+
+**TODO**: benchmark MAML and CNP examples with typical implementation and other repos.
+
 
 ## License
 
 MetaBatch is released under the MIT License. See the LICENSE file for more information.
```

