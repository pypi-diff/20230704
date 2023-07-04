# Comparing `tmp/proteusPy-0.681.tar.gz` & `tmp/proteusPy-0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteusPy-0.681.tar", last modified: Mon Jul  3 00:45:03 2023, max compression
+gzip compressed data, was "proteusPy-0.69.tar", last modified: Tue Jul  4 00:25:34 2023, max compression
```

## Comparing `proteusPy-0.681.tar` & `proteusPy-0.69.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.177892 proteusPy-0.681/
--rw-r--r--   0 egs        (505) staff       (20)     3420 2023-07-03 00:45:03.177996 proteusPy-0.681/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)     2281 2023-07-02 23:22:12.000000 proteusPy-0.681/README.md
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.174466 proteusPy-0.681/proteusPy/
--rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.681/proteusPy/Disulfide.py
--rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.681/proteusPy/DisulfideClass_Constructor.py
--rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.681/proteusPy/DisulfideClasses.py
--rw-r--r--   0 egs        (505) staff       (20)     1027 2023-01-04 04:03:30.000000 proteusPy-0.681/proteusPy/DisulfideExceptions.py
--rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.681/proteusPy/DisulfideList.py
--rw-r--r--   0 egs        (505) staff       (20)    24238 2023-07-03 00:32:10.000000 proteusPy-0.681/proteusPy/DisulfideLoader.py
--rw-r--r--   0 egs        (505) staff       (20)      833 2023-07-02 19:47:15.000000 proteusPy-0.681/proteusPy/ProteusGlobals.py
--rw-r--r--   0 egs        (505) staff       (20)     1642 2023-07-03 00:44:38.000000 proteusPy-0.681/proteusPy/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.681/proteusPy/angle_annotation.py
--rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.681/proteusPy/atoms.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.177469 proteusPy-0.681/proteusPy/data/
--rw-r--r--   0 egs        (505) staff       (20)     2514 2023-07-02 22:23:54.000000 proteusPy-0.681/proteusPy/data/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.681/proteusPy/data/ss_completed.txt
--rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.681/proteusPy/data/ss_ids.txt
--rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.681/proteusPy/data/ss_query.json
--rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.681/proteusPy/proteusPyWarning.py
--rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.681/proteusPy/residue.py
--rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.681/proteusPy/turtle3D.py
--rw-r--r--   0 egs        (505) staff       (20)    12468 2023-03-13 16:49:31.000000 proteusPy-0.681/proteusPy/utility.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-03 00:45:03.175554 proteusPy-0.681/proteusPy.egg-info/
--rw-r--r--   0 egs        (505) staff       (20)     3420 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)      713 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/SOURCES.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/dependency_links.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.681/proteusPy.egg-info/not-zip-safe
--rw-r--r--   0 egs        (505) staff       (20)       36 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/requires.txt
--rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-03 00:45:03.000000 proteusPy-0.681/proteusPy.egg-info/top_level.txt
--rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-03 00:45:03.178375 proteusPy-0.681/setup.cfg
--rw-r--r--   0 egs        (505) staff       (20)     3676 2023-07-02 20:46:16.000000 proteusPy-0.681/setup.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-04 00:25:34.805653 proteusPy-0.69/
+-rw-r--r--   0 egs        (505) staff       (20)     4951 2023-07-04 00:25:34.805746 proteusPy-0.69/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)     3813 2023-07-03 22:44:55.000000 proteusPy-0.69/README.md
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-04 00:25:34.802750 proteusPy-0.69/proteusPy/
+-rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.69/proteusPy/Disulfide.py
+-rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.69/proteusPy/DisulfideClass_Constructor.py
+-rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.69/proteusPy/DisulfideClasses.py
+-rw-r--r--   0 egs        (505) staff       (20)     1027 2023-01-04 04:03:30.000000 proteusPy-0.69/proteusPy/DisulfideExceptions.py
+-rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.69/proteusPy/DisulfideList.py
+-rw-r--r--   0 egs        (505) staff       (20)    24248 2023-07-03 23:29:07.000000 proteusPy-0.69/proteusPy/DisulfideLoader.py
+-rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.69/proteusPy/ProteusGlobals.py
+-rw-r--r--   0 egs        (505) staff       (20)     1641 2023-07-03 22:24:20.000000 proteusPy-0.69/proteusPy/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.69/proteusPy/angle_annotation.py
+-rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.69/proteusPy/atoms.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-04 00:25:34.805395 proteusPy-0.69/proteusPy/data/
+-rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-03 22:51:30.000000 proteusPy-0.69/proteusPy/data/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.69/proteusPy/data/ss_completed.txt
+-rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.69/proteusPy/data/ss_ids.txt
+-rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.69/proteusPy/data/ss_query.json
+-rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.69/proteusPy/proteusPyWarning.py
+-rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.69/proteusPy/residue.py
+-rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.69/proteusPy/turtle3D.py
+-rw-r--r--   0 egs        (505) staff       (20)    12468 2023-03-13 16:49:31.000000 proteusPy-0.69/proteusPy/utility.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-04 00:25:34.803833 proteusPy-0.69/proteusPy.egg-info/
+-rw-r--r--   0 egs        (505) staff       (20)     4951 2023-07-04 00:25:34.000000 proteusPy-0.69/proteusPy.egg-info/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)      713 2023-07-04 00:25:34.000000 proteusPy-0.69/proteusPy.egg-info/SOURCES.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-04 00:25:34.000000 proteusPy-0.69/proteusPy.egg-info/dependency_links.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.69/proteusPy.egg-info/not-zip-safe
+-rw-r--r--   0 egs        (505) staff       (20)       36 2023-07-04 00:25:34.000000 proteusPy-0.69/proteusPy.egg-info/requires.txt
+-rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-04 00:25:34.000000 proteusPy-0.69/proteusPy.egg-info/top_level.txt
+-rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-04 00:25:34.806012 proteusPy-0.69/setup.cfg
+-rw-r--r--   0 egs        (505) staff       (20)     3676 2023-07-02 20:46:16.000000 proteusPy-0.69/setup.py
```

### Comparing `proteusPy-0.681/proteusPy/Disulfide.py` & `proteusPy-0.69/proteusPy/Disulfide.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/DisulfideClass_Constructor.py` & `proteusPy-0.69/proteusPy/DisulfideClass_Constructor.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/DisulfideClasses.py` & `proteusPy-0.69/proteusPy/DisulfideClasses.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/DisulfideExceptions.py` & `proteusPy-0.69/proteusPy/DisulfideExceptions.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/DisulfideList.py` & `proteusPy-0.69/proteusPy/DisulfideList.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/DisulfideLoader.py` & `proteusPy-0.69/proteusPy/DisulfideLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import numpy as np
 
 import proteusPy
 from proteusPy.ProteusGlobals import PDB_DIR, MODEL_DIR,  REPO_DATA_DIR
 from proteusPy.atoms import *
 
 from proteusPy.data import SS_PICKLE_FILE, SS_TORSIONS_FILE, SS_DICT_PICKLE_FILE, DATA_DIR
-from proteusPy.data import LOADER_FNAME, LOADER_SUBSET_FNAME
+from proteusPy.data import LOADER_FNAME, LOADER_SUBSET_FNAME, LOADER_ALL_URL, LOADER_SUBSET_URL
 
 from proteusPy.DisulfideList import DisulfideList
 from proteusPy.Disulfide import Disulfide
 
 from proteusPy.DisulfideExceptions import *
 from proteusPy.data import *
 from proteusPy.DisulfideClass_Constructor import DisulfideClass_Constructor
@@ -554,65 +554,65 @@
     :param subset: If True, load the subset DB, otherwise load the full database
     '''
     # normally the .pkl files are local, EXCEPT for the first run from a newly-installed proteusPy 
     # distribution. In that case we need to download the files for all disulfides and the subset
     # from the Google Drive storage.
     
     import gdown
-    url_all = "https://drive.google.com/uc?id=1igF-sppLPaNsBaUS7nkb13vtOGZZmsFp"
-    url_subset = "https://drive.google.com/uc?id=1puy9pxrClFks0KN9q5PPV_ONKvL-hg33"
     
     _good1 = False # all data
     _good2 = False # subset data
     
     _fname_sub = f'{loadpath}{LOADER_SUBSET_FNAME}'
     _fname_all = f'{loadpath}{LOADER_FNAME}'
     
     if subset:
         _fname = _fname_sub
     else:
         _fname = _fname_all
     
+    # first attempt to read the local copy of the loader
     if verbose:
         print(f'-> load_PDB_SS(): Reading {_fname}... ', end='')
 
     try:
         with open(_fname, 'rb') as f:
             res = pickle.load(f)
         if verbose:
             print(f'done.')
         return res
     
+    # we don't have it locally, so download both from google drive
     except IOError:
         if verbose:
-            print(f'-> DisulfideLoader(): Reading disulfides from Google Drive... ')
+            print(f'\n-> DisulfideLoader(): Reading disulfides from Google Drive... ')
         
         #PDB_SS_ALL_LOADER.pkl
         if verbose:
             destination = _fname_all
             print(f'-> DisulfideLoader(): Downloading the RCSB Disulfide Database from Google Drive to {destination}... ', end='')
         
-        if gdown.download(url_all, _fname_all) is not None:
+        if gdown.download(LOADER_ALL_URL, _fname_all) is not None:
             _good1 = True
             if verbose:
                 print(f' done.')
         else:
-            print('Error downloading RCSB database!')
+            print('\nError downloading RCSB database!')
 
         #PDB_ss_subset.pkl
         destination = _fname_sub
         if verbose:
             print(f'-> DisulfideLoader(): Downloading disulfide subset database from Google Drive to {destination}... ', end='')
         
-        if gdown.download(url_subset, _fname_sub) is not None:
+        if gdown.download(LOADER_SUBSET_URL, _fname_sub) is not None:
             _good2 = True
             if verbose:
                 print(f' done.')
         else:
-            print('Error downloading RCSB subset database!')
+            print('\nError downloading RCSB subset database!')
 
     if subset:
         _fname = _fname_sub
     else:
         _fname = _fname_all
 
     if verbose:
@@ -634,10 +634,10 @@
             mess = f'!!! FATAL: load_PDB_SS(): cannot rebuild primary SS file!'
             raise DisulfideIOException(mess)
         else:
             pdb.save()
         print(f'-> Load_PDB_SS(): rebuild complete.')
         '''
 
-    return pdb
+    return
 
 # End of file
```

### Comparing `proteusPy-0.681/proteusPy/ProteusGlobals.py` & `proteusPy-0.69/proteusPy/ProteusGlobals.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,7 @@
 WINSIZE = (1024, 1024)
 CAMERA_POS = ((0, 0, -10), (0,0,0), (0,1,0))
 
 PBAR_COLS = 105
 # nominal macbook Pro screen resolution
 DPI = 220
 
-
-
-
```

### Comparing `proteusPy-0.681/proteusPy/__init__.py` & `proteusPy-0.69/proteusPy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Eric G. Suchanek, PhD., all rights reserved
 # Subject to the MIT public license.
 
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.681"
+__version__ = "0.69"
 
 import sys
 import os
 import glob
 import warnings
 import copy
```

### Comparing `proteusPy-0.681/proteusPy/angle_annotation.py` & `proteusPy-0.69/proteusPy/angle_annotation.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/atoms.py` & `proteusPy-0.69/proteusPy/atoms.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/data/__init__.py` & `proteusPy-0.69/proteusPy/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
 LOADER_FNAME = "PDB_SS_ALL_LOADER.pkl"
 LOADER_SUBSET_FNAME = "PDB_SS_SUBSET_LOADER.pkl"
 
 LOADER_FNAME_URL = "https://raw.githubusercontent.com/suchanek/proteusPy/master/proteusPy/data/PDB_SS_ALL_LOADER.pkl"
 LOADER_SUBSET_FNAME_URL = "https://raw.githubusercontent.com/suchanek/proteusPy/blob/master/proteusPy/data/PDB_SS_SUBSET_LOADER.pkl"
 
+LOADER_ALL_URL = "https://drive.google.com/uc?id=1igF-sppLPaNsBaUS7nkb13vtOGZZmsFp"
+LOADER_SUBSET_URL = "https://drive.google.com/uc?id=1puy9pxrClFks0KN9q5PPV_ONKvL-hg33"
+
+
 SS_CLASS_DEFINITIONS = '''
 Idx,chi1_s,chi2_s,chi3_s,chi4_s,chi5_s,class_id,SS_Classname,FXN
 0,-1,-1,-1,-1,-1,00000,-LHSpiral,UNK
 1,-1,-1,-1,-1,1,00002,00002,UNK
 2,-1,-1,-1,1,-1,00020,-LHHook,UNK
 3,-1,-1,-1,1,1,00022,00022,UNK
 4,-1,-1,1,-1,-1,00200,-RHStaple,Allosteric
```

### Comparing `proteusPy-0.681/proteusPy/data/ss_completed.txt` & `proteusPy-0.69/proteusPy/data/ss_completed.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/data/ss_ids.txt` & `proteusPy-0.69/proteusPy/data/ss_ids.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/data/ss_query.json` & `proteusPy-0.69/proteusPy/data/ss_query.json`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/residue.py` & `proteusPy-0.69/proteusPy/residue.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/turtle3D.py` & `proteusPy-0.69/proteusPy/turtle3D.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy/utility.py` & `proteusPy-0.69/proteusPy/utility.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/proteusPy.egg-info/SOURCES.txt` & `proteusPy-0.69/proteusPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.681/setup.py` & `proteusPy-0.69/setup.py`

 * *Files identical despite different names*

