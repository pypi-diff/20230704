# Comparing `tmp/crtoolbox-0.1.5.tar.gz` & `tmp/crtoolbox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crtoolbox-0.1.5.tar", last modified: Mon Jul  3 16:44:34 2023, max compression
+gzip compressed data, was "dist/crtoolbox-0.1.6.tar", last modified: Tue Jul  4 13:15:42 2023, max compression
```

## Comparing `crtoolbox-0.1.5.tar` & `crtoolbox-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       32 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/MANIFEST.in
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      464 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/PKG-INFO
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/README.md
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/crtoolbox/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8117 2023-07-03 16:39:07.000000 crtoolbox-0.1.5/crtoolbox/bootstrap.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    14328 2023-07-03 16:38:57.000000 crtoolbox-0.1.5/crtoolbox/coverage.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    17000 2023-07-03 16:38:23.000000 crtoolbox-0.1.5/crtoolbox/generate.py
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox/lib/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/crtoolbox/lib/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    32639 2023-07-03 16:38:47.000000 crtoolbox-0.1.5/crtoolbox/lib/boundary.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     9679 2023-07-03 16:37:54.000000 crtoolbox-0.1.5/crtoolbox/lib/cohens.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26142 2023-07-03 16:37:21.000000 crtoolbox-0.1.5/crtoolbox/lib/display.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    11545 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/crtoolbox/lib/fileio.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8277 2023-07-03 16:38:35.000000 crtoolbox-0.1.5/crtoolbox/lib/regression.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      694 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/crtoolbox/lib/set_theory.py
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox/tests/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/crtoolbox/tests/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    27054 2023-07-03 16:37:38.000000 crtoolbox-0.1.5/crtoolbox/tests/generate_2d_data.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    12001 2023-07-03 16:38:07.000000 crtoolbox-0.1.5/crtoolbox/tests/generate_ni_data.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000) 13824352 2023-07-03 16:18:27.000000 crtoolbox-0.1.5/crtoolbox/tests/mask.nii
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox.egg-info/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      464 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      676 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        1 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       54 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox.egg-info/requires.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       15 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/crtoolbox.egg-info/top_level.txt
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       38 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/setup.cfg
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      801 2023-07-03 16:43:46.000000 crtoolbox-0.1.5/setup.py
-drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:44:34.000000 crtoolbox-0.1.5/sims/
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    12928 2023-07-03 16:17:49.000000 crtoolbox-0.1.5/sims/SpatialSims_Mmu.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:17:49.000000 crtoolbox-0.1.5/sims/__init__.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    17027 2023-07-03 16:17:49.000000 crtoolbox-0.1.5/sims/genCfgs_Mmu.py
--rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26300 2023-07-03 16:17:49.000000 crtoolbox-0.1.5/sims/join_and_plot_Mmu.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       32 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/MANIFEST.in
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      408 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/PKG-INFO
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/README.md
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/crtoolbox/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8117 2023-07-03 16:39:07.000000 crtoolbox-0.1.6/crtoolbox/bootstrap.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    14328 2023-07-03 16:38:57.000000 crtoolbox-0.1.6/crtoolbox/coverage.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    17000 2023-07-03 16:38:23.000000 crtoolbox-0.1.6/crtoolbox/generate.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox/lib/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/crtoolbox/lib/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    32639 2023-07-03 16:38:47.000000 crtoolbox-0.1.6/crtoolbox/lib/boundary.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     9679 2023-07-03 16:37:54.000000 crtoolbox-0.1.6/crtoolbox/lib/cohens.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26142 2023-07-03 16:37:21.000000 crtoolbox-0.1.6/crtoolbox/lib/display.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    11545 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/crtoolbox/lib/fileio.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)     8277 2023-07-03 16:38:35.000000 crtoolbox-0.1.6/crtoolbox/lib/regression.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      694 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/crtoolbox/lib/set_theory.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox/tests/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/crtoolbox/tests/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    27054 2023-07-03 16:37:38.000000 crtoolbox-0.1.6/crtoolbox/tests/generate_2d_data.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    12001 2023-07-04 13:05:13.000000 crtoolbox-0.1.6/crtoolbox/tests/generate_ni_data.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000) 13824352 2023-07-03 16:18:27.000000 crtoolbox-0.1.6/crtoolbox/tests/mask.nii
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox.egg-info/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      408 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      676 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        1 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       70 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox.egg-info/requires.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       15 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/crtoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)       38 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/setup.cfg
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)      868 2023-07-04 12:45:34.000000 crtoolbox-0.1.6/setup.py
+drwxrwxr-x   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-04 13:15:42.000000 crtoolbox-0.1.6/sims/
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    12928 2023-07-03 16:17:49.000000 crtoolbox-0.1.6/sims/SpatialSims_Mmu.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)        0 2023-07-03 16:17:49.000000 crtoolbox-0.1.6/sims/__init__.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    17027 2023-07-03 16:17:49.000000 crtoolbox-0.1.6/sims/genCfgs_Mmu.py
+-rw-rw-r--   0 tommaullin  (1000) tommaullin  (1000)    26300 2023-07-03 16:17:49.000000 crtoolbox-0.1.6/sims/join_and_plot_Mmu.py
```

### Comparing `crtoolbox-0.1.5/crtoolbox/bootstrap.py` & `crtoolbox-0.1.6/crtoolbox/bootstrap.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/coverage.py` & `crtoolbox-0.1.6/crtoolbox/coverage.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/generate.py` & `crtoolbox-0.1.6/crtoolbox/generate.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/lib/boundary.py` & `crtoolbox-0.1.6/crtoolbox/lib/boundary.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/lib/cohens.py` & `crtoolbox-0.1.6/crtoolbox/lib/cohens.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/lib/display.py` & `crtoolbox-0.1.6/crtoolbox/lib/display.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/lib/fileio.py` & `crtoolbox-0.1.6/crtoolbox/lib/fileio.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/lib/regression.py` & `crtoolbox-0.1.6/crtoolbox/lib/regression.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/lib/set_theory.py` & `crtoolbox-0.1.6/crtoolbox/lib/set_theory.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/tests/generate_2d_data.py` & `crtoolbox-0.1.6/crtoolbox/tests/generate_2d_data.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox/tests/generate_ni_data.py` & `crtoolbox-0.1.6/crtoolbox/tests/generate_ni_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import shutil
 import yaml
 from crtoolbox.lib.fileio import *
 import time
 import pandas as pd
 from scipy import ndimage
 
-def generate_data(n, p, OutDir, dim=np.array([100,100,100]), mask_type='fixed', sigma=5):
+def generate_data(n, p, OutDir, dim=np.array([100,100,100]), mask_type='fixed', sigma=3):
     """
     Generates simulated data with the specified dimensions and other parameters.
     
     Parameters
     ----------
     n : int
         Number of observations.
```

### Comparing `crtoolbox-0.1.5/crtoolbox/tests/mask.nii` & `crtoolbox-0.1.6/crtoolbox/tests/mask.nii`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/crtoolbox.egg-info/SOURCES.txt` & `crtoolbox-0.1.6/crtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/sims/SpatialSims_Mmu.py` & `crtoolbox-0.1.6/sims/SpatialSims_Mmu.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/sims/genCfgs_Mmu.py` & `crtoolbox-0.1.6/sims/genCfgs_Mmu.py`

 * *Files identical despite different names*

### Comparing `crtoolbox-0.1.5/sims/join_and_plot_Mmu.py` & `crtoolbox-0.1.6/sims/join_and_plot_Mmu.py`

 * *Files identical despite different names*

