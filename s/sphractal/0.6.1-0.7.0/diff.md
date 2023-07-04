# Comparing `tmp/sphractal-0.6.1.tar.gz` & `tmp/sphractal-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.6.1.tar", max compression
+gzip compressed data, was "sphractal-0.7.0.tar", max compression
```

## Comparing `sphractal-0.6.1.tar` & `sphractal-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-04 06:37:07.800645 sphractal-0.6.1/LICENSE
--rw-r--r--   0        0        0     4059 2023-07-04 06:37:07.800645 sphractal-0.6.1/README.md
--rw-r--r--   0        0        0     2056 2023-07-04 06:37:57.708943 sphractal-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-04 06:37:57.708943 sphractal-0.6.1/setup.py
--rw-r--r--   0        0        0     1406 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/__init__.py
--rw-r--r--   0        0        0    22919 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4302 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      279 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/datasets.py
--rw-r--r--   0        0        0      405 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/pybind11/example.cpp
--rw-r--r--   0        0        0     2520 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/pybind11/pybindtest.cpp
--rw-r--r--   0        0        0     8881 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8119 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11480 2023-07-04 06:37:07.872645 sphractal-0.6.1/src/sphractal/utils.py
--rw-r--r--   0        0        0    94223 2023-07-04 06:37:07.872645 sphractal-0.6.1/tests/fixtures.py
--rw-r--r--   0        0        0    17688 2023-07-04 06:37:07.872645 sphractal-0.6.1/tests/test_sphractal.py
--rw-r--r--   0        0        0     5328 1970-01-01 00:00:00.000000 sphractal-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-04 16:13:08.575564 sphractal-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4015 2023-07-04 16:13:08.575564 sphractal-0.7.0/README.md
+-rw-r--r--   0        0        0     2056 2023-07-04 16:13:49.076139 sphractal-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-04 16:13:49.076139 sphractal-0.7.0/setup.py
+-rw-r--r--   0        0        0     1406 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    22696 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4302 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      279 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8953 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8119 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11480 2023-07-04 16:13:08.635565 sphractal-0.7.0/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94223 2023-07-04 16:13:08.635565 sphractal-0.7.0/tests/fixtures.py
+-rw-r--r--   0        0        0    17688 2023-07-04 16:13:08.635565 sphractal-0.7.0/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sphractal-0.7.0/PKG-INFO
```

### Comparing `sphractal-0.6.1/LICENSE` & `sphractal-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/README.md` & `sphractal-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 ### Aims
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### Under Development
-* Nested multiprocessing (boxLenConc=True).
 * Optional input argument of surface atoms (to guarantee accurate box counts).
 * Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 * Integration of C++ code for point cloud surface representation into the package.
 
 ## Installation
 
 Use `pip` or `conda` to install `Sphractal`:
```

### Comparing `sphractal-0.6.1/pyproject.toml` & `sphractal-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.6.1"
+version = "0.7.0"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.6.1/setup.py` & `sphractal-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.6.1'
+__version__ = '0.7.0'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.6.1/src/sphractal/__init__.py` & `sphractal-0.7.0/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/src/sphractal/boxCnt.py` & `sphractal-0.7.0/src/sphractal/boxCnt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from concurrent.futures import ProcessPoolExecutor as Pool
-from math import log10
+from math import ceil, log10
+from multiprocessing import cpu_count
 from os import mkdir, system
 from os.path import isdir
 from warnings import warn
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 import numpy as np
@@ -104,15 +105,15 @@
             counts.append(log10(int(line.split()[1])))
     return scales[::-1], counts[::-1]
 
 
 # @annotate('getSphereBoxCnts', color='blue')
 def getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                      maxRange, minMaxBoxLens, minXYZ, npName, writeFileDir='boxCntOutputs', numBoxLenSample=10,
-                     rmInSurf=True, writeBox=True, verbose=False, boxLenConc=False, maxWorkers=2):
+                     rmInSurf=True, writeBox=True, verbose=False):
     """
     Count the boxes that cover the outer surface of a set of overlapping spheres represented as exact spheres for
     different box sizes.
     
     Parameters
     ----------
     atomsEle : 1D ndarray
@@ -139,19 +140,14 @@
         Number of box lengths to use for the collection of the box count data, spaced evenly on logarithmic scale.
     rmInSurf : bool, optional
         Whether to remove the surface points on the inner surface.
     writeBox : bool, optional
         Whether to generate output files for visualisation.
     verbose : bool, optional
         Whether to display the details.
-    boxLenConc : bool, optional
-        Whether to parallelise the box-counting across different box lengths (under development, stick to default for now).
-    maxWorkers : int, optional
-        Maximum number of processes to spawn for parallelisation of box-counting across different box lengths, only used
-        if 'boxLenConc' is True.
     
     Returns
     -------
     scales : list
         Box lengths.
     counts : list
         Number of boxes that cover the exact spherical surface of interest.
@@ -159,47 +155,53 @@
     Examples
     --------
     >>> eles, rads, xyzs, _, minxyz, maxxyz = readXYZ('example.xyz')
     >>> neighs, _ = findNN(rads, xyzs, minxyz, maxxyz, 1.2)
     >>> surfs = findSurf(xyzs, neighs, 'alphaShape', 2.0)
     >>> scales, counts = getSphereBoxCnts(eles, rads, surfs, xyzs, neighs, 100, (0.2, 1), minxyz, 'example')
     """
+    atomsIdxs = atomsSurfIdxs if rmInSurf else findTargetAtoms(atomsNeighIdxs)
+    numCPUs = cpu_count()
+    boxLenScanMaxWorkers = ceil(numCPUs * numBoxLenSample / len(atomsIdxs))
+    boxLenConc = False if boxLenScanMaxWorkers < 2 else True
+    atomScanMaxWorkers = numCPUs - boxLenScanMaxWorkers if boxLenConc else numCPUs
+
     if verbose:
         print(f"  Representing the surface by treating each atom as exact spheres...")
+        print(f"  Parallelised with {atomScanMaxWorkers} out of {numCPUs} cores for scanning over atoms, the rest over box lengths...")
         print(f"    (1/eps)    (# bulk)    (# surf)")
     if writeBox:
         if not isdir(writeFileDir):
             mkdir(writeFileDir)
 
-    atomsIdxs = atomsSurfIdxs if rmInSurf else findTargetAtoms(atomsNeighIdxs)
     overallBoxLen = maxRange + MIN_VAL_FROM_BOUND * 2
     allLensSurfBoxs, allLensBulkBoxs, allLensSurfCnts, allLensBulkCnts = [], [], [], []
     scales, scanBoxLens, scanAllAtomsInps = [], [], []
     approxScanBoxLens = np.geomspace(minMaxBoxLens[1], minMaxBoxLens[0], num=numBoxLenSample)
     for approxScanBoxLen in approxScanBoxLens:  # Evenly reduced box lengths on log scale
         magnFac = int(overallBoxLen / approxScanBoxLen)
         scanBoxLen = overallBoxLen / magnFac
         scanAllAtomsInp = (magnFac, scanBoxLen, atomsIdxs, minXYZ,
                            atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, 
-                           rmInSurf, verbose)
+                           rmInSurf, verbose, atomScanMaxWorkers)
         if boxLenConc:
             scanAllAtomsInps.append(scanAllAtomsInp) 
         else:
             scanAllAtomsResult = scanAllAtoms(scanAllAtomsInp) 
             allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
             allLensSurfBoxs.append(allAtomsSurfBoxs)
             allLensBulkBoxs.append(allAtomsBulkBoxs)
             allLensSurfCnts.append(len(allAtomsSurfBoxs))
 
         scales.append(log10(magnFac / overallBoxLen))
         scanBoxLens.append(scanBoxLen)
 
     if boxLenConc:
-        with Pool(max_workers=maxWorkers) as pool:
-            for scanAllAtomsResult in pool.map(scanAllAtoms, scanAllAtomsInps):
+        with Pool(max_workers=boxLenScanMaxWorkers) as pool:
+            for scanAllAtomsResult in pool.map(scanAllAtoms, scanAllAtomsInps, chunksize=ceil(numBoxLenSample / boxLenScanMaxWorkers)):
                 allAtomsSurfBoxs, allAtomsBulkBoxs = scanAllAtomsResult
                 allLensSurfBoxs.append(allAtomsSurfBoxs)
                 allLensBulkBoxs.append(allAtomsBulkBoxs)
                 allLensSurfCnts.append(len(allAtomsSurfBoxs))
     counts = [log10(sCnt) if sCnt != 0 else np.nan for sCnt in allLensSurfCnts]
 
     if writeBox:
@@ -336,16 +338,15 @@
 # @annotate('runCase', color='cyan')
 # @estDuration
 def runBoxCnt(xyzFilePath, 
               radType='atomic', calcBL=False, findSurfOption='alphaShape', alphaMult=2.0,
               writeFileDir='boxCntOutputs', lenRange='trim', minSampleNum=5, confLvl=95, 
               rmInSurf=True, vis=True, figType='article', saveFig=False, showPlot=False, verbose=False,
               runPointCloudBoxCnt=True, numPoints=300, gridNum=1024, exePath='$FASTBC_EXE', genPCD=False,
-              runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, writeBox=True, 
-              boxLenConc=False, maxWorkers=2):
+              runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, writeBox=True): 
     """
     Run box-counting algorithm on the surface of a given object consisting of a set of spheres represented as either
     point clouds or exact spherical surface.
     
     Parameters
     ----------
     xyzFilePath : str
@@ -396,19 +397,14 @@
         Multiplier to the minimum radii to determine the minimum box length for box-counting dimension estimation.
     maxLenMult : float, optional
         Multiplier to the minimum radii to determine the maximum box length for box-counting dimension estimation.
     numBoxLenSample : int, optional
         Number of box lengths to use for the collection of the box count data, spaced evenly on logarithmic scale.
     writeBox : bool, optional
         Whether to generate output files for visualisation.
-    boxLenConc : bool, optional
-        Whether to parallelise the box-counting across different box lengths.
-    maxWorkers : int, optional
-        Maximum number of processes to spawn for parallelisation of box-counting across different box sizes, only used
-        if 'boxLenConc' is True.
     
     Returns
     -------
     r2PC : float
         Coefficient of determination from determination of the dimension of point clouds surface.
     bcDimPC : float
         Box-counting dimension of the point clouds representation of the surface.
@@ -445,15 +441,15 @@
         r2PC, bcDimPC, confIntPC = findSlope(scalesPC, countsPC, f"{testCase}_PC", writeFileDir, lenRange,
                                              minSampleNum, confLvl, vis, figType, saveFig, showPlot)
     if runExactSphereBoxCnt:
         minAtomRad = atomsRad.min()
         scalesES, countsES = getSphereBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                                               maxRange, (minAtomRad * minLenMult, minAtomRad * maxLenMult),
                                               minXYZ, testCase, writeFileDir, numBoxLenSample,
-                                              rmInSurf, writeBox, verbose, boxLenConc, maxWorkers)
+                                              rmInSurf, writeBox, verbose)
         r2ES, bcDimES, confIntES = findSlope(scalesES, countsES, f"{testCase}_ES", writeFileDir, lenRange,
                                              minSampleNum, confLvl, vis, figType, saveFig, showPlot)
     if verbose:
         if runPointCloudBoxCnt:
             print(f"  Point clouds  D_Box: {bcDimPC:.4f} [{confIntPC[0]:.4f}, {confIntPC[1]:.4f}],  R2: {r2PC:.4f}")
         if runExactSphereBoxCnt:
             print(f"  Exact surface D_Box: {bcDimES:.4f} [{confIntES[0]:.4f}, {confIntES[1]:.4f}],  R2: {r2ES:.4f}")
```

### Comparing `sphractal-0.6.1/src/sphractal/constants.py` & `sphractal-0.7.0/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/src/sphractal/data/example.xyz` & `sphractal-0.7.0/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/src/sphractal/surfExact.py` & `sphractal-0.7.0/src/sphractal/surfExact.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,25 +119,25 @@
         allAtomsBulkBoxs.extend(atomBulkBoxs)
     return allAtomsSurfBoxs, allAtomsBulkBoxs
 
 
 # @annotate('scanAllAtoms', color='magenta')
 def scanAllAtoms(args):
     """Count the number of boxes that cover the outer spherical surface of a set of atoms for a given box size."""
-    magnFac, scanBoxLen, atomsIdxs, minXYZ, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf, verbose = args
+    magnFac, scanBoxLen, atomsIdxs, minXYZ, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf, verbose, maxWorkers = args
     scanAtomInps = [(magnFac, scanBoxLen, minXYZ, atomIdx, atomsRad[atomIdx],
                      atomsSurfIdxs, atomsXYZ, atomsNeighIdxs, rmInSurf) for atomIdx in atomsIdxs]
     allAtomsSurfBoxs, allAtomsBulkBoxs = [], []
-    with Pool() as pool:
-        for scanAtomResult in pool.map(scanAtom, scanAtomInps):
+    with Pool(max_workers=maxWorkers) as pool:
+        for scanAtomResult in pool.map(scanAtom, scanAtomInps, chunksize=ceil(len(atomsIdxs) / maxWorkers)):
             allAtomsSurfBoxs.extend(scanAtomResult[0])
             allAtomsBulkBoxs.extend(scanAtomResult[1])
-    # allAtomsSurfBoxs, allAtomsBulkBoxs = scanAtomsForLoop(atomsIdxs, magnFac, scanBoxLen, minXYZ,
-    #                                                         atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
-    #                                                         rmInSurf)
+    #allAtomsSurfBoxs, allAtomsBulkBoxs = scanAtomsForLoop(atomsIdxs, magnFac, scanBoxLen, minXYZ,
+    #                                                      atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
+    #                                                      rmInSurf)
     allAtomsSurfBoxs, allAtomsBulkBoxs = set(allAtomsSurfBoxs), set(allAtomsBulkBoxs)
     allAtomsSurfBoxs.difference_update(allAtomsBulkBoxs)
 
     if verbose:
         epsInvStr = f"{1 / scanBoxLen:.2f}"
         print(f"{epsInvStr.rjust(10)}{str(len(allAtomsBulkBoxs)).rjust(12)}{str(len(allAtomsSurfBoxs)).rjust(12)}")
     return allAtomsSurfBoxs, allAtomsBulkBoxs
```

### Comparing `sphractal-0.6.1/src/sphractal/surfPointClouds.py` & `sphractal-0.7.0/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/src/sphractal/utils.py` & `sphractal-0.7.0/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/tests/fixtures.py` & `sphractal-0.7.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/tests/test_sphractal.py` & `sphractal-0.7.0/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.1/PKG-INFO` & `sphractal-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.6.1
+Version: 0.7.0
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
@@ -40,15 +40,14 @@
 
 ### Aims
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### Under Development
-* Nested multiprocessing (boxLenConc=True).
 * Optional input argument of surface atoms (to guarantee accurate box counts).
 * Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 * Integration of C++ code for point cloud surface representation into the package.
 
 ## Installation
 
 Use `pip` or `conda` to install `Sphractal`:
```

