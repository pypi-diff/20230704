# Comparing `tmp/vbpr_pytorch-0.0.5.tar.gz` & `tmp/vbpr_pytorch-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpr_pytorch-0.0.5.tar", max compression
+gzip compressed data, was "vbpr_pytorch-0.0.6a0.tar", max compression
```

## Comparing `vbpr_pytorch-0.0.5.tar` & `vbpr_pytorch-0.0.6a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1097 2023-01-06 20:18:08.961388 vbpr_pytorch-0.0.5/LICENSE
--rwxr-xr-x   0        0        0     4048 2023-02-24 19:56:16.771939 vbpr_pytorch-0.0.5/README.md
--rwxr-xr-x   0        0        0       97 2023-02-24 19:56:16.771939 vbpr_pytorch-0.0.5/examples/README.md
--rwxr-xr-x   0        0        0     3748 2023-02-24 19:56:16.771939 vbpr_pytorch-0.0.5/examples/tradesy.py
--rwxr-xr-x   0        0        0     1504 2023-07-04 13:37:50.884125 vbpr_pytorch-0.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      126 2023-02-24 19:56:16.774598 vbpr_pytorch-0.0.5/vbpr/__init__.py
--rwxr-xr-x   0        0        0      971 2023-01-12 15:43:43.412370 vbpr_pytorch-0.0.5/vbpr/datasets/README.md
--rwxr-xr-x   0        0        0      115 2023-01-12 15:43:43.412370 vbpr_pytorch-0.0.5/vbpr/datasets/__init__.py
--rwxr-xr-x   0        0        0     6112 2023-02-21 20:50:52.972344 vbpr_pytorch-0.0.5/vbpr/datasets/tradesy.py
--rwxr-xr-x   0        0        0     9373 2023-02-24 19:56:16.776343 vbpr_pytorch-0.0.5/vbpr/trainer.py
--rwxr-xr-x   0        0        0     8337 2023-02-21 21:17:53.952676 vbpr_pytorch-0.0.5/vbpr/vbpr.py
--rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 vbpr_pytorch-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2023-01-06 20:18:08.961388 vbpr_pytorch-0.0.6a0/LICENSE
+-rwxr-xr-x   0        0        0     4048 2023-02-24 19:56:16.771939 vbpr_pytorch-0.0.6a0/README.md
+-rwxr-xr-x   0        0        0       97 2023-02-24 19:56:16.771939 vbpr_pytorch-0.0.6a0/examples/README.md
+-rwxr-xr-x   0        0        0     3748 2023-02-24 19:56:16.771939 vbpr_pytorch-0.0.6a0/examples/tradesy.py
+-rwxr-xr-x   0        0        0     1503 2023-07-04 17:37:27.895247 vbpr_pytorch-0.0.6a0/pyproject.toml
+-rwxr-xr-x   0        0        0      126 2023-02-24 19:56:16.774598 vbpr_pytorch-0.0.6a0/vbpr/__init__.py
+-rwxr-xr-x   0        0        0      971 2023-01-12 15:43:43.412370 vbpr_pytorch-0.0.6a0/vbpr/datasets/README.md
+-rwxr-xr-x   0        0        0      115 2023-01-12 15:43:43.412370 vbpr_pytorch-0.0.6a0/vbpr/datasets/__init__.py
+-rwxr-xr-x   0        0        0     6112 2023-02-21 20:50:52.972344 vbpr_pytorch-0.0.6a0/vbpr/datasets/tradesy.py
+-rwxr-xr-x   0        0        0     9373 2023-02-24 19:56:16.776343 vbpr_pytorch-0.0.6a0/vbpr/trainer.py
+-rwxr-xr-x   0        0        0     8337 2023-02-21 21:17:53.952676 vbpr_pytorch-0.0.6a0/vbpr/vbpr.py
+-rw-r--r--   0        0        0     5148 1970-01-01 00:00:00.000000 vbpr_pytorch-0.0.6a0/PKG-INFO
```

### Comparing `vbpr_pytorch-0.0.5/LICENSE` & `vbpr_pytorch-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/README.md` & `vbpr_pytorch-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/examples/tradesy.py` & `vbpr_pytorch-0.0.6a0/examples/tradesy.py`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/pyproject.toml` & `vbpr_pytorch-0.0.6a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbpr-pytorch"
-version = "0.0.5"
+version = "0.0.6a0"
 description = "Implementation of VBPR, a visual recommender model, from the paper 'VBPR: Visual Bayesian Personalized Ranking from Implicit Feedback'"
 authors = [
     "Antonio Ossa-Guerra <aaossa@uc.cl>",
 ]
 license = "MIT"
 
 readme = "README.md"
@@ -30,18 +30,18 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.13"
+python = ">=3.8.1,<3.12"
 
 numpy = "^1.24.2"
-pandas = "^1.5.3"
+pandas = ">=1"
 tqdm = "^4.64.1"
 wandb = { version = "^0.13.10", optional = true}
 torch = {version = "^1.13.1", source = "pytorch"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
```

### Comparing `vbpr_pytorch-0.0.5/vbpr/datasets/README.md` & `vbpr_pytorch-0.0.6a0/vbpr/datasets/README.md`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/vbpr/datasets/tradesy.py` & `vbpr_pytorch-0.0.6a0/vbpr/datasets/tradesy.py`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/vbpr/trainer.py` & `vbpr_pytorch-0.0.6a0/vbpr/trainer.py`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/vbpr/vbpr.py` & `vbpr_pytorch-0.0.6a0/vbpr/vbpr.py`

 * *Files identical despite different names*

### Comparing `vbpr_pytorch-0.0.5/PKG-INFO` & `vbpr_pytorch-0.0.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: vbpr-pytorch
-Version: 0.0.5
+Version: 0.0.6a0
 Summary: Implementation of VBPR, a visual recommender model, from the paper 'VBPR: Visual Bayesian Personalized Ranking from Implicit Feedback'
 Home-page: https://github.com/aaossa/VBPR-PyTorch
 License: MIT
 Keywords: artificial intelligence,recommender systems,vbpr
 Author: Antonio Ossa-Guerra
 Author-email: aaossa@uc.cl
-Requires-Python: >=3.8.1,<3.13
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: wandb
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=1)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: wandb (>=0.13.10,<0.14.0) ; extra == "wandb"
 Project-URL: Repository, https://github.com/aaossa/VBPR-PyTorch
 Description-Content-Type: text/markdown
 
 ![VBPR model architecture](https://raw.githubusercontent.com/aaossa/VBPR-PyTorch/main/vbpr.png?raw=True)
```

