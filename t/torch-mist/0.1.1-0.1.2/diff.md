# Comparing `tmp/torch_mist-0.1.1.tar.gz` & `tmp/torch_mist-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_mist-0.1.1.tar", max compression
+gzip compressed data, was "torch_mist-0.1.2.tar", max compression
```

## Comparing `torch_mist-0.1.1.tar` & `torch_mist-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rwxr-xr-x   0        0        0     1073 2023-06-20 12:29:18.481563 torch_mist-0.1.1/LICENSE
--rw-r--r--   0        0        0     9170 2023-07-04 12:17:42.418951 torch_mist-0.1.1/README.md
--rw-r--r--   0        0        0      640 2023-07-04 12:27:19.053207 torch_mist-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-06-20 13:16:41.292074 torch_mist-0.1.1/src/torch_mist/__init__.py
--rw-r--r--   0        0        0     5184 2023-07-03 07:16:14.892467 torch_mist-0.1.1/src/torch_mist/baselines.py
--rw-r--r--   0        0        0      153 2023-06-21 12:06:46.937453 torch_mist-0.1.1/src/torch_mist/critic/__init__.py
--rw-r--r--   0        0        0      589 2023-06-26 13:14:22.335963 torch_mist-0.1.1/src/torch_mist/critic/base.py
--rw-r--r--   0        0        0     1025 2023-06-30 12:05:05.855795 torch_mist-0.1.1/src/torch_mist/critic/joint.py
--rw-r--r--   0        0        0     1526 2023-06-30 12:05:56.280011 torch_mist-0.1.1/src/torch_mist/critic/separable.py
--rw-r--r--   0        0        0     2460 2023-07-03 10:00:44.180879 torch_mist-0.1.1/src/torch_mist/critic/utils.py
--rw-r--r--   0        0        0        0 2023-06-26 14:28:06.302414 torch_mist-0.1.1/src/torch_mist/data/__init__.py
--rw-r--r--   0        0        0     1750 2023-06-29 13:36:27.280021 torch_mist-0.1.1/src/torch_mist/data/multimixture.py
--rw-r--r--   0        0        0        0 2023-06-21 14:21:09.749889 torch_mist-0.1.1/src/torch_mist/distributions/__init__.py
--rw-r--r--   0        0        0     3670 2023-07-03 13:25:21.611585 torch_mist-0.1.1/src/torch_mist/distributions/joint.py
--rw-r--r--   0        0        0      219 2023-06-15 14:06:39.255551 torch_mist-0.1.1/src/torch_mist/distributions/parametrizations/__init__.py
--rw-r--r--   0        0        0     3874 2023-06-26 14:59:12.573939 torch_mist-0.1.1/src/torch_mist/distributions/parametrizations/map.py
--rw-r--r--   0        0        0     1342 2023-06-26 14:58:04.105670 torch_mist-0.1.1/src/torch_mist/distributions/product.py
--rw-r--r--   0        0        0      314 2023-06-21 15:01:15.039823 torch_mist-0.1.1/src/torch_mist/distributions/transforms/__init__.py
--rw-r--r--   0        0        0     3915 2023-06-29 13:24:05.088354 torch_mist-0.1.1/src/torch_mist/distributions/transforms/base.py
--rw-r--r--   0        0        0     5651 2023-06-20 13:57:58.756420 torch_mist-0.1.1/src/torch_mist/distributions/transforms/linear.py
--rw-r--r--   0        0        0     2054 2023-06-12 08:43:58.195274 torch_mist-0.1.1/src/torch_mist/distributions/transforms/permute.py
--rw-r--r--   0        0        0     1581 2023-06-12 08:43:58.195274 torch_mist-0.1.1/src/torch_mist/distributions/transforms/split.py
--rw-r--r--   0        0        0     6295 2023-07-03 15:01:29.619928 torch_mist-0.1.1/src/torch_mist/distributions/utils.py
--rw-r--r--   0        0        0      156 2023-06-30 11:45:57.146840 torch_mist-0.1.1/src/torch_mist/estimators/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-03 13:33:39.329253 torch_mist-0.1.1/src/torch_mist/estimators/base.py
--rw-r--r--   0        0        0      249 2023-06-27 09:36:52.566843 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/__init__.py
--rw-r--r--   0        0        0     1731 2023-07-03 09:57:24.636452 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/alpha_tuba.py
--rw-r--r--   0        0        0     5896 2023-07-03 13:34:00.917327 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/base.py
--rw-r--r--   0        0        0     1767 2023-07-03 09:58:09.012542 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/flo.py
--rw-r--r--   0        0        0     1417 2023-07-03 09:57:01.348407 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/infonce.py
--rw-r--r--   0        0        0     1315 2023-07-03 13:08:07.680695 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/js.py
--rw-r--r--   0        0        0     1129 2023-07-03 15:03:43.628481 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/mine.py
--rw-r--r--   0        0        0     1341 2023-07-03 09:59:07.316664 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/nwj.py
--rw-r--r--   0        0        0     1620 2023-07-03 09:59:27.344708 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/smile.py
--rw-r--r--   0        0        0     3171 2023-07-03 13:37:23.682021 torch_mist-0.1.1/src/torch_mist/estimators/discriminative/tuba.py
--rw-r--r--   0        0        0      278 2023-06-30 08:58:23.817826 torch_mist-0.1.1/src/torch_mist/estimators/generative/__init__.py
--rw-r--r--   0        0        0     1698 2023-07-03 13:08:42.736762 torch_mist-0.1.1/src/torch_mist/estimators/generative/ba.py
--rw-r--r--   0        0        0     2331 2023-07-03 13:38:48.850314 torch_mist-0.1.1/src/torch_mist/estimators/generative/base.py
--rw-r--r--   0        0        0     2351 2023-06-30 07:57:23.457408 torch_mist-0.1.1/src/torch_mist/estimators/generative/club.py
--rw-r--r--   0        0        0     4151 2023-07-03 13:09:46.680895 torch_mist-0.1.1/src/torch_mist/estimators/generative/discrete.py
--rw-r--r--   0        0        0     2326 2023-07-03 13:40:37.562720 torch_mist-0.1.1/src/torch_mist/estimators/generative/doe.py
--rw-r--r--   0        0        0     3292 2023-07-03 13:10:47.665031 torch_mist-0.1.1/src/torch_mist/estimators/generative/gm.py
--rw-r--r--   0        0        0     2579 2023-07-03 13:10:47.677031 torch_mist-0.1.1/src/torch_mist/estimators/generative/l1out.py
--rw-r--r--   0        0        0     2915 2023-07-03 13:10:47.657031 torch_mist-0.1.1/src/torch_mist/estimators/generative/pq.py
--rw-r--r--   0        0        0     2398 2023-07-03 13:17:29.754105 torch_mist-0.1.1/src/torch_mist/estimators/hybrid.py
--rw-r--r--   0        0        0        0 2023-06-21 14:31:37.640402 torch_mist-0.1.1/src/torch_mist/nn/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-20 16:19:50.201850 torch_mist-0.1.1/src/torch_mist/nn/utils.py
--rw-r--r--   0        0        0      233 2023-06-26 12:40:43.800056 torch_mist-0.1.1/src/torch_mist/quantization/__init__.py
--rw-r--r--   0        0        0     4882 2023-06-28 14:40:38.679965 torch_mist-0.1.1/src/torch_mist/quantization/functions.py
--rw-r--r--   0        0        0     5282 2023-07-03 10:01:48.889030 torch_mist-0.1.1/src/torch_mist/quantization/vqvae.py
--rw-r--r--   0        0        0       57 2023-07-03 09:53:52.180083 torch_mist-0.1.1/src/torch_mist/utils/__init__.py
--rw-r--r--   0        0        0     2410 2023-07-03 13:45:24.711861 torch_mist-0.1.1/src/torch_mist/utils/caching.py
--rw-r--r--   0        0        0     1450 2023-06-27 09:02:37.531485 torch_mist-0.1.1/src/torch_mist/utils/data.py
--rw-r--r--   0        0        0     2088 2023-07-04 11:41:02.705745 torch_mist-0.1.1/src/torch_mist/utils/estimate.py
--rw-r--r--   0        0        0     9813 1970-01-01 00:00:00.000000 torch_mist-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-06-20 12:29:18.481563 torch_mist-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9163 2023-07-04 15:02:00.505522 torch_mist-0.1.2/README.md
+-rw-r--r--   0        0        0      640 2023-07-04 15:02:22.413576 torch_mist-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-20 13:16:41.292074 torch_mist-0.1.2/src/torch_mist/__init__.py
+-rw-r--r--   0        0        0     5184 2023-07-03 07:16:14.892467 torch_mist-0.1.2/src/torch_mist/baselines.py
+-rw-r--r--   0        0        0      153 2023-06-21 12:06:46.937453 torch_mist-0.1.2/src/torch_mist/critic/__init__.py
+-rw-r--r--   0        0        0      589 2023-06-26 13:14:22.335963 torch_mist-0.1.2/src/torch_mist/critic/base.py
+-rw-r--r--   0        0        0     1025 2023-06-30 12:05:05.855795 torch_mist-0.1.2/src/torch_mist/critic/joint.py
+-rw-r--r--   0        0        0     1526 2023-06-30 12:05:56.280011 torch_mist-0.1.2/src/torch_mist/critic/separable.py
+-rw-r--r--   0        0        0     2460 2023-07-03 10:00:44.180879 torch_mist-0.1.2/src/torch_mist/critic/utils.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:28:06.302414 torch_mist-0.1.2/src/torch_mist/data/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-04 13:51:56.083200 torch_mist-0.1.2/src/torch_mist/data/multimixture.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:21:09.749889 torch_mist-0.1.2/src/torch_mist/distributions/__init__.py
+-rw-r--r--   0        0        0     3670 2023-07-03 13:25:21.611585 torch_mist-0.1.2/src/torch_mist/distributions/joint.py
+-rw-r--r--   0        0        0      219 2023-06-15 14:06:39.255551 torch_mist-0.1.2/src/torch_mist/distributions/parametrizations/__init__.py
+-rw-r--r--   0        0        0     3874 2023-06-26 14:59:12.573939 torch_mist-0.1.2/src/torch_mist/distributions/parametrizations/map.py
+-rw-r--r--   0        0        0     1342 2023-06-26 14:58:04.105670 torch_mist-0.1.2/src/torch_mist/distributions/product.py
+-rw-r--r--   0        0        0      314 2023-06-21 15:01:15.039823 torch_mist-0.1.2/src/torch_mist/distributions/transforms/__init__.py
+-rw-r--r--   0        0        0     3915 2023-06-29 13:24:05.088354 torch_mist-0.1.2/src/torch_mist/distributions/transforms/base.py
+-rw-r--r--   0        0        0     5651 2023-06-20 13:57:58.756420 torch_mist-0.1.2/src/torch_mist/distributions/transforms/linear.py
+-rw-r--r--   0        0        0     2054 2023-06-12 08:43:58.195274 torch_mist-0.1.2/src/torch_mist/distributions/transforms/permute.py
+-rw-r--r--   0        0        0     1581 2023-06-12 08:43:58.195274 torch_mist-0.1.2/src/torch_mist/distributions/transforms/split.py
+-rw-r--r--   0        0        0     6295 2023-07-03 15:01:29.619928 torch_mist-0.1.2/src/torch_mist/distributions/utils.py
+-rw-r--r--   0        0        0      156 2023-06-30 11:45:57.146840 torch_mist-0.1.2/src/torch_mist/estimators/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-03 13:33:39.329253 torch_mist-0.1.2/src/torch_mist/estimators/base.py
+-rw-r--r--   0        0        0      249 2023-06-27 09:36:52.566843 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/__init__.py
+-rw-r--r--   0        0        0     1731 2023-07-03 09:57:24.636452 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/alpha_tuba.py
+-rw-r--r--   0        0        0     5896 2023-07-03 13:34:00.917327 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/base.py
+-rw-r--r--   0        0        0     1767 2023-07-03 09:58:09.012542 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/flo.py
+-rw-r--r--   0        0        0     1417 2023-07-03 09:57:01.348407 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/infonce.py
+-rw-r--r--   0        0        0     1315 2023-07-03 13:08:07.680695 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/js.py
+-rw-r--r--   0        0        0     1129 2023-07-03 15:03:43.628481 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/mine.py
+-rw-r--r--   0        0        0     1341 2023-07-03 09:59:07.316664 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/nwj.py
+-rw-r--r--   0        0        0     1620 2023-07-03 09:59:27.344708 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/smile.py
+-rw-r--r--   0        0        0     3171 2023-07-03 13:37:23.682021 torch_mist-0.1.2/src/torch_mist/estimators/discriminative/tuba.py
+-rw-r--r--   0        0        0      278 2023-06-30 08:58:23.817826 torch_mist-0.1.2/src/torch_mist/estimators/generative/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-03 13:08:42.736762 torch_mist-0.1.2/src/torch_mist/estimators/generative/ba.py
+-rw-r--r--   0        0        0     2331 2023-07-03 13:38:48.850314 torch_mist-0.1.2/src/torch_mist/estimators/generative/base.py
+-rw-r--r--   0        0        0     2351 2023-06-30 07:57:23.457408 torch_mist-0.1.2/src/torch_mist/estimators/generative/club.py
+-rw-r--r--   0        0        0     4151 2023-07-03 13:09:46.680895 torch_mist-0.1.2/src/torch_mist/estimators/generative/discrete.py
+-rw-r--r--   0        0        0     2326 2023-07-03 13:40:37.562720 torch_mist-0.1.2/src/torch_mist/estimators/generative/doe.py
+-rw-r--r--   0        0        0     3292 2023-07-03 13:10:47.665031 torch_mist-0.1.2/src/torch_mist/estimators/generative/gm.py
+-rw-r--r--   0        0        0     2579 2023-07-03 13:10:47.677031 torch_mist-0.1.2/src/torch_mist/estimators/generative/l1out.py
+-rw-r--r--   0        0        0     2915 2023-07-03 13:10:47.657031 torch_mist-0.1.2/src/torch_mist/estimators/generative/pq.py
+-rw-r--r--   0        0        0     2398 2023-07-03 13:17:29.754105 torch_mist-0.1.2/src/torch_mist/estimators/hybrid.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:31:37.640402 torch_mist-0.1.2/src/torch_mist/nn/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-20 16:19:50.201850 torch_mist-0.1.2/src/torch_mist/nn/utils.py
+-rw-r--r--   0        0        0      233 2023-06-26 12:40:43.800056 torch_mist-0.1.2/src/torch_mist/quantization/__init__.py
+-rw-r--r--   0        0        0     4882 2023-06-28 14:40:38.679965 torch_mist-0.1.2/src/torch_mist/quantization/functions.py
+-rw-r--r--   0        0        0     5282 2023-07-03 10:01:48.889030 torch_mist-0.1.2/src/torch_mist/quantization/vqvae.py
+-rw-r--r--   0        0        0       57 2023-07-03 09:53:52.180083 torch_mist-0.1.2/src/torch_mist/utils/__init__.py
+-rw-r--r--   0        0        0     2410 2023-07-03 13:45:24.711861 torch_mist-0.1.2/src/torch_mist/utils/caching.py
+-rw-r--r--   0        0        0     1203 2023-07-04 14:53:55.404224 torch_mist-0.1.2/src/torch_mist/utils/data.py
+-rw-r--r--   0        0        0     2688 2023-07-04 14:53:18.792064 torch_mist-0.1.2/src/torch_mist/utils/estimate.py
+-rw-r--r--   0        0        0     9806 1970-01-01 00:00:00.000000 torch_mist-0.1.2/PKG-INFO
```

### Comparing `torch_mist-0.1.1/LICENSE` & `torch_mist-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/README.md` & `torch_mist-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,25 +66,25 @@
 
 
 ### Estimators
 The basic estimators implemented in this package are summarized in the following table:
 
 | Estimator                                     | Type                  | Models                                    |
 |-----------------------------------------------|-----------------------|-------------------------------------------|
-| NWJ [[1]](#references)                        | Discriminative        | $f_\phi(x,y)$                              |
-| MINE  [[2]](#references)                      | Discriminative        | $f_\phi(x,y)$                              |
-| InfoNCE [[3]](#references)                    | Discriminative        | $f_\phi(x,y)$                              |
-| TUBA  [[4]](#references)                      | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                  | 
-| AlphaTUBA [[4]](#references)                  | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                  |
-| JS [[5]](#references)                         | Discriminative        | $f_\phi(x,y)$                              |
-| SMILE [[6]](#references)                      | Discriminative        | $f_\phi(x,y)$                              |
+| NWJ [[1]](#references)                        | Discriminative        | $f_\phi(x,y)$                             |
+| MINE  [[2]](#references)                      | Discriminative        | $f_\phi(x,y)$                             |
+| InfoNCE [[3]](#references)                    | Discriminative        | $f_\phi(x,y)$                             |
+| TUBA  [[4]](#references)                      | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                 | 
+| AlphaTUBA [[4]](#references)                  | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                 |
+| JS [[5]](#references)                         | Discriminative        | $f_\phi(x,y)$                             |
+| SMILE [[6]](#references)                      | Discriminative        | $f_\phi(x,y)$                             |
 | FLO [[7]](#references)                        | Discriminative        | $f_\phi(x,y)$, $b_\xi(x,y)$               | 
 | BA [[8]](#references)                         | Generative            | $q_\theta(y\|x)$                          |          
 | DoE [[9]](#references)                        | Generative            | $q_\theta(y\|x)$, $q_\psi(y)$             | 
-| GM [[6]](#references)                         | Generative            | $q_\theta(x,y)$, $q_\psi(x)$, $r_\psi(y)$ |
+| GM [[6]](#references)                         | Generative            | $q_\theta(x,y)$, $q_\psi(x)$, $q_\psi(y)$ |
 | L1OUT [[4]](#references) [[10]](#references)  | Generative            | $q_\theta(y\|x)$                          |                  
 | CLUB [[10]](#references)                      | Generative            | $q_\theta(y\|x)$                          |
 | Discrete [[]](#references)                    | Generative (Discrete) | $Q(x)$, $Q(y)$                            |
 | PQ [[11]](#references)                        | Generative (Discrete) | $Q(y)$, $q_\theta(Q(y)\|x)$               |
 
 in which:
 - $f_\phi(x,y)$ is a `critic` neural network with parameters $\phi, which maps pairs of observations to a scalar value.
```

### Comparing `torch_mist-0.1.1/pyproject.toml` & `torch_mist-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch_mist"
-version = "0.1.1"
+version = "0.1.2"
 description = "Mutual Information Estimation toolkit based on pytorch"
 authors = ["Marco Federici"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `torch_mist-0.1.1/src/torch_mist/baselines.py` & `torch_mist-0.1.2/src/torch_mist/baselines.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/critic/base.py` & `torch_mist-0.1.2/src/torch_mist/critic/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/critic/joint.py` & `torch_mist-0.1.2/src/torch_mist/critic/joint.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/critic/separable.py` & `torch_mist-0.1.2/src/torch_mist/critic/separable.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/critic/utils.py` & `torch_mist-0.1.2/src/torch_mist/critic/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/data/multimixture.py` & `torch_mist-0.1.2/src/torch_mist/data/multimixture.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,52 +8,45 @@
             self,
             rho: float = 0.95,
             sigma: float = 0.1,
             epsilon: float = 0.15,
             delta: float = 1.5,
             n_dim: int = 5
     ):
-        covariance = torch.FloatTensor([
-            [1, rho],
-            [rho, 1]
-        ])*sigma
-
-        mu_1 = torch.zeros(n_dim, 1, 2)
-        # offset1 = torch.Tensor([-epsilon, epsilon])
-        # offset2 = torch.Tensor([-delta, delta])
-
-        mu_1[:, :, 0] = epsilon + delta
-        mu_1[:, :, 1] = -epsilon + delta
-
-        mu_2 = torch.zeros(n_dim, 1, 2)
-        mu_2[:, :, 0] = -epsilon - delta
-        mu_2[:, :, 1] = epsilon - delta
-
-        mu_3 = torch.zeros(n_dim, 1, 2)
-        mu_3[:, :, 0] = epsilon - delta
-        mu_3[:, :, 1] = -epsilon - delta
-
-        mu_4 = torch.zeros(n_dim, 1, 2)
-        mu_4[:, :, 0] = -epsilon + delta
-        mu_4[:, :, 1] = epsilon + delta
-
-        loc = torch.cat([mu_1, mu_2, mu_3, mu_4], -2)
+        covariance = torch.eye(n_dim * 2)
+        for dim in range(n_dim):
+            covariance[dim, n_dim + dim] = covariance[n_dim + dim, dim] = rho
+
+        covariance = covariance * sigma
+
+        mu = torch.zeros(4, 2, n_dim)
+
+        mu[0, 0] = epsilon + delta
+        mu[0, 1] = -epsilon + delta
+        mu[1, 0] = -epsilon - delta
+        mu[1, 1] = epsilon - delta
+        mu[2, 0] = epsilon - delta
+        mu[2, 1] = -epsilon - delta
+        mu[3, 0] = -epsilon + delta
+        mu[3, 1] = epsilon + delta
 
         self.x_component_dist = Normal(
-            loc[:, :, 0],
-            covariance[0, 0]**0.5
+            mu[:, 0].T,
+            sigma**0.5
         )
 
         # Store the marginal distribution for one dimension
         self.p_x = Independent(MixtureSameFamily(
-            Categorical(probs=torch.zeros(n_dim, 4) + 0.25),
+            Categorical(
+                logits=torch.zeros(n_dim, 4)
+            ),
             self.x_component_dist
         ), 1)
 
         self.component_dist = MultivariateNormal(
-            loc,
-            covariance.unsqueeze(0).unsqueeze(1)
+            mu.view(4, -1),
+            covariance.unsqueeze(0)
         )
 
         super().__init__(
-            Categorical(probs=torch.zeros(n_dim, 4) + 0.25), self.component_dist
+            Categorical(logits=torch.zeros(4)), self.component_dist
         )
```

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/joint.py` & `torch_mist-0.1.2/src/torch_mist/distributions/joint.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/parametrizations/map.py` & `torch_mist-0.1.2/src/torch_mist/distributions/parametrizations/map.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/product.py` & `torch_mist-0.1.2/src/torch_mist/distributions/product.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/transforms/base.py` & `torch_mist-0.1.2/src/torch_mist/distributions/transforms/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/transforms/linear.py` & `torch_mist-0.1.2/src/torch_mist/distributions/transforms/linear.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/transforms/permute.py` & `torch_mist-0.1.2/src/torch_mist/distributions/transforms/permute.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/transforms/split.py` & `torch_mist-0.1.2/src/torch_mist/distributions/transforms/split.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/distributions/utils.py` & `torch_mist-0.1.2/src/torch_mist/distributions/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/base.py` & `torch_mist-0.1.2/src/torch_mist/estimators/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/alpha_tuba.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/alpha_tuba.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/base.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/flo.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/flo.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/infonce.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/infonce.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/js.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/js.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/mine.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/mine.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/nwj.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/nwj.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/smile.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/smile.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/discriminative/tuba.py` & `torch_mist-0.1.2/src/torch_mist/estimators/discriminative/tuba.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/ba.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/ba.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/base.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/base.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/club.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/club.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/discrete.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/discrete.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/doe.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/doe.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/gm.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/gm.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/l1out.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/l1out.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/generative/pq.py` & `torch_mist-0.1.2/src/torch_mist/estimators/generative/pq.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/estimators/hybrid.py` & `torch_mist-0.1.2/src/torch_mist/estimators/hybrid.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/nn/utils.py` & `torch_mist-0.1.2/src/torch_mist/nn/utils.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/quantization/functions.py` & `torch_mist-0.1.2/src/torch_mist/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/quantization/vqvae.py` & `torch_mist-0.1.2/src/torch_mist/quantization/vqvae.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/src/torch_mist/utils/caching.py` & `torch_mist-0.1.2/src/torch_mist/utils/caching.py`

 * *Files identical despite different names*

### Comparing `torch_mist-0.1.1/PKG-INFO` & `torch_mist-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-mist
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mutual Information Estimation toolkit based on pytorch
 License: MIT
 Author: Marco Federici
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -84,25 +84,25 @@
 
 
 ### Estimators
 The basic estimators implemented in this package are summarized in the following table:
 
 | Estimator                                     | Type                  | Models                                    |
 |-----------------------------------------------|-----------------------|-------------------------------------------|
-| NWJ [[1]](#references)                        | Discriminative        | $f_\phi(x,y)$                              |
-| MINE  [[2]](#references)                      | Discriminative        | $f_\phi(x,y)$                              |
-| InfoNCE [[3]](#references)                    | Discriminative        | $f_\phi(x,y)$                              |
-| TUBA  [[4]](#references)                      | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                  | 
-| AlphaTUBA [[4]](#references)                  | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                  |
-| JS [[5]](#references)                         | Discriminative        | $f_\phi(x,y)$                              |
-| SMILE [[6]](#references)                      | Discriminative        | $f_\phi(x,y)$                              |
+| NWJ [[1]](#references)                        | Discriminative        | $f_\phi(x,y)$                             |
+| MINE  [[2]](#references)                      | Discriminative        | $f_\phi(x,y)$                             |
+| InfoNCE [[3]](#references)                    | Discriminative        | $f_\phi(x,y)$                             |
+| TUBA  [[4]](#references)                      | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                 | 
+| AlphaTUBA [[4]](#references)                  | Discriminative        | $f_\phi(x,y)$, $b_\xi(x)$                 |
+| JS [[5]](#references)                         | Discriminative        | $f_\phi(x,y)$                             |
+| SMILE [[6]](#references)                      | Discriminative        | $f_\phi(x,y)$                             |
 | FLO [[7]](#references)                        | Discriminative        | $f_\phi(x,y)$, $b_\xi(x,y)$               | 
 | BA [[8]](#references)                         | Generative            | $q_\theta(y\|x)$                          |          
 | DoE [[9]](#references)                        | Generative            | $q_\theta(y\|x)$, $q_\psi(y)$             | 
-| GM [[6]](#references)                         | Generative            | $q_\theta(x,y)$, $q_\psi(x)$, $r_\psi(y)$ |
+| GM [[6]](#references)                         | Generative            | $q_\theta(x,y)$, $q_\psi(x)$, $q_\psi(y)$ |
 | L1OUT [[4]](#references) [[10]](#references)  | Generative            | $q_\theta(y\|x)$                          |                  
 | CLUB [[10]](#references)                      | Generative            | $q_\theta(y\|x)$                          |
 | Discrete [[]](#references)                    | Generative (Discrete) | $Q(x)$, $Q(y)$                            |
 | PQ [[11]](#references)                        | Generative (Discrete) | $Q(y)$, $q_\theta(Q(y)\|x)$               |
 
 in which:
 - $f_\phi(x,y)$ is a `critic` neural network with parameters $\phi, which maps pairs of observations to a scalar value.
```

