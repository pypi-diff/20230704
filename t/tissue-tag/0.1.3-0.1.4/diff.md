# Comparing `tmp/tissue-tag-0.1.3.tar.gz` & `tmp/tissue-tag-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-tag-0.1.3.tar", last modified: Tue Jul  4 15:50:02 2023, max compression
+gzip compressed data, was "tissue-tag-0.1.4.tar", last modified: Tue Jul  4 15:58:45 2023, max compression
```

## Comparing `tissue-tag-0.1.3.tar` & `tissue-tag-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.3/LICENSE
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      650 2023-07-01 12:02:23.000000 tissue-tag-0.1.3/README.md
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/setup.cfg
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-04 15:49:38.000000 tissue-tag-0.1.3/setup.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:50:02.023293 tissue-tag-0.1.3/tissue-tag/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:49:10.000000 tissue-tag-0.1.3/tissue-tag/__init__.py
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)    42646 2023-07-01 11:59:22.000000 tissue-tag-0.1.3/tissue-tag/tissue_tag.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/tissue_tag.egg-info/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      243 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/requires.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       11 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/top_level.txt
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.4/LICENSE
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1764 2023-07-04 15:55:26.000000 tissue-tag-0.1.4/README.md
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/setup.cfg
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-04 15:58:37.000000 tissue-tag-0.1.4/setup.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/tissue_tag/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:55:26.000000 tissue-tag-0.1.4/tissue_tag/__init__.py
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)    45249 2023-07-04 15:55:26.000000 tissue-tag-0.1.4/tissue_tag/tissue_tag.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/tissue_tag.egg-info/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      243 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/SOURCES.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/dependency_links.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/requires.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       11 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/top_level.txt
```

### Comparing `tissue-tag-0.1.3/LICENSE` & `tissue-tag-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.3/PKG-INFO` & `tissue-tag-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPMPLHBMH5KAQK74NAYZFACXRA" width="300" >
+	<img src="https://github.com/nadavyayon/TissueTag/blob/main/tissueTag_logo.png" width="300" >
 </p>
 
 # Tissue Tag jupyter image annotator
-??? What does it do, small intro ???
+A jupyter-based image annotation tool - TissueTag is powered by the Bokeh python library (http://www.bokeh.pydata.org) and provides a simple annotation solution with subpixel resolution for fast interactive annotation of any image type or kind (brightfield, fluorescence, etc) as well as spatial omics. TissueTag generates discrete annotations (e.g. cortex, medulla etc) but can also output the euclidean distance of each spot/cell to the closest part of a given morphological structure, enabling continuous annotation. This thus holds spatial neighbourhood information that goes beyond the x-y coordinates of a given spot or cell. 
 
+### We see this tool as a basic start and feel there are many useful applicaitons that could be added, so we welcome any contibution and look forward to suggestions!
 
 ## Installation
 
 1) You need to install either [jupyter-lab](https://jupyter.org/install) or [jupyter-notebook](https://jupyter.org/install)
 2) Install TissueTag using pip:
 ```
 pip install tissue-tag
 ```
 
 ## General instructions and examples:
 
-1) 
-3) When running on farm, you need to set the port (e.g., 5011) you are using to get it plot properly in the correct place 
+When running on farm, you need to set the port (e.g., 5011) you are using to get it plot properly in the correct place.
 
+### setting up an environment for visium annotation
+
+1) create env `conda create -n tissuetag python=3.9` `conda activate tissuetag`
+
+2) install tissuetag, scanpy and jupyterlab `pip install tissue-tag` `pip install scanpy` `conda install -c conda-forge jupyterlab`
+
+3) install kernel  `ipython kernel install --name tissuetag --user`
+
+### importing in a notebook 
+`import tissue_tag as tt`
 
 ## How to cite:
+preprint coming! stay tuned
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tissue-tag-0.1.3/setup.py` & `tissue-tag-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tissue-tag',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'opencv-python',
         'Pillow',
         'bokeh',
         'jupyter-bokeh',
         'matplotlib',
```

### Comparing `tissue-tag-0.1.3/tissue-tag/tissue_tag.py` & `tissue-tag-0.1.4/tissue_tag/tissue_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1261,7 +1261,74 @@
     return out_img
 
 def find_files(directory, query):
     for root, dirs, files in os.walk(directory):
         for file in files:
             if query in file:
                 return os.path.join(root, file)
+
+
+def migrate_annotations(df_source, df_target, ppm_source, ppm_target, plot=True, how='nearest', max_distance=10e10):
+    """
+    Maps tissue annotations from the source DataFrame to the target DataFrame according to the nearest neighbors.
+    
+    Parameters
+    ----------
+    df_source : pandas.DataFrame
+        Source DataFrame with annotations.
+    df_target : pandas.DataFrame
+        Target DataFrame where annotations will be migrated.
+    ppm_source : float 
+        pixels per micron of the source DataFrame
+    ppm_target : float 
+        pixels per micron of the target DataFrame
+    plot : bool, optional
+        If true, plots the coordinates of the source and target spaces to make sure 
+        they are aligned. Default is True.
+    how : string, optional
+        This determines how the association between the 2 grids is made from the scipy.interpolate.griddata function. Default is 'nearest'
+    max_distance : int, optional
+        maximal distance where points are not migrated. Default is 10e10
+
+    Returns
+    -------
+    df_target : pandas.DataFrame
+        Updated target DataFrame with annotations migrated from the source DataFrame.
+    """
+    import numpy as np
+    from scipy.interpolate import griddata
+    from scipy.spatial import cKDTree
+    import matplotlib.pyplot as plt
+    
+    print('Make sure the coordinate systems are aligned, e.g., axes are not flipped.') 
+    source_coords = np.vstack([df_source['x']*ppm_source, df_source['y']*ppm_source])
+    target_coords = np.vstack([df_target['x']*ppm_target, df_target['y']*ppm_target])
+    
+    if plot:
+        plt.figure(dpi=100, figsize=[10, 10])
+        plt.title('Target space')
+        plt.plot(target_coords[0], target_coords[1], '.', markersize=1)
+        plt.show()
+        
+        plt.figure(dpi=100, figsize=[10, 10])
+        plt.plot(source_coords[0], source_coords[1], '.', markersize=1)
+        plt.title('Source space')
+        plt.show()
+    
+    annotations = df_source.columns[~df_source.columns.isin(['x', 'y'])]
+    
+    for k in annotations:
+        print('Migrating - ' + k + ' to target DataFrame.')
+        
+        # Interpolation
+        df_target[k] = griddata(points=source_coords.T, values=df_source[k], xi=target_coords.T, method=how)
+        
+        # Create KDTree
+        tree = cKDTree(source_coords.T)
+        
+        # Query tree for nearest distance
+        distances, _ = tree.query(target_coords.T, distance_upper_bound=max_distance)
+        
+        # Mask df_target where the distance is too high
+        df_target[k][distances==np.inf] = None
+  
+    return df_target
```

### Comparing `tissue-tag-0.1.3/tissue_tag.egg-info/PKG-INFO` & `tissue-tag-0.1.4/tissue_tag.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPMPLHBMH5KAQK74NAYZFACXRA" width="300" >
+	<img src="https://github.com/nadavyayon/TissueTag/blob/main/tissueTag_logo.png" width="300" >
 </p>
 
 # Tissue Tag jupyter image annotator
-??? What does it do, small intro ???
+A jupyter-based image annotation tool - TissueTag is powered by the Bokeh python library (http://www.bokeh.pydata.org) and provides a simple annotation solution with subpixel resolution for fast interactive annotation of any image type or kind (brightfield, fluorescence, etc) as well as spatial omics. TissueTag generates discrete annotations (e.g. cortex, medulla etc) but can also output the euclidean distance of each spot/cell to the closest part of a given morphological structure, enabling continuous annotation. This thus holds spatial neighbourhood information that goes beyond the x-y coordinates of a given spot or cell. 
 
+### We see this tool as a basic start and feel there are many useful applicaitons that could be added, so we welcome any contibution and look forward to suggestions!
 
 ## Installation
 
 1) You need to install either [jupyter-lab](https://jupyter.org/install) or [jupyter-notebook](https://jupyter.org/install)
 2) Install TissueTag using pip:
 ```
 pip install tissue-tag
 ```
 
 ## General instructions and examples:
 
-1) 
-3) When running on farm, you need to set the port (e.g., 5011) you are using to get it plot properly in the correct place 
+When running on farm, you need to set the port (e.g., 5011) you are using to get it plot properly in the correct place.
 
+### setting up an environment for visium annotation
+
+1) create env `conda create -n tissuetag python=3.9` `conda activate tissuetag`
+
+2) install tissuetag, scanpy and jupyterlab `pip install tissue-tag` `pip install scanpy` `conda install -c conda-forge jupyterlab`
+
+3) install kernel  `ipython kernel install --name tissuetag --user`
+
+### importing in a notebook 
+`import tissue_tag as tt`
 
 ## How to cite:
+preprint coming! stay tuned
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

