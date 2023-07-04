# Comparing `tmp/SPLayout-0.4.8.tar.gz` & `tmp/SPLayout-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPLayout-0.4.8.tar", last modified: Tue Jun 20 11:36:18 2023, max compression
+gzip compressed data, was "SPLayout-0.4.9.tar", last modified: Tue Jul  4 01:34:46 2023, max compression
```

## Comparing `SPLayout-0.4.8.tar` & `SPLayout-0.4.9.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.115325 SPLayout-0.4.8/
--rw-rw-rw-   0        0        0    35803 2023-06-20 10:20:16.000000 SPLayout-0.4.8/LICENSE
--rw-rw-rw-   0        0        0     1719 2023-06-20 11:36:18.115325 SPLayout-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     1473 2023-06-20 10:20:16.000000 SPLayout-0.4.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.084071 SPLayout-0.4.8/SPLayout.egg-info/
--rw-rw-rw-   0        0        0     1719 2023-06-20 11:36:17.000000 SPLayout-0.4.8/SPLayout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1489 2023-06-20 11:36:18.000000 SPLayout-0.4.8/SPLayout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:36:17.000000 SPLayout-0.4.8/SPLayout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 11:36:17.000000 SPLayout-0.4.8/SPLayout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 11:36:17.000000 SPLayout-0.4.8/SPLayout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 11:36:18.115325 SPLayout-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-06-20 10:20:16.000000 SPLayout-0.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.084071 SPLayout-0.4.8/splayout/
--rw-rw-rw-   0        0        0     1987 2023-06-20 11:31:12.000000 SPLayout-0.4.8/splayout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.099697 SPLayout-0.4.8/splayout/adjointmethod/
--rw-rw-rw-   0        0        0      293 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/__init__.py
--rw-rw-rw-   0        0        0    10984 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/adjointshapeopt.py
--rw-rw-rw-   0        0        0    10645 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/adjointtopologyopt.py
--rw-rw-rw-   0        0        0    10586 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/shaperegion2d.py
--rw-rw-rw-   0        0        0    10652 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/shaperegion3d.py
--rw-rw-rw-   0        0        0    11374 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/topologyregion2d.py
--rw-rw-rw-   0        0        0    11304 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/adjointmethod/topologyregion3d.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.099697 SPLayout-0.4.8/splayout/algorithms/
--rw-rw-rw-   0        0        0      312 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5781 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/algorithms/binarybatalgorithm.py
--rw-rw-rw-   0        0        0     6360 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/algorithms/binarygeneticalgorithm.py
--rw-rw-rw-   0        0        0     5831 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-rw-rw-   0        0        0     4305 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/algorithms/directbinarysearchalgorithm.py
--rw-rw-rw-   0        0        0     7326 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/algorithms/particleswarmalgorithm.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.115325 SPLayout-0.4.8/splayout/components/
--rw-rw-rw-   0        0        0     3728 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/AEMDgrating.py
--rw-rw-rw-   0        0        0      714 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/__init__.py
--rw-rw-rw-   0        0        0     4403 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/bend.py
--rw-rw-rw-   0        0        0     9026 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/doubleconnector.py
--rw-rw-rw-   0        0        0     6092 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/filledpattern.py
--rw-rw-rw-   0        0        0    49359 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/microring.py
--rw-rw-rw-   0        0        0    21403 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/pixelsregion.py
--rw-rw-rw-   0        0        0     7433 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/polygon.py
--rw-rw-rw-   0        0        0    14219 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/quarbend.py
--rw-rw-rw-   0        0        0    18098 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/sbend.py
--rw-rw-rw-   0        0        0    13136 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/selfdefinecomponent.py
--rw-rw-rw-   0        0        0    28052 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-rw-rw-   0        0        0     7270 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/slowlyvaryingtaper.py
--rw-rw-rw-   0        0        0     6668 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/taper.py
--rw-rw-rw-   0        0        0     1269 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/text.py
--rw-rw-rw-   0        0        0     8908 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/components/waveguide.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.115325 SPLayout-0.4.8/splayout/lumericalcommun/
--rw-rw-rw-   0        0        0       72 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/lumericalcommun/__init__.py
--rw-rw-rw-   0        0        0    78118 2023-06-20 11:33:12.000000 SPLayout-0.4.8/splayout/lumericalcommun/fdtdapi.py
--rw-rw-rw-   0        0        0    44213 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/lumericalcommun/modeapi.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:36:18.115325 SPLayout-0.4.8/splayout/utils/
--rw-rw-rw-   0        0        0       20 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/utils/__init__.py
--rw-rw-rw-   0        0        0    14788 2023-06-20 10:20:16.000000 SPLayout-0.4.8/splayout/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.863259 SPLayout-0.4.9/
+-rw-rw-rw-   0        0        0    35803 2023-06-20 10:20:16.000000 SPLayout-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0     1719 2023-07-04 01:34:46.862264 SPLayout-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2023-06-20 10:20:16.000000 SPLayout-0.4.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.507701 SPLayout-0.4.9/SPLayout.egg-info/
+-rw-rw-rw-   0        0        0     1719 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1578 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 01:34:46.863259 SPLayout-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-06-20 10:20:16.000000 SPLayout-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.508717 SPLayout-0.4.9/splayout/
+-rw-rw-rw-   0        0        0     2120 2023-07-04 01:26:34.000000 SPLayout-0.4.9/splayout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.583254 SPLayout-0.4.9/splayout/adjointmethod/
+-rw-rw-rw-   0        0        0      398 2023-07-03 08:15:18.000000 SPLayout-0.4.9/splayout/adjointmethod/__init__.py
+-rw-rw-rw-   0        0        0    13624 2023-07-04 01:33:39.000000 SPLayout-0.4.9/splayout/adjointmethod/adjointmultitoopt.py
+-rw-rw-rw-   0        0        0    10984 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/adjointshapeopt.py
+-rw-rw-rw-   0        0        0    11728 2023-07-03 09:59:25.000000 SPLayout-0.4.9/splayout/adjointmethod/adjointtopologyopt.py
+-rw-rw-rw-   0        0        0    15991 2023-07-04 00:55:42.000000 SPLayout-0.4.9/splayout/adjointmethod/scalabletotegion3d.py
+-rw-rw-rw-   0        0        0    10586 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/shaperegion2d.py
+-rw-rw-rw-   0        0        0    10652 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/shaperegion3d.py
+-rw-rw-rw-   0        0        0    11374 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/topologyregion2d.py
+-rw-rw-rw-   0        0        0    11304 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/topologyregion3d.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.642426 SPLayout-0.4.9/splayout/algorithms/
+-rw-rw-rw-   0        0        0      312 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5781 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/binarybatalgorithm.py
+-rw-rw-rw-   0        0        0     6360 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/binarygeneticalgorithm.py
+-rw-rw-rw-   0        0        0     5831 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-rw-rw-   0        0        0     4305 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-rw-rw-   0        0        0     7326 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/particleswarmalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.802861 SPLayout-0.4.9/splayout/components/
+-rw-rw-rw-   0        0        0     3728 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/AEMDgrating.py
+-rw-rw-rw-   0        0        0      714 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/__init__.py
+-rw-rw-rw-   0        0        0     4403 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/bend.py
+-rw-rw-rw-   0        0        0     9026 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/doubleconnector.py
+-rw-rw-rw-   0        0        0     6092 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/filledpattern.py
+-rw-rw-rw-   0        0        0    49359 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/microring.py
+-rw-rw-rw-   0        0        0    21403 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/pixelsregion.py
+-rw-rw-rw-   0        0        0     7433 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/polygon.py
+-rw-rw-rw-   0        0        0    14219 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/quarbend.py
+-rw-rw-rw-   0        0        0    18098 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/sbend.py
+-rw-rw-rw-   0        0        0    13136 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/selfdefinecomponent.py
+-rw-rw-rw-   0        0        0    28052 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-rw-rw-   0        0        0     7270 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/slowlyvaryingtaper.py
+-rw-rw-rw-   0        0        0     6668 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/taper.py
+-rw-rw-rw-   0        0        0     1269 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/text.py
+-rw-rw-rw-   0        0        0     8908 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/waveguide.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.841989 SPLayout-0.4.9/splayout/lumericalcommun/
+-rw-rw-rw-   0        0        0       72 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/lumericalcommun/__init__.py
+-rw-rw-rw-   0        0        0    78118 2023-06-20 11:33:12.000000 SPLayout-0.4.9/splayout/lumericalcommun/fdtdapi.py
+-rw-rw-rw-   0        0        0    44213 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/lumericalcommun/modeapi.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.860203 SPLayout-0.4.9/splayout/utils/
+-rw-rw-rw-   0        0        0       20 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/utils/__init__.py
+-rw-rw-rw-   0        0        0    14788 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/utils/utils.py
```

### Comparing `SPLayout-0.4.8/LICENSE` & `SPLayout-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/PKG-INFO` & `SPLayout-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.4.8
+Version: 0.4.9
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 
 SPLayout
```

### Comparing `SPLayout-0.4.8/README.rst` & `SPLayout-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/SPLayout.egg-info/PKG-INFO` & `SPLayout-0.4.9/SPLayout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.4.8
+Version: 0.4.9
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 
 SPLayout
```

### Comparing `SPLayout-0.4.8/SPLayout.egg-info/SOURCES.txt` & `SPLayout-0.4.9/SPLayout.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 SPLayout.egg-info/PKG-INFO
 SPLayout.egg-info/SOURCES.txt
 SPLayout.egg-info/dependency_links.txt
 SPLayout.egg-info/requires.txt
 SPLayout.egg-info/top_level.txt
 splayout/__init__.py
 splayout/adjointmethod/__init__.py
+splayout/adjointmethod/adjointmultitoopt.py
 splayout/adjointmethod/adjointshapeopt.py
 splayout/adjointmethod/adjointtopologyopt.py
+splayout/adjointmethod/scalabletotegion3d.py
 splayout/adjointmethod/shaperegion2d.py
 splayout/adjointmethod/shaperegion3d.py
 splayout/adjointmethod/topologyregion2d.py
 splayout/adjointmethod/topologyregion3d.py
 splayout/algorithms/__init__.py
 splayout/algorithms/binarybatalgorithm.py
 splayout/algorithms/binarygeneticalgorithm.py
```

### Comparing `SPLayout-0.4.8/setup.py` & `SPLayout-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/__init__.py` & `SPLayout-0.4.9/splayout/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
@@ -29,16 +29,18 @@
 from .lumericalcommun.modeapi import MODESimulation
 
 ## Adjoint Method
 from .adjointmethod.shaperegion2d import ShapeOptRegion2D
 from .adjointmethod.shaperegion3d import ShapeOptRegion3D
 from .adjointmethod.topologyregion2d import TopologyOptRegion2D
 from .adjointmethod.topologyregion3d import TopologyOptRegion3D
+from .adjointmethod.scalabletotegion3d import ScalableToOptRegion3D
 from .adjointmethod.adjointshapeopt import AdjointForShapeOpt
 from .adjointmethod.adjointtopologyopt import AdjointForTO
+from .adjointmethod.adjointmultitoopt import AdjointForMultiTO
 
 ## Algorithms
 from .algorithms.binarybatalgorithm import BinaryBatAlgorithm
 from .algorithms.directbinarysearchalgorithm import  DirectBinarySearchAlgorithm
 from .algorithms.particleswarmalgorithm import ParticleSwarmAlgorithm
 from .algorithms.binaryparticleswarmalgorithm import BinaryParticleSwarmAlgorithm
 from .algorithms.binarygeneticalgorithm import BinaryGeneticAlgorithm
```

### Comparing `SPLayout-0.4.8/splayout/adjointmethod/adjointshapeopt.py` & `SPLayout-0.4.9/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/adjointmethod/adjointtopologyopt.py` & `SPLayout-0.4.9/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from ..utils.utils import *
 from .topologyregion3d import TopologyOptRegion3D
+from .topologyregion2d import TopologyOptRegion2D
+from .scalabletotegion3d import ScalableToOptRegion3D
 import numpy as np
 import scipy.constants
 
 class AdjointForTO:
     """
     Adjoint Method for Topology Optimization.
 
@@ -11,15 +13,15 @@
     ----------
     fdtd_engine : FDTDSimulation
         The FDTDSimulation object.
     T_monitor_names : String or List of String
         Monitor names for deriving FoM.
     target_T : Array or List of Array
         Target Transmissions at different frequencies.
-    design_region : TopologyOptRegion2D or TopologyOptRegion3D
+    design_region : TopologyOptRegion2D or TopologyOptRegion3D or ScalableToOptRegion3D
         Design region for shape derivative method.
     forward_source_names : String or List of String
         Source names for Forward simulation.
     backward_source_names : String or List of String
         Source names for Adjoint simulation.
     sim_name : String
         Name of the temporary simulation(default: "Adjoint").
@@ -142,25 +144,36 @@
         d = np.diff(wavelength)
         T_fwd_partial_derivs = []
         for i in range(0, np.shape(self.backward_source_names)[0]):
             self.fdtd_engine.set_enable(self.backward_source_names[i])
             self.fdtd_engine.run()
             adjoint_source_power = self.fdtd_engine.get_source_power(self.backward_source_names[i])
             scaling_factor = np.conj(self.phase_prefactors[i]) * omega * 1j / np.sqrt(adjoint_source_power)
-            if (type(self.design_region) == TopologyOptRegion3D):
+            if type(self.design_region) == TopologyOptRegion3D:
                 self.adjoint_field, x_list, y_list, z_list = self.design_region.get_E_distribution(if_get_spatial=1)
                 cell = self.design_region.x_mesh * 1e-6 * self.design_region.y_mesh * 1e-6 * self.design_region.z_mesh * 1e-6
                 gradient_field = np.sum(
                     np.sum(2.0 * cell * scipy.constants.epsilon_0 * self.forward_field * self.adjoint_field, axis=4),
                     axis=2)
                 dF_dEps = gradient_field
-            else:
+            elif type(self.design_region) == TopologyOptRegion2D:
                 self.adjoint_field = self.design_region.get_E_distribution()
                 gradient_field = 2.0 * self.design_region.x_mesh * 1e-6 * self.design_region.y_mesh * 1e-6 * scipy.constants.epsilon_0 * self.forward_field * self.adjoint_field
                 dF_dEps = np.squeeze(np.sum(gradient_field, axis=-1), axis=2)
+            elif type(self.design_region) == ScalableToOptRegion3D:
+                self.adjoint_field, x_list, y_list, z_list = self.design_region.get_E_distribution(if_get_spatial=1)
+                cell = self.design_region.x_mesh * 1e-6 * self.design_region.y_mesh * 1e-6 * self.design_region.z_mesh * 1e-6
+                gradient_field = np.sum(
+                    np.sum(2.0 * cell * scipy.constants.epsilon_0 * self.forward_field * self.adjoint_field, axis=4),
+                    axis=2)
+                dF_dEps = np.zeros((self.design_region.get_x_size(), self.design_region.get_y_size(), gradient_field.shape[2]), dtype=gradient_field.dtype)
+                for k in range(0, gradient_field.shape[2]):
+                    dF_dEps[:, :, k] = self.design_region.scaling(gradient_field[:, :, k])
+            else:
+                raise Exception("Unacceptable design region provided.")
 
 
             for wl in range(0, len(omega)):
                 dF_dEps[:,:, wl] = dF_dEps[:,:, wl]*scaling_factor[wl]
 
             if (self.y_antisymmetric):
                 dF_dEps = np.real(dF_dEps)[:, int(dF_dEps.shape[1]/2):, :]
```

### Comparing `SPLayout-0.4.8/splayout/adjointmethod/shaperegion2d.py` & `SPLayout-0.4.9/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/adjointmethod/shaperegion3d.py` & `SPLayout-0.4.9/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/adjointmethod/topologyregion2d.py` & `SPLayout-0.4.9/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/adjointmethod/topologyregion3d.py` & `SPLayout-0.4.9/splayout/adjointmethod/topologyregion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/algorithms/binarybatalgorithm.py` & `SPLayout-0.4.9/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/algorithms/binarygeneticalgorithm.py` & `SPLayout-0.4.9/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/algorithms/binaryparticleswarmalgorithm.py` & `SPLayout-0.4.9/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/algorithms/directbinarysearchalgorithm.py` & `SPLayout-0.4.9/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/algorithms/particleswarmalgorithm.py` & `SPLayout-0.4.9/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/AEMDgrating.py` & `SPLayout-0.4.9/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/__init__.py` & `SPLayout-0.4.9/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/bend.py` & `SPLayout-0.4.9/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/doubleconnector.py` & `SPLayout-0.4.9/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/filledpattern.py` & `SPLayout-0.4.9/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/microring.py` & `SPLayout-0.4.9/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/pixelsregion.py` & `SPLayout-0.4.9/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/polygon.py` & `SPLayout-0.4.9/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/quarbend.py` & `SPLayout-0.4.9/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/sbend.py` & `SPLayout-0.4.9/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/selfdefinecomponent.py` & `SPLayout-0.4.9/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/simpleasymmetricdirectionalcoupler.py` & `SPLayout-0.4.9/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/slowlyvaryingtaper.py` & `SPLayout-0.4.9/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/taper.py` & `SPLayout-0.4.9/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/text.py` & `SPLayout-0.4.9/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/components/waveguide.py` & `SPLayout-0.4.9/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/lumericalcommun/fdtdapi.py` & `SPLayout-0.4.9/splayout/lumericalcommun/fdtdapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/lumericalcommun/modeapi.py` & `SPLayout-0.4.9/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.8/splayout/utils/utils.py` & `SPLayout-0.4.9/splayout/utils/utils.py`

 * *Files identical despite different names*

