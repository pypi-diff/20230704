# Comparing `tmp/hyperelastic-0.2.0.tar.gz` & `tmp/hyperelastic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.2.0.tar", last modified: Mon Jul  3 23:09:31 2023, max compression
+gzip compressed data, was "hyperelastic-0.3.0.tar", last modified: Tue Jul  4 09:06:04 2023, max compression
```

## Comparing `hyperelastic-0.2.0.tar` & `hyperelastic-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50086 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.811092 hyperelastic-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.811092 hyperelastic-0.2.0/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50086 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 23:09:31.000000 hyperelastic-0.2.0/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:09:31.815092 hyperelastic-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-03 23:09:22.000000 hyperelastic-0.2.0/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50329 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.795304 hyperelastic-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.799304 hyperelastic-0.3.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.799304 hyperelastic-0.3.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50329 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.2.0/LICENSE` & `hyperelastic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.2.0/PKG-INFO` & `hyperelastic-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.2.0
+Version: 0.3.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -708,17 +708,17 @@
   <p align="center">Constitutive <b>hyperelastic</b> material formulations for <a href="https://github.com/adtzlr/felupe">FElupe</a>.</p>
 </p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
 This package provides the essential building blocks for constitutive hyperelastic material formulations. This includes material behaviour-independent spaces and frameworks as well as material behaviour-dependent model formulations.
 
-**Spaces** are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
+**Spaces** ([`hyperelastic.spaces`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/spaces)) are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** ([`hyperelastic.frameworks`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/frameworks)) for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
 
-The math-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
+The [`hyperelastic.math`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/math)-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
 
 $$ \boldsymbol{C} = \begin{bmatrix} C_{11} & C_{22} & C_{33} & C_{12} & C_{23} & C_{13} \end{bmatrix}^T $$
 
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
@@ -770,16 +770,16 @@
         d2WdI2I3 = None
         d2WdI1I3 = None
 
         return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
 
 
 model = MyInvariantsModel()
-framework = hel.frameworks.InvariantsFramework(model)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.InvariantsFramework(model)
+umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
@@ -810,28 +810,28 @@
         d2Wdλ2dλ3 = None
         d2Wdλ1dλ3 = None
 
         return d2Wdλ1dλ1, d2Wdλ2dλ2, d2Wdλ3dλ3, d2Wdλ1dλ2, d2Wdλ2dλ3, d2Wdλ1dλ3
 
 
 model = MyStretchesModel()
-framework = hel.frameworks.StretchesFramework(model)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.StretchesFramework(model)
+umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic stretch-based material formulations
 - [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/stretches/_ogden.py))
 
 ## Lab
 By using [matadi](https://github.com/adtzlr/matadi)'s `LabIncompressible`, numeric experiments on homogeneous incompressible loadcases on hyperelastic material formulations are performed. Ensure to have [matadi](https://github.com/adtzlr/matadi) installed - run `pip install matadi` in your terminal.
 
 ```python
 mooney_rivlin = hel.models.invariants.ThirdOrderDeformation(C10=0.3, C01=0.2)
-framework = hel.frameworks.InvariantsFramework(mooney_rivlin)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.InvariantsFramework(mooney_rivlin)
+umat = hel.DistortionalSpace(framework)
 
 import matadi
 
 lab = matadi.LabIncompressible(umat, title="Mooney Rivlin")
 data = lab.run(
     ux=True,
     bx=True,
```

### Comparing `hyperelastic-0.2.0/README.md` & `hyperelastic-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
   <p align="center">Constitutive <b>hyperelastic</b> material formulations for <a href="https://github.com/adtzlr/felupe">FElupe</a>.</p>
 </p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
 This package provides the essential building blocks for constitutive hyperelastic material formulations. This includes material behaviour-independent spaces and frameworks as well as material behaviour-dependent model formulations.
 
-**Spaces** are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
+**Spaces** ([`hyperelastic.spaces`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/spaces)) are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** ([`hyperelastic.frameworks`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/frameworks)) for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
 
-The math-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
+The [`hyperelastic.math`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/math)-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
 
 $$ \boldsymbol{C} = \begin{bmatrix} C_{11} & C_{22} & C_{33} & C_{12} & C_{23} & C_{13} \end{bmatrix}^T $$
 
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
@@ -65,16 +65,16 @@
         d2WdI2I3 = None
         d2WdI1I3 = None
 
         return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
 
 
 model = MyInvariantsModel()
-framework = hel.frameworks.InvariantsFramework(model)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.InvariantsFramework(model)
+umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
@@ -105,28 +105,28 @@
         d2Wdλ2dλ3 = None
         d2Wdλ1dλ3 = None
 
         return d2Wdλ1dλ1, d2Wdλ2dλ2, d2Wdλ3dλ3, d2Wdλ1dλ2, d2Wdλ2dλ3, d2Wdλ1dλ3
 
 
 model = MyStretchesModel()
-framework = hel.frameworks.StretchesFramework(model)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.StretchesFramework(model)
+umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic stretch-based material formulations
 - [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/stretches/_ogden.py))
 
 ## Lab
 By using [matadi](https://github.com/adtzlr/matadi)'s `LabIncompressible`, numeric experiments on homogeneous incompressible loadcases on hyperelastic material formulations are performed. Ensure to have [matadi](https://github.com/adtzlr/matadi) installed - run `pip install matadi` in your terminal.
 
 ```python
 mooney_rivlin = hel.models.invariants.ThirdOrderDeformation(C10=0.3, C01=0.2)
-framework = hel.frameworks.InvariantsFramework(mooney_rivlin)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.InvariantsFramework(mooney_rivlin)
+umat = hel.DistortionalSpace(framework)
 
 import matadi
 
 lab = matadi.LabIncompressible(umat, title="Mooney Rivlin")
 data = lab.run(
     ux=True,
     bx=True,
```

### Comparing `hyperelastic-0.2.0/pyproject.toml` & `hyperelastic-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.2.0/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.3.0/src/hyperelastic/frameworks/_invariants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from ..math import cdya, ddot, det, dya, eye, inv, trace
 
 
-class InvariantsFramework:
+class Invariants:
     r"""The Framework for a Total-Lagrangian invariant-based isotropic hyperelastic
     material formulation provides the material behaviour-independent parts for
     evaluating the second Piola-Kirchhoff stress tensor as well as its associated
     fourth-order elasticity tensor.
 
     The gradient as well as the hessian of the strain energy function are carried out
     w.r.t. the right Cauchy-Green deformation tensor. Hence, the work-conjugate stress
```

### Comparing `hyperelastic-0.2.0/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.3.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from ..math import cdya, dya, eigh, transpose
 
 
-class StretchesFramework:
+class Stretches:
     r"""The Framework for a Total-Lagrangian stretch-based isotropic hyperelastic
     material formulation provides the material behaviour-independent parts for
     evaluating the second Piola-Kirchhoff stress tensor as well as its associated
     fourth-order elasticity tensor.
 
     The gradient as well as the hessian of the strain energy function are carried out
     w.r.t. the right Cauchy-Green deformation tensor. Hence, the work-conjugate stress
```

### Comparing `hyperelastic-0.2.0/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.3.0/src/hyperelastic/math/_voigt.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.2.0/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.3.0/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.2.0/src/hyperelastic/models/stretches/_ogden.py` & `hyperelastic-0.3.0/src/hyperelastic/models/stretches/_ogden.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.2.0/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.3.0/src/hyperelastic/spaces/_deformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya_ik, eye
 
 
-class DeformationSpace:
+class Deformation:
     r"""The deformation space.
 
     This class takes a Total-Lagrange material formulation and applies it on the
     deformation space.
 
     ..  math::
```

### Comparing `hyperelastic-0.2.0/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.3.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya, cdya_ik, ddot, det, dya, eye, inv, trace
 
 
-class DilatationalSpace:
+class Dilatational:
     def __init__(self, material, parallel=False):
         self.parallel = parallel
         self.material = material
 
         if self.parallel:
             from einsumt import einsumt
```

### Comparing `hyperelastic-0.2.0/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.3.0/src/hyperelastic/spaces/_distortional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya, cdya_ik, ddot, det, dya, eye, inv, transpose
 
 
-class DistortionalSpace:
+class Distortional:
     r"""The distortional (part of the deformation) space is a partial deformation with
     constant volume. For a given deformation map :math:`x(X)` and its deformation
     gradient :math:`\boldsymbol{F}`, the distortional part of the deformation gradient
     :math:`\hat{\boldsymbol{F}}` is obtained by a multiplicative (consecutive) split
     into a volume-changing (dilatational) and a constant-volume (distortional) part of
     the deformation gradient. Due to the fact that the dilatational part is proportional
     to the unit tensor, the order of these partial deformations is not unique.
```

### Comparing `hyperelastic-0.2.0/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.3.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.2.0
+Version: 0.3.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -708,17 +708,17 @@
   <p align="center">Constitutive <b>hyperelastic</b> material formulations for <a href="https://github.com/adtzlr/felupe">FElupe</a>.</p>
 </p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
 
 This package provides the essential building blocks for constitutive hyperelastic material formulations. This includes material behaviour-independent spaces and frameworks as well as material behaviour-dependent model formulations.
 
-**Spaces** are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
+**Spaces** ([`hyperelastic.spaces`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/spaces)) are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** ([`hyperelastic.frameworks`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/frameworks)) for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
 
-The math-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
+The [`hyperelastic.math`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/math)-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
 
 $$ \boldsymbol{C} = \begin{bmatrix} C_{11} & C_{22} & C_{33} & C_{12} & C_{23} & C_{13} \end{bmatrix}^T $$
 
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
@@ -770,16 +770,16 @@
         d2WdI2I3 = None
         d2WdI1I3 = None
 
         return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
 
 
 model = MyInvariantsModel()
-framework = hel.frameworks.InvariantsFramework(model)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.InvariantsFramework(model)
+umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
@@ -810,28 +810,28 @@
         d2Wdλ2dλ3 = None
         d2Wdλ1dλ3 = None
 
         return d2Wdλ1dλ1, d2Wdλ2dλ2, d2Wdλ3dλ3, d2Wdλ1dλ2, d2Wdλ2dλ3, d2Wdλ1dλ3
 
 
 model = MyStretchesModel()
-framework = hel.frameworks.StretchesFramework(model)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.StretchesFramework(model)
+umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic stretch-based material formulations
 - [Ogden](https://en.wikipedia.org/wiki/Ogden_(hyperelastic_model)) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/stretches/_ogden.py))
 
 ## Lab
 By using [matadi](https://github.com/adtzlr/matadi)'s `LabIncompressible`, numeric experiments on homogeneous incompressible loadcases on hyperelastic material formulations are performed. Ensure to have [matadi](https://github.com/adtzlr/matadi) installed - run `pip install matadi` in your terminal.
 
 ```python
 mooney_rivlin = hel.models.invariants.ThirdOrderDeformation(C10=0.3, C01=0.2)
-framework = hel.frameworks.InvariantsFramework(mooney_rivlin)
-umat = hel.spaces.DistortionalSpace(framework)
+framework = hel.InvariantsFramework(mooney_rivlin)
+umat = hel.DistortionalSpace(framework)
 
 import matadi
 
 lab = matadi.LabIncompressible(umat, title="Mooney Rivlin")
 data = lab.run(
     ux=True,
     bx=True,
```

### Comparing `hyperelastic-0.2.0/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.3.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.2.0/tests/test_sympy.py` & `hyperelastic-0.3.0/tests/test_sympy.py`

 * *Files 26% similar despite different names*

```diff
@@ -40,39 +40,43 @@
         self.d2Wdydy = sym.lambdify(
             [self.x, self.y, self.z], self.W.diff(self.y, self.y)
         )
         self.d2Wdzdz = sym.lambdify(
             [self.x, self.y, self.z], self.W.diff(self.z, self.z)
         )
 
-        self.d2Wdxdy = lambda x, y, z: np.zeros_like(x)
-        self.d2Wdydz = lambda x, y, z: np.zeros_like(x)
-        self.d2Wdxdz = lambda x, y, z: np.zeros_like(x)
+        self.d2Wdxdy = sym.lambdify(
+            [self.x, self.y, self.z], self.W.diff(self.x, self.y)
+        )
+        self.d2Wdydz = sym.lambdify(
+            [self.x, self.y, self.z], self.W.diff(self.y, self.z)
+        )
+        self.d2Wdxdz = sym.lambdify(
+            [self.x, self.y, self.z], self.W.diff(self.x, self.z)
+        )
 
     def gradient(self, stretches, statevars):
         return [
             self.dWdx(*stretches),
             self.dWdy(*stretches),
             self.dWdz(*stretches),
         ], statevars
 
     def hessian(self, stretches, statevars):
-        return np.array(
-            [
-                self.d2Wdxdx(*stretches),
-                self.d2Wdydy(*stretches),
-                self.d2Wdzdz(*stretches),
-                self.d2Wdxdy(*stretches),
-                self.d2Wdydz(*stretches),
-                self.d2Wdxdz(*stretches),
-            ]
-        )
+        return [
+            self.d2Wdxdx(*stretches),
+            self.d2Wdydy(*stretches),
+            self.d2Wdzdz(*stretches),
+            self.d2Wdxdy(*stretches),
+            self.d2Wdydz(*stretches),
+            self.d2Wdxdz(*stretches),
+        ]
 
 
 def test_distortional_stretches_sympy():
     model = SymbolicMaterialFormulation(ogden, mu=1, alpha=0.436)
-    umat = hel.spaces.DistortionalSpace(hel.frameworks.StretchesFramework(model))
+    umat = hel.DistortionalSpace(hel.StretchesFramework(model))
     fea(umat).evaluate(verbose=2)
 
 
 if __name__ == "__main__":
     test_distortional_stretches_sympy()
```

