# Comparing `tmp/numgrids-0.2.3.tar.gz` & `tmp/numgrids-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numgrids-0.2.3.tar", last modified: Sat Jul  1 06:29:16 2023, max compression
+gzip compressed data, was "numgrids-0.2.4.tar", last modified: Tue Jul  4 14:43:10 2023, max compression
```

## Comparing `numgrids-0.2.3.tar` & `numgrids-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-01 06:29:16.497814 numgrids-0.2.3/
--rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-06-30 04:56:35.000000 numgrids-0.2.3/LICENSE
--rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-01 06:29:16.497354 numgrids-0.2.3/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     3381 2023-07-01 06:16:40.000000 numgrids-0.2.3/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-01 06:29:16.495217 numgrids-0.2.3/numgrids/
--rw-r--r--   0 mbaer    (671849960) 579947404      146 2023-07-01 06:15:06.000000 numgrids-0.2.3/numgrids/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4402 2023-07-01 06:16:12.000000 numgrids-0.2.3/numgrids/api.py
--rw-r--r--   0 mbaer    (671849960) 579947404     7127 2023-06-30 13:37:54.000000 numgrids-0.2.3/numgrids/axes.py
--rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.2.3/numgrids/diff.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1929 2023-06-30 13:36:37.000000 numgrids-0.2.3/numgrids/grids.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-06-30 04:55:14.000000 numgrids-0.2.3/numgrids/integration.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1294 2023-07-01 06:03:13.000000 numgrids-0.2.3/numgrids/interpol.py
--rw-r--r--   0 mbaer    (671849960) 579947404      163 2023-06-30 06:18:32.000000 numgrids-0.2.3/numgrids/utils.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-01 06:29:16.496789 numgrids-0.2.3/numgrids.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-01 06:29:16.000000 numgrids-0.2.3/numgrids.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      337 2023-07-01 06:29:16.000000 numgrids-0.2.3/numgrids.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-01 06:29:16.000000 numgrids-0.2.3/numgrids.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       39 2023-07-01 06:29:16.000000 numgrids-0.2.3/numgrids.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-07-01 06:29:16.000000 numgrids-0.2.3/numgrids.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-07-01 06:29:16.497936 numgrids-0.2.3/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404      998 2023-07-01 06:29:11.000000 numgrids-0.2.3/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-04 14:43:10.157045 numgrids-0.2.4/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-07-03 11:28:15.000000 numgrids-0.2.4/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-04 14:43:10.156410 numgrids-0.2.4/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     4203 2023-07-01 06:53:26.000000 numgrids-0.2.4/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-04 14:43:10.152349 numgrids-0.2.4/numgrids/
+-rw-r--r--   0 mbaer    (671849960) 579947404      169 2023-07-04 14:37:32.000000 numgrids-0.2.4/numgrids/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4402 2023-07-03 12:45:13.000000 numgrids-0.2.4/numgrids/api.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     7127 2023-06-30 13:37:54.000000 numgrids-0.2.4/numgrids/axes.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.2.4/numgrids/diff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4311 2023-07-04 14:37:13.000000 numgrids-0.2.4/numgrids/grids.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-07-04 14:37:13.000000 numgrids-0.2.4/numgrids/integration.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     2001 2023-07-03 11:10:56.000000 numgrids-0.2.4/numgrids/interpol.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      957 2023-07-04 14:37:13.000000 numgrids-0.2.4/numgrids/plots.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      163 2023-06-30 06:18:32.000000 numgrids-0.2.4/numgrids/utils.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-04 14:43:10.155679 numgrids-0.2.4/numgrids.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      355 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       39 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-07-04 14:43:10.157191 numgrids-0.2.4/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404     1282 2023-07-04 14:42:04.000000 numgrids-0.2.4/setup.py
```

### Comparing `numgrids-0.2.3/LICENSE` & `numgrids-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.3/PKG-INFO` & `numgrids-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numgrids
-Version: 0.2.3
+Version: 0.2.4
 Summary: Working with numerical grids made easy.
 Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Platform: ALL
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: numgrids Version: 0.2.3 Summary: Working with
+Metadata-Version: 2.1 Name: numgrids Version: 0.2.4 Summary: Working with
 numerical grids made easy. Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer Author-email: matthias.r.baer@googlemail.com License: MIT
 Platform: ALL Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
                             ****** numgrids ******
                     Working with numerical grids made easy.
```

### Comparing `numgrids-0.2.3/README.md` & `numgrids-0.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">numgrids</h1>
 <p align="center"> Working with numerical grids made easy.</p>
 
-<p align="center"><a href="https://badge.fury.io/py/numgrids"> <img src="https://badge.fury.io/py/numgrids.svg" alt="PyPI version"></a><a href=""> <img src="https://github.com/maroba/numgrids/actions/workflows/checks.yml/badge.svg" alt="build"></a><a href="https://codecov.io/gh/maroba/numgrids"> <img src="https://codecov.io/gh/maroba/numgrids/branch/main/graph/badge.svg?token=JNH9SP7BRG" alt=""></a></p>
+<p align="center"><a href="https://badge.fury.io/py/numgrids"> <img src="https://badge.fury.io/py/numgrids.svg?branch=main&kill_cache=1" alt="PyPI version"></a> <a href=""> <img src="https://github.com/maroba/numgrids/actions/workflows/checks.yml/badge.svg" alt="build"></a><a href="https://codecov.io/gh/maroba/numgrids"> <img src="https://codecov.io/gh/maroba/numgrids/branch/main/graph/badge.svg?token=JNH9SP7BRG" alt=""></a></p>
 
   <div align="center"><img src="docs/assets/torus.png" width="25%">  <img src="docs/assets/disk320.png" width="25%"> <img src="docs/assets/cubic.png" width="25%"></div>
 
 **Main Features**
 
 - Quickly define numerical grids for any rectangular or curvilinear coordinate system
 - Differentiation and integration
@@ -38,51 +38,51 @@
 
 ```python
 axis_radial = Axis(AxisType.CHEBYSHEV, 20, 0, 1)
 ```
 
 <img src="docs/assets/cheby.png" height="91">
 
-Now combine the axes to a grid:
+Now combine the axes to a **grid**:
 
 ```python
 grid = Grid(axis_radial, axis_phi)
 ```
 <img src="docs/assets/disk320.png">
 
-Sample a meshed function on this grid:
+**Sample** a meshed function on this grid:
 
 ```python
 from numpy import exp, sin
 
 R, Phi = grid.meshed_coords
 f = R**2 * sin(Phi)**2
 ```
-Define partial derivatives $\partial/\partial r$ and $\partial/\partial \varphi$ and apply them:
+Define **partial derivatives** $\partial/\partial r$ and $\partial/\partial \varphi$ and apply them:
 
 ```python
 # second argument means derivative order, third argument means axis index:
 d_dr = Diff(grid, 1, 0) 
 d_dphi = Diff(grid, 1, 1)
 
 df_dr = d_dr(f)
 df_dphi = d_dphi(f)
 ```
 
-Obtain the matrix representation of the differential operators:
+Obtain the **matrix representation** of the differential operators:
 
 ```python
 d_dr.as_matrix()
 
 Out: <1000x1000 sparse matrix of type '<class 'numpy.float64'>'
 	with 20000 stored elements in COOrdinate format>
 ```
 
 
-Define integration operator
+Define **integration operator**
 
 $$
 \int \dots dr d\varphi
 $$
 
 ```python
 I = Integral(grid)
@@ -96,28 +96,82 @@
 
 (taking into account the appropriate integration measure  $r$  for polar coordinates):
 
 ```python
 I(f * R)
 ```
 
-Setting boundary values to zero
+Setting **boundary** values to zero
 
 ```python
 f[grid.boundary] = 0  # grid.boundary is boolean mask selecting boundary grid points
 ```
 
 or to something more complicated:
 
 ```python
 f[grid.boundary] = exp(-R[grid.boundary])
 ```
 
+Create an **interpolation function**
+
+```python
+inter = Interpolator(grid, f)
+```
+
+Interpolate for a single point
+
+```python
+point = (0.1, 0.5)
+inter(point)
+```
+
+or for many points at once, like for a parametrized curve:
+
+```python
+t = np.linspace(0, 1, 100)
+points = zip(2*t, t**2)
+inter(points)
+```
+
+
 ## Usage / Example Notebooks
 
 To get an idea how *numgrids* can be used, have a look at the following example notebooks:
 
 - [How to define grids](examples/how-to-define-grids.ipynb)
 - [Partial derivatives in any dimension](examples/partial-derivatives.ipynb)
 - [Polar coordinates on unit disk](examples/polar-cooordinates-on-unit-disk.ipynb)
 - [Spherical Grid and the Spherical Laplacian](examples/spherical-grid.ipynb)
 - [Solving the Schrödinger equation for the quantum harmonic oscillator](examples/quantum-harmonic-oscillator.ipynb)
+
+## Development
+
+### Setting up the project
+
+Clone the repository
+
+```
+git clone https://github.com/maroba/numgrids.git
+```
+
+In the project root directory, submit
+
+```
+python setup.py develop
+```
+
+to install the package in development mode.
+
+Run the tests:
+
+```
+python -m unittest discover tests
+```
+
+### Contributing
+
+1. Fork the repository
+2. Develop
+3. Write tests!
+4. Create an [issue](https://github.com/maroba/numgrids/issues)
+5. Create a pull request, when done
```

#### html2text {}

```diff
@@ -1,39 +1,50 @@
                             ****** numgrids ******
                     Working with numerical grids made easy.
-                             [PyPI_version][build]
+                            [PyPI_version] [build]
    [docs/assets/torus.png] [docs/assets/disk320.png] [docs/assets/cubic.png]
 **Main Features** - Quickly define numerical grids for any rectangular or
 curvilinear coordinate system - Differentiation and integration - Interpolation
 - Easy manipulation of meshed functions - Using high precision spectral methods
 (FFT + Chebyshev) wherever possible - Fully compatible with *numpy* ##
 Installation ```shell pip install numgrids ``` ## Quick Start As a quick
 example, here is how you define a grid on the unit disk using polar
 coordinates. Along the azimuthal (angular) direction, choose an equidistant
 spacing with periodic boundary conditions: ```python from numgrids import *
 from numpy import pi axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi,
 periodic=True) ``` [docs/assets/equi_periodic.png] Along the radial axis, let's
 choose a non-equidistant spacing: ```python axis_radial = Axis
 (AxisType.CHEBYSHEV, 20, 0, 1) ``` [docs/assets/cheby.png] Now combine the axes
-to a grid: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/assets/
-disk320.png] Sample a meshed function on this grid: ```python from numpy import
-exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ``` Define partial
-derivatives $\partial/\partial r$ and $\partial/\partial \varphi$ and apply
-them: ```python # second argument means derivative order, third argument means
-axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1, 1) df_dr = d_dr(f)
-df_dphi = d_dphi(f) ``` Obtain the matrix representation of the differential
-operators: ```python d_dr.as_matrix() Out: <1000x1000 sparse matrix of type '
+to a **grid**: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/assets/
+disk320.png] **Sample** a meshed function on this grid: ```python from numpy
+import exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ``` Define
+**partial derivatives** $\partial/\partial r$ and $\partial/\partial \varphi$
+and apply them: ```python # second argument means derivative order, third
+argument means axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1, 1)
+df_dr = d_dr(f) df_dphi = d_dphi(f) ``` Obtain the **matrix representation** of
+the differential operators: ```python d_dr.as_matrix() Out: <1000x1000 sparse
+matrix of type '
 numpy.float64'>' with 20000 stored elements in COOrdinate format> ``` Define
-integration operator $$ \int \dots dr d\varphi $$ ```python I = Integral(grid)
-``` Calculate the area integral $$ \int f(r, \varphi) r dr d\varphi $$ (taking
-into account the appropriate integration measure $r$ for polar coordinates):
-```python I(f * R) ``` Setting boundary values to zero ```python f
-[grid.boundary] = 0 # grid.boundary is boolean mask selecting boundary grid
-points ``` or to something more complicated: ```python f[grid.boundary] = exp(-
-R[grid.boundary]) ``` ## Usage / Example Notebooks To get an idea how
-*numgrids* can be used, have a look at the following example notebooks: - [How
-to define grids](examples/how-to-define-grids.ipynb) - [Partial derivatives in
-any dimension](examples/partial-derivatives.ipynb) - [Polar coordinates on unit
-disk](examples/polar-cooordinates-on-unit-disk.ipynb) - [Spherical Grid and the
-Spherical Laplacian](examples/spherical-grid.ipynb) - [Solving the SchrÃ¶dinger
-equation for the quantum harmonic oscillator](examples/quantum-harmonic-
-oscillator.ipynb)
+**integration operator** $$ \int \dots dr d\varphi $$ ```python I = Integral
+(grid) ``` Calculate the area integral $$ \int f(r, \varphi) r dr d\varphi $$
+(taking into account the appropriate integration measure $r$ for polar
+coordinates): ```python I(f * R) ``` Setting **boundary** values to zero
+```python f[grid.boundary] = 0 # grid.boundary is boolean mask selecting
+boundary grid points ``` or to something more complicated: ```python f
+[grid.boundary] = exp(-R[grid.boundary]) ``` Create an **interpolation
+function** ```python inter = Interpolator(grid, f) ``` Interpolate for a single
+point ```python point = (0.1, 0.5) inter(point) ``` or for many points at once,
+like for a parametrized curve: ```python t = np.linspace(0, 1, 100) points =
+zip(2*t, t**2) inter(points) ``` ## Usage / Example Notebooks To get an idea
+how *numgrids* can be used, have a look at the following example notebooks: -
+[How to define grids](examples/how-to-define-grids.ipynb) - [Partial
+derivatives in any dimension](examples/partial-derivatives.ipynb) - [Polar
+coordinates on unit disk](examples/polar-cooordinates-on-unit-disk.ipynb) -
+[Spherical Grid and the Spherical Laplacian](examples/spherical-grid.ipynb) -
+[Solving the SchrÃ¶dinger equation for the quantum harmonic oscillator]
+(examples/quantum-harmonic-oscillator.ipynb) ## Development ### Setting up the
+project Clone the repository ``` git clone https://github.com/maroba/
+numgrids.git ``` In the project root directory, submit ``` python setup.py
+develop ``` to install the package in development mode. Run the tests: ```
+python -m unittest discover tests ``` ### Contributing 1. Fork the repository
+2. Develop 3. Write tests! 4. Create an [issue](https://github.com/maroba/
+numgrids/issues) 5. Create a pull request, when done
```

### Comparing `numgrids-0.2.3/numgrids/api.py` & `numgrids-0.2.4/numgrids/api.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.3/numgrids/axes.py` & `numgrids-0.2.4/numgrids/axes.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.3/numgrids/diff.py` & `numgrids-0.2.4/numgrids/diff.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.3/numgrids/integration.py` & `numgrids-0.2.4/numgrids/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from numgrids.axes import EquidistantAxis
 from numgrids.utils import multi_kron
 
 
 class Integral:
     """
-    The integration operotor for integrating on a grid.
+    The integration operator for integrating on a grid.
 
         .. math::
             \int_V ... dV
 
     Integration always runs over the whole grid.
     """
```

### Comparing `numgrids-0.2.3/numgrids.egg-info/PKG-INFO` & `numgrids-0.2.4/numgrids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numgrids
-Version: 0.2.3
+Version: 0.2.4
 Summary: Working with numerical grids made easy.
 Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Platform: ALL
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: numgrids Version: 0.2.3 Summary: Working with
+Metadata-Version: 2.1 Name: numgrids Version: 0.2.4 Summary: Working with
 numerical grids made easy. Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer Author-email: matthias.r.baer@googlemail.com License: MIT
 Platform: ALL Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
                             ****** numgrids ******
                     Working with numerical grids made easy.
```

### Comparing `numgrids-0.2.3/setup.py` & `numgrids-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+import os.path
+import re
 from os.path import exists
 from setuptools import setup, find_packages
 
 author = 'Matthias Baer'
 email = 'matthias.r.baer@googlemail.com'
 description = 'Working with numerical grids made easy.'
 name = 'numgrids'
 year = '2023'
 url = 'https://github.com/maroba/numgrids'
-version = '0.2.3'
+
+with open(os.path.join('numgrids', '__init__.py'), 'r') as fh:
+    match = re.match('__version__ *= *"([^"]+)"', fh.readline())
+    if match:
+        version = match.group(1)
+    else:
+        raise ValueError('numgrids.__init__.py must define version string as first line.')
 
 setup(
     name=name,
     author=author,
     author_email=email,
     url=url,
     version=version,
```

