# Comparing `tmp/OptiPRISMS-1.1.0.tar.gz` & `tmp/OptiPRISMS-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OptiPRISMS-1.1.0.tar", last modified: Fri May 12 14:44:14 2023, max compression
+gzip compressed data, was "OptiPRISMS-1.1.1.tar", last modified: Tue Jul  4 07:47:32 2023, max compression
```

## Comparing `OptiPRISMS-1.1.0.tar` & `OptiPRISMS-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/CfgGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/ComputeCostFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/costFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/misor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/triangulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/vtk_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:47:32.992737 OptiPRISMS-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-07-04 07:47:32.992737 OptiPRISMS-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:47:32.992737 OptiPRISMS-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:47:32.988736 OptiPRISMS-1.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/CfgGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/ComputeCostFunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:47:32.992737 OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-07-04 07:47:32.000000 OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 07:47:32.000000 OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:47:32.000000 OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 07:47:32.000000 OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:47:32.000000 OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/OptiPRISMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/costFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/misor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/triangulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-04 07:47:19.000000 OptiPRISMS-1.1.1/src/vtk_utils.py
```

### Comparing `OptiPRISMS-1.1.0/LICENSE` & `OptiPRISMS-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/PKG-INFO` & `OptiPRISMS-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OptiPRISMS
-Version: 1.1.0
+Version: 1.1.1
 Summary: Identifies Crystal Plasticity (CP) parameters by inverse analysis based on CPFEM simulations performed using PRISMS-Plasticity
 Home-page: https://github.com/DorianDepriester/OptiPRISMS
 Author: Dorian Depriester
 Author-email: dorian.depriester@ensam.eu
 License: GNU Lesser General Public License v2.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,30 +24,48 @@
 4. return a cost function, evidencing *how far* the simulation is, compared to the experiment,
 5. remove simulation files.
 
 In order to generate the PRISMS configuration files, this software will parse *template* files in order to retrieve which parameters it shall optimize.
 
 Records for each optimization loop will be stored in a log file, so that the user can track the evolution of optimized parameters and cost functions. In addition, OptiPRISMS will use this file to avoid reruning preexisting simulations, so that the optimization can be stopped then resumed.
 
+Full description of the algorithm is provided in [[2]](#paper).
+
 ## Required materials
 
-- The mesh of the microstructure (in .msh format). One can use [MTEX2Gmsh](https://github.com/DorianDepriester/MTEX2Gmsh/blob/master/MTEX2prisms/MTEX2PRISMS.pdf) [[2]](#mtex2gmsh) to generate a conforming mesh directly from EBSD data.
+- The mesh of the microstructure (in .msh format). One can use [MTEX2Gmsh](https://github.com/DorianDepriester/MTEX2Gmsh/blob/master/MTEX2prisms/MTEX2PRISMS.pdf) [[3]](#mtex2gmsh) to generate a conforming mesh directly from EBSD data.
 - [PRISMS-Plasticity software](https://github.com/prisms-center/plasticity).
 - Python 3.6 (or later) with the following modules: numpy, scipy, vtk, pandas and optimparallel (optional).
 - Experimental data, consisting in:
     - a macroscopic tensile curve (strain-stress values as a CSV file),
 	- SEM-DIC displacement measurements, stored as individual CSV files named sequentially (eg. "DIC_1.csv", "DIC_2.csv" and so on).
 	
 Each of these files must have tabular data, ordered this way:
 1. x coordinates of DIC points where DIC measurements are performed,
 2. y coordinates of DIC points where DIC measurements are performed,
 3. x displacements,
 4. y displacements,
 5. correlation coefficients (optional, see [Cost Function](#cost-function) section)
 
+## Cite this project
+If you use this project, please cite ref. [[2]](#paper). You can use the following BibTeX entry:
+
+```bibtex
+@article{OptiPRISMS,
+title = {Crystal Plasticity simulations of in situ tensile tests: A two-step inverse method for identification of CP parameters, and assessment of CPFEM capabilities},
+journal = {International Journal of Plasticity},
+pages = {103695},
+year = {2023},
+issn = {0749-6419},
+doi = {https://doi.org/10.1016/j.ijplas.2023.103695},
+url = {https://www.sciencedirect.com/science/article/pii/S074964192300181X},
+author = {D. Depriester and J.P. Goulmy and L. Barrallier},
+}
+```
+
 ## Installation
 You can install the latest release of OptiPRISMS with pip:
 ```bash
 pip install OptiPRISMS
 ```
 Otherwise, you can install the development version from sources:
 ```bash
@@ -137,10 +155,12 @@
 
 - **fake simulations**: If Yes, each simulation is not computed. The related commands are printed instead. Default is No.
 - **fake deletions**: Turn off automatic removal of simulation results (step 5 in [How it works](#how-it-works) section). Default is No.
 
 ## References
 <a id="prisms">[1]</a> Yaghoobi et al., (2019). Prisms-plasticity: An open-source crystal plasticity finite element software. Computational Materials Science, 169:109078, https://doi.org/10.1016/j.commatsci.2019.109078
 
-<a id="mtex2gmsh">[2]</a> Depriester et al., (2020). MTEX2Gmsh: a tool for generating 2D meshes from EBSD data. Journal of Open Source Software, 5(52):2094, https://doi.org/10.21105/joss.02094
+<a id="paper">[2]</a> Depriester et al., (2023). Crystal Plasticity Simulations of in Situ Tensile Tests: A Two-Step Inverse Method for Identification of CP Parameters, and Assessment of CPFEM Capabilities. International Journal of Plasticity, https://doi.org/10.1016/j.ijplas.2023.103695
+
+<a id="mtex2gmsh">[3]</a> Depriester et al., (2020). MTEX2Gmsh: a tool for generating 2D meshes from EBSD data. Journal of Open Source Software, 5(52):2094, https://doi.org/10.21105/joss.02094
 
-<a id="optim_parallel">[3]</a> Gerber, F. and Furrer, R. (2019). optimParallel: An R package providing a parallel version of the L-BFGS-B optimization method, The R Journal, 11(1):352–358, http://doi.org/10.32614/RJ-2019-030
+<a id="optim_parallel">[4]</a> Gerber, F. and Furrer, R. (2019). optimParallel: An R package providing a parallel version of the L-BFGS-B optimization method, The R Journal, 11(1):352–358, http://doi.org/10.32614/RJ-2019-030
```

### Comparing `OptiPRISMS-1.1.0/README.md` & `OptiPRISMS-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,30 +13,48 @@
 4. return a cost function, evidencing *how far* the simulation is, compared to the experiment,
 5. remove simulation files.
 
 In order to generate the PRISMS configuration files, this software will parse *template* files in order to retrieve which parameters it shall optimize.
 
 Records for each optimization loop will be stored in a log file, so that the user can track the evolution of optimized parameters and cost functions. In addition, OptiPRISMS will use this file to avoid reruning preexisting simulations, so that the optimization can be stopped then resumed.
 
+Full description of the algorithm is provided in [[2]](#paper).
+
 ## Required materials
 
-- The mesh of the microstructure (in .msh format). One can use [MTEX2Gmsh](https://github.com/DorianDepriester/MTEX2Gmsh/blob/master/MTEX2prisms/MTEX2PRISMS.pdf) [[2]](#mtex2gmsh) to generate a conforming mesh directly from EBSD data.
+- The mesh of the microstructure (in .msh format). One can use [MTEX2Gmsh](https://github.com/DorianDepriester/MTEX2Gmsh/blob/master/MTEX2prisms/MTEX2PRISMS.pdf) [[3]](#mtex2gmsh) to generate a conforming mesh directly from EBSD data.
 - [PRISMS-Plasticity software](https://github.com/prisms-center/plasticity).
 - Python 3.6 (or later) with the following modules: numpy, scipy, vtk, pandas and optimparallel (optional).
 - Experimental data, consisting in:
     - a macroscopic tensile curve (strain-stress values as a CSV file),
 	- SEM-DIC displacement measurements, stored as individual CSV files named sequentially (eg. "DIC_1.csv", "DIC_2.csv" and so on).
 	
 Each of these files must have tabular data, ordered this way:
 1. x coordinates of DIC points where DIC measurements are performed,
 2. y coordinates of DIC points where DIC measurements are performed,
 3. x displacements,
 4. y displacements,
 5. correlation coefficients (optional, see [Cost Function](#cost-function) section)
 
+## Cite this project
+If you use this project, please cite ref. [[2]](#paper). You can use the following BibTeX entry:
+
+```bibtex
+@article{OptiPRISMS,
+title = {Crystal Plasticity simulations of in situ tensile tests: A two-step inverse method for identification of CP parameters, and assessment of CPFEM capabilities},
+journal = {International Journal of Plasticity},
+pages = {103695},
+year = {2023},
+issn = {0749-6419},
+doi = {https://doi.org/10.1016/j.ijplas.2023.103695},
+url = {https://www.sciencedirect.com/science/article/pii/S074964192300181X},
+author = {D. Depriester and J.P. Goulmy and L. Barrallier},
+}
+```
+
 ## Installation
 You can install the latest release of OptiPRISMS with pip:
 ```bash
 pip install OptiPRISMS
 ```
 Otherwise, you can install the development version from sources:
 ```bash
@@ -126,10 +144,12 @@
 
 - **fake simulations**: If Yes, each simulation is not computed. The related commands are printed instead. Default is No.
 - **fake deletions**: Turn off automatic removal of simulation results (step 5 in [How it works](#how-it-works) section). Default is No.
 
 ## References
 <a id="prisms">[1]</a> Yaghoobi et al., (2019). Prisms-plasticity: An open-source crystal plasticity finite element software. Computational Materials Science, 169:109078, https://doi.org/10.1016/j.commatsci.2019.109078
 
-<a id="mtex2gmsh">[2]</a> Depriester et al., (2020). MTEX2Gmsh: a tool for generating 2D meshes from EBSD data. Journal of Open Source Software, 5(52):2094, https://doi.org/10.21105/joss.02094
+<a id="paper">[2]</a> Depriester et al., (2023). Crystal Plasticity Simulations of in Situ Tensile Tests: A Two-Step Inverse Method for Identification of CP Parameters, and Assessment of CPFEM Capabilities. International Journal of Plasticity, https://doi.org/10.1016/j.ijplas.2023.103695
+
+<a id="mtex2gmsh">[3]</a> Depriester et al., (2020). MTEX2Gmsh: a tool for generating 2D meshes from EBSD data. Journal of Open Source Software, 5(52):2094, https://doi.org/10.21105/joss.02094
 
-<a id="optim_parallel">[3]</a> Gerber, F. and Furrer, R. (2019). optimParallel: An R package providing a parallel version of the L-BFGS-B optimization method, The R Journal, 11(1):352–358, http://doi.org/10.32614/RJ-2019-030
+<a id="optim_parallel">[4]</a> Gerber, F. and Furrer, R. (2019). optimParallel: An R package providing a parallel version of the L-BFGS-B optimization method, The R Journal, 11(1):352–358, http://doi.org/10.32614/RJ-2019-030
```

### Comparing `OptiPRISMS-1.1.0/setup.py` & `OptiPRISMS-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='OptiPRISMS',
-    version='1.1.0',
+    version='1.1.1',
     packages=[''],
     package_dir={'': 'src'},
     url='https://github.com/DorianDepriester/OptiPRISMS',
     license='GNU Lesser General Public License v2.1',
     author='Dorian Depriester',
     author_email='dorian.depriester@ensam.eu',
     description='Identifies Crystal Plasticity (CP) parameters by inverse analysis based on CPFEM simulations performed using PRISMS-Plasticity',
```

### Comparing `OptiPRISMS-1.1.0/src/CfgGenerator.py` & `OptiPRISMS-1.1.1/src/CfgGenerator.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/src/ComputeCostFunctions.py` & `OptiPRISMS-1.1.1/src/ComputeCostFunctions.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/PKG-INFO` & `OptiPRISMS-1.1.1/src/OptiPRISMS.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OptiPRISMS
-Version: 1.1.0
+Version: 1.1.1
 Summary: Identifies Crystal Plasticity (CP) parameters by inverse analysis based on CPFEM simulations performed using PRISMS-Plasticity
 Home-page: https://github.com/DorianDepriester/OptiPRISMS
 Author: Dorian Depriester
 Author-email: dorian.depriester@ensam.eu
 License: GNU Lesser General Public License v2.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,30 +24,48 @@
 4. return a cost function, evidencing *how far* the simulation is, compared to the experiment,
 5. remove simulation files.
 
 In order to generate the PRISMS configuration files, this software will parse *template* files in order to retrieve which parameters it shall optimize.
 
 Records for each optimization loop will be stored in a log file, so that the user can track the evolution of optimized parameters and cost functions. In addition, OptiPRISMS will use this file to avoid reruning preexisting simulations, so that the optimization can be stopped then resumed.
 
+Full description of the algorithm is provided in [[2]](#paper).
+
 ## Required materials
 
-- The mesh of the microstructure (in .msh format). One can use [MTEX2Gmsh](https://github.com/DorianDepriester/MTEX2Gmsh/blob/master/MTEX2prisms/MTEX2PRISMS.pdf) [[2]](#mtex2gmsh) to generate a conforming mesh directly from EBSD data.
+- The mesh of the microstructure (in .msh format). One can use [MTEX2Gmsh](https://github.com/DorianDepriester/MTEX2Gmsh/blob/master/MTEX2prisms/MTEX2PRISMS.pdf) [[3]](#mtex2gmsh) to generate a conforming mesh directly from EBSD data.
 - [PRISMS-Plasticity software](https://github.com/prisms-center/plasticity).
 - Python 3.6 (or later) with the following modules: numpy, scipy, vtk, pandas and optimparallel (optional).
 - Experimental data, consisting in:
     - a macroscopic tensile curve (strain-stress values as a CSV file),
 	- SEM-DIC displacement measurements, stored as individual CSV files named sequentially (eg. "DIC_1.csv", "DIC_2.csv" and so on).
 	
 Each of these files must have tabular data, ordered this way:
 1. x coordinates of DIC points where DIC measurements are performed,
 2. y coordinates of DIC points where DIC measurements are performed,
 3. x displacements,
 4. y displacements,
 5. correlation coefficients (optional, see [Cost Function](#cost-function) section)
 
+## Cite this project
+If you use this project, please cite ref. [[2]](#paper). You can use the following BibTeX entry:
+
+```bibtex
+@article{OptiPRISMS,
+title = {Crystal Plasticity simulations of in situ tensile tests: A two-step inverse method for identification of CP parameters, and assessment of CPFEM capabilities},
+journal = {International Journal of Plasticity},
+pages = {103695},
+year = {2023},
+issn = {0749-6419},
+doi = {https://doi.org/10.1016/j.ijplas.2023.103695},
+url = {https://www.sciencedirect.com/science/article/pii/S074964192300181X},
+author = {D. Depriester and J.P. Goulmy and L. Barrallier},
+}
+```
+
 ## Installation
 You can install the latest release of OptiPRISMS with pip:
 ```bash
 pip install OptiPRISMS
 ```
 Otherwise, you can install the development version from sources:
 ```bash
@@ -137,10 +155,12 @@
 
 - **fake simulations**: If Yes, each simulation is not computed. The related commands are printed instead. Default is No.
 - **fake deletions**: Turn off automatic removal of simulation results (step 5 in [How it works](#how-it-works) section). Default is No.
 
 ## References
 <a id="prisms">[1]</a> Yaghoobi et al., (2019). Prisms-plasticity: An open-source crystal plasticity finite element software. Computational Materials Science, 169:109078, https://doi.org/10.1016/j.commatsci.2019.109078
 
-<a id="mtex2gmsh">[2]</a> Depriester et al., (2020). MTEX2Gmsh: a tool for generating 2D meshes from EBSD data. Journal of Open Source Software, 5(52):2094, https://doi.org/10.21105/joss.02094
+<a id="paper">[2]</a> Depriester et al., (2023). Crystal Plasticity Simulations of in Situ Tensile Tests: A Two-Step Inverse Method for Identification of CP Parameters, and Assessment of CPFEM Capabilities. International Journal of Plasticity, https://doi.org/10.1016/j.ijplas.2023.103695
+
+<a id="mtex2gmsh">[3]</a> Depriester et al., (2020). MTEX2Gmsh: a tool for generating 2D meshes from EBSD data. Journal of Open Source Software, 5(52):2094, https://doi.org/10.21105/joss.02094
 
-<a id="optim_parallel">[3]</a> Gerber, F. and Furrer, R. (2019). optimParallel: An R package providing a parallel version of the L-BFGS-B optimization method, The R Journal, 11(1):352–358, http://doi.org/10.32614/RJ-2019-030
+<a id="optim_parallel">[4]</a> Gerber, F. and Furrer, R. (2019). optimParallel: An R package providing a parallel version of the L-BFGS-B optimization method, The R Journal, 11(1):352–358, http://doi.org/10.32614/RJ-2019-030
```

### Comparing `OptiPRISMS-1.1.0/src/OptiPRISMS.py` & `OptiPRISMS-1.1.1/src/OptiPRISMS.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/src/costFunctions.py` & `OptiPRISMS-1.1.1/src/costFunctions.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/src/misor.py` & `OptiPRISMS-1.1.1/src/misor.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/src/triangulate.py` & `OptiPRISMS-1.1.1/src/triangulate.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.1.0/src/vtk_utils.py` & `OptiPRISMS-1.1.1/src/vtk_utils.py`

 * *Files identical despite different names*

