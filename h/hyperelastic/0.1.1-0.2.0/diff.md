# Comparing `tmp/hyperelastic-0.1.1.tar.gz` & `tmp/hyperelastic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.1.1.tar", last modified: Sun Jul  2 22:30:41 2023, max compression
+gzip compressed data, was "hyperelastic-0.2.0.tar", last modified: Mon Jul  3 23:09:31 2023, max compression
```

## Comparing `hyperelastic-0.1.1.tar` & `hyperelastic-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.555144 hyperelastic-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48635 2023-07-02 22:30:41.555144 hyperelastic-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:30:41.555144 hyperelastic-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.543144 hyperelastic-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.547144 hyperelastic-0.1.1/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.547144 hyperelastic-0.1.1/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48635 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50086 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.811092 hyperelastic-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.811092 hyperelastic-0.2.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50086 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.1.1/LICENSE` & `hyperelastic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/PKG-INFO` & `hyperelastic-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.1.1
+Version: 0.2.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -722,15 +722,15 @@
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install hyperelastic
 ```
 
 # Usage
-Material model formulations have to be created as classes with methods for the evaluation of the `gradient` (stress) and the `hessian` of the strain energy function (elasticity). It depends on the framework which derivatives have to be defined, e.g. the derivatives w.r.t. the invariants of the right Cauchy-Green deformation tensor or w.r.t. the principal stretches. An instance of a **Framework** has to be *finalized* by the application on a **Space**.
+Material model formulations have to be created as classes with methods for the evaluation of the `gradient` (stress) and the `hessian` (elasticity) of the strain energy function. It depends on the framework which derivatives have to be defined, e.g. the derivatives w.r.t. the invariants of the right Cauchy-Green deformation tensor or w.r.t. the principal stretches. An instance of a **Framework** has to be *finalized* by the application on a **Space**.
 
 - [Deformation (Full) Space](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/spaces/_deformation.py)
 - [Distortional Space](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/spaces/_distortional.py)
 - [Dilatational Space](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/spaces/_dilatational.py)
 
 > ⓘ **Note**
 > Define your own material model formulation with manual, automatic or symbolic differentiation with the help of your favourite package, e.g. [PyTorch](https://pytorch.org/), [JAX](https://jax.readthedocs.io/en/latest/), [Tensorflow](https://www.tensorflow.org/), [TensorTRAX](https://github.com/adtzlr/tensortrax), [SymPy](https://www.sympy.org/en/index.html), etc.
@@ -742,63 +742,112 @@
 import hyperelastic.math as hm
 ```
 
 ## Invariant-based material formulations
 A minimal template for an invariant-based material formulation applied on the distortional space:
 
 ```python
-class MyModel1:
-    def gradient(self, I1, I2, statevars):
+class MyInvariantsModel:
+    def gradient(self, I1, I2, I3, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the invariants of the right Cauchy-Green deformation tensor."""
 
-        return dWdI1, dWdI2, statevars
+        # user code
+        dWdI1 = None
+        dWdI2 = None
+        dWdI3 = None
 
-    def hessian(self, I1, I2, statevars_old):
+        return dWdI1, dWdI2, dWdI3, statevars
+
+    def hessian(self, I1, I2, I3, statevars_old):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the invariants of the right Cauchy-Green deformation tensor."""
 
-        return d2WdI1I1, d2WdI2I2, d2WdI1I2
+        # user code
+        d2WdI1I1 = None
+        d2WdI2I2 = None
+        d2WdI3I3 = None
+        d2WdI1I2 = None
+        d2WdI2I3 = None
+        d2WdI1I3 = None
+
+        return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
 
 
-model1 = MyModel1()
-umat1 = hel.spaces.DistortionalSpace(hel.frameworks.InvariantsFramework(model1))
+model = MyInvariantsModel()
+framework = hel.frameworks.InvariantsFramework(model)
+umat = hel.spaces.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
 
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
-class MyModel2:
+class MyStretchesModel:
     def gradient(self, λ, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the principal stretches."""
 
+        # user code
+        dWdλ1, dWdλ2, dWdλ3 = 0 * λ
+
         return [dWdλ1, dWdλ2, dWdλ3], statevars
 
     def hessian(self, λ, statevars_old):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the principal stretches."""
 
+        # user code
+        d2Wdλ1dλ1 = None
+        d2Wdλ2dλ2 = None
+        d2Wdλ3dλ3 = None
+        d2Wdλ1dλ2 = None
+        d2Wdλ2dλ3 = None
+        d2Wdλ1dλ3 = None
+
         return d2Wdλ1dλ1, d2Wdλ2dλ2, d2Wdλ3dλ3, d2Wdλ1dλ2, d2Wdλ2dλ3, d2Wdλ1dλ3
 
 
-model2 = MyModel2()
-umat2 = hel.spaces.DistortionalSpace(hel.frameworks.StretchesFramework(model2))
+model = MyStretchesModel()
+framework = hel.frameworks.StretchesFramework(model)
+umat = hel.spaces.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic stretch-based material formulations
 - [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/stretches/_ogden.py))
 
+## Lab
+By using [matadi](https://github.com/adtzlr/matadi)'s `LabIncompressible`, numeric experiments on homogeneous incompressible loadcases on hyperelastic material formulations are performed. Ensure to have [matadi](https://github.com/adtzlr/matadi) installed - run `pip install matadi` in your terminal.
+
+```python
+mooney_rivlin = hel.models.invariants.ThirdOrderDeformation(C10=0.3, C01=0.2)
+framework = hel.frameworks.InvariantsFramework(mooney_rivlin)
+umat = hel.spaces.DistortionalSpace(framework)
+
+import matadi
+
+lab = matadi.LabIncompressible(umat, title="Mooney Rivlin")
+data = lab.run(
+    ux=True,
+    bx=True,
+    ps=True,
+    stretch_min=0.7,
+    stretch_max=2.5,
+)
+fig, ax = lab.plot(data, stability=True)
+```
+
+![lab_mooney-rivlin](https://github.com/adtzlr/hyperelastic/assets/5793153/1b21df81-e0fd-4ea1-9bd7-24d4d70ba801)
+
 # License
 Hyperelastic - Constitutive hyperelastic material formulations for FElupe (C) 2023 Andreas Dutzler, Graz (Austria).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `hyperelastic-0.1.1/README.md` & `hyperelastic-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -143,17 +143,17 @@
 000008e0: 726d 756c 6174 696f 6e73 2068 6176 6520  rmulations have 
 000008f0: 746f 2062 6520 6372 6561 7465 6420 6173  to be created as
 00000900: 2063 6c61 7373 6573 2077 6974 6820 6d65   classes with me
 00000910: 7468 6f64 7320 666f 7220 7468 6520 6576  thods for the ev
 00000920: 616c 7561 7469 6f6e 206f 6620 7468 6520  aluation of the 
 00000930: 6067 7261 6469 656e 7460 2028 7374 7265  `gradient` (stre
 00000940: 7373 2920 616e 6420 7468 6520 6068 6573  ss) and the `hes
-00000950: 7369 616e 6020 6f66 2074 6865 2073 7472  sian` of the str
-00000960: 6169 6e20 656e 6572 6779 2066 756e 6374  ain energy funct
-00000970: 696f 6e20 2865 6c61 7374 6963 6974 7929  ion (elasticity)
+00000950: 7369 616e 6020 2865 6c61 7374 6963 6974  sian` (elasticit
+00000960: 7929 206f 6620 7468 6520 7374 7261 696e  y) of the strain
+00000970: 2065 6e65 7267 7920 6675 6e63 7469 6f6e   energy function
 00000980: 2e20 4974 2064 6570 656e 6473 206f 6e20  . It depends on 
 00000990: 7468 6520 6672 616d 6577 6f72 6b20 7768  the framework wh
 000009a0: 6963 6820 6465 7269 7661 7469 7665 7320  ich derivatives 
 000009b0: 6861 7665 2074 6f20 6265 2064 6566 696e  have to be defin
 000009c0: 6564 2c20 652e 672e 2074 6865 2064 6572  ed, e.g. the der
 000009d0: 6976 6174 6976 6573 2077 2e72 2e74 2e20  ivatives w.r.t. 
 000009e0: 7468 6520 696e 7661 7269 616e 7473 206f  the invariants o
@@ -227,196 +227,287 @@
 00000e20: 6d69 6e69 6d61 6c20 7465 6d70 6c61 7465  minimal template
 00000e30: 2066 6f72 2061 6e20 696e 7661 7269 616e   for an invarian
 00000e40: 742d 6261 7365 6420 6d61 7465 7269 616c  t-based material
 00000e50: 2066 6f72 6d75 6c61 7469 6f6e 2061 7070   formulation app
 00000e60: 6c69 6564 206f 6e20 7468 6520 6469 7374  lied on the dist
 00000e70: 6f72 7469 6f6e 616c 2073 7061 6365 3a0a  ortional space:.
 00000e80: 0a60 6060 7079 7468 6f6e 0a63 6c61 7373  .```python.class
-00000e90: 204d 794d 6f64 656c 313a 0a20 2020 2064   MyModel1:.    d
-00000ea0: 6566 2067 7261 6469 656e 7428 7365 6c66  ef gradient(self
-00000eb0: 2c20 4931 2c20 4932 2c20 7374 6174 6576  , I1, I2, statev
-00000ec0: 6172 7329 3a0a 2020 2020 2020 2020 2222  ars):.        ""
-00000ed0: 2254 6865 2067 7261 6469 656e 7420 6173  "The gradient as
-00000ee0: 2074 6865 2070 6172 7469 616c 2064 6572   the partial der
-00000ef0: 6976 6174 6976 6520 6f66 2074 6865 2073  ivative of the s
-00000f00: 7472 6169 6e20 656e 6572 6779 2066 756e  train energy fun
-00000f10: 6374 696f 6e20 772e 722e 742e 0a20 2020  ction w.r.t..   
-00000f20: 2020 2020 2074 6865 2069 6e76 6172 6961       the invaria
-00000f30: 6e74 7320 6f66 2074 6865 2072 6967 6874  nts of the right
-00000f40: 2043 6175 6368 792d 4772 6565 6e20 6465   Cauchy-Green de
-00000f50: 666f 726d 6174 696f 6e20 7465 6e73 6f72  formation tensor
-00000f60: 2e22 2222 0a0a 2020 2020 2020 2020 7265  ."""..        re
-00000f70: 7475 726e 2064 5764 4931 2c20 6457 6449  turn dWdI1, dWdI
-00000f80: 322c 2073 7461 7465 7661 7273 0a0a 2020  2, statevars..  
-00000f90: 2020 6465 6620 6865 7373 6961 6e28 7365    def hessian(se
-00000fa0: 6c66 2c20 4931 2c20 4932 2c20 7374 6174  lf, I1, I2, stat
-00000fb0: 6576 6172 735f 6f6c 6429 3a0a 2020 2020  evars_old):.    
-00000fc0: 2020 2020 2222 2254 6865 2068 6573 7369      """The hessi
-00000fd0: 616e 2061 7320 7468 6520 7365 636f 6e64  an as the second
-00000fe0: 2070 6172 7469 616c 2064 6572 6976 6174   partial derivat
-00000ff0: 6976 6573 206f 6620 7468 6520 7374 7261  ives of the stra
-00001000: 696e 2065 6e65 7267 7920 6675 6e63 7469  in energy functi
-00001010: 6f6e 0a20 2020 2020 2020 2077 2e72 2e74  on.        w.r.t
-00001020: 2e20 7468 6520 696e 7661 7269 616e 7473  . the invariants
-00001030: 206f 6620 7468 6520 7269 6768 7420 4361   of the right Ca
-00001040: 7563 6879 2d47 7265 656e 2064 6566 6f72  uchy-Green defor
-00001050: 6d61 7469 6f6e 2074 656e 736f 722e 2222  mation tensor.""
-00001060: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00001070: 6e20 6432 5764 4931 4931 2c20 6432 5764  n d2WdI1I1, d2Wd
-00001080: 4932 4932 2c20 6432 5764 4931 4932 0a0a  I2I2, d2WdI1I2..
-00001090: 0a6d 6f64 656c 3120 3d20 4d79 4d6f 6465  .model1 = MyMode
-000010a0: 6c31 2829 0a75 6d61 7431 203d 2068 656c  l1().umat1 = hel
-000010b0: 2e73 7061 6365 732e 4469 7374 6f72 7469  .spaces.Distorti
-000010c0: 6f6e 616c 5370 6163 6528 6865 6c2e 6672  onalSpace(hel.fr
-000010d0: 616d 6577 6f72 6b73 2e49 6e76 6172 6961  ameworks.Invaria
-000010e0: 6e74 7346 7261 6d65 776f 726b 286d 6f64  ntsFramework(mod
-000010f0: 656c 3129 290a 6060 600a 0a23 2323 2041  el1)).```..### A
-00001100: 7661 696c 6162 6c65 2069 736f 7472 6f70  vailable isotrop
-00001110: 6963 2068 7970 6572 656c 6173 7469 6320  ic hyperelastic 
-00001120: 696e 7661 7269 616e 742d 6261 7365 6420  invariant-based 
-00001130: 6d61 7465 7269 616c 2066 6f72 6d75 6c61  material formula
-00001140: 7469 6f6e 730a 5468 6520 7479 7069 6361  tions.The typica
-00001150: 6c20 706f 6c79 6e6f 6d69 616c 2d62 6173  l polynomial-bas
-00001160: 6564 206d 6174 6572 6961 6c20 666f 726d  ed material form
-00001170: 756c 6174 696f 6e73 2028 5b4e 656f 2d48  ulations ([Neo-H
-00001180: 6f6f 6b65 5d28 6874 7470 733a 2f2f 656e  ooke](https://en
-00001190: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-000011a0: 696b 692f 4e65 6f2d 486f 6f6b 6561 6e5f  iki/Neo-Hookean_
-000011b0: 736f 6c69 6429 2c20 5b4d 6f6f 6e65 792d  solid), [Mooney-
-000011c0: 5269 766c 696e 5d28 6874 7470 733a 2f2f  Rivlin](https://
-000011d0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-000011e0: 2f77 696b 692f 4d6f 6f6e 6579 2545 3225  /wiki/Mooney%E2%
-000011f0: 3830 2539 3352 6976 6c69 6e5f 736f 6c69  80%93Rivlin_soli
-00001200: 6429 2c20 5b59 656f 685d 2868 7474 7073  d), [Yeoh](https
-00001210: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00001220: 6f72 672f 7769 6b69 2f59 656f 685f 6879  org/wiki/Yeoh_hy
-00001230: 7065 7265 6c61 7374 6963 5f6d 6f64 656c  perelastic_model
-00001240: 2920 6172 6520 616c 6c20 6176 6169 6c61  ) are all availa
-00001250: 626c 6520 6173 2073 7562 6d6f 6465 6c73  ble as submodels
-00001260: 206f 6620 7468 6520 7468 6972 6420 6f72   of the third or
-00001270: 6465 7220 6465 666f 726d 6174 696f 6e20  der deformation 
-00001280: 6d61 7465 7269 616c 2066 6f72 6d75 6c61  material formula
-00001290: 7469 6f6e 2e0a 0a2d 205b 5468 6972 642d  tion...- [Third-
-000012a0: 4f72 6465 722d 4465 666f 726d 6174 696f  Order-Deformatio
-000012b0: 6e20 284a 616d 6573 2d47 7265 656e 2d53  n (James-Green-S
-000012c0: 696d 7073 6f6e 295d 2868 7474 7073 3a2f  impson)](https:/
-000012d0: 2f6f 6e6c 696e 656c 6962 7261 7279 2e77  /onlinelibrary.w
-000012e0: 696c 6579 2e63 6f6d 2f64 6f69 2f61 6273  iley.com/doi/abs
-000012f0: 2f31 302e 3130 3032 2f61 7070 2e31 3937  /10.1002/app.197
-00001300: 352e 3037 3031 3930 3732 3329 2028 5b63  5.070190723) ([c
-00001310: 6f64 655d 2868 7474 7073 3a2f 2f67 6974  ode](https://git
-00001320: 6875 622e 636f 6d2f 6164 747a 6c72 2f68  hub.com/adtzlr/h
-00001330: 7970 6572 656c 6173 7469 632f 626c 6f62  yperelastic/blob
-00001340: 2f6d 6169 6e2f 7372 632f 6879 7065 7265  /main/src/hypere
-00001350: 6c61 7374 6963 2f6d 6f64 656c 732f 696e  lastic/models/in
-00001360: 7661 7269 616e 7473 2f5f 7468 6972 645f  variants/_third_
-00001370: 6f72 6465 725f 6465 666f 726d 6174 696f  order_deformatio
-00001380: 6e2e 7079 2929 0a0a 0a23 2320 5072 696e  n.py))...## Prin
-00001390: 6369 7061 6c20 7374 7265 7463 682d 6261  cipal stretch-ba
-000013a0: 7365 6420 6d61 7465 7269 616c 2066 6f72  sed material for
-000013b0: 6d75 6c61 7469 6f6e 730a 4120 6d69 6e69  mulations.A mini
-000013c0: 6d61 6c20 7465 6d70 6c61 7465 2066 6f72  mal template for
-000013d0: 2061 2070 7269 6e63 6970 616c 2073 7472   a principal str
-000013e0: 6574 6368 2d62 6173 6564 206d 6174 6572  etch-based mater
-000013f0: 6961 6c20 666f 726d 756c 6174 696f 6e20  ial formulation 
-00001400: 6170 706c 6965 6420 6f6e 2074 6865 2064  applied on the d
-00001410: 6973 746f 7274 696f 6e61 6c20 7370 6163  istortional spac
-00001420: 653a 0a0a 6060 6070 7974 686f 6e0a 636c  e:..```python.cl
-00001430: 6173 7320 4d79 4d6f 6465 6c32 3a0a 2020  ass MyModel2:.  
-00001440: 2020 6465 6620 6772 6164 6965 6e74 2873    def gradient(s
-00001450: 656c 662c 20ce bb2c 2073 7461 7465 7661  elf, .., stateva
-00001460: 7273 293a 0a20 2020 2020 2020 2022 2222  rs):.        """
-00001470: 5468 6520 6772 6164 6965 6e74 2061 7320  The gradient as 
-00001480: 7468 6520 7061 7274 6961 6c20 6465 7269  the partial deri
-00001490: 7661 7469 7665 206f 6620 7468 6520 7374  vative of the st
-000014a0: 7261 696e 2065 6e65 7267 7920 6675 6e63  rain energy func
-000014b0: 7469 6f6e 2077 2e72 2e74 2e0a 2020 2020  tion w.r.t..    
-000014c0: 2020 2020 7468 6520 7072 696e 6369 7061      the principa
-000014d0: 6c20 7374 7265 7463 6865 732e 2222 220a  l stretches.""".
-000014e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000014f0: 5b64 5764 cebb 312c 2064 5764 cebb 322c  [dWd..1, dWd..2,
-00001500: 2064 5764 cebb 335d 2c20 7374 6174 6576   dWd..3], statev
-00001510: 6172 730a 0a20 2020 2064 6566 2068 6573  ars..    def hes
-00001520: 7369 616e 2873 656c 662c 20ce bb2c 2073  sian(self, .., s
-00001530: 7461 7465 7661 7273 5f6f 6c64 293a 0a20  tatevars_old):. 
-00001540: 2020 2020 2020 2022 2222 5468 6520 6865         """The he
-00001550: 7373 6961 6e20 6173 2074 6865 2073 6563  ssian as the sec
-00001560: 6f6e 6420 7061 7274 6961 6c20 6465 7269  ond partial deri
-00001570: 7661 7469 7665 7320 6f66 2074 6865 2073  vatives of the s
-00001580: 7472 6169 6e20 656e 6572 6779 2066 756e  train energy fun
-00001590: 6374 696f 6e0a 2020 2020 2020 2020 772e  ction.        w.
-000015a0: 722e 742e 2074 6865 2070 7269 6e63 6970  r.t. the princip
-000015b0: 616c 2073 7472 6574 6368 6573 2e22 2222  al stretches."""
-000015c0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000015d0: 2064 3257 64ce bb31 64ce bb31 2c20 6432   d2Wd..1d..1, d2
-000015e0: 5764 cebb 3264 cebb 322c 2064 3257 64ce  Wd..2d..2, d2Wd.
-000015f0: bb33 64ce bb33 2c20 6432 5764 cebb 3164  .3d..3, d2Wd..1d
-00001600: cebb 322c 2064 3257 64ce bb32 64ce bb33  ..2, d2Wd..2d..3
-00001610: 2c20 6432 5764 cebb 3164 cebb 330a 0a0a  , d2Wd..1d..3...
-00001620: 6d6f 6465 6c32 203d 204d 794d 6f64 656c  model2 = MyModel
-00001630: 3228 290a 756d 6174 3220 3d20 6865 6c2e  2().umat2 = hel.
-00001640: 7370 6163 6573 2e44 6973 746f 7274 696f  spaces.Distortio
-00001650: 6e61 6c53 7061 6365 2868 656c 2e66 7261  nalSpace(hel.fra
-00001660: 6d65 776f 726b 732e 5374 7265 7463 6865  meworks.Stretche
-00001670: 7346 7261 6d65 776f 726b 286d 6f64 656c  sFramework(model
-00001680: 3229 290a 6060 600a 0a23 2323 2041 7661  2)).```..### Ava
-00001690: 696c 6162 6c65 2069 736f 7472 6f70 6963  ilable isotropic
-000016a0: 2068 7970 6572 656c 6173 7469 6320 7374   hyperelastic st
-000016b0: 7265 7463 682d 6261 7365 6420 6d61 7465  retch-based mate
-000016c0: 7269 616c 2066 6f72 6d75 6c61 7469 6f6e  rial formulation
-000016d0: 730a 2d20 5b4f 6764 656e 5d28 6874 7470  s.- [Ogden](http
-000016e0: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-000016f0: 2e6f 7267 2f77 696b 692f 4f67 6465 6e5f  .org/wiki/Ogden_
-00001700: 2868 7970 6572 656c 6173 7469 635f 6d6f  (hyperelastic_mo
-00001710: 6465 6c29 2920 285b 636f 6465 5d28 6874  del)) ([code](ht
-00001720: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001730: 2f61 6474 7a6c 722f 6879 7065 7265 6c61  /adtzlr/hyperela
-00001740: 7374 6963 2f62 6c6f 622f 6d61 696e 2f73  stic/blob/main/s
-00001750: 7263 2f68 7970 6572 656c 6173 7469 632f  rc/hyperelastic/
-00001760: 6d6f 6465 6c73 2f73 7472 6574 6368 6573  models/stretches
-00001770: 2f5f 6f67 6465 6e2e 7079 2929 0a0a 2320  /_ogden.py))..# 
-00001780: 4c69 6365 6e73 650a 4879 7065 7265 6c61  License.Hyperela
-00001790: 7374 6963 202d 2043 6f6e 7374 6974 7574  stic - Constitut
-000017a0: 6976 6520 6879 7065 7265 6c61 7374 6963  ive hyperelastic
-000017b0: 206d 6174 6572 6961 6c20 666f 726d 756c   material formul
-000017c0: 6174 696f 6e73 2066 6f72 2046 456c 7570  ations for FElup
-000017d0: 6520 2843 2920 3230 3233 2041 6e64 7265  e (C) 2023 Andre
-000017e0: 6173 2044 7574 7a6c 6572 2c20 4772 617a  as Dutzler, Graz
-000017f0: 2028 4175 7374 7269 6129 2e0a 0a54 6869   (Austria)...Thi
-00001800: 7320 7072 6f67 7261 6d20 6973 2066 7265  s program is fre
-00001810: 6520 736f 6674 7761 7265 3a20 796f 7520  e software: you 
-00001820: 6361 6e20 7265 6469 7374 7269 6275 7465  can redistribute
-00001830: 2069 7420 616e 642f 6f72 206d 6f64 6966   it and/or modif
-00001840: 7920 6974 2075 6e64 6572 2074 6865 2074  y it under the t
-00001850: 6572 6d73 206f 6620 7468 6520 474e 5520  erms of the GNU 
-00001860: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00001870: 6963 656e 7365 2061 7320 7075 626c 6973  icense as publis
-00001880: 6865 6420 6279 2074 6865 2046 7265 6520  hed by the Free 
-00001890: 536f 6674 7761 7265 2046 6f75 6e64 6174  Software Foundat
-000018a0: 696f 6e2c 2065 6974 6865 7220 7665 7273  ion, either vers
-000018b0: 696f 6e20 3320 6f66 2074 6865 204c 6963  ion 3 of the Lic
-000018c0: 656e 7365 2c20 6f72 2028 6174 2079 6f75  ense, or (at you
-000018d0: 7220 6f70 7469 6f6e 2920 616e 7920 6c61  r option) any la
-000018e0: 7465 7220 7665 7273 696f 6e2e 0a0a 5468  ter version...Th
-000018f0: 6973 2070 726f 6772 616d 2069 7320 6469  is program is di
-00001900: 7374 7269 6275 7465 6420 696e 2074 6865  stributed in the
-00001910: 2068 6f70 6520 7468 6174 2069 7420 7769   hope that it wi
-00001920: 6c6c 2062 6520 7573 6566 756c 2c20 6275  ll be useful, bu
-00001930: 7420 5749 5448 4f55 5420 414e 5920 5741  t WITHOUT ANY WA
-00001940: 5252 414e 5459 3b20 7769 7468 6f75 7420  RRANTY; without 
-00001950: 6576 656e 2074 6865 2069 6d70 6c69 6564  even the implied
-00001960: 2077 6172 7261 6e74 7920 6f66 204d 4552   warranty of MER
-00001970: 4348 414e 5441 4249 4c49 5459 206f 7220  CHANTABILITY or 
-00001980: 4649 544e 4553 5320 464f 5220 4120 5041  FITNESS FOR A PA
-00001990: 5254 4943 554c 4152 2050 5552 504f 5345  RTICULAR PURPOSE
-000019a0: 2e20 5365 6520 7468 6520 474e 5520 4765  . See the GNU Ge
-000019b0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000019c0: 656e 7365 2066 6f72 206d 6f72 6520 6465  ense for more de
-000019d0: 7461 696c 732e 0a0a 596f 7520 7368 6f75  tails...You shou
-000019e0: 6c64 2068 6176 6520 7265 6365 6976 6564  ld have received
-000019f0: 2061 2063 6f70 7920 6f66 2074 6865 2047   a copy of the G
-00001a00: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
-00001a10: 6320 4c69 6365 6e73 6520 616c 6f6e 6720  c License along 
-00001a20: 7769 7468 2074 6869 7320 7072 6f67 7261  with this progra
-00001a30: 6d2e 2049 6620 6e6f 742c 2073 6565 203c  m. If not, see <
-00001a40: 6874 7470 733a 2f2f 7777 772e 676e 752e  https://www.gnu.
-00001a50: 6f72 672f 6c69 6365 6e73 6573 2f3e 2e0a  org/licenses/>..
+00000e90: 204d 7949 6e76 6172 6961 6e74 734d 6f64   MyInvariantsMod
+00000ea0: 656c 3a0a 2020 2020 6465 6620 6772 6164  el:.    def grad
+00000eb0: 6965 6e74 2873 656c 662c 2049 312c 2049  ient(self, I1, I
+00000ec0: 322c 2049 332c 2073 7461 7465 7661 7273  2, I3, statevars
+00000ed0: 293a 0a20 2020 2020 2020 2022 2222 5468  ):.        """Th
+00000ee0: 6520 6772 6164 6965 6e74 2061 7320 7468  e gradient as th
+00000ef0: 6520 7061 7274 6961 6c20 6465 7269 7661  e partial deriva
+00000f00: 7469 7665 206f 6620 7468 6520 7374 7261  tive of the stra
+00000f10: 696e 2065 6e65 7267 7920 6675 6e63 7469  in energy functi
+00000f20: 6f6e 2077 2e72 2e74 2e0a 2020 2020 2020  on w.r.t..      
+00000f30: 2020 7468 6520 696e 7661 7269 616e 7473    the invariants
+00000f40: 206f 6620 7468 6520 7269 6768 7420 4361   of the right Ca
+00000f50: 7563 6879 2d47 7265 656e 2064 6566 6f72  uchy-Green defor
+00000f60: 6d61 7469 6f6e 2074 656e 736f 722e 2222  mation tensor.""
+00000f70: 220a 0a20 2020 2020 2020 2023 2075 7365  "..        # use
+00000f80: 7220 636f 6465 0a20 2020 2020 2020 2064  r code.        d
+00000f90: 5764 4931 203d 204e 6f6e 650a 2020 2020  WdI1 = None.    
+00000fa0: 2020 2020 6457 6449 3220 3d20 4e6f 6e65      dWdI2 = None
+00000fb0: 0a20 2020 2020 2020 2064 5764 4933 203d  .        dWdI3 =
+00000fc0: 204e 6f6e 650a 0a20 2020 2020 2020 2072   None..        r
+00000fd0: 6574 7572 6e20 6457 6449 312c 2064 5764  eturn dWdI1, dWd
+00000fe0: 4932 2c20 6457 6449 332c 2073 7461 7465  I2, dWdI3, state
+00000ff0: 7661 7273 0a0a 2020 2020 6465 6620 6865  vars..    def he
+00001000: 7373 6961 6e28 7365 6c66 2c20 4931 2c20  ssian(self, I1, 
+00001010: 4932 2c20 4933 2c20 7374 6174 6576 6172  I2, I3, statevar
+00001020: 735f 6f6c 6429 3a0a 2020 2020 2020 2020  s_old):.        
+00001030: 2222 2254 6865 2068 6573 7369 616e 2061  """The hessian a
+00001040: 7320 7468 6520 7365 636f 6e64 2070 6172  s the second par
+00001050: 7469 616c 2064 6572 6976 6174 6976 6573  tial derivatives
+00001060: 206f 6620 7468 6520 7374 7261 696e 2065   of the strain e
+00001070: 6e65 7267 7920 6675 6e63 7469 6f6e 0a20  nergy function. 
+00001080: 2020 2020 2020 2077 2e72 2e74 2e20 7468         w.r.t. th
+00001090: 6520 696e 7661 7269 616e 7473 206f 6620  e invariants of 
+000010a0: 7468 6520 7269 6768 7420 4361 7563 6879  the right Cauchy
+000010b0: 2d47 7265 656e 2064 6566 6f72 6d61 7469  -Green deformati
+000010c0: 6f6e 2074 656e 736f 722e 2222 220a 0a20  on tensor.""".. 
+000010d0: 2020 2020 2020 2023 2075 7365 7220 636f         # user co
+000010e0: 6465 0a20 2020 2020 2020 2064 3257 6449  de.        d2WdI
+000010f0: 3149 3120 3d20 4e6f 6e65 0a20 2020 2020  1I1 = None.     
+00001100: 2020 2064 3257 6449 3249 3220 3d20 4e6f     d2WdI2I2 = No
+00001110: 6e65 0a20 2020 2020 2020 2064 3257 6449  ne.        d2WdI
+00001120: 3349 3320 3d20 4e6f 6e65 0a20 2020 2020  3I3 = None.     
+00001130: 2020 2064 3257 6449 3149 3220 3d20 4e6f     d2WdI1I2 = No
+00001140: 6e65 0a20 2020 2020 2020 2064 3257 6449  ne.        d2WdI
+00001150: 3249 3320 3d20 4e6f 6e65 0a20 2020 2020  2I3 = None.     
+00001160: 2020 2064 3257 6449 3149 3320 3d20 4e6f     d2WdI1I3 = No
+00001170: 6e65 0a0a 2020 2020 2020 2020 7265 7475  ne..        retu
+00001180: 726e 2064 3257 6449 3149 312c 2064 3257  rn d2WdI1I1, d2W
+00001190: 6449 3249 322c 2064 3257 6449 3349 332c  dI2I2, d2WdI3I3,
+000011a0: 2064 3257 6449 3149 322c 2064 3257 6449   d2WdI1I2, d2WdI
+000011b0: 3249 332c 2064 3257 6449 3149 330a 0a0a  2I3, d2WdI1I3...
+000011c0: 6d6f 6465 6c20 3d20 4d79 496e 7661 7269  model = MyInvari
+000011d0: 616e 7473 4d6f 6465 6c28 290a 6672 616d  antsModel().fram
+000011e0: 6577 6f72 6b20 3d20 6865 6c2e 6672 616d  ework = hel.fram
+000011f0: 6577 6f72 6b73 2e49 6e76 6172 6961 6e74  eworks.Invariant
+00001200: 7346 7261 6d65 776f 726b 286d 6f64 656c  sFramework(model
+00001210: 290a 756d 6174 203d 2068 656c 2e73 7061  ).umat = hel.spa
+00001220: 6365 732e 4469 7374 6f72 7469 6f6e 616c  ces.Distortional
+00001230: 5370 6163 6528 6672 616d 6577 6f72 6b29  Space(framework)
+00001240: 0a60 6060 0a0a 2323 2320 4176 6169 6c61  .```..### Availa
+00001250: 626c 6520 6973 6f74 726f 7069 6320 6879  ble isotropic hy
+00001260: 7065 7265 6c61 7374 6963 2069 6e76 6172  perelastic invar
+00001270: 6961 6e74 2d62 6173 6564 206d 6174 6572  iant-based mater
+00001280: 6961 6c20 666f 726d 756c 6174 696f 6e73  ial formulations
+00001290: 0a54 6865 2074 7970 6963 616c 2070 6f6c  .The typical pol
+000012a0: 796e 6f6d 6961 6c2d 6261 7365 6420 6d61  ynomial-based ma
+000012b0: 7465 7269 616c 2066 6f72 6d75 6c61 7469  terial formulati
+000012c0: 6f6e 7320 285b 4e65 6f2d 486f 6f6b 655d  ons ([Neo-Hooke]
+000012d0: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+000012e0: 7065 6469 612e 6f72 672f 7769 6b69 2f4e  pedia.org/wiki/N
+000012f0: 656f 2d48 6f6f 6b65 616e 5f73 6f6c 6964  eo-Hookean_solid
+00001300: 292c 205b 4d6f 6f6e 6579 2d52 6976 6c69  ), [Mooney-Rivli
+00001310: 6e5d 2868 7474 7073 3a2f 2f65 6e2e 7769  n](https://en.wi
+00001320: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00001330: 2f4d 6f6f 6e65 7925 4532 2538 3025 3933  /Mooney%E2%80%93
+00001340: 5269 766c 696e 5f73 6f6c 6964 292c 205b  Rivlin_solid), [
+00001350: 5965 6f68 5d28 6874 7470 733a 2f2f 656e  Yeoh](https://en
+00001360: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00001370: 696b 692f 5965 6f68 5f68 7970 6572 656c  iki/Yeoh_hyperel
+00001380: 6173 7469 635f 6d6f 6465 6c29 2061 7265  astic_model) are
+00001390: 2061 6c6c 2061 7661 696c 6162 6c65 2061   all available a
+000013a0: 7320 7375 626d 6f64 656c 7320 6f66 2074  s submodels of t
+000013b0: 6865 2074 6869 7264 206f 7264 6572 2064  he third order d
+000013c0: 6566 6f72 6d61 7469 6f6e 206d 6174 6572  eformation mater
+000013d0: 6961 6c20 666f 726d 756c 6174 696f 6e2e  ial formulation.
+000013e0: 0a0a 2d20 5b54 6869 7264 2d4f 7264 6572  ..- [Third-Order
+000013f0: 2d44 6566 6f72 6d61 7469 6f6e 2028 4a61  -Deformation (Ja
+00001400: 6d65 732d 4772 6565 6e2d 5369 6d70 736f  mes-Green-Simpso
+00001410: 6e29 5d28 6874 7470 733a 2f2f 6f6e 6c69  n)](https://onli
+00001420: 6e65 6c69 6272 6172 792e 7769 6c65 792e  nelibrary.wiley.
+00001430: 636f 6d2f 646f 692f 6162 732f 3130 2e31  com/doi/abs/10.1
+00001440: 3030 322f 6170 702e 3139 3735 2e30 3730  002/app.1975.070
+00001450: 3139 3037 3233 2920 285b 636f 6465 5d28  190723) ([code](
+00001460: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001470: 6f6d 2f61 6474 7a6c 722f 6879 7065 7265  om/adtzlr/hypere
+00001480: 6c61 7374 6963 2f62 6c6f 622f 6d61 696e  lastic/blob/main
+00001490: 2f73 7263 2f68 7970 6572 656c 6173 7469  /src/hyperelasti
+000014a0: 632f 6d6f 6465 6c73 2f69 6e76 6172 6961  c/models/invaria
+000014b0: 6e74 732f 5f74 6869 7264 5f6f 7264 6572  nts/_third_order
+000014c0: 5f64 6566 6f72 6d61 7469 6f6e 2e70 7929  _deformation.py)
+000014d0: 290a 0a0a 2323 2050 7269 6e63 6970 616c  )...## Principal
+000014e0: 2073 7472 6574 6368 2d62 6173 6564 206d   stretch-based m
+000014f0: 6174 6572 6961 6c20 666f 726d 756c 6174  aterial formulat
+00001500: 696f 6e73 0a41 206d 696e 696d 616c 2074  ions.A minimal t
+00001510: 656d 706c 6174 6520 666f 7220 6120 7072  emplate for a pr
+00001520: 696e 6369 7061 6c20 7374 7265 7463 682d  incipal stretch-
+00001530: 6261 7365 6420 6d61 7465 7269 616c 2066  based material f
+00001540: 6f72 6d75 6c61 7469 6f6e 2061 7070 6c69  ormulation appli
+00001550: 6564 206f 6e20 7468 6520 6469 7374 6f72  ed on the distor
+00001560: 7469 6f6e 616c 2073 7061 6365 3a0a 0a60  tional space:..`
+00001570: 6060 7079 7468 6f6e 0a63 6c61 7373 204d  ``python.class M
+00001580: 7953 7472 6574 6368 6573 4d6f 6465 6c3a  yStretchesModel:
+00001590: 0a20 2020 2064 6566 2067 7261 6469 656e  .    def gradien
+000015a0: 7428 7365 6c66 2c20 cebb 2c20 7374 6174  t(self, .., stat
+000015b0: 6576 6172 7329 3a0a 2020 2020 2020 2020  evars):.        
+000015c0: 2222 2254 6865 2067 7261 6469 656e 7420  """The gradient 
+000015d0: 6173 2074 6865 2070 6172 7469 616c 2064  as the partial d
+000015e0: 6572 6976 6174 6976 6520 6f66 2074 6865  erivative of the
+000015f0: 2073 7472 6169 6e20 656e 6572 6779 2066   strain energy f
+00001600: 756e 6374 696f 6e20 772e 722e 742e 0a20  unction w.r.t.. 
+00001610: 2020 2020 2020 2074 6865 2070 7269 6e63         the princ
+00001620: 6970 616c 2073 7472 6574 6368 6573 2e22  ipal stretches."
+00001630: 2222 0a0a 2020 2020 2020 2020 2320 7573  ""..        # us
+00001640: 6572 2063 6f64 650a 2020 2020 2020 2020  er code.        
+00001650: 6457 64ce bb31 2c20 6457 64ce bb32 2c20  dWd..1, dWd..2, 
+00001660: 6457 64ce bb33 203d 2030 202a 20ce bb0a  dWd..3 = 0 * ...
+00001670: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001680: 5b64 5764 cebb 312c 2064 5764 cebb 322c  [dWd..1, dWd..2,
+00001690: 2064 5764 cebb 335d 2c20 7374 6174 6576   dWd..3], statev
+000016a0: 6172 730a 0a20 2020 2064 6566 2068 6573  ars..    def hes
+000016b0: 7369 616e 2873 656c 662c 20ce bb2c 2073  sian(self, .., s
+000016c0: 7461 7465 7661 7273 5f6f 6c64 293a 0a20  tatevars_old):. 
+000016d0: 2020 2020 2020 2022 2222 5468 6520 6865         """The he
+000016e0: 7373 6961 6e20 6173 2074 6865 2073 6563  ssian as the sec
+000016f0: 6f6e 6420 7061 7274 6961 6c20 6465 7269  ond partial deri
+00001700: 7661 7469 7665 7320 6f66 2074 6865 2073  vatives of the s
+00001710: 7472 6169 6e20 656e 6572 6779 2066 756e  train energy fun
+00001720: 6374 696f 6e0a 2020 2020 2020 2020 772e  ction.        w.
+00001730: 722e 742e 2074 6865 2070 7269 6e63 6970  r.t. the princip
+00001740: 616c 2073 7472 6574 6368 6573 2e22 2222  al stretches."""
+00001750: 0a0a 2020 2020 2020 2020 2320 7573 6572  ..        # user
+00001760: 2063 6f64 650a 2020 2020 2020 2020 6432   code.        d2
+00001770: 5764 cebb 3164 cebb 3120 3d20 4e6f 6e65  Wd..1d..1 = None
+00001780: 0a20 2020 2020 2020 2064 3257 64ce bb32  .        d2Wd..2
+00001790: 64ce bb32 203d 204e 6f6e 650a 2020 2020  d..2 = None.    
+000017a0: 2020 2020 6432 5764 cebb 3364 cebb 3320      d2Wd..3d..3 
+000017b0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2064  = None.        d
+000017c0: 3257 64ce bb31 64ce bb32 203d 204e 6f6e  2Wd..1d..2 = Non
+000017d0: 650a 2020 2020 2020 2020 6432 5764 cebb  e.        d2Wd..
+000017e0: 3264 cebb 3320 3d20 4e6f 6e65 0a20 2020  2d..3 = None.   
+000017f0: 2020 2020 2064 3257 64ce bb31 64ce bb33       d2Wd..1d..3
+00001800: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+00001810: 2072 6574 7572 6e20 6432 5764 cebb 3164   return d2Wd..1d
+00001820: cebb 312c 2064 3257 64ce bb32 64ce bb32  ..1, d2Wd..2d..2
+00001830: 2c20 6432 5764 cebb 3364 cebb 332c 2064  , d2Wd..3d..3, d
+00001840: 3257 64ce bb31 64ce bb32 2c20 6432 5764  2Wd..1d..2, d2Wd
+00001850: cebb 3264 cebb 332c 2064 3257 64ce bb31  ..2d..3, d2Wd..1
+00001860: 64ce bb33 0a0a 0a6d 6f64 656c 203d 204d  d..3...model = M
+00001870: 7953 7472 6574 6368 6573 4d6f 6465 6c28  yStretchesModel(
+00001880: 290a 6672 616d 6577 6f72 6b20 3d20 6865  ).framework = he
+00001890: 6c2e 6672 616d 6577 6f72 6b73 2e53 7472  l.frameworks.Str
+000018a0: 6574 6368 6573 4672 616d 6577 6f72 6b28  etchesFramework(
+000018b0: 6d6f 6465 6c29 0a75 6d61 7420 3d20 6865  model).umat = he
+000018c0: 6c2e 7370 6163 6573 2e44 6973 746f 7274  l.spaces.Distort
+000018d0: 696f 6e61 6c53 7061 6365 2866 7261 6d65  ionalSpace(frame
+000018e0: 776f 726b 290a 6060 600a 0a23 2323 2041  work).```..### A
+000018f0: 7661 696c 6162 6c65 2069 736f 7472 6f70  vailable isotrop
+00001900: 6963 2068 7970 6572 656c 6173 7469 6320  ic hyperelastic 
+00001910: 7374 7265 7463 682d 6261 7365 6420 6d61  stretch-based ma
+00001920: 7465 7269 616c 2066 6f72 6d75 6c61 7469  terial formulati
+00001930: 6f6e 730a 2d20 5b4f 6764 656e 5d28 6874  ons.- [Ogden](ht
+00001940: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00001950: 6961 2e6f 7267 2f77 696b 692f 4f67 6465  ia.org/wiki/Ogde
+00001960: 6e5f 2868 7970 6572 656c 6173 7469 635f  n_(hyperelastic_
+00001970: 6d6f 6465 6c29 2920 285b 636f 6465 5d28  model)) ([code](
+00001980: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001990: 6f6d 2f61 6474 7a6c 722f 6879 7065 7265  om/adtzlr/hypere
+000019a0: 6c61 7374 6963 2f62 6c6f 622f 6d61 696e  lastic/blob/main
+000019b0: 2f73 7263 2f68 7970 6572 656c 6173 7469  /src/hyperelasti
+000019c0: 632f 6d6f 6465 6c73 2f73 7472 6574 6368  c/models/stretch
+000019d0: 6573 2f5f 6f67 6465 6e2e 7079 2929 0a0a  es/_ogden.py))..
+000019e0: 2323 204c 6162 0a42 7920 7573 696e 6720  ## Lab.By using 
+000019f0: 5b6d 6174 6164 695d 2868 7474 7073 3a2f  [matadi](https:/
+00001a00: 2f67 6974 6875 622e 636f 6d2f 6164 747a  /github.com/adtz
+00001a10: 6c72 2f6d 6174 6164 6929 2773 2060 4c61  lr/matadi)'s `La
+00001a20: 6249 6e63 6f6d 7072 6573 7369 626c 6560  bIncompressible`
+00001a30: 2c20 6e75 6d65 7269 6320 6578 7065 7269  , numeric experi
+00001a40: 6d65 6e74 7320 6f6e 2068 6f6d 6f67 656e  ments on homogen
+00001a50: 656f 7573 2069 6e63 6f6d 7072 6573 7369  eous incompressi
+00001a60: 626c 6520 6c6f 6164 6361 7365 7320 6f6e  ble loadcases on
+00001a70: 2068 7970 6572 656c 6173 7469 6320 6d61   hyperelastic ma
+00001a80: 7465 7269 616c 2066 6f72 6d75 6c61 7469  terial formulati
+00001a90: 6f6e 7320 6172 6520 7065 7266 6f72 6d65  ons are performe
+00001aa0: 642e 2045 6e73 7572 6520 746f 2068 6176  d. Ensure to hav
+00001ab0: 6520 5b6d 6174 6164 695d 2868 7474 7073  e [matadi](https
+00001ac0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6164  ://github.com/ad
+00001ad0: 747a 6c72 2f6d 6174 6164 6929 2069 6e73  tzlr/matadi) ins
+00001ae0: 7461 6c6c 6564 202d 2072 756e 2060 7069  talled - run `pi
+00001af0: 7020 696e 7374 616c 6c20 6d61 7461 6469  p install matadi
+00001b00: 6020 696e 2079 6f75 7220 7465 726d 696e  ` in your termin
+00001b10: 616c 2e0a 0a60 6060 7079 7468 6f6e 0a6d  al...```python.m
+00001b20: 6f6f 6e65 795f 7269 766c 696e 203d 2068  ooney_rivlin = h
+00001b30: 656c 2e6d 6f64 656c 732e 696e 7661 7269  el.models.invari
+00001b40: 616e 7473 2e54 6869 7264 4f72 6465 7244  ants.ThirdOrderD
+00001b50: 6566 6f72 6d61 7469 6f6e 2843 3130 3d30  eformation(C10=0
+00001b60: 2e33 2c20 4330 313d 302e 3229 0a66 7261  .3, C01=0.2).fra
+00001b70: 6d65 776f 726b 203d 2068 656c 2e66 7261  mework = hel.fra
+00001b80: 6d65 776f 726b 732e 496e 7661 7269 616e  meworks.Invarian
+00001b90: 7473 4672 616d 6577 6f72 6b28 6d6f 6f6e  tsFramework(moon
+00001ba0: 6579 5f72 6976 6c69 6e29 0a75 6d61 7420  ey_rivlin).umat 
+00001bb0: 3d20 6865 6c2e 7370 6163 6573 2e44 6973  = hel.spaces.Dis
+00001bc0: 746f 7274 696f 6e61 6c53 7061 6365 2866  tortionalSpace(f
+00001bd0: 7261 6d65 776f 726b 290a 0a69 6d70 6f72  ramework)..impor
+00001be0: 7420 6d61 7461 6469 0a0a 6c61 6220 3d20  t matadi..lab = 
+00001bf0: 6d61 7461 6469 2e4c 6162 496e 636f 6d70  matadi.LabIncomp
+00001c00: 7265 7373 6962 6c65 2875 6d61 742c 2074  ressible(umat, t
+00001c10: 6974 6c65 3d22 4d6f 6f6e 6579 2052 6976  itle="Mooney Riv
+00001c20: 6c69 6e22 290a 6461 7461 203d 206c 6162  lin").data = lab
+00001c30: 2e72 756e 280a 2020 2020 7578 3d54 7275  .run(.    ux=Tru
+00001c40: 652c 0a20 2020 2062 783d 5472 7565 2c0a  e,.    bx=True,.
+00001c50: 2020 2020 7073 3d54 7275 652c 0a20 2020      ps=True,.   
+00001c60: 2073 7472 6574 6368 5f6d 696e 3d30 2e37   stretch_min=0.7
+00001c70: 2c0a 2020 2020 7374 7265 7463 685f 6d61  ,.    stretch_ma
+00001c80: 783d 322e 352c 0a29 0a66 6967 2c20 6178  x=2.5,.).fig, ax
+00001c90: 203d 206c 6162 2e70 6c6f 7428 6461 7461   = lab.plot(data
+00001ca0: 2c20 7374 6162 696c 6974 793d 5472 7565  , stability=True
+00001cb0: 290a 6060 600a 0a21 5b6c 6162 5f6d 6f6f  ).```..![lab_moo
+00001cc0: 6e65 792d 7269 766c 696e 5d28 6874 7470  ney-rivlin](http
+00001cd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00001ce0: 6474 7a6c 722f 6879 7065 7265 6c61 7374  dtzlr/hyperelast
+00001cf0: 6963 2f61 7373 6574 732f 3537 3933 3135  ic/assets/579315
+00001d00: 332f 3162 3231 6466 3831 2d65 3066 642d  3/1b21df81-e0fd-
+00001d10: 3465 6131 2d39 6264 372d 3234 6434 6437  4ea1-9bd7-24d4d7
+00001d20: 3062 6138 3031 290a 0a23 204c 6963 656e  0ba801)..# Licen
+00001d30: 7365 0a48 7970 6572 656c 6173 7469 6320  se.Hyperelastic 
+00001d40: 2d20 436f 6e73 7469 7475 7469 7665 2068  - Constitutive h
+00001d50: 7970 6572 656c 6173 7469 6320 6d61 7465  yperelastic mate
+00001d60: 7269 616c 2066 6f72 6d75 6c61 7469 6f6e  rial formulation
+00001d70: 7320 666f 7220 4645 6c75 7065 2028 4329  s for FElupe (C)
+00001d80: 2032 3032 3320 416e 6472 6561 7320 4475   2023 Andreas Du
+00001d90: 747a 6c65 722c 2047 7261 7a20 2841 7573  tzler, Graz (Aus
+00001da0: 7472 6961 292e 0a0a 5468 6973 2070 726f  tria)...This pro
+00001db0: 6772 616d 2069 7320 6672 6565 2073 6f66  gram is free sof
+00001dc0: 7477 6172 653a 2079 6f75 2063 616e 2072  tware: you can r
+00001dd0: 6564 6973 7472 6962 7574 6520 6974 2061  edistribute it a
+00001de0: 6e64 2f6f 7220 6d6f 6469 6679 2069 7420  nd/or modify it 
+00001df0: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
+00001e00: 6f66 2074 6865 2047 4e55 2047 656e 6572  of the GNU Gener
+00001e10: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+00001e20: 6520 6173 2070 7562 6c69 7368 6564 2062  e as published b
+00001e30: 7920 7468 6520 4672 6565 2053 6f66 7477  y the Free Softw
+00001e40: 6172 6520 466f 756e 6461 7469 6f6e 2c20  are Foundation, 
+00001e50: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
+00001e60: 206f 6620 7468 6520 4c69 6365 6e73 652c   of the License,
+00001e70: 206f 7220 2861 7420 796f 7572 206f 7074   or (at your opt
+00001e80: 696f 6e29 2061 6e79 206c 6174 6572 2076  ion) any later v
+00001e90: 6572 7369 6f6e 2e0a 0a54 6869 7320 7072  ersion...This pr
+00001ea0: 6f67 7261 6d20 6973 2064 6973 7472 6962  ogram is distrib
+00001eb0: 7574 6564 2069 6e20 7468 6520 686f 7065  uted in the hope
+00001ec0: 2074 6861 7420 6974 2077 696c 6c20 6265   that it will be
+00001ed0: 2075 7365 6675 6c2c 2062 7574 2057 4954   useful, but WIT
+00001ee0: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
+00001ef0: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
+00001f00: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
+00001f10: 616e 7479 206f 6620 4d45 5243 4841 4e54  anty of MERCHANT
+00001f20: 4142 494c 4954 5920 6f72 2046 4954 4e45  ABILITY or FITNE
+00001f30: 5353 2046 4f52 2041 2050 4152 5449 4355  SS FOR A PARTICU
+00001f40: 4c41 5220 5055 5250 4f53 452e 2053 6565  LAR PURPOSE. See
+00001f50: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
+00001f60: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00001f70: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
+00001f80: 2e0a 0a59 6f75 2073 686f 756c 6420 6861  ...You should ha
+00001f90: 7665 2072 6563 6569 7665 6420 6120 636f  ve received a co
+00001fa0: 7079 206f 6620 7468 6520 474e 5520 4765  py of the GNU Ge
+00001fb0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+00001fc0: 656e 7365 2061 6c6f 6e67 2077 6974 6820  ense along with 
+00001fd0: 7468 6973 2070 726f 6772 616d 2e20 4966  this program. If
+00001fe0: 206e 6f74 2c20 7365 6520 3c68 7474 7073   not, see <https
+00001ff0: 3a2f 2f77 7777 2e67 6e75 2e6f 7267 2f6c  ://www.gnu.org/l
+00002000: 6963 656e 7365 732f 3e2e 0a              icenses/>..
```

### Comparing `hyperelastic-0.1.1/pyproject.toml` & `hyperelastic-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.2.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,115 @@
 import numpy as np
 
-from ..math import cdya, ddot, dya, eye, trace
+from ..math import cdya, dya, eigh, transpose
 
 
-class InvariantsFramework:
-    r"""The Framework for a Total-Lagrangian invariant-based isotropic hyperelastic
+class StretchesFramework:
+    r"""The Framework for a Total-Lagrangian stretch-based isotropic hyperelastic
     material formulation provides the material behaviour-independent parts for
     evaluating the second Piola-Kirchhoff stress tensor as well as its associated
     fourth-order elasticity tensor.
 
     The gradient as well as the hessian of the strain energy function are carried out
     w.r.t. the right Cauchy-Green deformation tensor. Hence, the work-conjugate stress
     tensor is one half of the second Piola-Kirchhoff stress tensor and the fourth-order
     elasticitiy tensor used here is a quarter of the Total-Lagrangian elasticity tensor.
 
     ..  math::
 
-        \psi(\boldsymbol{C}) =
-            \psi(I_1(\boldsymbol{C}), I_2(\boldsymbol{C}), I_3(\boldsymbol{C}))
+        \psi(\boldsymbol{C}) = \psi(\lambda_\alpha(\boldsymbol{C}))
 
-    The first and second invariants of the left or right Cauchy-Green deformation tensor
-    are identified as factors of their characteristic polynomial,
+    The principal stretches (the square roots of the eigenvalues) of the left or right
+    Cauchy-Green deformation tensor are obtained by the solution of the eigenvalue
+    problem,
 
     ..  math::
 
-        I_1 &= \text{tr}(\boldsymbol{C})
-
-        I_2 &= \frac{1}{2}
-            \left( \text{tr}(\boldsymbol{C})^2 - \text{tr}(\boldsymbol{C}^2) \right)
+        \left( \boldsymbol{C} - \lambda^2_\alpha \boldsymbol{I} \right)
+            \boldsymbol{N}_\alpha = \boldsymbol{0}
 
     where the Cauchy-Green deformation tensors eliminate the rigid body rotations
     of the deformation gradient and serve as a quadratic change-of-length measure of
     the deformation.
 
     ..  math::
 
         \boldsymbol{C} &= \boldsymbol{F}^T \boldsymbol{F}
 
         \boldsymbol{b} &= \boldsymbol{F} \boldsymbol{F}^T
 
-    The first partial derivatives of the strain energy function w.r.t. the invariants
+    The first partial derivative of the strain energy function w.r.t. a principal
+    stretch
 
     ..  math::
 
-        \psi_{,1} &= \frac{\partial \psi}{\partial I_1}
-
-        \psi_{,2} &= \frac{\partial \psi}{\partial I_2}
+        \psi_{,\alpha} = \frac{\partial \psi}{\partial \lambda_\alpha}
 
-    and the partial derivatives of the invariants w.r.t. the right Cauchy-Green
-    deformation tensor are defined.
+    and the partial derivative of a principal strech w.r.t. the right Cauchy-Green
+    deformation tensor is defined
 
     ..  math::
 
-        \frac{\partial I_1}{\partial \boldsymbol{C}} &= 2 \boldsymbol{1}
+        \frac{\partial \lambda_\alpha}{\partial \boldsymbol{C}} =
+            \frac{\partial (\lambda^2_\alpha)^{1/2}}{\partial \boldsymbol{C}} =
+            \frac{1}{2 \lambda_\alpha} \boldsymbol{M}_\alpha
+
+    with the eigenbase as the dyadic (outer vector) product of eigenvectors.
+
+    ..  math::
 
-        \frac{\partial I_2}{\partial \boldsymbol{C}} &=
-            2 \left( I_1 \boldsymbol{1} - \boldsymbol{C} \right)
+        \boldsymbol{M}_\alpha = \boldsymbol{N}_\alpha \otimes \boldsymbol{N}_\alpha
 
     The second Piola-Kirchhoff stress tensor is formulated by the application of the
-    chain rule.
+    chain rule and a sum of all principal stretch contributions.
 
     ..  math::
 
-        \frac{\partial \psi}{\partial \boldsymbol{C}} =
-            \frac{\partial \psi}{\partial I_1}
-            \frac{\partial I_1}{\partial \boldsymbol{C}}
-            + \frac{\partial \psi}{\partial I_2}
-            \frac{\partial I_2}{\partial \boldsymbol{C}}
+        \frac{\partial \psi}{\partial \boldsymbol{C}} &=
+            \sum_\alpha \frac{\partial \psi}{\partial \lambda_\alpha}
+                \frac{\partial \lambda_\alpha}{\partial \boldsymbol{C}}
+
+        \boldsymbol{S} &= 2 \frac{\partial \psi}{\partial \boldsymbol{C}}
 
     Furthermore, the second partial derivatives of the elasticity tensor are carried
     out.
 
     ..  math::
 
-        \mathbb{C} &= \frac{\partial^2 \psi}{\partial I_1~\partial I_1}
-            \left( \frac{\partial I_1}{\partial \boldsymbol{C}} \otimes
-            \frac{\partial I_1}{\partial \boldsymbol{C}} \right)
-            + \frac{\partial^2 \psi}{\partial I_2~\partial I_2}
-            \left( \frac{\partial I_2}{\partial \boldsymbol{C}} \otimes
-            \frac{\partial I_2}{\partial \boldsymbol{C}} \right)
-
-            &+ \frac{\partial^2 \psi}{\partial I_1~\partial I_2}
-            \left( \frac{\partial I_1}{\partial \boldsymbol{C}} \otimes
-            \frac{\partial I_2}{\partial \boldsymbol{C}}
-            + \frac{\partial I_2}{\partial \boldsymbol{C}} \otimes
-            \frac{\partial I_1}{\partial \boldsymbol{C}} \right)
-
-            &+ \frac{\partial \psi}{\partial I_1}
-            \frac{\partial^2 I_1}{\partial \boldsymbol{C}~\partial \boldsymbol{C}}
-            + \frac{\partial \psi}{\partial I_2}
-            \frac{\partial^2 I_2}{\partial \boldsymbol{C}~\partial \boldsymbol{C}}
-
-    The only non material behaviour-related term which is not already defined during
-    stress evaluation is the second partial derivatives of the second invariant w.r.t.
-    the right Cauchy-Green deformation tensor.
+        \frac{\partial^2 \psi}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
+            \sum_\alpha \sum_\beta \frac{\partial^2 \psi}
+            {\partial \lambda_\alpha~\partial \lambda_\beta}
+            \frac{\partial \lambda_\alpha}{\partial \boldsymbol{C}} \otimes
+            \frac{\partial \lambda_\beta}{\partial \boldsymbol{C}}
+
+            &+ \sum_\alpha \sum_{\beta \ne \alpha} \frac{
+                \frac{\partial \psi}{\partial \lambda^2_\alpha} -
+                \frac{\partial \psi}{\partial \lambda^2_\beta}
+            }{\lambda^2_\alpha - \lambda^2_\beta} \left( \boldsymbol{M}_\alpha \odot
+                \boldsymbol{M}_\beta + \boldsymbol{M}_\beta \odot
+            \boldsymbol{M}_\alpha \right)
+
 
     ..  math::
 
-        \frac{\partial^2 I_2}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
-            \boldsymbol{I} \otimes \boldsymbol{I} - \boldsymbol{I} \odot \boldsymbol{I}
+        \mathbb{C} = 4 \frac{\partial^2 \psi}
+            {\partial \boldsymbol{C}~\partial \boldsymbol{C}}
+
+    In case of repeated equal principal stretches, the rule of d'Hospital is applied.
+
+    ..  math::
+
+        \lim_{\lambda^2_\beta \rightarrow \lambda^2_\alpha} \left(
+                \frac{\frac{\partial \psi}{\partial \lambda^2_\alpha} -
+                    \frac{\partial \psi}{\partial \lambda^2_\beta}
+                }{\lambda^2_\alpha - \lambda^2_\beta}
+            \right) = \left(
+            - \frac{\partial^2 \psi}{\partial \lambda^2_\alpha~\partial \lambda^2_\beta}
+            + \frac{\partial^2 \psi}{\partial \lambda^2_\beta~\partial \lambda^2_\beta}
+        \right)
 
     """
 
     def __init__(self, material, nstatevars=0, parallel=False):
         """Initialize the Framework for an invariant-based isotropic hyperelastic
         material formulation."""
 
@@ -112,52 +119,67 @@
         self.x = [np.eye(3), np.zeros(nstatevars)]
 
     def gradient(self, C, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the right Cauchy-Green deformation tensor (one half of the second Piola
         Kirchhoff stress tensor)."""
 
-        self.I = I = eye(C)
+        self.λ, self.M = eigh(C, fun=np.sqrt)
 
-        self.I1 = I1 = trace(C)
-        self.I2 = (I1**2 - ddot(C, C)) / 2
+        self.dWdλ, statevars_new = self.material.gradient(self.λ, statevars)
+        self.dWdλ = np.asarray(self.dWdλ)
 
-        self.dWdI1, self.dWdI2, statevars_new = self.material.gradient(
-            self.I1, self.I2, statevars
-        )
+        self.dWdλC = self.dWdλ / (2 * self.λ)
 
-        self.dI1dC = I
-        self.dI2dC = I1 * I - C
-
-        dWdC = self.dWdI1 * self.dI1dC + self.dWdI2 * self.dI2dC
+        dWdC = np.sum(np.expand_dims(self.dWdλC, axis=1) * self.M, axis=0)
 
         return dWdC, statevars_new
 
     def hessian(self, C, statevars):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the right Cauchy-Green deformation tensor (a quarter of the Lagrangian
         fourth-order elasticity tensor associated to the second Piola-Kirchhoff stress
         tensor)."""
 
         dWdC, statevars = self.gradient(C, statevars)
-        d2WdI1dI1, d2WdI2dI2, d2WdI1dI2 = self.material.hessian(
-            self.I1, self.I2, statevars
-        )
-        I = self.I
-        dI1dC = self.dI1dC
-        dI2dC = self.dI2dC
-
-        ntrax = len(C.shape[1:])
-        d2WdCdC = np.zeros((6, 6, *np.ones(ntrax, dtype=int)))
-
-        if not np.allclose(d2WdI1dI1, 0):
-            d2WdCdC = d2WdCdC + d2WdI1dI1 * dya(dI1dC, dI1dC)
-
-        if not np.allclose(d2WdI1dI2, 0):
-            d2WdCdC = d2WdCdC + d2WdI1dI2 * (dya(dI1dC, dI2dC) + dya(dI2dC, dI1dC))
-
-        if not np.allclose(self.dWdI2, 0):
-            d2I2dCdC = dya(I, I) - cdya(I, I)
+        d2Wdλdλ = self.material.hessian(self.λ, statevars)
 
-            d2WdCdC = d2WdCdC + self.dWdI2 * d2I2dCdC + d2WdI2dI2 * dya(dI2dC, dI2dC)
+        if not isinstance(d2Wdλdλ, np.ndarray):
+            newshape = self.λ[0].shape
+            _d2Wdλdλ = np.zeros((6, *self.λ[0].shape))
+            for a in range(6):
+                if d2Wdλdλ[a] is not None:
+                    _d2Wdλdλ[a] = np.broadcast_to(d2Wdλdλ[a], newshape)
+            d2Wdλdλ = _d2Wdλdλ
+
+        λ = self.λ
+        M = self.M
+        dWdλC = self.dWdλC
+
+        a = [0, 1, 2, 0, 1, 0]
+        b = [0, 1, 2, 1, 2, 2]
+
+        d2WdλC2 = d2Wdλdλ / (4 * λ[a] * λ[b])
+        d2WdλC2[:3] -= dWdλC / (2 * λ**2)
+
+        d2WdCdC = np.zeros((6, 6, *dWdλC.shape[1:]))
+
+        a = [0, 1, 2, 0, 1, 0]
+        b = [0, 1, 2, 1, 2, 2]
+
+        for m, (α, β) in enumerate(zip(a, b)):
+            M4 = dya(M[α], M[β])
+            d2WdCdC += d2WdλC2[m] * M4
+
+            if β != α:
+                v = λ[α] ** 2 - λ[β] ** 2
+                mask = np.isclose(v, 0)
+
+                f = np.zeros_like(v)
+                f[~mask] = (dWdλC[α][~mask] - dWdλC[β][~mask]) / v[~mask]
+                f[mask] = d2WdλC2[β][mask] - d2WdλC2[m][mask]
+
+                d2WdCdC += d2WdλC2[m] * transpose(M4) + f * (
+                    cdya(M[α], M[β]) + cdya(M[β], M[α])
+                )
 
         return d2WdCdC
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hyperelastic-0.1.1/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.2.0/src/hyperelastic/math/_voigt.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.2.0/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,30 +44,34 @@
 
         self.C10 = C10
         self.C01 = C01
         self.C11 = C11
         self.C20 = C20
         self.C30 = C30
 
-    def gradient(self, I1, I2, statevars):
+    def gradient(self, I1, I2, I3, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the invariants."""
 
         dWdI1 = (
             self.C10
             + self.C11 * (I2 - 3)
             + self.C20 * 2 * (I1 - 3)
             + self.C30 * 3 * (I1 - 3) ** 2
         )
         dWdI2 = self.C01 + self.C11 * (I1 - 3)
+        dWdI3 = None
 
-        return dWdI1, dWdI2, statevars
+        return dWdI1, dWdI2, dWdI3, statevars
 
-    def hessian(self, I1, I2, statevars):
+    def hessian(self, I1, I2, I3, statevars):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the invariants."""
 
         d2WdI1I1 = self.C20 * 2 + self.C30 * 6 * (I1 - 3)
-        d2WdI2I2 = 0
+        d2WdI2I2 = None
+        d2WdI3I3 = None
         d2WdI1I2 = self.C11
+        d2WdI2I3 = None
+        d2WdI1I3 = None
 
-        return d2WdI1I1, d2WdI2I2, d2WdI1I2
+        return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
```

### Comparing `hyperelastic-0.1.1/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.2.0/src/hyperelastic/spaces/_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.2.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.2.0/src/hyperelastic/spaces/_distortional.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.2.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.1.1
+Version: 0.2.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -722,15 +722,15 @@
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install hyperelastic
 ```
 
 # Usage
-Material model formulations have to be created as classes with methods for the evaluation of the `gradient` (stress) and the `hessian` of the strain energy function (elasticity). It depends on the framework which derivatives have to be defined, e.g. the derivatives w.r.t. the invariants of the right Cauchy-Green deformation tensor or w.r.t. the principal stretches. An instance of a **Framework** has to be *finalized* by the application on a **Space**.
+Material model formulations have to be created as classes with methods for the evaluation of the `gradient` (stress) and the `hessian` (elasticity) of the strain energy function. It depends on the framework which derivatives have to be defined, e.g. the derivatives w.r.t. the invariants of the right Cauchy-Green deformation tensor or w.r.t. the principal stretches. An instance of a **Framework** has to be *finalized* by the application on a **Space**.
 
 - [Deformation (Full) Space](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/spaces/_deformation.py)
 - [Distortional Space](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/spaces/_distortional.py)
 - [Dilatational Space](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/spaces/_dilatational.py)
 
 > ⓘ **Note**
 > Define your own material model formulation with manual, automatic or symbolic differentiation with the help of your favourite package, e.g. [PyTorch](https://pytorch.org/), [JAX](https://jax.readthedocs.io/en/latest/), [Tensorflow](https://www.tensorflow.org/), [TensorTRAX](https://github.com/adtzlr/tensortrax), [SymPy](https://www.sympy.org/en/index.html), etc.
@@ -742,63 +742,112 @@
 import hyperelastic.math as hm
 ```
 
 ## Invariant-based material formulations
 A minimal template for an invariant-based material formulation applied on the distortional space:
 
 ```python
-class MyModel1:
-    def gradient(self, I1, I2, statevars):
+class MyInvariantsModel:
+    def gradient(self, I1, I2, I3, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the invariants of the right Cauchy-Green deformation tensor."""
 
-        return dWdI1, dWdI2, statevars
+        # user code
+        dWdI1 = None
+        dWdI2 = None
+        dWdI3 = None
 
-    def hessian(self, I1, I2, statevars_old):
+        return dWdI1, dWdI2, dWdI3, statevars
+
+    def hessian(self, I1, I2, I3, statevars_old):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the invariants of the right Cauchy-Green deformation tensor."""
 
-        return d2WdI1I1, d2WdI2I2, d2WdI1I2
+        # user code
+        d2WdI1I1 = None
+        d2WdI2I2 = None
+        d2WdI3I3 = None
+        d2WdI1I2 = None
+        d2WdI2I3 = None
+        d2WdI1I3 = None
+
+        return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
 
 
-model1 = MyModel1()
-umat1 = hel.spaces.DistortionalSpace(hel.frameworks.InvariantsFramework(model1))
+model = MyInvariantsModel()
+framework = hel.frameworks.InvariantsFramework(model)
+umat = hel.spaces.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
 
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
-class MyModel2:
+class MyStretchesModel:
     def gradient(self, λ, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the principal stretches."""
 
+        # user code
+        dWdλ1, dWdλ2, dWdλ3 = 0 * λ
+
         return [dWdλ1, dWdλ2, dWdλ3], statevars
 
     def hessian(self, λ, statevars_old):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the principal stretches."""
 
+        # user code
+        d2Wdλ1dλ1 = None
+        d2Wdλ2dλ2 = None
+        d2Wdλ3dλ3 = None
+        d2Wdλ1dλ2 = None
+        d2Wdλ2dλ3 = None
+        d2Wdλ1dλ3 = None
+
         return d2Wdλ1dλ1, d2Wdλ2dλ2, d2Wdλ3dλ3, d2Wdλ1dλ2, d2Wdλ2dλ3, d2Wdλ1dλ3
 
 
-model2 = MyModel2()
-umat2 = hel.spaces.DistortionalSpace(hel.frameworks.StretchesFramework(model2))
+model = MyStretchesModel()
+framework = hel.frameworks.StretchesFramework(model)
+umat = hel.spaces.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic stretch-based material formulations
 - [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/stretches/_ogden.py))
 
+## Lab
+By using [matadi](https://github.com/adtzlr/matadi)'s `LabIncompressible`, numeric experiments on homogeneous incompressible loadcases on hyperelastic material formulations are performed. Ensure to have [matadi](https://github.com/adtzlr/matadi) installed - run `pip install matadi` in your terminal.
+
+```python
+mooney_rivlin = hel.models.invariants.ThirdOrderDeformation(C10=0.3, C01=0.2)
+framework = hel.frameworks.InvariantsFramework(mooney_rivlin)
+umat = hel.spaces.DistortionalSpace(framework)
+
+import matadi
+
+lab = matadi.LabIncompressible(umat, title="Mooney Rivlin")
+data = lab.run(
+    ux=True,
+    bx=True,
+    ps=True,
+    stretch_min=0.7,
+    stretch_max=2.5,
+)
+fig, ax = lab.plot(data, stability=True)
+```
+
+![lab_mooney-rivlin](https://github.com/adtzlr/hyperelastic/assets/5793153/1b21df81-e0fd-4ea1-9bd7-24d4d70ba801)
+
 # License
 Hyperelastic - Constitutive hyperelastic material formulations for FElupe (C) 2023 Andreas Dutzler, Graz (Austria).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `hyperelastic-0.1.1/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.2.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.1/tests/test_space.py` & `hyperelastic-0.2.0/tests/test_space.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     )
     job = fem.Job(steps=[step])
 
     return job
 
 
 def test_distortional_stretches():
-    model = hel.models.stretches.Ogden(mu=1, alpha=0.436)
+    model = hel.models.stretches.Ogden(mu=[1], alpha=[0.436])
     umat = hel.spaces.DistortionalSpace(hel.frameworks.StretchesFramework(model))
     fea(umat).evaluate(verbose=2)
 
 
 def test_distortional_invariants():
     model = hel.models.invariants.ThirdOrderDeformation(
         C10=0.4, C01=0.1, C11=0.02, C20=-0.05, C30=0.01
```

### Comparing `hyperelastic-0.1.1/tests/test_sympy.py` & `hyperelastic-0.2.0/tests/test_sympy.py`

 * *Files identical despite different names*

