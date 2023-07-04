# Comparing `tmp/sphractal-0.4.4.tar.gz` & `tmp/sphractal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.4.4.tar", max compression
+gzip compressed data, was "sphractal-0.6.0.tar", max compression
```

## Comparing `sphractal-0.4.4.tar` & `sphractal-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,18 @@
--rw-r--r--   0        0        0     1082 2023-07-01 12:37:51.500012 sphractal-0.4.4/LICENSE
--rw-r--r--   0        0        0     3398 2023-07-01 12:37:51.500012 sphractal-0.4.4/README.md
--rw-r--r--   0        0        0     1990 2023-07-01 12:38:30.775572 sphractal-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      710 2023-07-01 12:37:51.560011 sphractal-0.4.4/setup.py
--rw-r--r--   0        0        0     2288 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/3DbinImBCcpu.cpp
--rw-r--r--   0        0        0     3111 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/3DbinImBCgpu.cpp
--rw-r--r--   0        0        0     2084 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/README.txt
--rw-r--r--   0        0        0     3581 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCPU.cpp
--rw-r--r--   0        0        0      979 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCPU.h
--rw-r--r--   0        0        0     4378 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA2D.cu
--rw-r--r--   0        0        0     1056 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA2D.cuh
--rw-r--r--   0        0        0     4947 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA3D.cu
--rw-r--r--   0        0        0     1056 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA3D.cuh
--rw-r--r--   0        0        0     5867 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA4D.cu
--rw-r--r--   0        0        0     1056 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA4D.cuh
--rw-r--r--   0        0        0    10330 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/test.cpp
--rw-r--r--   0        0        0     1394 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/__init__.py
--rw-r--r--   0        0        0    21444 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     3821 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      279 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8881 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8119 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11480 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/utils.py
--rw-r--r--   0        0        0    94223 2023-07-01 12:37:51.560011 sphractal-0.4.4/tests/fixtures.py
--rw-r--r--   0        0        0    17404 2023-07-01 12:37:51.560011 sphractal-0.4.4/tests/test_sphractal.py
--rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 sphractal-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-04 02:45:03.637258 sphractal-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3652 2023-07-04 02:45:03.637258 sphractal-0.6.0/README.md
+-rw-r--r--   0        0        0     2056 2023-07-04 02:45:42.821337 sphractal-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-04 02:45:42.821337 sphractal-0.6.0/setup.py
+-rw-r--r--   0        0        0     1406 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    22847 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4302 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      279 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/datasets.py
+-rw-r--r--   0        0        0      405 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/pybind11/example.cpp
+-rw-r--r--   0        0        0     2520 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/pybind11/pybindtest.cpp
+-rw-r--r--   0        0        0     8881 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8119 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11480 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94223 2023-07-04 02:45:03.697258 sphractal-0.6.0/tests/fixtures.py
+-rw-r--r--   0        0        0    17688 2023-07-04 02:45:03.697258 sphractal-0.6.0/tests/test_sphractal.py
+-rw-r--r--   0        0        0     4921 1970-01-01 00:00:00.000000 sphractal-0.6.0/PKG-INFO
```

### Comparing `sphractal-0.4.4/LICENSE` & `sphractal-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.4/README.md` & `sphractal-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -6,64 +6,58 @@
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Current
-* Representation of the surface as either point clouds (feature yet to be made available due to C++ compilation issues) or exact surfaces.
+* Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
-### To be Done
-* Set path for exeDir.
-* Publish to Conda.
-  * cd condaForge/
-  * conda skeleton pypi sphractal
-  * vim sphractal/meta.yaml ('name', 'version', 'git_rev', 'git_url', 'imports', 'home', 'noarch', 'maintainer')
-  * vim build.sh
-  * vim bld.bat
-  * conda-build sphractal (record path)
-  * conda install --use-local sphractal
-  * conda list
-  * anaconda login
-  * anaconda upload PATH_TO_BZ2
-  * conda config --set anaconda_upload yes
-  * anaconda logout
-* Nested multiprocessing.
-* Better looking plots, allow figure size to be specified, allow choice for 'paper' and 'presentation'.
-* Consider transforming xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
+### Under Development
+* Nested multiprocessing (boxLenConc=True).
+* Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
+* Integration of C++ code for point cloud surface representation into the package.
 
 ## Installation
 
-Use `pip` or `conda` (yet to be implemented) to install `Sphractal`:
+Use `pip` or `conda` to install `Sphractal`:
 
 ```bash
 $ pip install sphractal
 ```
 ```bash
 $ conda install -c conda-forge sphractal
 ```
 
-`Sphractal` requires a C++ code to be compiled for the functionalities related to point clouds surface representation 
-to work. This could be done by first changing into the director containing the C++ source code: 
+### Special Requirement for Point Cloud Surface Representation
+`Sphractal` requires an executable compiled from another freely available repository for the functionalities related 
+to point clouds surface representation to operate properly. 
 
+This could be done by:
+
+* Downloading the source code from the [repository](https://github.com/Jon-Ting/fastBC.git) to a directory of your choice:
 ```bash
-$ cd {SPHRACTAL_DIR_PATH}/src/fbc/
+git clone https://github.com/Jon-Ting/fastBC.git
 ```
 
-And then compile either of the two file using respective C++ compiler. 
-The second option is only viable for machines with `CUDA` platform available.
-
+* Building an executable by doing either one of the following compilations according to the instructions on the [README.md](https://github.com/Jon-Ting/fastBC/blob/main/README.md) page. This will decide whether you will be running the box counting algorithm with GPU acceleration. Feel free to rename the executables to any other sensible names:
 ```bash
-$ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o {SPHRACTAL_DIR_PATH}/bin/3DbinImBCcpu.exe
+$ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o 3DbinImBCcpu.exe
 ```
 ```bash
-$ nvcc -O3 bcCUDA3D.cu 3DbinImBCgpu.cpp -o {SPHRACTAL_DIR_PATH}/bin/3DbinImBCgpu.exe
+$ nvcc -O3 3DbinImBCgpu.cpp bcCUDA3D.cu -o 3DbinImBCgpu.exe
+```
+
+* (Optional) Setting the path to the executable as an environment variable accessible by Python (replace `PATH_TO_EXE` by the absolute path to the executable file you just built), otherwise you could always pass the path to the executable to the relevant functions:
+```bash
+$ export FASTBC_EXE={PATH_TO_EXE}
 ```
+Note that for the environment variable to be persistent (to still exist after the terminal is closed), the line should be added to your `~/.bashrc`.
 
 ## Usage
 
 ```python
 from sphractal import getExampleDataPath, runBoxCnt
 
 xyzFilePath = getExampleDataPath()  # Replace with the path to your xyz or lmp file
```

### Comparing `sphractal-0.4.4/pyproject.toml` & `sphractal-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.4.4"
+version = "0.6.0"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
@@ -13,35 +13,38 @@
     "Intended Audience :: Science/Research", 
     "Natural Language :: English", 
     "Operating System :: OS Independent", 
     "Programming Language :: C++", 
     "Programming Language :: Python :: 3", 
     "Topic :: Scientific/Engineering", 
 ]
-include = ["tests/*", "src/fbc/*", "setup.py"]
+include = ["tests/*", "setup.py"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 matplotlib = ">=3.7.1"
 statsmodels = ">=0.14.0"
-scipy = {version = ">=1.11.0", python = ">=3.9,<3.13"}
+scipy = {version = ">=1.11.1", python = ">=3.9,<3.13"}
 numba = ">=0.57.1"
 numpy = ">=1.22,<1.25"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.0"
 pytest-cov = ">=4.1.0"
 jupyter = ">=1.0.0"
 myst-nb = {version = ">=0.17.2", python = "^3.9"}
 sphinx-autoapi = ">=2.1.1"
 sphinx-rtd-theme = ">=1.2.2"
 python-semantic-release = ">=7.34.6"
 
 [tool.semantic_release]
-version_variable = "pyproject.toml:version" # version location
+version_variable = [
+    "setup.py:__version__",
+    "pyproject.toml:version",
+]                                           # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = false                      # don't auto-upload to PyPI
 remove_dist = false                         # don't remove dists
```

### Comparing `sphractal-0.4.4/src/fbc/3DbinImBCcpu.cpp` & `sphractal-0.6.0/src/sphractal/pybind11/pybindtest.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+#include <pybind11/pybind11.h>
 #include <iostream>
 #include <cmath>
 #include <chrono>
 #include <cstring>
 #include <fstream>
 #include "bcCPU.h"
 
 void pointsTo3DImage(unsigned char* matrix, int* idxarr, int n) {
     for (int i = 0; i < n; i++)
         matrix[idxarr[i]] = 1;
 }
 
-int main(int argc, char* argv[]) {
+int boxCnt3DbinIm(int argc, char* argv[]) {
     // Check command line arguments
     if (argc != 4) {
         std::cerr << "Usage: " << argv[0] << " <input_file> <output_file> <grid_num>\n";
         return 1;
     }
 
     // Constants
@@ -70,7 +71,12 @@
     // std::cout << "    3D CPU box-counting duration: " << time_cpu.count() << " seconds" << std::endl;
 
     // Clean up memory
     delete[] Icpu3d, idxarr, I3d, n3d;
     return 0;
 }
 
+PYBIND11_MODULE(runBoxCnt3DbinIm, m) {
+    m.doc() = "pybind11 example plugin"; // optional module docstring
+
+    m.def("boxCnt3DbinIm", &boxCnt3DbinIm, "A function that adds two numbers");
+}
```

### Comparing `sphractal-0.4.4/src/sphractal/__init__.py` & `sphractal-0.6.0/src/sphractal/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 
 # Read version from installed package
 from importlib.metadata import version
 __version__ = version('sphractal')
 
 # Populate package namespace
 __all__ = ['constants', 'datasets', 'utils', 'boxCnt']
-from sphractal.constants import ATOMIC_RAD_DICT, METALLIC_RAD_DICT
+from sphractal.constants import ATOMIC_RAD_DICT, METALLIC_RAD_DICT, PLT_PARAMS
 from sphractal.datasets import getExampleDataPath
 from sphractal.utils import readXYZ, findNN, findSurf
 from sphractal.boxCnt import getVoxelBoxCnts, getSphereBoxCnts, findSlope, runBoxCnt
```

### Comparing `sphractal-0.4.4/src/sphractal/boxCnt.py` & `sphractal-0.6.0/src/sphractal/boxCnt.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from warnings import warn
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 import numpy as np
 from statsmodels.api import OLS, add_constant
 
-from sphractal.surfExact import findTargetAtoms, MIN_VAL_FROM_BOUND, scanAllAtoms, writeBoxCoords
-from sphractal.surfPointClouds import genSurfPoints
+from sphractal.constants import PLT_PARAMS
 from sphractal.utils import findNN, findSurf, readXYZ
 # from sphractal.utils import estDuration, annotate
+from sphractal.surfPointClouds import genSurfPoints
+from sphractal.surfExact import findTargetAtoms, MIN_VAL_FROM_BOUND, scanAllAtoms, writeBoxCoords
 
 
 # @annotate('getVoxelBoxCnts', color='blue')
 def getVoxelBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-                    npName, writeFileDir='boxCntOutputs', exeDir='../bin', procUnit='cpu',
+                    npName, writeFileDir='boxCntOutputs', exePath='$FASTBC_EXE',
                     radType='atomic', numPoint=300, gridNum=1024,
                     rmInSurf=True, vis=True, verbose=False, genPCD=False):
     """
     Count the boxes that cover the outer surface of a set of overlapping spheres represented as point clouds for
-    different box sizes, using 3D box-counting algorithm written by Ruiz de Miras et al. in C++. All source codes are
-    provided under {SPHRACTAL_DIR_PATH}/src/fbc/.
+    different box sizes, using 3D box-counting algorithm written by Ruiz de Miras et al. in C++. 
+
+    IMPORTANT: Make sure the source code has been downloaded from https://github.com/Jon-Ting/fastBC and compiled 
+    on your machine. 'exePath' should point to the right directory if FASTBC_EXE is not set as an environment variable.
     
     Parameters
     ----------
     atomsEle : 1D ndarray
         Element type of each atom.
     atomsRad : 1D ndarray
         Radius of each atom.
@@ -37,18 +40,16 @@
         Cartesian coordinates of each atom.
     atomsNeighIdxs : 2D ndarray
         Neighbour atoms indices of each atom.
     npName : str
         Identifier of the measured object, which forms part of the output file name, ideally unique.
     writeFileDir : str, optional
         Path to the directory to store the output files.
-    exeDir : str, optional
+    exePath : str, optional
         Path to the compiled C++ executable for box-counting.
-    procUnit : {'cpu', 'gpu'}, optional
-        Type of C++ executable to run for box-counting.
     radType : {'atomic', 'metallic'}, optional
         Type of radii to use for the spheres.
     numPoint : int, optional
         Number of surface points to be generated around each atom.
     gridNum : int, optional
         Resolution of the 3D binary image.
     rmInSurf : bool, optional
@@ -78,29 +79,28 @@
     -----
     The 3D binary image resolution (gridNum) is restricted by RAM size available, the relationship is illustrated below:
     -  1024 ->    2 GB (laptops -> typically 8 GB)
     -  2048 ->   16 GB (HPC nodes with GPUs like NCI Gadi gpuvolta queue -> max 32 GB/node)
     -  4096 ->  128 GB
     -  8192 -> 1024 GB (HPC node with huge memories like NCI Gadi megamem queue -> max 2990 GB/node)
     - 16384 -> 8192 GB
-    Further details about maximum grid size and memory estimation could be found in original codes of the authors in
-    {SPHRACTAL_DIR_PATH}/src/fbc/test.cpp.
-    As a reference, when 8192 grids are used, allocation of memory took 25 min; while the CPU algorithm runs for 18 min.
+    Further details about maximum grid size and memory estimation could be found in 'test.cpp' documented by the authors 
+    (https://www.ugr.es/~demiras/fbc/). As a reference, when 8192 grids are used, allocation of memory took 25 min; while 
+    the CPU algorithm runs for 18 min.
     """
     if verbose:
         print(f"  Approximating the surface with {numPoint} point clouds for each atom...")
     if not isdir(writeFileDir):
         mkdir(writeFileDir)
 
     genSurfPoints(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                   npName, writeFileDir,
                   radType, numPoint, gridNum,
                   rmInSurf, vis, verbose, genPCD)
-    system(f"{exeDir}/3DbinImBC{procUnit}.exe {gridNum} {writeFileDir}/surfVoxelIdxs.txt "
-           f"{writeFileDir}/surfVoxelBoxCnts.txt")
+    system(f"{exePath} {gridNum} {writeFileDir}/surfVoxelIdxs.txt {writeFileDir}/surfVoxelBoxCnts.txt")
     scales, counts = [], []
     with open(f"{writeFileDir}/surfVoxelBoxCnts.txt", 'r') as f:
         for line in f:
             scales.append(log10(1 / int(line.split()[0])))
             counts.append(log10(int(line.split()[1])))
     return scales[::-1], counts[::-1]
 
@@ -140,15 +140,15 @@
     rmInSurf : bool, optional
         Whether to remove the surface points on the inner surface.
     writeBox : bool, optional
         Whether to generate output files for visualisation.
     verbose : bool, optional
         Whether to display the details.
     boxLenConc : bool, optional
-        Whether to parallelise the box-counting across different box lengths.
+        Whether to parallelise the box-counting across different box lengths (under development, stick to default for now).
     maxWorkers : int, optional
         Maximum number of processes to spawn for parallelisation of box-counting across different box lengths, only used
         if 'boxLenConc' is True.
     
     Returns
     -------
     scales : list
@@ -205,15 +205,16 @@
     if writeBox:
         writeBoxCoords(atomsEle, atomsXYZ, allLensSurfBoxs, allLensBulkBoxs, minXYZ, scanBoxLens, writeFileDir, npName)
     return scales, counts
 
 
 # @annotate('findSlope', color='green')
 def findSlope(scales, counts, npName='', writeFileDir='boxCntOutputs', lenRange='trim',
-              minSampleNum=5, confLvl=95, visReg=True, saveFig=False, showPlot=False):
+              minSampleNum=5, confLvl=95, 
+              visReg=True, figType='article', saveFig=False, showPlot=False):
     """
     Compute the slope (box counting dimension) from the box-counting data collected.
 
     Parameters
     ----------
     scales : list
         Box lengths.
@@ -228,28 +229,37 @@
         coefficient of determination by iteratively removing the box counts obtained using boxes of extreme sizes.
     minSampleNum : int, optional
         Minimum number of box count data points to be retained for slope estimation from the linear regression fitting.
     confLvl : Union[int, float]
         Confidence level of confidence interval in percentage.
     visReg : bool, optional
         Whether to generate figures from the linear regression fitting process.
+    figType : {'article', 'poster', 'ppt'}
+        Type of figures to be generated.
     saveFig : bool, optional
         Whether to save the plots generated, only works when 'visReg' is True.
     showPlot : bool, optional
         Whether to show the plots generated, only works when 'visReg' is True.
     
     Returns
     -------
     r2score : float
         Coefficient of determination from determination of the dimension of point clouds surface.
     boxCntDim : float
         Box-counting dimension of the point clouds representation of the surface.
     slopeCI : tuple
         Confidence interval of the box-counting dimension of the point clouds surface.
     """
+    if visReg:
+        plt.rc('font', family='sans-serif')
+        plt.rc('xtick', labelsize='x-small')
+        plt.rc('ytick', labelsize='x-small')
+        params = PLT_PARAMS[figType]
+        figsize, dpi, fontsize, labelsize, legendsize, linewidth, markersize = params['figsize'], params['dpi'], params['fontsize'], params['labelsize'], params['legendsize'], params['linewidth'], params['markersize']
+
     while np.nan in counts:
         nanIdx = counts.index(np.nan)
         del counts[nanIdx]
         del scales[nanIdx]
     firstPointIdx, lastPointIdx, removeSmallBoxes = 0, len(scales), True  # countChange.count(countChange[0])
 
     if abs(confLvl) > 100:
@@ -259,26 +269,32 @@
     while len(scales[firstPointIdx:lastPointIdx]) > minSampleNum:
         x, y = scales[firstPointIdx:lastPointIdx], counts[firstPointIdx:lastPointIdx]
         regModel = OLS(endog=y, exog=add_constant(x)).fit()
         r2score, boxCntDim, slopeCI = regModel.rsquared, regModel.params[1], regModel.conf_int(alpha=alphaCI)[1]
         yPred = regModel.predict()  # Returns ndarray, allowing subtraction later
         if visReg:
             plt.close()
-            _, ax = plt.subplots()
-            ax.scatter(x, y)
-            ax.plot(x, yPred, label='OLS')
+            fig = plt.figure(figsize=figsize, dpi=dpi)
+            ax = fig.add_subplot(1, 1, 1)
+            handleScatter = ax.scatter(x, y, marker='o', s=markersize, c='r', alpha=1, edgecolors='k', linewidths=1.2, zorder=3)
+            handleBestFit = ax.plot(x, yPred, linestyle='-', linewidth=1., color='k', label='OLS')
+            ax.grid(linestyle='dotted')
             predOLS = regModel.get_prediction()
             lowCIvals, upCIvals = predOLS.summary_frame()['mean_ci_lower'], predOLS.summary_frame()['mean_ci_upper']
-            ax.plot(x, upCIvals, 'r--')
-            ax.plot(x, lowCIvals, 'r--')
-            ax.set_xlabel('log(1/r)')
-            ax.set_ylabel('log(N)')
+            handleConfBand = ax.plot(x, upCIvals, linestyle='--', linewidth=linewidth, color='b')
+            ax.plot(x, lowCIvals, linestyle='--', linewidth=linewidth, color='b')
+            ax.fill_between(x, upCIvals, lowCIvals, alpha=0.2)
+            ax.set_xlabel(r'log$(1/\epsilon)$', fontsize=labelsize)
+            ax.set_ylabel(r'log$(N)$', fontsize=labelsize)
             ax.yaxis.set_major_formatter(FormatStrFormatter('% 1.1f'))
-            ax.set_title(f"{npName} R2: {r2score:.3f}, D_Box: {boxCntDim:.3f}, {confLvl}% CI: "
-                      f"[{slopeCI[0]:.3f}, {slopeCI[1]:.3f}]");
+            ax.legend(handles=(handleScatter, handleBestFit[0], handleConfBand[0]), 
+                      labels=('Actual box counts', fr"Best fit line ($R^2$: {r2score:.3f})", f"{confLvl}% confidence bands"), 
+                      title=fr"$D_{{box}}$: {boxCntDim:.3f} [{slopeCI[0]:.3f}, {slopeCI[1]:.3f}]", title_fontsize=legendsize, 
+                      fontsize=legendsize)
+            #plt.tight_layout()
         # Removal of next point (beware of weird behaviour in middle range)
         # lstSqErrs = np.subtract(y, yPred) ** 2
         # if len(y) % 2 == 0:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2:].sum()
         # else:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2 + 1:].sum()
         # if lowBoundErrSum > upBoundErrSum: firstPointIdx += 1
@@ -294,30 +310,30 @@
                 firstPointIdx += 1
         if saveFig:
             boxCntDimsDir = f"{writeFileDir}/boxCntDims"
             if not isdir(boxCntDimsDir):
                 if not isdir(writeFileDir):
                     mkdir(writeFileDir)
                 mkdir(boxCntDimsDir)
-            plt.savefig(f"{boxCntDimsDir}/{npName}_boxCntDim.png")
+            plt.savefig(f"{boxCntDimsDir}/{npName}_boxCntDim.png", bbox_inches='tight')
         if showPlot:
             plt.show()
         r2scorePrev, boxCntDimPrev, slopeCIPrev = r2score, boxCntDim, slopeCI
         if lenRange == 'full':
             break
     return r2score, boxCntDim, slopeCI
 
 
 # @annotate('runCase', color='cyan')
 # @estDuration
 def runBoxCnt(xyzFilePath, 
               radType='atomic', calcBL=False, findSurfOption='alphaShape', alphaMult=2.0,
               writeFileDir='boxCntOutputs', lenRange='trim', minSampleNum=5, confLvl=95, 
-              rmInSurf=True, vis=True, saveFig=False, showPlot=False, verbose=False,
-              runPointCloudBoxCnt=True, numPoints=300, gridNum=1024, exeDir='../bin', procUnit='cpu', genPCD=False,
+              rmInSurf=True, vis=True, figType='article', saveFig=False, showPlot=False, verbose=False,
+              runPointCloudBoxCnt=True, numPoints=300, gridNum=1024, exePath='$FASTBC_EXE', genPCD=False,
               runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, writeBox=True, 
               boxLenConc=False, maxWorkers=2):
     """
     Run box-counting algorithm on the surface of a given object consisting of a set of spheres represented as either
     point clouds or exact spherical surface.
     
     Parameters
@@ -342,30 +358,30 @@
         Minimum number of box count data points to be retained for slope estimation from the linear regression fitting.
     confLvl : Union[int, float], optional
         Confidence level of confidence interval in percentage.
     rmInSurf : bool, optional
         Whether to remove the surface points on the inner surface.
     vis : bool, optional
         Whether to generate output files for visualisation.
+    figType : {'article', 'poster', 'ppt'}
+        Type of figures to be generated.
     saveFig : bool, optional
         Whether to save the plots generated, only used if 'vis' is True.
     showPlot : bool, optional
         Whether to show the plots generated, only used if 'vis' is True.
     verbose : bool, optional
         Whether to display the details.
     runPointCloudBoxCnt : bool, optional
         Whether to represent the surface as point clouds.
     numPoints : int, optional
         Number of surface points to be generated around each atom.
     gridNum : int, optional
         Resolution of the 3D binary image.
-    exeDir : str, optional
+    exePath : str, optional
         Path to the compiled C++ executable for box-counting.
-    procUnit : {'cpu', 'gpu'}
-        Type of C++ executable to run for box-counting.
     genPCD : bool, optional
         Whether to generate pcd file for box-counting using MATLAB code written by Kazuaki Iida.
     runExactSphereBoxCnt : bool, optional
         Whether to represent the surface as exact spheres.
     minLenMult : float, optional
         Multiplier to the minimum radii to determine the minimum box length for box-counting dimension estimation.
     maxLenMult : float, optional
@@ -409,26 +425,26 @@
 
     r2PC, bcDimPC, confIntPC = np.nan, np.nan, (np.nan, np.nan)
     r2ES, bcDimES, confIntES = np.nan, np.nan, (np.nan, np.nan)
     if not isdir(writeFileDir):
         mkdir(writeFileDir)
     if runPointCloudBoxCnt:
         scalesPC, countsPC = getVoxelBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-                                             testCase, writeFileDir, exeDir, procUnit,
+                                             testCase, writeFileDir, exePath,
                                              radType, numPoints, gridNum,
                                              rmInSurf, vis, verbose, genPCD)
         r2PC, bcDimPC, confIntPC = findSlope(scalesPC, countsPC, f"{testCase}_PC", writeFileDir, lenRange,
-                                             minSampleNum, confLvl, vis, saveFig, showPlot)
+                                             minSampleNum, confLvl, vis, figType, saveFig, showPlot)
     if runExactSphereBoxCnt:
         minAtomRad = atomsRad.min()
         scalesES, countsES = getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                                               maxRange, (minAtomRad * minLenMult, minAtomRad * maxLenMult),
                                               minXYZ, testCase, writeFileDir, numBoxLenSample,
                                               rmInSurf, writeBox, verbose, boxLenConc, maxWorkers)
         r2ES, bcDimES, confIntES = findSlope(scalesES, countsES, f"{testCase}_ES", writeFileDir, lenRange,
-                                             minSampleNum, confLvl, vis, saveFig, showPlot)
+                                             minSampleNum, confLvl, vis, figType, saveFig, showPlot)
     if verbose:
         if runPointCloudBoxCnt:
             print(f"  Point clouds  D_Box: {bcDimPC:.4f} [{confIntPC[0]:.4f}, {confIntPC[1]:.4f}],  R2: {r2PC:.4f}")
         if runExactSphereBoxCnt:
             print(f"  Exact surface D_Box: {bcDimES:.4f} [{confIntES[0]:.4f}, {confIntES[1]:.4f}],  R2: {r2ES:.4f}")
     return r2PC, bcDimPC, confIntPC, r2ES, bcDimES, confIntES
```

### Comparing `sphractal-0.4.4/src/sphractal/constants.py` & `sphractal-0.6.0/src/sphractal/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,7 +35,11 @@
     'Hf': 1.59, 'Ta': 1.46, 'W': 1.39, 'Re': 1.37, 'Os': 1.35, 'Ir': 1.355, 'Pt': 1.385, 'Au': 1.44, 'Hg': 1.51,
     'Tl': 1.70, 'Pb': defRad, 'Bi': defRad, 'Po': defRad, 'At': defRad, 'Rn': defRad, 'Fr': defRad, 'Ra': defRad,
     'Ac': defRad, 'Th': 1.79, 'Pa': 1.63, 'U': 1.56, 'Np': 1.55, 'Pu': 1.59, 'Am': 1.73, 'Cm': 1.74, 'Bk': 1.70,
     'Cf': 1.86, 'Es': 1.86, 'Fm': defRad, 'Md': defRad, 'No': defRad, 'Lr': defRad, 'Rf': defRad, 'Db': defRad,
     'Sg': defRad, 'Bh': defRad, 'Hs': defRad, 'Mt': defRad, 'Ds': defRad, 'Rg': defRad, 'Cn': defRad, 'Nh': defRad,
     'Fl': defRad, 'Mc': defRad, 'Lv': defRad, 'Ts': defRad, 'Og': defRad
 }
+PLT_PARAMS = {'article': {'figsize': (3.5, 2.5), 'dpi': 300, 'fontsize': 'medium', 'labelsize': 'small', 'legendsize': 'x-small', 'linewidth': 0.5, 'markersize': 24}, 
+        'poster': {'figsize': (4.5, 3.5), 'dpi': 600, 'fontsize': 'x-large', 'labelsize': 'large', 'legendsize': 'medium', 'linewidth': 1.0, 'markersize': 48}, 
+        'ppt': {'figsize': (4, 3), 'dpi': 144, 'fontsize': 'large', 'labelsize': 'medium', 'legendsize': 'small', 'linewidth': 1.0, 'markersize': 36}}
+
```

### Comparing `sphractal-0.4.4/src/sphractal/data/example.xyz` & `sphractal-0.6.0/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.4/src/sphractal/surfExact.py` & `sphractal-0.6.0/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.4/src/sphractal/surfPointClouds.py` & `sphractal-0.6.0/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.4/src/sphractal/utils.py` & `sphractal-0.6.0/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.4/tests/fixtures.py` & `sphractal-0.6.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.4/tests/test_sphractal.py` & `sphractal-0.6.0/tests/test_sphractal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from math import dist
+from os import environ
 from os.path import exists, isdir, isfile
 from shutil import rmtree
 
 from pytest import approx, mark
 
 from fixtures import fixture, np, egAtomsXYZ, egAtomsNeighIdxs, egAtomsSurfIdxs, egTargetAtomIdxs
 from sphractal.datasets import getExampleDataPath
 from sphractal.utils import estDuration, getMinMaxXYZ, readXYZ, findNN, findSurf, calcDist, closestSurfAtoms, oppositeInnerAtoms
 from sphractal.surfPointClouds import fibonacciSphere, pointsOnAtom, pointsToVoxels
 from sphractal.surfExact import getNearFarCoord, scanBox, writeBoxCoords, findTargetAtoms
-from sphractal.boxCnt import getVoxelBoxCnts, getSphereBoxCnts, findSlope
-from sphractal import runBoxCnt
+from sphractal.boxCnt import getVoxelBoxCnts, getSphereBoxCnts, findSlope, runBoxCnt
 
 
 EG_XYZ_ATOM_NUM = 670
 ATOM_RAD = 1.69
 MAX_RANGE = 36.58499999999998
 
 
@@ -182,15 +182,14 @@
 #    assert len(innerSurfsAct) == numInnerPointsExp, 'Incorrect number of inner surface points'
 
 
 #@mark.parametrize('gridSize, numVoxelsExp', [(1024, 33204), (512, 33168), (256, 32888), (128, 29901), (64, 11329), (32, 3104)])
 #def test_pointsToVoxels(gridSize, numVoxelsExp, egPointXYZs):
 #    """Unit test of pointsToVoxels(). (To be implemented)"""
 #    voxelXYZs, voxelIdxs = pointsToVoxels(egPointXYZs, gridSize)
-#
 #    assert len(voxelIdxs) == numVoxelsExp, 'Incorrect number of voxels'
 
 
 #@mark.parametrize('scanBoxIdx, atomCoord', [(), (), ()])
 #def test_getNearFarCoord(scanBoxIdx, atomCoord, scanBoxNearFarExp):
 #    """Unit test of getNearFarCoord(). (To be implemented)"""
 #    scanBoxNearFarAct = getNearFarCoord(scanBoxIdx, scanBoxLen, lowBound, atomCoord)
@@ -228,28 +227,29 @@
 @mark.parametrize('confLvl, isFinite2', [(-101, False), (99.9, True), (100, False)])
 def test_findSlopeConfInt(minSampleNum, isFinite1, confLvl, isFinite2, egSphereBoxCnts):
     """Unit test of findSlope() outputs for different 'minSampleNum' and 'confLvl' values."""
     boxCntDimsAct = findSlope(egSphereBoxCnts[0], egSphereBoxCnts[1], minSampleNum=minSampleNum, confLvl=confLvl)
     assert np.all(np.isfinite(boxCntDimsAct[2])) == (isFinite1 and isFinite2), 'Incorrect confidence interval'
 
 
-#@mark.parametrize('scales, counts, boxCntDimsExp', [([-2.70926996, -2.40823997, -2.10720997, -1.80617997, -1.50514998, -1.20411998, -0.90308999, -0.60205999, -0.30103], [0.90308999, 1.50514998, 2.30963017, 2.91855453, 3.49192171, 4.05419158, 4.47568571, 4.51703746, 4.52071928], (0.99646974, 2.11889159, np.array((1.94381059, 2.29397261)))), ([-0.23688234, -0.16309612, -0.10004438, -0.03477764, 0.03932408, 0.10260591, 0.17060299, 0.24023892, 0.30488175, 0.37314659], [3.20194306, 3.32139128, 3.5171959 , 3.68142216, 3.80522891, 3.9531796 , 4.09272064, 4.27207379, 4.38937875, 4.52953301], (0.99660096, 2.24426950, np.array((2.11334077, 2.37519824))))])
-#def test_findSlopeAcc(scales, counts, boxCntDimsExp):
-#    """Unit test of findSlope() outputs accuracy."""
-#    boxCntDimsAct = findSlope(scales, counts)
-#    assert isinstance(boxCntDimsAct[2], np.ndarray), 'Confidence interval returned is not ndarray'
-#    assert len(boxCntDimsAct[2]) == 2, 'Confidence interval returned is not two numbers'
-#    assert np.all(boxCntDimsAct[2] == approx(boxCntDimsExp[2])), 'Incorrect estimation of box-counting dimensions by findSlope()'
-#    assert boxCntDimsAct[:2] == approx(boxCntDimsExp[:2]), 'Incorrect estimation of box-counting dimensions by findSlope()'
+@mark.parametrize('scales, counts, boxCntDimsExp', [([-2.70926996, -2.40823997, -2.10720997, -1.80617997, -1.50514998, -1.20411998, -0.90308999, -0.60205999, -0.30103], [0.90308999, 1.50514998, 2.30963017, 2.91855453, 3.49192171, 4.05419158, 4.47568571, 4.51703746, 4.52071928], (0.99646974, 2.11889159, np.array((1.94381059, 2.29397261)))), ([-0.23688234, -0.16309612, -0.10004438, -0.03477764, 0.03932408, 0.10260591, 0.17060299, 0.24023892, 0.30488175, 0.37314659], [3.20194306, 3.32139128, 3.5171959 , 3.68142216, 3.80522891, 3.9531796 , 4.09272064, 4.27207379, 4.38937875, 4.52953301], (0.99660096, 2.24426950, np.array((2.11334077, 2.37519824))))])
+def test_findSlopeAcc(scales, counts, boxCntDimsExp):
+    """Unit test of findSlope() outputs accuracy."""
+    boxCntDimsAct = findSlope(scales, counts)
+    assert isinstance(boxCntDimsAct[2], np.ndarray), 'Confidence interval returned is not ndarray'
+    assert len(boxCntDimsAct[2]) == 2, 'Confidence interval returned is not two numbers'
+    assert np.all(boxCntDimsAct[2] == approx(boxCntDimsExp[2])), 'Incorrect estimation of box-counting dimensions by findSlope()'
+    assert boxCntDimsAct[:2] == approx(boxCntDimsExp[:2]), 'Incorrect estimation of box-counting dimensions by findSlope()'
 
 
 #def test_getVoxelBoxCntVis(egAtomsEle, egAtomsRad, egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs):
-#    """Unit test of getVoxelBoxCnts() functionalities to generate output files for visualisation."""
+#    """Unit test of getVoxelBoxCnts() functionalities to generate output files for visualisation (To be uncommented when compiled C++ code could be shipped together)."""
+#    assert isfile(os.environ['FASTBC_EXE']), 'Executable not found at FASTBC_EXE'
 #    voxelScalesAct, voxelCountsAct = getVoxelBoxCnts(egAtomsEle, egAtomsRad, egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs,
-#                                                     'example', 'tests/boxCntOutputs', 'bin', verbose=True, genPCD=True)
+#                                                     'example', 'tests/boxCntOutputs', verbose=True, genPCD=True)
 #    assert exists('./tests/boxCntOutputs/surfVoxelIdxs.txt'), 'surfVoxelBoxIdxs.txt is not found'
 #    assert isfile('./tests/boxCntOutputs/surfVoxelIdxs.txt'), 'surfVoxelBoxIdxs.txt is a file'
 #    assert exists('./tests/boxCntOutputs/surfVoxelBoxCnts.txt'), 'surfVoxelBoxCnts is not found'
 #    assert isfile('./tests/boxCntOutputs/surfVoxelBoxCnts.txt'), 'surfVoxelBoxCnts is not a file'
 #    assert exists('./tests/boxCntOutputs/surfPoints/example_surfPoints.xyz'), 'example_surfPoints.xyz is not found'
 #    assert isfile('./tests/boxCntOutputs/surfPoints/example_surfPoints.xyz'), 'example_surfPoints.xyz is not a file'
 #    assert exists('./tests/boxCntOutputs/surfPoints/example_surfPoints.pcd'), 'example_surfPoints.pcd is not found'
@@ -258,17 +258,17 @@
 #    assert isfile('./tests/boxCntOutputs/surfVoxels/example_surfVoxels.xyz'), 'example_surfVoxels.xyz is not a file'
 #    if isdir('./tests/boxCntOutputs'):
 #        rmtree('./tests/boxCntOutputs')
 
 
 #@mark.parametrize('rmInSurf, voxelScalesExp, voxelCountsExp', [(True, [-2.70926996, -2.40823997, -2.10720997, -1.80617997, -1.50514998, -1.20411998, -0.90308999, -0.60205999, -0.30103], [0.90308999, 1.50514998, 2.30963017, 2.91855453, 3.49192171, 4.05419158, 4.47568571, 4.51703746, 4.52071928]), (False, [-2.70926996, -2.40823997, -2.10720997, -1.80617997, -1.50514998, -1.20411998, -0.90308999, -0.60205999, -0.30103], [0.90308999, 1.50514998, 2.35024802, 3.02530587, 3.62479758, 4.14640714, 4.54740546, 4.5884958, 4.59508819])])
 #def test_getVoxelBoxCntAcc(rmInSurf, voxelScalesExp, voxelCountsExp, egAtomsEle, egAtomsRad, egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs):
-#    """Unit test of getVoxelBoxCnts() outputs accuracy."""
+#    """Unit test of getVoxelBoxCnts() outputs accuracy (To be uncommented when compiled C++ code could be shipped together)."""
 #    voxelScalesAct, voxelCountsAct = getVoxelBoxCnts(egAtomsEle, egAtomsRad, egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs,
-#                                                     'example', 'tests/boxCntOutputs', 'bin', rmInSurf=rmInSurf, vis=False)
+#                                                     'example', 'tests/boxCntOutputs', rmInSurf=rmInSurf, vis=False)
 #    assert voxelScalesAct == approx(voxelScalesExp), 'Incorrect scales'
 #    assert voxelCountsAct == approx(voxelCountsExp), 'Incorrect box counts'
 
 
 @mark.parametrize('rmInSurf, sphereScalesExp, sphereCountsExp', [(True, [-0.23688234, -0.16309612, -0.10004438, -0.03477764, 0.03932408, 0.10260591, 0.17060299, 0.24023892, 0.30488175, 0.37314659], [3.20194306, 3.32139128, 3.5171959, 3.68142216, 3.80522891, 3.9531796, 4.09272064, 4.27207379, 4.38937875, 4.52953301]), (False, [-0.23688234, -0.16309612, -0.10004438, -0.03477764, 0.03932408, 0.10260591, 0.17060299, 0.24023892, 0.30488175, 0.37314659], [3.13289977, 3.35024802, 3.50920252, 3.66482994, 3.85564028, 4.01249978, 4.16524433, 4.31234664, 4.44814957, 4.58442169])])
 def test_getSphereBoxCnt(rmInSurf, sphereScalesExp, sphereCountsExp, egAtomsEle, egAtomsRad, egAtomsSurfIdxs, egAtomsXYZ, egAtomsNeighIdxs, egMinMaxXYZ):
     """Unit test of getSphereBoxCnts()."""
@@ -279,16 +279,17 @@
     assert exists('./tests/boxCntOutputs/boxCoords/example_boxCoords.xyz'), 'example_boxCoords.xyz is not found'
     assert isfile('./tests/boxCntOutputs/boxCoords/example_boxCoords.xyz'), 'example_boxCoords.xyz is not a file'
     if isdir('./tests/boxCntOutputs'):
         rmtree('./tests/boxCntOutputs')
 
 
 #def test_runBoxCnt(egVoxelBoxCntDims, egSphereBoxCntDims):
-#    """Unit and regression test of runBoxCnt()."""
-#    boxCntDimsAct = runBoxCnt(getExampleDataPath(), writeFileDir='tests/boxCntOutputs', runPointCloudBoxCnt=True, exeDir='bin', runExactSphereBoxCnt=True)
+#    """Unit and regression test of runBoxCnt() (To be uncommented when compiled C++ code could be shipped together)."""
+#    assert isfile(os.environ['FASTBC_EXE']), 'Executable not found at FASTBC_EXE'
+#    boxCntDimsAct = runBoxCnt(getExampleDataPath(), writeFileDir='tests/boxCntOutputs')
 #    assert boxCntDimsAct[:2] == approx(egVoxelBoxCntDims[:2]), 'Incorrect R2 and D_Box for point clouds representation'
 #    assert boxCntDimsAct[2] == approx(egVoxelBoxCntDims[2]), 'Incorrect confidence interval for point clouds representation'
 #    assert boxCntDimsAct[-3:-1] == approx(egSphereBoxCntDims[:2]), 'Incorrect R2 and D_Box for exact surface representation'
 #    assert boxCntDimsAct[-1] == approx(egSphereBoxCntDims[2]), 'Incorrect confidence interval for exact surface representation'
 #    if isdir('./tests/boxCntOutputs'):
 #        rmtree('./tests/boxCntOutputs')
```

### Comparing `sphractal-0.4.4/PKG-INFO` & `sphractal-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.4.4
+Version: 0.6.0
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: numba (>=0.57.1)
 Requires-Dist: numpy (>=1.22,<1.25)
-Requires-Dist: scipy (>=1.11.0) ; python_version >= "3.9" and python_version < "3.13"
+Requires-Dist: scipy (>=1.11.1) ; python_version >= "3.9" and python_version < "3.13"
 Requires-Dist: statsmodels (>=0.14.0)
 Project-URL: Documentation, https://sphractal.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Jon-Ting/sphractal
 Description-Content-Type: text/markdown
 
 # Sphractal
 
@@ -35,64 +35,58 @@
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Current
-* Representation of the surface as either point clouds (feature yet to be made available due to C++ compilation issues) or exact surfaces.
+* Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
-### To be Done
-* Set path for exeDir.
-* Publish to Conda.
-  * cd condaForge/
-  * conda skeleton pypi sphractal
-  * vim sphractal/meta.yaml ('name', 'version', 'git_rev', 'git_url', 'imports', 'home', 'noarch', 'maintainer')
-  * vim build.sh
-  * vim bld.bat
-  * conda-build sphractal (record path)
-  * conda install --use-local sphractal
-  * conda list
-  * anaconda login
-  * anaconda upload PATH_TO_BZ2
-  * conda config --set anaconda_upload yes
-  * anaconda logout
-* Nested multiprocessing.
-* Better looking plots, allow figure size to be specified, allow choice for 'paper' and 'presentation'.
-* Consider transforming xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
+### Under Development
+* Nested multiprocessing (boxLenConc=True).
+* Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
+* Integration of C++ code for point cloud surface representation into the package.
 
 ## Installation
 
-Use `pip` or `conda` (yet to be implemented) to install `Sphractal`:
+Use `pip` or `conda` to install `Sphractal`:
 
 ```bash
 $ pip install sphractal
 ```
 ```bash
 $ conda install -c conda-forge sphractal
 ```
 
-`Sphractal` requires a C++ code to be compiled for the functionalities related to point clouds surface representation 
-to work. This could be done by first changing into the director containing the C++ source code: 
+### Special Requirement for Point Cloud Surface Representation
+`Sphractal` requires an executable compiled from another freely available repository for the functionalities related 
+to point clouds surface representation to operate properly. 
 
+This could be done by:
+
+* Downloading the source code from the [repository](https://github.com/Jon-Ting/fastBC.git) to a directory of your choice:
 ```bash
-$ cd {SPHRACTAL_DIR_PATH}/src/fbc/
+git clone https://github.com/Jon-Ting/fastBC.git
 ```
 
-And then compile either of the two file using respective C++ compiler. 
-The second option is only viable for machines with `CUDA` platform available.
-
+* Building an executable by doing either one of the following compilations according to the instructions on the [README.md](https://github.com/Jon-Ting/fastBC/blob/main/README.md) page. This will decide whether you will be running the box counting algorithm with GPU acceleration. Feel free to rename the executables to any other sensible names:
 ```bash
-$ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o {SPHRACTAL_DIR_PATH}/bin/3DbinImBCcpu.exe
+$ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o 3DbinImBCcpu.exe
 ```
 ```bash
-$ nvcc -O3 bcCUDA3D.cu 3DbinImBCgpu.cpp -o {SPHRACTAL_DIR_PATH}/bin/3DbinImBCgpu.exe
+$ nvcc -O3 3DbinImBCgpu.cpp bcCUDA3D.cu -o 3DbinImBCgpu.exe
+```
+
+* (Optional) Setting the path to the executable as an environment variable accessible by Python (replace `PATH_TO_EXE` by the absolute path to the executable file you just built), otherwise you could always pass the path to the executable to the relevant functions:
+```bash
+$ export FASTBC_EXE={PATH_TO_EXE}
 ```
+Note that for the environment variable to be persistent (to still exist after the terminal is closed), the line should be added to your `~/.bashrc`.
 
 ## Usage
 
 ```python
 from sphractal import getExampleDataPath, runBoxCnt
 
 xyzFilePath = getExampleDataPath()  # Replace with the path to your xyz or lmp file
```

