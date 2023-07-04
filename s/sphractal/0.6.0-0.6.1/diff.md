# Comparing `tmp/sphractal-0.6.0.tar.gz` & `tmp/sphractal-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.6.0.tar", max compression
+gzip compressed data, was "sphractal-0.6.1.tar", max compression
```

## Comparing `sphractal-0.6.0.tar` & `sphractal-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2023-07-04 02:45:03.637258 sphractal-0.6.0/LICENSE
--rw-r--r--   0        0        0     3652 2023-07-04 02:45:03.637258 sphractal-0.6.0/README.md
--rw-r--r--   0        0        0     2056 2023-07-04 02:45:42.821337 sphractal-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-04 02:45:42.821337 sphractal-0.6.0/setup.py
--rw-r--r--   0        0        0     1406 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/__init__.py
--rw-r--r--   0        0        0    22847 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4302 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      279 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/datasets.py
--rw-r--r--   0        0        0      405 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/pybind11/example.cpp
--rw-r--r--   0        0        0     2520 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/pybind11/pybindtest.cpp
--rw-r--r--   0        0        0     8881 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8119 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11480 2023-07-04 02:45:03.697258 sphractal-0.6.0/src/sphractal/utils.py
--rw-r--r--   0        0        0    94223 2023-07-04 02:45:03.697258 sphractal-0.6.0/tests/fixtures.py
--rw-r--r--   0        0        0    17688 2023-07-04 02:45:03.697258 sphractal-0.6.0/tests/test_sphractal.py
--rw-r--r--   0        0        0     4921 1970-01-01 00:00:00.000000 sphractal-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-04 06:37:07.800645 sphractal-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4059 2023-07-04 06:37:07.800645 sphractal-0.6.1/README.md
+-rw-r--r--   0        0        0     2056 2023-07-04 06:37:57.708943 sphractal-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-04 06:37:57.708943 sphractal-0.6.1/setup.py
+-rw-r--r--   0        0        0     1406 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    22919 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4302 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      279 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/datasets.py
+-rw-r--r--   0        0        0      405 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/pybind11/example.cpp
+-rw-r--r--   0        0        0     2520 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/pybind11/pybindtest.cpp
+-rw-r--r--   0        0        0     8881 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8119 2023-07-04 06:37:07.868645 sphractal-0.6.1/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11480 2023-07-04 06:37:07.872645 sphractal-0.6.1/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94223 2023-07-04 06:37:07.872645 sphractal-0.6.1/tests/fixtures.py
+-rw-r--r--   0        0        0    17688 2023-07-04 06:37:07.872645 sphractal-0.6.1/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5328 1970-01-01 00:00:00.000000 sphractal-0.6.1/PKG-INFO
```

### Comparing `sphractal-0.6.0/LICENSE` & `sphractal-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/README.md` & `sphractal-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 ## Description
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
-### Current
+### Aims
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### Under Development
 * Nested multiprocessing (boxLenConc=True).
+* Optional input argument of surface atoms (to guarantee accurate box counts).
 * Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 * Integration of C++ code for point cloud surface representation into the package.
 
 ## Installation
 
 Use `pip` or `conda` to install `Sphractal`:
 
@@ -45,30 +46,30 @@
 ```bash
 $ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o 3DbinImBCcpu.exe
 ```
 ```bash
 $ nvcc -O3 3DbinImBCgpu.cpp bcCUDA3D.cu -o 3DbinImBCgpu.exe
 ```
 
-* (Optional) Setting the path to the executable as an environment variable accessible by Python (replace `PATH_TO_EXE` by the absolute path to the executable file you just built), otherwise you could always pass the path to the executable to the relevant functions:
+* (Optional) Setting the path to the executable as an environment variable accessible by Python (replace `<PATH_TO_EXE>` by the absolute path to the executable file you just built), otherwise you could always pass the path to the executable to the relevant functions:
 ```bash
-$ export FASTBC_EXE={PATH_TO_EXE}
+$ export FASTBC_EXE=<PATH_TO_EXE>
 ```
 Note that for the environment variable to be persistent (to still exist after the terminal is closed), the line should be added to your `~/.bashrc`.
 
 ## Usage
 
 ```python
 from sphractal import getExampleDataPath, runBoxCnt
 
 xyzFilePath = getExampleDataPath()  # Replace with the path to your xyz or lmp file
 boxCntResults = runBoxCnt(xyzFilePath)
 ```
 
-Check out the [notebook tutorial](example.ipynb) for more detailed examples!
+Check out the [notebook tutorial](https://github.com/Jon-Ting/sphractal/blob/main/docs/example.ipynb) for further explanations and demonstrations!
 
 ## Documentation
 
 Detailed documentation and usage examples are hosted by [Read the Docs](https://sphractal.readthedocs.io/en/latest/).
 
 ## Contributing
 
@@ -82,13 +83,14 @@
 
 The project is distributed under an [MIT License](https://github.com/Jon-Ting/sphractal/blob/main/LICENSE).
 
 ## Credits
 
 The package was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) using the 
 `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+The speeding up of the inner functions via just-in-time compilations with [Numba](https://numba.pydata.org/) was inspired by the advice received during the [NCI-NVIDIA Open Hackathon 2023](https://opus.nci.org.au/display/Help/NCI-NVIDIA+Open+Hackathon+2023).
 
 ## Contact
 
 Email: `Jonathan.Ting@anu.edu.au`/`jonting97@gmail.com`
 
 Feel free to reach out if you have any questions, suggestions, or feedback.
```

### Comparing `sphractal-0.6.0/pyproject.toml` & `sphractal-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.6.0"
+version = "0.6.1"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.6.0/setup.py` & `sphractal-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.6.0'
+__version__ = '0.6.1'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.6.0/src/sphractal/__init__.py` & `sphractal-0.6.1/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/src/sphractal/boxCnt.py` & `sphractal-0.6.1/src/sphractal/boxCnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,76 +252,86 @@
     if visReg:
         plt.rc('font', family='sans-serif')
         plt.rc('xtick', labelsize='x-small')
         plt.rc('ytick', labelsize='x-small')
         params = PLT_PARAMS[figType]
         figsize, dpi, fontsize, labelsize, legendsize, linewidth, markersize = params['figsize'], params['dpi'], params['fontsize'], params['labelsize'], params['legendsize'], params['linewidth'], params['markersize']
 
+    # Remove invalid entries in the box counts data collected
     while np.nan in counts:
         nanIdx = counts.index(np.nan)
         del counts[nanIdx]
         del scales[nanIdx]
-    firstPointIdx, lastPointIdx, removeSmallBoxes = 0, len(scales), True  # countChange.count(countChange[0])
 
     if abs(confLvl) > 100:
         warn(f"Confidence level out of range, confidence intervals are unreliable! 'confLvl' should be within [0, 100) instead of {confLvl}")
     alphaCI = 1 - confLvl/100
+
+    firstPointIdx, lastPointIdx, removeSmallBoxes = 0, len(scales), True
     r2score, boxCntDim, slopeCI, r2scorePrev, boxCntDimPrev, slopeCIPrev = 0.0, 0.0, np.array((np.inf, np.inf)), 0.0, 0.0, np.array((np.inf, np.inf))
     while len(scales[firstPointIdx:lastPointIdx]) > minSampleNum:
+
         x, y = scales[firstPointIdx:lastPointIdx], counts[firstPointIdx:lastPointIdx]
         regModel = OLS(endog=y, exog=add_constant(x)).fit()
         r2score, boxCntDim, slopeCI = regModel.rsquared, regModel.params[1], regModel.conf_int(alpha=alphaCI)[1]
         yPred = regModel.predict()  # Returns ndarray, allowing subtraction later
+
         if visReg:
             plt.close()
             fig = plt.figure(figsize=figsize, dpi=dpi)
             ax = fig.add_subplot(1, 1, 1)
             handleScatter = ax.scatter(x, y, marker='o', s=markersize, c='r', alpha=1, edgecolors='k', linewidths=1.2, zorder=3)
             handleBestFit = ax.plot(x, yPred, linestyle='-', linewidth=1., color='k', label='OLS')
             ax.grid(linestyle='dotted')
+
+            # Compute confidence bands
             predOLS = regModel.get_prediction()
             lowCIvals, upCIvals = predOLS.summary_frame()['mean_ci_lower'], predOLS.summary_frame()['mean_ci_upper']
             handleConfBand = ax.plot(x, upCIvals, linestyle='--', linewidth=linewidth, color='b')
             ax.plot(x, lowCIvals, linestyle='--', linewidth=linewidth, color='b')
             ax.fill_between(x, upCIvals, lowCIvals, alpha=0.2)
+
             ax.set_xlabel(r'log$(1/\epsilon)$', fontsize=labelsize)
             ax.set_ylabel(r'log$(N)$', fontsize=labelsize)
             ax.yaxis.set_major_formatter(FormatStrFormatter('% 1.1f'))
             ax.legend(handles=(handleScatter, handleBestFit[0], handleConfBand[0]), 
                       labels=('Actual box counts', fr"Best fit line ($R^2$: {r2score:.3f})", f"{confLvl}% confidence bands"), 
                       title=fr"$D_{{box}}$: {boxCntDim:.3f} [{slopeCI[0]:.3f}, {slopeCI[1]:.3f}]", title_fontsize=legendsize, 
                       fontsize=legendsize)
             #plt.tight_layout()
+
         # Removal of next point (beware of weird behaviour in middle range)
         # lstSqErrs = np.subtract(y, yPred) ** 2
         # if len(y) % 2 == 0:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2:].sum()
         # else:
         #     lowBoundErrSum, upBoundErrSum = lstSqErrs[:len(y) // 2].sum(), lstSqErrs[len(y) // 2 + 1:].sum()
         # if lowBoundErrSum > upBoundErrSum: firstPointIdx += 1
         # else: lastPointIdx -= 1
+
         if lenRange == 'trim':
             if removeSmallBoxes:
                 if round(r2score, 3) < round(r2scorePrev, 3):
                     removeSmallBoxes = False
                 lastPointIdx -= 1
             else:
                 if round(r2score, 3) < round(r2scorePrev, 3):
                     return r2scorePrev, boxCntDimPrev, slopeCIPrev
                 firstPointIdx += 1
+        r2scorePrev, boxCntDimPrev, slopeCIPrev = r2score, boxCntDim, slopeCI
+
         if saveFig:
             boxCntDimsDir = f"{writeFileDir}/boxCntDims"
             if not isdir(boxCntDimsDir):
                 if not isdir(writeFileDir):
                     mkdir(writeFileDir)
                 mkdir(boxCntDimsDir)
             plt.savefig(f"{boxCntDimsDir}/{npName}_boxCntDim.png", bbox_inches='tight')
         if showPlot:
             plt.show()
-        r2scorePrev, boxCntDimPrev, slopeCIPrev = r2score, boxCntDim, slopeCI
         if lenRange == 'full':
             break
     return r2score, boxCntDim, slopeCI
 
 
 # @annotate('runCase', color='cyan')
 # @estDuration
```

### Comparing `sphractal-0.6.0/src/sphractal/constants.py` & `sphractal-0.6.1/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/src/sphractal/data/example.xyz` & `sphractal-0.6.1/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/src/sphractal/pybind11/pybindtest.cpp` & `sphractal-0.6.1/src/sphractal/pybind11/pybindtest.cpp`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/src/sphractal/surfExact.py` & `sphractal-0.6.1/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/src/sphractal/surfPointClouds.py` & `sphractal-0.6.1/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/src/sphractal/utils.py` & `sphractal-0.6.1/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/tests/fixtures.py` & `sphractal-0.6.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/tests/test_sphractal.py` & `sphractal-0.6.1/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.6.0/PKG-INFO` & `sphractal-0.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.6.0
+Version: 0.6.1
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
@@ -34,21 +34,22 @@
 ## Description
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
-### Current
+### Aims
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### Under Development
 * Nested multiprocessing (boxLenConc=True).
+* Optional input argument of surface atoms (to guarantee accurate box counts).
 * Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 * Integration of C++ code for point cloud surface representation into the package.
 
 ## Installation
 
 Use `pip` or `conda` to install `Sphractal`:
 
@@ -74,30 +75,30 @@
 ```bash
 $ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o 3DbinImBCcpu.exe
 ```
 ```bash
 $ nvcc -O3 3DbinImBCgpu.cpp bcCUDA3D.cu -o 3DbinImBCgpu.exe
 ```
 
-* (Optional) Setting the path to the executable as an environment variable accessible by Python (replace `PATH_TO_EXE` by the absolute path to the executable file you just built), otherwise you could always pass the path to the executable to the relevant functions:
+* (Optional) Setting the path to the executable as an environment variable accessible by Python (replace `<PATH_TO_EXE>` by the absolute path to the executable file you just built), otherwise you could always pass the path to the executable to the relevant functions:
 ```bash
-$ export FASTBC_EXE={PATH_TO_EXE}
+$ export FASTBC_EXE=<PATH_TO_EXE>
 ```
 Note that for the environment variable to be persistent (to still exist after the terminal is closed), the line should be added to your `~/.bashrc`.
 
 ## Usage
 
 ```python
 from sphractal import getExampleDataPath, runBoxCnt
 
 xyzFilePath = getExampleDataPath()  # Replace with the path to your xyz or lmp file
 boxCntResults = runBoxCnt(xyzFilePath)
 ```
 
-Check out the [notebook tutorial](example.ipynb) for more detailed examples!
+Check out the [notebook tutorial](https://github.com/Jon-Ting/sphractal/blob/main/docs/example.ipynb) for further explanations and demonstrations!
 
 ## Documentation
 
 Detailed documentation and usage examples are hosted by [Read the Docs](https://sphractal.readthedocs.io/en/latest/).
 
 ## Contributing
 
@@ -111,14 +112,15 @@
 
 The project is distributed under an [MIT License](https://github.com/Jon-Ting/sphractal/blob/main/LICENSE).
 
 ## Credits
 
 The package was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) using the 
 `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+The speeding up of the inner functions via just-in-time compilations with [Numba](https://numba.pydata.org/) was inspired by the advice received during the [NCI-NVIDIA Open Hackathon 2023](https://opus.nci.org.au/display/Help/NCI-NVIDIA+Open+Hackathon+2023).
 
 ## Contact
 
 Email: `Jonathan.Ting@anu.edu.au`/`jonting97@gmail.com`
 
 Feel free to reach out if you have any questions, suggestions, or feedback.
```

