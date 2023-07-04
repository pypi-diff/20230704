# Comparing `tmp/torch_mist-0.1.0.tar.gz` & `tmp/torch_mist-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_mist-0.1.0.tar", max compression
+gzip compressed data, was "torch_mist-0.1.1.tar", max compression
```

## Comparing `torch_mist-0.1.0.tar` & `torch_mist-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,55 @@
--rwxr-xr-x   0        0        0     1073 2023-06-20 12:29:18.481563 torch_mist-0.1.0/LICENSE
--rw-r--r--   0        0        0     1295 2023-06-21 15:06:40.740837 torch_mist-0.1.0/README.md
--rw-r--r--   0        0        0      623 2023-06-20 13:52:25.056289 torch_mist-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-06-20 13:16:41.292074 torch_mist-0.1.0/src/torch_mist/__init__.py
--rw-r--r--   0        0        0     4717 2023-06-21 11:51:25.062984 torch_mist-0.1.0/src/torch_mist/baselines.py
--rw-r--r--   0        0        0      153 2023-06-21 12:06:46.937453 torch_mist-0.1.0/src/torch_mist/critic/__init__.py
--rw-r--r--   0        0        0      592 2023-06-21 12:06:46.949453 torch_mist-0.1.0/src/torch_mist/critic/base.py
--rw-r--r--   0        0        0      786 2023-06-21 12:06:46.957453 torch_mist-0.1.0/src/torch_mist/critic/joint.py
--rw-r--r--   0        0        0     1441 2023-06-21 12:06:46.925453 torch_mist-0.1.0/src/torch_mist/critic/separable.py
--rw-r--r--   0        0        0     2228 2023-06-21 12:06:46.953453 torch_mist-0.1.0/src/torch_mist/critic/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 14:21:09.749889 torch_mist-0.1.0/src/torch_mist/distributions/__init__.py
--rw-r--r--   0        0        0      142 2023-06-12 08:43:58.195274 torch_mist-0.1.0/src/torch_mist/distributions/conditional/__init__.py
--rw-r--r--   0        0        0      784 2023-06-12 08:43:58.195274 torch_mist-0.1.0/src/torch_mist/distributions/conditional/categorical.py
--rw-r--r--   0        0        0     3151 2023-06-12 08:43:58.195274 torch_mist-0.1.0/src/torch_mist/distributions/conditional/correlated_normal.py
--rw-r--r--   0        0        0      219 2023-06-15 14:06:39.255551 torch_mist-0.1.0/src/torch_mist/distributions/parametrizations/__init__.py
--rw-r--r--   0        0        0     4422 2023-06-15 13:56:24.677843 torch_mist-0.1.0/src/torch_mist/distributions/parametrizations/map.py
--rw-r--r--   0        0        0     1287 2023-06-12 09:14:10.064574 torch_mist-0.1.0/src/torch_mist/distributions/product.py
--rw-r--r--   0        0        0      314 2023-06-21 15:01:15.039823 torch_mist-0.1.0/src/torch_mist/distributions/transforms/__init__.py
--rw-r--r--   0        0        0     3914 2023-06-22 12:19:45.078198 torch_mist-0.1.0/src/torch_mist/distributions/transforms/base.py
--rw-r--r--   0        0        0     5651 2023-06-20 13:57:58.756420 torch_mist-0.1.0/src/torch_mist/distributions/transforms/linear.py
--rw-r--r--   0        0        0     2054 2023-06-12 08:43:58.195274 torch_mist-0.1.0/src/torch_mist/distributions/transforms/permute.py
--rw-r--r--   0        0        0     1581 2023-06-12 08:43:58.195274 torch_mist-0.1.0/src/torch_mist/distributions/transforms/split.py
--rw-r--r--   0        0        0     5209 2023-06-22 12:33:39.891363 torch_mist-0.1.0/src/torch_mist/distributions/utils.py
--rw-r--r--   0        0        0      258 2023-06-22 12:06:45.238036 torch_mist-0.1.0/src/torch_mist/estimators/__init__.py
--rw-r--r--   0        0        0     2450 2023-06-19 09:38:20.837508 torch_mist-0.1.0/src/torch_mist/estimators/base.py
--rw-r--r--   0        0        0    15801 2023-06-21 14:47:16.624204 torch_mist-0.1.0/src/torch_mist/estimators/discriminative.py
--rw-r--r--   0        0        0      176 2023-06-22 12:46:48.685026 torch_mist-0.1.0/src/torch_mist/estimators/generative/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-22 12:51:00.677253 torch_mist-0.1.0/src/torch_mist/estimators/generative/ba.py
--rw-r--r--   0        0        0     2574 2023-06-22 13:16:56.867138 torch_mist-0.1.0/src/torch_mist/estimators/generative/base.py
--rw-r--r--   0        0        0     1789 2023-06-22 12:11:23.507661 torch_mist-0.1.0/src/torch_mist/estimators/generative/doe.py
--rw-r--r--   0        0        0     5100 2023-06-22 13:23:37.027279 torch_mist-0.1.0/src/torch_mist/estimators/generative/gm.py
--rw-r--r--   0        0        0     8156 2023-06-22 12:36:54.576290 torch_mist-0.1.0/src/torch_mist/estimators/generative/others.py
--rw-r--r--   0        0        0     1080 2023-06-20 14:13:49.026951 torch_mist-0.1.0/src/torch_mist/estimators/hybrid.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:37.640402 torch_mist-0.1.0/src/torch_mist/nn/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-20 16:19:50.201850 torch_mist-0.1.0/src/torch_mist/nn/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 12:38:35.690908 torch_mist-0.1.0/src/torch_mist/utils/__init__.py
--rw-r--r--   0        0        0     1149 2023-06-22 11:03:06.506402 torch_mist-0.1.0/src/torch_mist/utils/data.py
--rw-r--r--   0        0        0     1872 2023-06-21 14:13:17.383815 torch_mist-0.1.0/src/torch_mist/utils/estimate.py
--rw-r--r--   0        0        0      243 2023-06-15 13:19:26.314708 torch_mist-0.1.0/src/torch_mist/utils/quantization.py
--rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 torch_mist-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-06-20 12:29:18.481563 torch_mist-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9170 2023-07-04 12:17:42.418951 torch_mist-0.1.1/README.md
+-rw-r--r--   0        0        0      640 2023-07-04 12:27:19.053207 torch_mist-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-20 13:16:41.292074 torch_mist-0.1.1/src/torch_mist/__init__.py
+-rw-r--r--   0        0        0     5184 2023-07-03 07:16:14.892467 torch_mist-0.1.1/src/torch_mist/baselines.py
+-rw-r--r--   0        0        0      153 2023-06-21 12:06:46.937453 torch_mist-0.1.1/src/torch_mist/critic/__init__.py
+-rw-r--r--   0        0        0      589 2023-06-26 13:14:22.335963 torch_mist-0.1.1/src/torch_mist/critic/base.py
+-rw-r--r--   0        0        0     1025 2023-06-30 12:05:05.855795 torch_mist-0.1.1/src/torch_mist/critic/joint.py
+-rw-r--r--   0        0        0     1526 2023-06-30 12:05:56.280011 torch_mist-0.1.1/src/torch_mist/critic/separable.py
+-rw-r--r--   0        0        0     2460 2023-07-03 10:00:44.180879 torch_mist-0.1.1/src/torch_mist/critic/utils.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:28:06.302414 torch_mist-0.1.1/src/torch_mist/data/__init__.py
+-rw-r--r--   0        0        0     1750 2023-06-29 13:36:27.280021 torch_mist-0.1.1/src/torch_mist/data/multimixture.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:21:09.749889 torch_mist-0.1.1/src/torch_mist/distributions/__init__.py
+-rw-r--r--   0        0        0     3670 2023-07-03 13:25:21.611585 torch_mist-0.1.1/src/torch_mist/distributions/joint.py
+-rw-r--r--   0        0        0      219 2023-06-15 14:06:39.255551 torch_mist-0.1.1/src/torch_mist/distributions/parametrizations/__init__.py
+-rw-r--r--   0        0        0     3874 2023-06-26 14:59:12.573939 torch_mist-0.1.1/src/torch_mist/distributions/parametrizations/map.py
+-rw-r--r--   0        0        0     1342 2023-06-26 14:58:04.105670 torch_mist-0.1.1/src/torch_mist/distributions/product.py
+-rw-r--r--   0        0        0      314 2023-06-21 15:01:15.039823 torch_mist-0.1.1/src/torch_mist/distributions/transforms/__init__.py
+-rw-r--r--   0        0        0     3915 2023-06-29 13:24:05.088354 torch_mist-0.1.1/src/torch_mist/distributions/transforms/base.py
+-rw-r--r--   0        0        0     5651 2023-06-20 13:57:58.756420 torch_mist-0.1.1/src/torch_mist/distributions/transforms/linear.py
+-rw-r--r--   0        0        0     2054 2023-06-12 08:43:58.195274 torch_mist-0.1.1/src/torch_mist/distributions/transforms/permute.py
+-rw-r--r--   0        0        0     1581 2023-06-12 08:43:58.195274 torch_mist-0.1.1/src/torch_mist/distributions/transforms/split.py
+-rw-r--r--   0        0        0     6295 2023-07-03 15:01:29.619928 torch_mist-0.1.1/src/torch_mist/distributions/utils.py
+-rw-r--r--   0        0        0      156 2023-06-30 11:45:57.146840 torch_mist-0.1.1/src/torch_mist/estimators/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-03 13:33:39.329253 torch_mist-0.1.1/src/torch_mist/estimators/base.py
+-rw-r--r--   0        0        0      249 2023-06-27 09:36:52.566843 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/__init__.py
+-rw-r--r--   0        0        0     1731 2023-07-03 09:57:24.636452 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/alpha_tuba.py
+-rw-r--r--   0        0        0     5896 2023-07-03 13:34:00.917327 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/base.py
+-rw-r--r--   0        0        0     1767 2023-07-03 09:58:09.012542 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/flo.py
+-rw-r--r--   0        0        0     1417 2023-07-03 09:57:01.348407 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/infonce.py
+-rw-r--r--   0        0        0     1315 2023-07-03 13:08:07.680695 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/js.py
+-rw-r--r--   0        0        0     1129 2023-07-03 15:03:43.628481 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/mine.py
+-rw-r--r--   0        0        0     1341 2023-07-03 09:59:07.316664 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/nwj.py
+-rw-r--r--   0        0        0     1620 2023-07-03 09:59:27.344708 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/smile.py
+-rw-r--r--   0        0        0     3171 2023-07-03 13:37:23.682021 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/tuba.py
+-rw-r--r--   0        0        0      278 2023-06-30 08:58:23.817826 torch_mist-0.1.1/src/torch_mist/estimators/generative/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-03 13:08:42.736762 torch_mist-0.1.1/src/torch_mist/estimators/generative/ba.py
+-rw-r--r--   0        0        0     2331 2023-07-03 13:38:48.850314 torch_mist-0.1.1/src/torch_mist/estimators/generative/base.py
+-rw-r--r--   0        0        0     2351 2023-06-30 07:57:23.457408 torch_mist-0.1.1/src/torch_mist/estimators/generative/club.py
+-rw-r--r--   0        0        0     4151 2023-07-03 13:09:46.680895 torch_mist-0.1.1/src/torch_mist/estimators/generative/discrete.py
+-rw-r--r--   0        0        0     2326 2023-07-03 13:40:37.562720 torch_mist-0.1.1/src/torch_mist/estimators/generative/doe.py
+-rw-r--r--   0        0        0     3292 2023-07-03 13:10:47.665031 torch_mist-0.1.1/src/torch_mist/estimators/generative/gm.py
+-rw-r--r--   0        0        0     2579 2023-07-03 13:10:47.677031 torch_mist-0.1.1/src/torch_mist/estimators/generative/l1out.py
+-rw-r--r--   0        0        0     2915 2023-07-03 13:10:47.657031 torch_mist-0.1.1/src/torch_mist/estimators/generative/pq.py
+-rw-r--r--   0        0        0     2398 2023-07-03 13:17:29.754105 torch_mist-0.1.1/src/torch_mist/estimators/hybrid.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:31:37.640402 torch_mist-0.1.1/src/torch_mist/nn/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-20 16:19:50.201850 torch_mist-0.1.1/src/torch_mist/nn/utils.py
+-rw-r--r--   0        0        0      233 2023-06-26 12:40:43.800056 torch_mist-0.1.1/src/torch_mist/quantization/__init__.py
+-rw-r--r--   0        0        0     4882 2023-06-28 14:40:38.679965 torch_mist-0.1.1/src/torch_mist/quantization/functions.py
+-rw-r--r--   0        0        0     5282 2023-07-03 10:01:48.889030 torch_mist-0.1.1/src/torch_mist/quantization/vqvae.py
+-rw-r--r--   0        0        0       57 2023-07-03 09:53:52.180083 torch_mist-0.1.1/src/torch_mist/utils/__init__.py
+-rw-r--r--   0        0        0     2410 2023-07-03 13:45:24.711861 torch_mist-0.1.1/src/torch_mist/utils/caching.py
+-rw-r--r--   0        0        0     1450 2023-06-27 09:02:37.531485 torch_mist-0.1.1/src/torch_mist/utils/data.py
+-rw-r--r--   0        0        0     2088 2023-07-04 11:41:02.705745 torch_mist-0.1.1/src/torch_mist/utils/estimate.py
+-rw-r--r--   0        0        0     9813 1970-01-01 00:00:00.000000 torch_mist-0.1.1/PKG-INFO
```

### Comparing `torch_mist-0.1.0/LICENSE` & `torch_mist-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.0/pyproject.toml` & `torch_mist-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "torch_mist"
-version = "0.1.0"
+version = "0.1.1"
 description = "Mutual Information Estimation toolkit based on pytorch"
 authors = ["Marco Federici"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pyro-ppl = "^1.8.5"
-numpy = "^1.25.0"
+numpy = "^1.24.0"
+torch = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 myst-nb = {version = "^0.17.2", python = "^3.9"}
 sphinx-autoapi = "^2.1.1"
```

### Comparing `torch_mist-0.1.0/src/torch_mist/baselines.py` & `torch_mist-0.1.1/src/torch_mist/baselines.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from abc import abstractmethod
-from typing import Optional, List, Any
+from typing import Optional, List, Any, Callable, Union
 
+import numpy as np
 import torch
-from pyro.nn import DenseNN
 from torch import nn
 
 
 class Baseline(nn.Module):
     @abstractmethod
     def forward(self, f_: torch.Tensor, x: torch.Tensor, y: Optional[torch.Tensor] = None) -> torch.Tensor:
         raise NotImplementedError()
@@ -40,72 +40,65 @@
             if self.training:
                 ema = self.gamma * self.ema + (1 - self.gamma) * average
                 self.ema = ema
             else:
                 ema = self.ema
 
         ma = ema.log()
-
-        return ma.unsqueeze(0).repeat(f_.shape[0])
+        for _ in range(x.ndim - 1):
+            ma = ma.unsqueeze(0)
+        ma = ma.expand_as(x[..., 0])
+        return ma
 
 
 class BatchLogMeanExp(Baseline):
-    def __init__(self, dim=1):
+    def __init__(self, dims: str):
+        assert dims in ['first', 'all']
         super(BatchLogMeanExp, self).__init__()
-        self.dim = dim
+        self.dims = dims
 
     def forward(self, f_: torch.Tensor, x: torch.Tensor, y: Optional[torch.Tensor] = None) -> torch.Tensor:
-        N, M = f_.shape[0], f_.shape[1]
+        # log 1/M \sum e^f_ = logsumexp(f_) - log M
+        if self.dims == 'all':
+            f_ = f_.view(-1)
+
+        M = f_.shape[0]
+        b = torch.logsumexp(f_, 0) - math.log(M)
 
-        # log 1/M \sum_{j=1}^M f_[i,j] = logsumexp(f_, 1) - log M
-        b = torch.logsumexp(f_, 1).unsqueeze(1) - math.log(M)
+        if self.dims == 'all':
+            for _ in range(x.ndim - 1):
+                b = b.unsqueeze(0)
+            b = b.expand_as(x[..., 0])
 
-        if self.dim == 2:
-            b = torch.logsumexp(b, 0).unsqueeze(0) - math.log(N)
         return b
 
 
 class LearnableBaseline(Baseline):
     def __init__(self, net: nn.Module):
         super(LearnableBaseline, self).__init__()
         self.net = net
 
     def forward(self, f_: torch.Tensor, x: torch.Tensor, y: Optional[torch.Tensor] = None) -> torch.Tensor:
-        return self.net(x)
-
-
-class LearnableMLPBaseline(LearnableBaseline):
-    def __init__(self, x_dim: int, hidden_dims: List[int], nonlinearity: Any = nn.ReLU(True)):
-        net = DenseNN(
-            input_dim=x_dim,
-            hidden_dims=hidden_dims,
-            param_dims=[1],
-            nonlinearity=nonlinearity
-        )
-
-        super(LearnableMLPBaseline, self).__init__(net)
+        return self.net(x).squeeze(-1)
 
 
 class LearnableJointBaseline(LearnableBaseline):
     def forward(self, f_: torch.Tensor, x: torch.Tensor, y: Optional[torch.Tensor] = None) -> torch.Tensor:
-        x = x.unsqueeze(1)+y*0
+        n_dims = x.ndim
+        # Find the maximum shape
+        max_shape = [max(x.shape[i], y.shape[i]) for i in range(n_dims - 1)]
+        # Expand x and y to the maximum shape
+        x = x.expand(max_shape + [-1])
+        y = y.expand(max_shape + [-1])
+
+        assert x.shape[:-1] == y.shape[:-1]
         xy = torch.cat([x, y], -1)
         return self.net(xy).squeeze(-1)
 
 
-class LearnableJointMLPBaseline(LearnableJointBaseline):
-    def __init__(self, x_dim: int, y_dim: int, hidden_dims: List[int], nonlinearity: Any = nn.ReLU(True)):
-        net = DenseNN(
-            input_dim=x_dim+y_dim,
-            hidden_dims=hidden_dims,
-            param_dims=[1],
-            nonlinearity=nonlinearity
-        )
-        super(LearnableJointMLPBaseline, self).__init__(net)
-
 
 class InterpolatedBaseline(Baseline):
     def __init__(self, baseline_1: Baseline, baseline_2: Baseline, alpha: float):
         super(InterpolatedBaseline, self).__init__()
         assert 0 <= alpha <= 1
         self.alpha = alpha
         self.baseline_1 = baseline_1
@@ -133,10 +126,43 @@
 
             return b
 
 
 class AlphaTUBABaseline(InterpolatedBaseline):
     def __init__(self, x_dim: int, hidden_dims: List[int], alpha: float):
         baseline_1 = BatchLogMeanExp(dim=1)
-        baseline_2 = LearnableMLPBaseline(x_dim, hidden_dims)
+        baseline_2 = baseline_nn(x_dim, hidden_dims)
         super(AlphaTUBABaseline, self).__init__(baseline_1=baseline_1, baseline_2=baseline_2, alpha=alpha)
 
+
+def baseline_nn(
+        x_dim: int,
+        hidden_dims: List[int],
+        nonlinearity: Callable = nn.ReLU(True)
+) -> LearnableBaseline:
+    from pyro.nn import DenseNN
+
+    net = DenseNN(
+        input_dim=x_dim,
+        hidden_dims=hidden_dims,
+        param_dims=[1],
+        nonlinearity=nonlinearity
+    )
+
+    return LearnableBaseline(net)
+
+
+def joint_baseline_nn(
+        x_dim: int,
+        y_dim: int,
+        hidden_dims: List[int],
+        nonlinearity: Any = nn.ReLU(True)
+) -> LearnableJointBaseline:
+    from pyro.nn import DenseNN
+
+    net = DenseNN(
+            input_dim=x_dim+y_dim,
+            hidden_dims=hidden_dims,
+            param_dims=[1],
+            nonlinearity=nonlinearity
+        )
+    return LearnableJointBaseline(net)
```

### Comparing `torch_mist-0.1.0/src/torch_mist/critic/base.py` & `torch_mist-0.1.1/src/torch_mist/critic/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,7 @@
         '''
         Compute the value of the critic evaluated at the pair (x, y)
         :param x: a tensor representing x
         :param y: a tensor representing y
         :return: The value of the ratio estimator on the given pair
         '''
         raise NotImplemented()
-
-
-
```

### Comparing `torch_mist-0.1.0/src/torch_mist/critic/separable.py` & `torch_mist-0.1.1/src/torch_mist/critic/separable.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,17 @@
             x: torch.Tensor,
             y: torch.Tensor,
     ) -> torch.Tensor:
         f_x = self.f_x(x)
         f_y = self.f_y(y)
 
         if f_x.ndim < f_y.ndim:
-            f_x = f_x.unsqueeze(1)
+            f_x = f_x.unsqueeze(0)
+
+        assert f_x.ndim == f_y.ndim, f'f_x.ndim={f_x.ndim}, f_y.ndim={f_y.ndim}'
 
         # hack to expand to the same shape without specifying the number of repeats
         f_x = f_x + f_y * 0
         f_y = f_y + f_x * 0
 
-        K = torch.einsum('acb, acb -> ac', f_x, f_y)
+        K = torch.einsum('...b, ...b -> ...', f_x, f_y)
         return K / self.temperature
```

### Comparing `torch_mist-0.1.0/src/torch_mist/critic/utils.py` & `torch_mist-0.1.1/src/torch_mist/critic/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from typing import List
+from typing import List, Optional, Dict, Any, Callable
 
 from pyro.nn import DenseNN
 from torch import nn
 
-from torch_mist.critic import JointCritic, SeparableCritic
+from torch_mist.critic.separable import SeparableCritic
+from torch_mist.critic.joint import JointCritic
 
 
 def separable_critic(
         x_dim: int,
         y_dim: int,
         hidden_dims: List[int],
         projection_head: str = 'symmetric',
         output_dim: int = 128,
         nonlinearity=nn.ReLU(True),
-        temperature: float=0.1
+        temperature: float = 0.1
 ):
     assert projection_head in ['symmetric', 'asymmetric', 'one'], \
         F"projection_heads must be one of ['symmetric', 'asymmetric', 'one'], got {projection_head}"
 
     if projection_head == 'one':
         output_dim = y_dim
 
     f_y = None
 
     assert len(hidden_dims) > 0
     f_x = DenseNN(
         input_dim=x_dim,
-        hidden_dims=[int(h ** 0.5) for h in hidden_dims],
+        hidden_dims=hidden_dims,
         param_dims=[output_dim],
         nonlinearity=nonlinearity,
     )
 
     if projection_head == 'symmetric':
         f_y = f_x
     elif projection_head == 'asymmetric':
@@ -65,25 +66,34 @@
     unnormalized_log_ratio = JointCritic(
         joint_net=joint_net,
     )
 
     return unnormalized_log_ratio
 
 
-def critic(x_dim, y_dim, hidden_dims, critic_type, **kwargs):
+def critic(
+        x_dim: int,
+        y_dim: int,
+        hidden_dims: List[int],
+        critic_type: str,
+        critic_params: Optional[Dict[str, Any]] = None,
+):
     assert critic_type in ['joint', 'separable'], \
         f'critic must be one of [joint, separable, separable_asymm], got {critic_type}'
 
+    if critic_params is None:
+        critic_params = {}
+
     if critic_type == 'joint':
         return joint_critic(
             x_dim=x_dim,
             y_dim=y_dim,
             hidden_dims=hidden_dims,
-            **kwargs
+            **critic_params
         )
     else:
         return separable_critic(
             x_dim=x_dim,
             y_dim=y_dim,
             hidden_dims=hidden_dims,
-            **kwargs
+            **critic_params
         )
```

### Comparing `torch_mist-0.1.0/src/torch_mist/distributions/parametrizations/map.py` & `torch_mist-0.1.1/src/torch_mist/distributions/parametrizations/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,14 @@
         # Check the mapping is compatible with the specified distributions
         for distribution_class in self.supported_distributions:
             for parameter_name in mapped_parameters:
                 assert parameter_name in inspect.signature(distribution_class).parameters
 
         return mapped_parameters
 
-    def extra_repr(self):
-        return ""
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.extra_repr()})"
-
 
 class DeltaMap(ParameterMap):
     """
     Delta Parameter mapping: maps a list of one tensor into a delta distribution at the same location
     """
 
     supported_distributions: List[Type[Distribution]] = [Delta]
@@ -113,20 +107,7 @@
         OneHotCategorical,
     ]
     n_parameters: int = 1
 
     def map_parameters(self, parameter_list: List[torch.Tensor]) -> Dict[str, torch.Tensor]:
         logits = parameter_list[0]
         return {"logits": logits}
-
-
-class TemperatureLogitsMap(ParameterMap):
-    supported_distributions: List[Type[Distribution]] = [
-        Categorical,
-        OneHotCategorical,
-    ]
-    n_parameters: int = 2
-
-    def map_parameters(self, parameter_list: List[torch.Tensor]) -> Dict[str, torch.Tensor]:
-        temperature = parameter_list[0]
-        logits = parameter_list[1]
-        return {"temperature": temperature, "logits": logits}
```

### Comparing `torch_mist-0.1.0/src/torch_mist/distributions/product.py` & `torch_mist-0.1.1/src/torch_mist/distributions/product.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from torch.distributions import Distribution
-
-
-class ShuffledBatchDistribution(Distribution):
-    def __init__(self, y: torch.Tensor):
-        super().__init__(validate_args=False)
-        assert y.shape[1] == 1, f"The input tensor must have shape [N, 1, ...]. {y.shape} was given."
-        self.y = y
-
-    def rsample(self, sample_shape=torch.Size()):
-        assert sample_shape.ndim == 1, "Only 1D sample shapes are supported."
-        n_samples = sample_shape[0]
-
-        # if the sample shape is zero we use the whole batch as negatives
-        if n_samples == 0:
-            # simply unsqueeze an empty dimension at the beginning (we don't repeat to save memory)
-            return self.y[:, 0].unsqueeze(0)
-        elif n_samples < 0:
-            n_samples = self.y.shape[0] + n_samples
-
-        assert n_samples > 0, "Invalid sample shape."
-
-        N = self.y.shape[0]
-        # This indexing operation takes care of selecting the appropriate (off-diagonal) y
-        idx = torch.arange(N * n_samples).to(self.y.device).view(N, n_samples).long()
-        idx = (idx % n_samples + torch.div(idx, n_samples, rounding_mode='floor') + 1) % N
-        return self.y[:, 0][idx]
-
-    def sample(self, sample_shape=torch.Size()):
-        return self.rsample(sample_shape).detach()
-
-
+# from torch.distributions import Distribution
+#
+#
+# class ShuffledBatchDistribution(Distribution):
+#     def __init__(self, y: torch.Tensor):
+#         super().__init__(validate_args=False)
+#         assert y.shape[1] == 1, f"The input tensor must have shape [N, 1, ...]. {y.shape} was given."
+#         self.y = y
+#
+#     def rsample(self, sample_shape=torch.Size()):
+#         assert sample_shape.ndim == 1, "Only 1D sample shapes are supported."
+#         n_samples = sample_shape[0]
+#
+#         # if the sample shape is zero we use the whole batch as negatives
+#         if n_samples == 0:
+#             # simply unsqueeze an empty dimension at the beginning (we don't repeat to save memory)
+#             return self.y[:, 0].unsqueeze(0)
+#         elif n_samples < 0:
+#             n_samples = self.y.shape[0] + n_samples
+#
+#         assert n_samples > 0, "Invalid sample shape."
+#
+#         N = self.y.shape[0]
+#         # This indexing operation takes care of selecting the appropriate (off-diagonal) y
+#         idx = torch.arange(N * n_samples).to(self.y.device).view(N, n_samples).long()
+#         idx = (idx % n_samples + torch.div(idx, n_samples, rounding_mode='floor') + 1) % N
+#         return self.y[:, 0][idx]
+#
+#     def sample(self, sample_shape=torch.Size()):
+#         return self.rsample(sample_shape).detach()
+#
+#
```

### Comparing `torch_mist-0.1.0/src/torch_mist/distributions/transforms/base.py` & `torch_mist-0.1.1/src/torch_mist/distributions/transforms/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,9 +111,9 @@
             validate_args=False
         ).log_prob(value)
 
     def __repr__(self):
         s = self.__class__.__name__+'('
         s += '\n  (base_dist): '+str(self.base_dist).replace('\n', '\n  ')
         s += '\n  (transforms): '+str(self.transforms).replace('\n', '\n  ')
-        s += '\n'
+        s += '\n)'
         return s
```

### Comparing `torch_mist-0.1.0/src/torch_mist/distributions/transforms/linear.py` & `torch_mist-0.1.1/src/torch_mist/distributions/transforms/linear.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.0/src/torch_mist/distributions/transforms/permute.py` & `torch_mist-0.1.1/src/torch_mist/distributions/transforms/permute.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.0/src/torch_mist/distributions/transforms/split.py` & `torch_mist-0.1.1/src/torch_mist/distributions/transforms/split.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.0/src/torch_mist/estimators/generative/ba.py` & `torch_mist-0.1.1/src/torch_mist/estimators/generative/ba.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,60 @@
 from typing import Optional, List, Union
 
 import torch
 
-from torch.distributions import Distribution
 from pyro.distributions import ConditionalDistribution
 
-from torch_mist.estimators.generative.base import VariationalProposalMutualInformationEstimator
+from torch_mist.estimators.generative.base import GenerativeMutualInformationEstimator
+from torch_mist.utils.caching import reset_cache_after_call
 
 
-class BA(VariationalProposalMutualInformationEstimator):
+class BA(GenerativeMutualInformationEstimator):
     def __init__(
             self,
-            conditional_y_x: ConditionalDistribution,
-            marginal_y: Optional[Distribution] = None,
+            q_Y_given_X: ConditionalDistribution,
             entropy_y: Optional[torch.Tensor] = None,
     ):
-        super().__init__(conditional_y_x)
-        self.conditional_y_x = conditional_y_x
-        assert (marginal_y is None) ^ (
-                entropy_y is None), 'Either the marginal distribution or the marginal entropy must be provided'
-
-        self.marginal_y = marginal_y
-        self.entropy_y = entropy_y
-
-    def log_prob_y(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        if self.entropy_y is not None:
-            return -torch.FloatTensor(self.entropy_y).unsqueeze(0).unsqueeze(1).to(y.device)
-        else:
-            log_q_y = self.marginal_y.log_prob(y)
-            assert log_q_y.shape == y.shape[:-1]
-            return log_q_y
-
-    def compute_loss(
-            self,
-            x: torch.Tensor,
-            y: torch.Tensor,
-            log_p_y: torch.Tensor,
-            log_p_y_x: torch.Tensor,
-    ) -> Optional[torch.Tensor]:
-        # Optimize using maximum likelihood
-        return -(log_p_y + log_p_y_x).mean()
-
+        super().__init__(q_Y_given_X=q_Y_given_X)
+        if not isinstance(entropy_y, torch.Tensor):
+            entropy_y = torch.tensor(entropy_y)
+        entropy_y = entropy_y.squeeze()
+        assert entropy_y.ndim == 0
+        self.register_buffer('entropy_y', entropy_y)
+
+    @reset_cache_after_call
+    def expected_log_ratio(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        entropy_y_given_x = -self.approx_log_p_y_given_x(x=x, y=y).mean()
+        return self.entropy_y-entropy_y_given_x
 
 def ba(
         x_dim: int,
         y_dim: int,
         hidden_dims: List[int],
         entropy_y: Union[float, torch.Tensor],
         transform_name: str = 'conditional_linear',
         n_transforms: int = 1,
 ) -> BA:
     from torch_mist.distributions.utils import conditional_transformed_normal
 
-    q_y_x = conditional_transformed_normal(
+    q_Y_given_X = conditional_transformed_normal(
         input_dim=y_dim,
         context_dim=x_dim,
         hidden_dims=hidden_dims,
         transform_name=transform_name,
         n_transforms=n_transforms,
     )
 
     if isinstance(entropy_y, float):
         entropy_y = torch.FloatTensor([entropy_y])
 
     entropy_y = entropy_y.squeeze()
 
     return BA(
-        conditional_y_x=q_y_x,
+        q_Y_given_X=q_Y_given_X,
         entropy_y=entropy_y,
     )
```

### Comparing `torch_mist-0.1.0/src/torch_mist/estimators/generative/base.py` & `torch_mist-0.1.1/src/torch_mist/estimators/generative/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,72 @@
-from typing import Optional
+from abc import abstractmethod, ABC
+from typing import Optional, List
 
 import torch
 from pyro.distributions import ConditionalDistribution
+from torch.distributions import Distribution
 
-from torch_mist.estimators.base import MutualInformationEstimator, Estimation
+from torch_mist.estimators.base import MutualInformationEstimator
+from torch_mist.utils.caching import cached, reset_cache_after_call, reset_cache_before_call
 
 
 class GenerativeMutualInformationEstimator(MutualInformationEstimator):
-    def log_prob_y(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        raise NotImplemented()
+    def __init__(
+            self,
+            q_Y_given_X: ConditionalDistribution
+    ):
+        super().__init__()
+        self.q_Y_given_X = q_Y_given_X
+
+    @cached
+    def q_Y_given_x(self, x: torch.Tensor) -> Distribution:
+        # q(Y|X=x)
+        q_Y_given_x = self.q_Y_given_X.condition(x)
+
+        return q_Y_given_x
+
+    @cached
+    def approx_log_p_y_given_x(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        q_Y_given_x = self.q_Y_given_x(x=x)
 
-    def log_prob_y_x(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        raise NotImplemented()
+        # Compute log q(Y=y|X=x)]
+        log_q_y_given_x = q_Y_given_x.log_prob(y)
 
-    def compute_loss(
+        assert log_q_y_given_x.ndim == y.ndim - 1, f'log_p_Y_X.shape={log_q_y_given_x.shape}, y.shape={y.shape}'
+        return log_q_y_given_x
+
+    @reset_cache_before_call
+    def loss(
             self,
             x: torch.Tensor,
             y: torch.Tensor,
-            log_p_y: torch.Tensor,
-            log_p_y_x: torch.Tensor,
-    ) -> Optional[torch.Tensor]:
-        raise NotImplemented()
+    ) -> torch.Tensor:
+        log_q_y_x = self.approx_log_p_y_given_x(x=x, y=y)
+        return -log_q_y_x.mean()
+
+    @abstractmethod
+    def approx_log_p_y(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        raise NotImplementedError()
 
     def log_ratio(
             self,
             x: torch.Tensor,
             y: torch.Tensor,
-    ) -> Estimation:
-        # Compute the ratio using the primal bound
-        estimates = {}
-        if x.ndim < y.ndim:
-            x = x.unsqueeze(1)
-        assert x.ndim == y.ndim
-
-        log_p_y_x = self.log_prob_y_x(x, y)  # [N, M]
-        log_p_y = self.log_prob_y(x, y)  # [N, M]
-
-        assert log_p_y_x.ndim == log_p_y.ndim == 2, f'log_p_y_x.ndim={log_p_y_x.ndim}, log_p_y.ndim={log_p_y.ndim}'
-
-        value = log_p_y_x - log_p_y
-        loss = self.compute_loss(x=x, y=y, log_p_y_x=log_p_y_x, log_p_y=log_p_y)
-
-        return Estimation(value=value, loss=loss)
+    ) -> torch.Tensor:
+        assert x.ndim == y.ndim, f'x.ndim={x.ndim}, y.ndim={y.ndim}'
 
+        # Compute the ratio using the primal KL bound
+        approx_log_p_y_given_x = self.approx_log_p_y_given_x(x=x, y=y)
+        approx_log_p_y = self.approx_log_p_y(x=x, y=y)
+
+        assert approx_log_p_y_given_x.ndim == approx_log_p_y.ndim == x.ndim - 1, \
+            f'log_p_y_x.ndim={approx_log_p_y_given_x.ndim}, log_p_y.ndim={approx_log_p_y.ndim}'
+        log_ratio = approx_log_p_y_given_x - approx_log_p_y
 
-class VariationalProposalMutualInformationEstimator(GenerativeMutualInformationEstimator):
-    def __init__(self, conditional_y_x: ConditionalDistribution):
-        super().__init__()
-        self.conditional_y_x = conditional_y_x
-
-        self._cached_p_y_X = None
-        self._cached_x = None
-        self._cached_y = None
-
-    def log_prob_y_x(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        # Compute E[log r(y|x)]
-        p_y_X = self.conditional_y_x.condition(x)
-        log_p_Y_X = p_y_X.log_prob(y)
-
-        assert log_p_Y_X.shape == y.shape[:-1]
-
-        # Cache the conditional p(y|X=x) and the inputs x, y
-        self._cached_p_y_X = p_y_X
-        self._cached_x = x
-        self._cached_y = y
-
-        return log_p_Y_X
-
-    def compute_loss(
-            self,
-            x: torch.Tensor,
-            y: torch.Tensor,
-            log_p_y: torch.Tensor,
-            log_p_y_x: torch.Tensor,
-    ) -> Optional[torch.Tensor]:
-        return -log_p_y_x.mean()
+        return log_ratio
 
     def __repr__(self):
         s = self.__class__.__name__ + '(\n'
-        s += '  ' + '(conditional_y_x): ' + str(self.conditional_y_x).replace('\n', '  \n') + '\n'
+        s += '  ' + '(q_Y_given_X): ' + str(self.q_Y_given_X).replace('\n', '  \n') + '\n'
         s += ')' + '\n'
 
         return s
```

### Comparing `torch_mist-0.1.0/src/torch_mist/nn/utils.py` & `torch_mist-0.1.1/src/torch_mist/nn/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.0/src/torch_mist/utils/data.py` & `torch_mist-0.1.1/src/torch_mist/utils/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,22 +20,28 @@
         self._n_samples = max_samples
 
     def __next__(self) -> Tuple[torch.Tensor, torch.Tensor]:
         if self._n_samples <= 0:
             self._n_samples = self.max_samples
             raise StopIteration
         else:
-            self._n_samples -= self.batch_size
-            x, y = torch.chunk(
-                self.joint_dist.sample(torch.Size([self.batch_size])),
-                2,
-                self.split_dim
-            )
-            x = x.squeeze(self.split_dim)
-            y = y.squeeze(self.split_dim)
+            samples = self.joint_dist.sample(torch.Size([self.batch_size]))
+
+            if isinstance(samples, tuple):
+                x, y = samples
+            else:
+                assert samples.shape[self.split_dim] == 2, f"Expected the shape of split_dimension to be 2, got {samples.shape[self.split_dim]}."
+                self._n_samples -= self.batch_size
+                x, y = torch.chunk(
+                    samples,
+                    2,
+                    self.split_dim
+                )
+                x = x.squeeze(self.split_dim)
+                y = y.squeeze(self.split_dim)
 
             return x, y
 
     def __len__(self):
         return self.max_samples // self.batch_size
```

### Comparing `torch_mist-0.1.0/src/torch_mist/utils/estimate.py` & `torch_mist-0.1.1/src/torch_mist/utils/estimate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,82 @@
 from typing import Tuple, Type, Optional, Dict, Any
 
 import torch
 import numpy as np
 import pandas as pd
 from torch.optim import Optimizer
-from torch_mist.estimators import MutualInformationEstimator
-from collections import Iterator
+from collections.abc import Iterator
 from tqdm.auto import tqdm
 from torch.optim import Adam
 
+from torch_mist.estimators.base import MutualInformationEstimator
+
 
 def optimize_mi_estimator(
         estimator: MutualInformationEstimator,
         dataloader: Iterator[Tuple[torch.Tensor, torch.Tensor]],
-        n_epochs: int = 1,
+        device: torch.device = torch.device('cpu'),
+        epochs: int = 1,
         optimizer_class: Type[Optimizer] = Adam,
         optimizer_params: Optional[Dict[str, Any]] = None,
-) -> pd.DataFrame:
+        verbose: bool = False,
+        return_log: bool = True,
+) -> Optional[pd.DataFrame]:
 
     opt_params = {"params": estimator.parameters()}
+
+    if optimizer_params is None:
+        optimizer_params = {"lr": 5e-4}
+
     opt_params.update(optimizer_params)
     
     opt = optimizer_class(
         [opt_params]
     )
 
     log = []
 
-    for epoch in range(n_epochs):
-        for iteration, (x, y) in enumerate(tqdm(dataloader)):
-            estimation = estimator(x, y)
-
-            loss = estimation.loss
-
-            log.append(
-                {
-                    'value': estimation.value.item(),
-                    'loss': estimation.loss.item(),
-                    'iteration': iteration,
-                }
-            )
+    estimator.train()
+    estimator = estimator.to(device)
+
+    dl = tqdm(dataloader) if verbose else dataloader
+    for epoch in range(epochs):
+        for x, y in dl:
+            x = x.to(device)
+            y = y.to(device)
+
+            loss = estimator.loss(x, y)
+
+            if return_log:
+                estimation = estimator(x, y)
+                log.append({
+                    'loss': loss.item(),
+                    'iteration': len(log),
+                    'value': estimation.item(),
+                })
 
             opt.zero_grad()
             loss.backward()
             opt.step()
 
-    return pd.DataFrame(log)
+    if return_log:
+        return pd.DataFrame(log)
 
 
 def estimate_mi(
         estimator: MutualInformationEstimator,
         dataloader: Iterator[Tuple[torch.Tensor, torch.Tensor]],
-) -> float:
-    mis = []
-
-    for x, y in dataloader:
-        estimation = estimator(x, y)
-        mis.append(estimation.value.item())
-
-    return np.mean(mis)
-
-
-def estimate_mi_std(
-        estimator: MutualInformationEstimator,
-        dataloader: Iterator[Tuple[torch.Tensor, torch.Tensor]],
+        device: torch.device = torch.device('cpu'),
 ) -> Tuple[float, float]:
     mis = []
 
+    estimator.eval()
+    estimator = estimator.to(device)
+
     for x, y in dataloader:
+        x = x.to(device)
+        y = y.to(device)
+
         estimation = estimator(x, y)
-        mis.append(estimation.value.item())
+        mis.append(estimation.item())
 
     return np.mean(mis), np.std(mis)
```

