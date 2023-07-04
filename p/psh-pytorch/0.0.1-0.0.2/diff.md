# Comparing `tmp/psh-pytorch-0.0.1.tar.gz` & `tmp/psh-pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psh-pytorch-0.0.1.tar", last modified: Mon Jul  3 21:52:39 2023, max compression
+gzip compressed data, was "psh-pytorch-0.0.2.tar", last modified: Tue Jul  4 01:11:00 2023, max compression
```

## Comparing `psh-pytorch-0.0.1.tar` & `psh-pytorch-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 21:52:39.683034 psh-pytorch-0.0.1/
--rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 13:56:32.000000 psh-pytorch-0.0.1/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)     1372 2023-07-03 21:52:39.683034 psh-pytorch-0.0.1/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      865 2023-07-03 21:51:51.000000 psh-pytorch-0.0.1/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      678 2023-07-03 21:40:38.000000 psh-pytorch-0.0.1/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       23 2023-07-03 19:52:00.000000 psh-pytorch-0.0.1/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-03 21:52:39.683034 psh-pytorch-0.0.1/setup.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 21:52:39.683034 psh-pytorch-0.0.1/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 21:52:39.683034 psh-pytorch-0.0.1/src/psh_pytorch/
--rw-rw-r--   0 david     (1000) david     (1000)       35 2023-07-03 21:42:08.000000 psh-pytorch-0.0.1/src/psh_pytorch/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    16644 2023-07-03 21:43:08.000000 psh-pytorch-0.0.1/src/psh_pytorch/psh.py
--rw-rw-r--   0 david     (1000) david     (1000)     1249 2023-07-03 17:59:41.000000 psh-pytorch-0.0.1/src/psh_pytorch/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 21:52:39.683034 psh-pytorch-0.0.1/src/psh_pytorch.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1372 2023-07-03 21:52:39.000000 psh-pytorch-0.0.1/src/psh_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      319 2023-07-03 21:52:39.000000 psh-pytorch-0.0.1/src/psh_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-03 21:52:39.000000 psh-pytorch-0.0.1/src/psh_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       24 2023-07-03 21:52:39.000000 psh-pytorch-0.0.1/src/psh_pytorch.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       12 2023-07-03 21:52:39.000000 psh-pytorch-0.0.1/src/psh_pytorch.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 13:56:32.000000 psh-pytorch-0.0.2/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)     2411 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1904 2023-07-03 23:21:44.000000 psh-pytorch-0.0.2/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      730 2023-07-04 01:10:49.000000 psh-pytorch-0.0.2/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       23 2023-07-03 19:52:00.000000 psh-pytorch-0.0.2/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/src/psh_pytorch/
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2023-07-03 21:42:08.000000 psh-pytorch-0.0.2/src/psh_pytorch/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16062 2023-07-04 00:22:51.000000 psh-pytorch-0.0.2/src/psh_pytorch/psh.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1969 2023-07-04 00:21:40.000000 psh-pytorch-0.0.2/src/psh_pytorch/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     2411 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      336 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       24 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       12 2023-07-04 01:11:00.000000 psh-pytorch-0.0.2/src/psh_pytorch.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-04 01:11:00.258708 psh-pytorch-0.0.2/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     3432 2023-07-04 00:55:28.000000 psh-pytorch-0.0.2/tests/test_2d.py
```

### Comparing `psh-pytorch-0.0.1/LICENSE` & `psh-pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psh-pytorch-0.0.1/PKG-INFO` & `psh-pytorch-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: psh-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Perfect Spatial Hashing in PyTorch
 Author-email: David Li <david@davidl.me>
 Project-URL: Homepage, https://github.com/dli7319/psh-pytorch
 Project-URL: Bug Tracker, https://github.com/dli7319/psh-pytorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# perfecthash-pytorch
-Perfect Spatial Hashing in PyTorch
+# Perfect Spatial Hashing in PyTorch
+This library is an unofficial implementation of [Perfect Spatial Hashing by Lefebvre and Hoppe](https://hhoppe.com/perfecthash.pdf).
 
 ## Usage
 Install the library with:
 ```bash
+# For the latest version:
 pip install git+https://github.com/dli7319/psh-pytorch.git
+
+# For the PyPI version:
+# pip install psh-pytorch
 ```
 
 Instantiate a `PerfectSpatialHash` object with:
 ```python
 from psh_pytorch import PerfectSpatialHash
 
 occupancy_grid # A 2D (or higher dimensional) occupancy grid
@@ -40,7 +44,34 @@
 #   Sparsity is of shape (128 * 128)
 #   Note that values are unmasked
 masked_values = values * sparsity.unsqueeze(-1)
 ```
 
 ## Examples
 See `examples/` for a simple example of how to use the library.
+
+## Limitations
+
+1. Currently, interpolation is not supported. Hence, you must use long indices and there are no gradients with respect to the indices.
+
+## Acknowledgement
+If you find this library useful, please consider citing the original paper:
+```bibtex
+@article{lefebvre2006perfect,
+author = {Lefebvre, Sylvain and Hoppe, Hugues},
+title = {Perfect Spatial Hashing},
+year = {2006},
+issue_date = {July 2006},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+volume = {25},
+number = {3},
+issn = {0730-0301},
+url = {https://doi.org/10.1145/1141911.1141926},
+doi = {10.1145/1141911.1141926},
+journal = {ACM Trans. Graph.},
+month = {jul},
+pages = {579–588},
+numpages = {10},
+keywords = {vector images, minimal perfect hash, sparse data, adaptive textures, multidimensional hashing, 3D-parameterized textures}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psh-pytorch-0.0.1/pyproject.toml` & `psh-pytorch-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "psh-pytorch"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="David Li", email="david@davidl.me" },
 ]
 description = "Perfect Spatial Hashing in PyTorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,8 +19,13 @@
 
 [project.urls]
 "Homepage" = "https://github.com/dli7319/psh-pytorch"
 "Bug Tracker" = "https://github.com/dli7319/psh-pytorch/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
```

### Comparing `psh-pytorch-0.0.1/src/psh_pytorch/psh.py` & `psh-pytorch-0.0.2/src/psh_pytorch/psh.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,16 @@
-from typing import Optional, Union
+from typing import Optional
 
 import numpy as np
 import torch
 from torch import nn
 import tqdm
 
 from . import utils
 
-C1 = 1178101
-
-
-def sparsity_hash(k: Union[int, torch.Tensor], p: torch.Tensor) -> torch.Tensor:
-    """Hash function used for sparsity encoding
-
-    Args:
-        k: Which hash to use.
-        p: Points to hash as (N, D) tensor.
-
-    Returns:
-        torch.Tensor: The hash as (N,) tensor.
-    """
-    if isinstance(k, int):
-        k = torch.tensor(k, device=p.device, dtype=torch.uint8)
-    k = k.unsqueeze(-1)
-    hk = (p * (p + k * C1).rsqrt()).sum(dim=-1).frac()
-    return (256 * hk).clamp(0, 255).to(torch.uint8)
-
 
 class PerfectSpatialHash(nn.Module):
     def __init__(self, occupancy_grid: torch.Tensor, feature_channels: int,
                  fast_construction: bool = True,
                  offset_table_size: Optional[int] = None,
                  fast_construction_offset_table_progression: float = 1.1,
                  verbose=False):
@@ -245,49 +226,47 @@
                                        f"pixels {occupied_indices_bincount[ordering[current_index]].item()}]")
                 return False
         # if self.verbose:
         #     print("offset_table_assigned", offset_table_assigned)
         return True
 
     def _build_sparsity_encoding(self, occupancy_grid: torch.Tensor):
-        unoccupied_grid = ~occupancy_grid
         sparsity_k = torch.zeros(
             self.hash_table[..., 0].shape, dtype=torch.uint8, device=self.hash_table.device)
         sparsity_hk = torch.zeros(
             self.hash_table[..., 0].shape, dtype=torch.uint8, device=self.hash_table.device)
 
         occupied_indices = occupancy_grid.nonzero(as_tuple=False)
         occupied_indices_hashed = self.compute_hash(occupied_indices)
         sparsity_k[occupied_indices_hashed.unbind(-1)] = 1
         sparsity_hk[occupied_indices_hashed.unbind(
-            -1)] = sparsity_hash(1, occupied_indices)
+            -1)] = utils.sparsity_hash(1, occupied_indices)
 
+        unoccupied_grid = ~occupancy_grid
         unoccupied_indices = unoccupied_grid.nonzero(as_tuple=False)
         unoccupied_indices_hashed = self.compute_hash(unoccupied_indices)
         for i in range(1, 256):
-            unoccupied_indices_shashed = sparsity_hash(
+            unoccupied_indices_shashed = utils.sparsity_hash(
                 sparsity_k[unoccupied_indices_hashed.unbind(-1)], unoccupied_indices)
             collisions = torch.logical_and(
                 sparsity_k[unoccupied_indices_hashed.unbind(-1)] != 0,
                 sparsity_hk[unoccupied_indices_hashed.unbind(-1)] == unoccupied_indices_shashed)
             number_of_collisions = collisions.sum()
             self.verbose and print(
                 f"Number of collisions for {i} is {number_of_collisions}")
             if number_of_collisions == 0:
                 break
             sparsity_k[unoccupied_indices_hashed[collisions].unbind(-1)] = 0
-            sparsity_hk[unoccupied_indices_hashed[collisions].unbind(-1)] = (
-                sparsity_hk[unoccupied_indices_hashed[collisions].unbind(-1)] + 1)
-            if i < 254:
+            if i < 255:
                 collided_indices = sparsity_k[occupied_indices_hashed.unbind(
                     -1)] == 0
                 sparsity_k[occupied_indices_hashed[collided_indices]
                            .unbind(-1)] = i+1
                 sparsity_hk[occupied_indices_hashed[collided_indices].unbind(
-                    -1)] = sparsity_hash(i+1, occupied_indices[collided_indices])
+                    -1)] = utils.sparsity_hash(i+1, occupied_indices[collided_indices])
         return nn.Parameter(torch.stack([sparsity_k, sparsity_hk], dim=-1),
                             requires_grad=False)
 
     def _compute_offset_hash(self, x: torch.Tensor) -> torch.Tensor:
         """Compute the hash of the input tensor into the offset table.
 
         Args:
@@ -319,15 +298,15 @@
             Tuple[torch.Tensor, torch.Tensor]: Hashed values and sparsity.
         """
         hash_indices = self.compute_hash(x)
         values = self.hash_table[hash_indices.unbind(-1)]
         sparsity_k, sparsity_hk = self.sparsity_encoding[hash_indices.unbind(
             -1)].unbind(-1)
         correct_hk = torch.logical_and(
-            sparsity_k > 0, sparsity_hash(sparsity_k, x) == sparsity_hk)
+            sparsity_k > 0, utils.sparsity_hash(sparsity_k, x) == sparsity_hk)
         return values, correct_hk
 
     def encode(self, positions: torch.Tensor, values: torch.Tensor):
         """Encode the input values into the hash table.
 
         Args:
             positions (torch.Tensor): Positions of the input values.
@@ -337,10 +316,13 @@
         self.hash_table.data[hash_indices.unbind(-1)] = values
 
     def check_collisions(self, positions: torch.Tensor) -> bool:
         """Check if there are any collisions at the given positions.
 
         Args:
             positions (torch.Tensor): Positions to check.
+
+        Returns:
+            bool: True if there are collisions, False otherwise.
         """
         hash_indices = self.compute_hash(positions)
         return torch.unique(hash_indices, dim=0).shape[0] != hash_indices.shape[0]
```

### Comparing `psh-pytorch-0.0.1/src/psh_pytorch.egg-info/PKG-INFO` & `psh-pytorch-0.0.2/src/psh_pytorch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: psh-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Perfect Spatial Hashing in PyTorch
 Author-email: David Li <david@davidl.me>
 Project-URL: Homepage, https://github.com/dli7319/psh-pytorch
 Project-URL: Bug Tracker, https://github.com/dli7319/psh-pytorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# perfecthash-pytorch
-Perfect Spatial Hashing in PyTorch
+# Perfect Spatial Hashing in PyTorch
+This library is an unofficial implementation of [Perfect Spatial Hashing by Lefebvre and Hoppe](https://hhoppe.com/perfecthash.pdf).
 
 ## Usage
 Install the library with:
 ```bash
+# For the latest version:
 pip install git+https://github.com/dli7319/psh-pytorch.git
+
+# For the PyPI version:
+# pip install psh-pytorch
 ```
 
 Instantiate a `PerfectSpatialHash` object with:
 ```python
 from psh_pytorch import PerfectSpatialHash
 
 occupancy_grid # A 2D (or higher dimensional) occupancy grid
@@ -40,7 +44,34 @@
 #   Sparsity is of shape (128 * 128)
 #   Note that values are unmasked
 masked_values = values * sparsity.unsqueeze(-1)
 ```
 
 ## Examples
 See `examples/` for a simple example of how to use the library.
+
+## Limitations
+
+1. Currently, interpolation is not supported. Hence, you must use long indices and there are no gradients with respect to the indices.
+
+## Acknowledgement
+If you find this library useful, please consider citing the original paper:
+```bibtex
+@article{lefebvre2006perfect,
+author = {Lefebvre, Sylvain and Hoppe, Hugues},
+title = {Perfect Spatial Hashing},
+year = {2006},
+issue_date = {July 2006},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+volume = {25},
+number = {3},
+issn = {0730-0301},
+url = {https://doi.org/10.1145/1141911.1141926},
+doi = {10.1145/1141911.1141926},
+journal = {ACM Trans. Graph.},
+month = {jul},
+pages = {579–588},
+numpages = {10},
+keywords = {vector images, minimal perfect hash, sparse data, adaptive textures, multidimensional hashing, 3D-parameterized textures}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

