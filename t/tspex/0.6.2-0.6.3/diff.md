# Comparing `tmp/tspex-0.6.2.tar.gz` & `tmp/tspex-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tspex-0.6.2.tar", last modified: Mon Jun  1 22:40:01 2020, max compression
+gzip compressed data, was "tspex-0.6.3.tar", last modified: Tue Jul  4 18:01:47 2023, max compression
```

## Comparing `tspex-0.6.2.tar` & `tspex-0.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 apcamargo  (1000) apcamargo  (1000)        0 2020-06-01 22:40:01.000000 tspex-0.6.2/
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)    35149 2020-06-01 22:13:36.000000 tspex-0.6.2/LICENSE
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)       16 2020-06-01 22:13:36.000000 tspex-0.6.2/MANIFEST.in
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     5960 2020-06-01 22:40:01.000000 tspex-0.6.2/PKG-INFO
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     4202 2020-06-01 22:13:36.000000 tspex-0.6.2/README.md
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)       38 2020-06-01 22:40:01.000000 tspex-0.6.2/setup.cfg
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     2037 2020-06-01 22:35:50.000000 tspex-0.6.2/setup.py
-drwxrwxr-x   0 apcamargo  (1000) apcamargo  (1000)        0 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex/
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)      910 2020-06-01 22:13:36.000000 tspex-0.6.2/tspex/__init__.py
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     3701 2020-06-01 22:13:36.000000 tspex-0.6.2/tspex/cli.py
-drwxrwxr-x   0 apcamargo  (1000) apcamargo  (1000)        0 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex/core/
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)      814 2020-06-01 22:13:36.000000 tspex-0.6.2/tspex/core/__init__.py
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     4195 2020-06-01 22:33:42.000000 tspex-0.6.2/tspex/core/auxiliary_functions.py
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     9651 2020-06-01 22:13:36.000000 tspex-0.6.2/tspex/core/specificity_class.py
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)    15110 2020-06-01 22:13:36.000000 tspex-0.6.2/tspex/core/specificity_functions.py
-drwxrwxr-x   0 apcamargo  (1000) apcamargo  (1000)        0 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)     5960 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/PKG-INFO
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)      370 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/SOURCES.txt
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)        1 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/dependency_links.txt
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)       42 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/entry_points.txt
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)       47 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/requires.txt
--rw-rw-r--   0 apcamargo  (1000) apcamargo  (1000)        6 2020-06-01 22:40:01.000000 tspex-0.6.2/tspex.egg-info/top_level.txt
+drwxr-xr-x   0 APCamargo-M55   (502) staff       (20)        0 2023-07-04 18:01:47.033312 tspex-0.6.3/
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)    35149 2023-07-04 17:59:28.000000 tspex-0.6.3/LICENSE
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)       16 2023-07-04 17:59:28.000000 tspex-0.6.3/MANIFEST.in
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     6710 2023-07-04 18:01:47.033071 tspex-0.6.3/PKG-INFO
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     4920 2023-07-04 17:59:28.000000 tspex-0.6.3/README.md
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)       38 2023-07-04 18:01:47.033403 tspex-0.6.3/setup.cfg
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     2037 2023-07-04 18:01:22.000000 tspex-0.6.3/setup.py
+drwxr-xr-x   0 APCamargo-M55   (502) staff       (20)        0 2023-07-04 18:01:47.029746 tspex-0.6.3/tspex/
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)      910 2023-07-04 17:59:28.000000 tspex-0.6.3/tspex/__init__.py
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     3701 2023-07-04 17:59:28.000000 tspex-0.6.3/tspex/cli.py
+drwxr-xr-x   0 APCamargo-M55   (502) staff       (20)        0 2023-07-04 18:01:47.032646 tspex-0.6.3/tspex/core/
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)      814 2023-07-04 17:59:28.000000 tspex-0.6.3/tspex/core/__init__.py
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     4247 2023-07-04 17:59:28.000000 tspex-0.6.3/tspex/core/auxiliary_functions.py
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     9652 2023-07-04 18:00:28.000000 tspex-0.6.3/tspex/core/specificity_class.py
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)    15930 2023-07-04 17:59:28.000000 tspex-0.6.3/tspex/core/specificity_functions.py
+drwxr-xr-x   0 APCamargo-M55   (502) staff       (20)        0 2023-07-04 18:01:47.031544 tspex-0.6.3/tspex.egg-info/
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)     6710 2023-07-04 18:01:46.000000 tspex-0.6.3/tspex.egg-info/PKG-INFO
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)      370 2023-07-04 18:01:46.000000 tspex-0.6.3/tspex.egg-info/SOURCES.txt
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)        1 2023-07-04 18:01:46.000000 tspex-0.6.3/tspex.egg-info/dependency_links.txt
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)       42 2023-07-04 18:01:46.000000 tspex-0.6.3/tspex.egg-info/entry_points.txt
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)       47 2023-07-04 18:01:46.000000 tspex-0.6.3/tspex.egg-info/requires.txt
+-rw-r--r--   0 APCamargo-M55   (502) staff       (20)        6 2023-07-04 18:01:46.000000 tspex-0.6.3/tspex.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tspex-0.6.2/LICENSE` & `tspex-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tspex-0.6.2/PKG-INFO` & `tspex-0.6.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: tspex
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python package for calculating tissue-specificity metrics for gene expression.
 Home-page: https://apcamargo.github.io/tspex/
 Author: Antonio Pedro Camargo
 Author-email: antoniop.camargo@gmail.com
 License: GNU General Public License v3.0
 Description: # tspex
         
+        [![DOI](https://img.shields.io/badge/DOI-10.21203%2Frs.3.rs--51998%2Fv1-red)](https://doi.org/10.21203/rs.3.rs-51998/v1)
+        [![PyPI](https://img.shields.io/pypi/v/tspex.svg?label=PyPI&color=green)](https://pypi.python.org/pypi/tspex)
+        [![Conda](https://img.shields.io/conda/vn/bioconda/tspex.svg?label=Conda&color=green)](https://anaconda.org/bioconda/tspex)
+        [![PyPI downloads](https://img.shields.io/pypi/dm/tspex?label=PyPI%20downloads&color=blue)](https://pypi.python.org/pypi/tspex)
+        [![Conda downloads](https://img.shields.io/conda/dn/bioconda/tspex.svg?label=Conda%20downloads&color=blue)](https://anaconda.org/bioconda/tspex)
         
         - [Overview](#overview)
+        - [Citation](#citation)
         - [Documentation](#documentation)
         - [Installation](#installation)
         - [Python API tutorial](#python-api-tutorial)
         - [Command-line interface](#command-line-interface)
         - [Examples](#examples)
         
         ## Overview
@@ -22,14 +28,21 @@
         
         tspex features include:
           - Twelve different tissue-specificity metrics.
           - Integration with popular data analysis libraries, such as NumPy, SciPy, and pandas.
           - Visualization functions.
           - Support for Jupyter notebooks.
         
+        
+        ## Citation
+        
+        If you use tspex in your research, it would be appreciated if you could cite it.
+        
+        > Camargo, A. P., Vasconcelos, A. A., Fiamenghi, M. B., Pereira, G. A. G. & Carazzolle, M. F.. "[tspex: a tissue-specificity calculator for gene expression data](https://www.researchsquare.com/article/rs-51998/v1)" *Preprint available at Research Square* (2020).
+        
         ## Web version
         
         tspex can be used through a web interface that is freely available online at [https://tspex.lge.ibi.unicamp.br/](https://tspex.lge.ibi.unicamp.br/). The source code of the web app can be found at [https://github.com/apcamargo/tspex-webapp/](https://github.com/apcamargo/tspex-webapp/).
         
         ## Documentation
         
         A complete documentation for tspex can be found at [https://apcamargo.github.io/tspex/](https://apcamargo.github.io/tspex/).
@@ -109,23 +122,14 @@
         
         - Using the `zscore` without transformation to quantify tissue-specificity as the number of standard deviations away from the mean gene expression:
         
         ```
         tspex --disable_transformation gene_expression.tsv tspex_zscore.tsv zscore
         ```
         
-        
-        ## Cite tspex
-        
-        If you use tspex in your research, it would be appreciated if you could cite it.
-        
-        [![DOI](https://zenodo.org/badge/172384291.svg)](https://zenodo.org/badge/latestdoi/172384291)
-        
-        > Camargo, Antonio P., "*tspex: tissue-specificity calculator*" (2019). doi:10.5281/zenodo.3558708
-        
 Keywords: bioinformatics,gene expression,tissue-specificity,transcriptomics
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `tspex-0.6.2/README.md` & `tspex-0.6.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # tspex
 
+[![DOI](https://img.shields.io/badge/DOI-10.21203%2Frs.3.rs--51998%2Fv1-red)](https://doi.org/10.21203/rs.3.rs-51998/v1)
+[![PyPI](https://img.shields.io/pypi/v/tspex.svg?label=PyPI&color=green)](https://pypi.python.org/pypi/tspex)
+[![Conda](https://img.shields.io/conda/vn/bioconda/tspex.svg?label=Conda&color=green)](https://anaconda.org/bioconda/tspex)
+[![PyPI downloads](https://img.shields.io/pypi/dm/tspex?label=PyPI%20downloads&color=blue)](https://pypi.python.org/pypi/tspex)
+[![Conda downloads](https://img.shields.io/conda/dn/bioconda/tspex.svg?label=Conda%20downloads&color=blue)](https://anaconda.org/bioconda/tspex)
 
 - [Overview](#overview)
+- [Citation](#citation)
 - [Documentation](#documentation)
 - [Installation](#installation)
 - [Python API tutorial](#python-api-tutorial)
 - [Command-line interface](#command-line-interface)
 - [Examples](#examples)
 
 ## Overview
@@ -14,14 +20,21 @@
 
 tspex features include:
   - Twelve different tissue-specificity metrics.
   - Integration with popular data analysis libraries, such as NumPy, SciPy, and pandas.
   - Visualization functions.
   - Support for Jupyter notebooks.
 
+
+## Citation
+
+If you use tspex in your research, it would be appreciated if you could cite it.
+
+> Camargo, A. P., Vasconcelos, A. A., Fiamenghi, M. B., Pereira, G. A. G. & Carazzolle, M. F.. "[tspex: a tissue-specificity calculator for gene expression data](https://www.researchsquare.com/article/rs-51998/v1)" *Preprint available at Research Square* (2020).
+
 ## Web version
 
 tspex can be used through a web interface that is freely available online at [https://tspex.lge.ibi.unicamp.br/](https://tspex.lge.ibi.unicamp.br/). The source code of the web app can be found at [https://github.com/apcamargo/tspex-webapp/](https://github.com/apcamargo/tspex-webapp/).
 
 ## Documentation
 
 A complete documentation for tspex can be found at [https://apcamargo.github.io/tspex/](https://apcamargo.github.io/tspex/).
@@ -100,16 +113,7 @@
 ```
 
 - Using the `zscore` without transformation to quantify tissue-specificity as the number of standard deviations away from the mean gene expression:
 
 ```
 tspex --disable_transformation gene_expression.tsv tspex_zscore.tsv zscore
 ```
-
-
-## Cite tspex
-
-If you use tspex in your research, it would be appreciated if you could cite it.
-
-[![DOI](https://zenodo.org/badge/172384291.svg)](https://zenodo.org/badge/latestdoi/172384291)
-
-> Camargo, Antonio P., "*tspex: tissue-specificity calculator*" (2019). doi:10.5281/zenodo.3558708
```

### Comparing `tspex-0.6.2/setup.py` & `tspex-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 setup(
     name='tspex',
-    version='0.6.2',
+    version='0.6.3',
     packages=find_packages(),
     license='GNU General Public License v3.0',
     description='A Python package for calculating tissue-specificity metrics for gene expression.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=['matplotlib >= 2.2', 'numpy', 'pandas >= 0.23', 'xlrd >= 1.1.0'],
     python_requires='>=3',
```

### Comparing `tspex-0.6.2/tspex/__init__.py` & `tspex-0.6.3/tspex/__init__.py`

 * *Files identical despite different names*

### Comparing `tspex-0.6.2/tspex/cli.py` & `tspex-0.6.3/tspex/cli.py`

 * *Files identical despite different names*

### Comparing `tspex-0.6.2/tspex/core/__init__.py` & `tspex-0.6.3/tspex/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tspex-0.6.2/tspex/core/auxiliary_functions.py` & `tspex-0.6.3/tspex/core/auxiliary_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,19 @@
     References
     ----------
     .. [1] Pan, Jian-Bo, et al. "PaGeFinder: quantitative identification of
            spatiotemporal pattern genes." Bioinformatics 28.11 (2012)
     """
 
     n = len(vector)
-    dispersion_measure = np.std(vector, ddof=1) * np.sqrt(n)
-    return dispersion_measure
+    if n == 1:
+        return 0.0
+    else:
+        dispersion_measure = np.std(vector, ddof=1) * np.sqrt(n)
+        return dispersion_measure
 
 
 def tukey_biweight(vector, c=5, epsilon=1e-4):
     """
     Compute the one-step Tukey's biweight of a vector. Taken from the affy R
     package.
```

### Comparing `tspex-0.6.2/tspex/core/specificity_class.py` & `tspex-0.6.3/tspex/core/specificity_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,17 @@
         if self.expression_data.shape[1] < expression_data.shape[1]:
             warnings.warn(
                 'The input DataFrame contains non-numerical columns. These columns were removed.'
             )
         if np.any(self.expression_data < 0):
             raise ValueError('Negative expression values are not allowed.')
         if self.expression_data.index.duplicated().any():
-            warnings.warn(
+            raise ValueError(
                 'There are duplicated gene names in the input DataFrame index. Please, correct this issue.'
             )
-            return None
         if log:
             self.expression_data = self.expression_data.apply(lambda x: np.log(x + 1))
         self._method = str(method)
         self._transform = kwargs.pop('transform', True)
         self._threshold = kwargs.pop('threshold', 0)
         self.tissue_specificity = self._compute_tissue_specificity()
 
@@ -214,15 +213,15 @@
             sorted_index = expr_data.idxmax(axis=1).sort_values().index
             expr_data = expr_data.reindex(sorted_index)
         if use_zscore:
             expr_data = expr_data.apply(
                 zscore, axis=1, result_type='broadcast', transform=False
             )
         fig, ax = plt.subplots(figsize=size, dpi=dpi, constrained_layout=True)
-        im = ax.imshow(expr_data, cmap=cmap, aspect='auto')
+        im = ax.imshow(expr_data, cmap=cmap, aspect='auto', interpolation='none')
         ax.set_ylabel('Genes')
         ax.set_xlabel('Tissues')
         ax.set_yticks(np.arange(0, len(expr_data.index), 1))
         ax.set_yticklabels(expr_data.index)
         ax.set_xticks(np.arange(0, len(expr_data.columns), 1))
         ax.set_xticklabels(expr_data.columns)
         ax.tick_params(length=0)
```

### Comparing `tspex-0.6.2/tspex/core/specificity_functions.py` & `tspex-0.6.3/tspex/core/specificity_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,17 +105,20 @@
            Bioinformatics 21.5 (2004)
     """
 
     if not np.any(vector):
         return 0.0
     else:
         n = len(vector)
-        vector_r = vector / np.max(vector)
-        tau_index = np.sum(1 - vector_r) / (n - 1)
-        return tau_index
+        if n == 1:
+            return 0.0
+        else:
+            vector_r = vector / np.max(vector)
+            tau_index = np.sum(1 - vector_r) / (n - 1)
+            return tau_index
 
 
 def gini(vector, **kwargs):
     """
     Quantify tissue-specificity as the Gini coefficient [1].
 
     Parameters
@@ -142,21 +145,24 @@
 
     transform = kwargs.pop('transform', True)
     if not np.any(vector):
         return 0.0
     else:
         vector = np.sort(vector)
         n = len(vector)
-        index = np.arange(1, n + 1)
-        gini_coefficient = (np.sum((2 * index - n - 1) * vector)) / (n * np.sum(vector))
-        if transform:
-            transformed_gini_coefficient = gini_coefficient * (n / (n - 1))
-            return transformed_gini_coefficient
+        if n == 1:
+            return 0.0
         else:
-            return gini_coefficient
+            index = np.arange(1, n + 1)
+            gini_coefficient = (np.sum((2 * index - n - 1) * vector)) / (n * np.sum(vector))
+            if transform:
+                transformed_gini_coefficient = gini_coefficient * (n / (n - 1))
+                return transformed_gini_coefficient
+            else:
+                return gini_coefficient
 
 
 def simpson(vector, **kwargs):
     """
     Quantify tissue-specificity as the Simpson index [1].
 
     Parameters
@@ -179,22 +185,26 @@
     .. [1] Simpson, Edward H. "Measurement of diversity." Nature 163.4148 (1949)
     """
 
     transform = kwargs.pop('transform', True)
     if not np.any(vector):
         return 0.0
     else:
-        p = vector / np.sum(vector)
-        simpson_index = np.sum(p ** 2)
-        if transform:
-            min_simpson = 1 / len(vector)
-            transformed_simpson_index = (simpson_index - min_simpson) / (1 - min_simpson)
-            return transformed_simpson_index
+        n = len(vector)
+        if n == 1:
+            return 0.0
         else:
-            return simpson_index
+            p = vector / np.sum(vector)
+            simpson_index = np.sum(p ** 2)
+            if transform:
+                min_simpson = 1 / len(vector)
+                transformed_simpson_index = (simpson_index - min_simpson) / (1 - min_simpson)
+                return transformed_simpson_index
+            else:
+                return simpson_index
 
 
 def shannon_specificity(vector, **kwargs):
     """
     Quantify tissue-specificity using Shannon entropy [1]. Specifically, this
     metric corresponds to the difference between the maximum and the observed
     vector entropy.
@@ -221,20 +231,23 @@
     """
 
     transform = kwargs.pop('transform', True)
     if not np.any(vector):
         return 0.0
     else:
         n = len(vector)
-        ss = np.log2(n) - entropy(vector)
-        if transform:
-            ss_transformed = ss / np.log2(n)
-            return ss_transformed
+        if n == 1:
+            return 0.0
         else:
-            return ss
+            ss = np.log2(n) - entropy(vector)
+            if transform:
+                ss_transformed = ss / np.log2(n)
+                return ss_transformed
+            else:
+                return ss
 
 
 def roku_specificity(vector, **kwargs):
     """
     Quantify tissue-specificity using the ROKU method [1], in which the
     expression vector is processed and used to compute the Shannon entropy [2].
     Data processing is done by subtracting the one-step Tukey's biweight and
@@ -265,20 +278,23 @@
     """
 
     transform = kwargs.pop('transform', True)
     if not np.any(vector):
         return 0.0
     else:
         n = len(vector)
-        rs = np.log2(n) - roku(vector)
-        if transform:
-            rs_transformed = rs / np.log2(n)
-            return rs_transformed
+        if n == 1:
+            return 0.0
         else:
-            return rs
+            rs = np.log2(n) - roku(vector)
+            if transform:
+                rs_transformed = rs / np.log2(n)
+                return rs_transformed
+            else:
+                return rs
 
 
 def tsi(vector, **kwargs):
     """
     Quantify tissue-specificity as the ratio between the expression vector
     and the sum of the expression values in all tissues.
 
@@ -297,18 +313,22 @@
     References
     ----------
     .. [1] Julien, Philippe, et al. "Mechanisms and evolutionary patterns of
            mammalian and avian dosage compensation." PLoS biology 10.5 (2012)
     """
 
     if not np.any(vector):
-        return 0.0
+        return np.array([0.0])
     else:
-        tissue_specificity_index = vector / np.sum(vector)
-        return tissue_specificity_index
+        n = len(vector)
+        if n == 1:
+            return np.array([0.0])
+        else:
+            tissue_specificity_index = vector / np.sum(vector)
+            return tissue_specificity_index
 
 
 def zscore(vector, **kwargs):
     """
     Quantify tissue-specificity as z-scores.
 
     Parameters
@@ -331,25 +351,28 @@
     .. [1] Kryuchkova-Mostacci, Nadezda, and Marc Robinson-Rechavi. "A benchmark
            of gene expression tissue-specificity metrics." Briefings in
            bioinformatics 18.2 (2017)
     """
 
     transform = kwargs.pop('transform', True)
     n = len(vector)
-    std = np.std(vector, ddof=1)
-    if std == 0:
-        return np.zeros(n)
+    if n == 1:
+        return np.array([0.0])
     else:
-        zs = (vector - np.mean(vector)) / std
-        if transform:
-            max_zs = (n - 1) / np.sqrt(n)
-            zs_transformed = (zs + max_zs) / (2 * max_zs)
-            return zs_transformed
+        std = np.std(vector, ddof=1)
+        if std == 0:
+            return np.zeros(n)
         else:
-            return zs
+            zs = (vector - np.mean(vector)) / std
+            if transform:
+                max_zs = (n - 1) / np.sqrt(n)
+                zs_transformed = (zs + max_zs) / (2 * max_zs)
+                return zs_transformed
+            else:
+                return zs
 
 
 def spm(vector, **kwargs):
     """
     Quantify tissue-specificity as the Specificity Measure (SPM) [1,2].
 
     Parameters
@@ -369,22 +392,25 @@
     .. [1] Xiao, Sheng-Jian, et al. "TiSGeD: a database for tissue-specific
            genes." Bioinformatics 26.9 (2010)
     .. [2] Pan, Jian-Bo, et al. "PaGeFinder: quantitative identification of
            spatiotemporal pattern genes." Bioinformatics 28.11 (2012)
     """
 
     n = len(vector)
-    spm_vector = []
-    for i in range(n):
-        if vector[i] == 0:
-            spm_vector.append(0)
-        else:
-            spm_i = (vector[i] ** 2) / (np.linalg.norm(vector) * vector[i])
-            spm_vector.append(spm_i)
-    return np.array(spm_vector)
+    if n == 1:
+        return np.array([0.0])
+    else:
+        spm_vector = []
+        for i in range(n):
+            if vector[i] == 0:
+                spm_vector.append(0)
+            else:
+                spm_i = (vector[i] ** 2) / (np.linalg.norm(vector) * vector[i])
+                spm_vector.append(spm_i)
+        return np.array(spm_vector)
 
 
 def spm_dpm(vector, **kwargs):
     """
     Quantify tissue-specificity as the Dispersion Measure (DPM) [1] computed
     with SPM values.
 
@@ -432,24 +458,27 @@
     ----------
     .. [1] Cabili, Moran N., et al. "Integrative annotation of human large
            intergenic noncoding RNAs reveals global properties and specific
            subclasses." Genes & development 25.18 (2011)
     """
 
     n = len(vector)
-    js_vector = []
-    for i in range(n):
-        if vector[i] == 0:
-            js_vector.append(0)
-        else:
-            vector_i = np.zeros(n)
-            vector_i[i] = vector[i]
-            js_i = 1 - js_distance(vector, vector_i)
-            js_vector.append(js_i)
-    return np.array(js_vector)
+    if n == 1:
+        return np.array([0.0])
+    else:
+        js_vector = []
+        for i in range(n):
+            if vector[i] == 0:
+                js_vector.append(0)
+            else:
+                vector_i = np.zeros(n)
+                vector_i[i] = vector[i]
+                js_i = 1 - js_distance(vector, vector_i)
+                js_vector.append(js_i)
+        return np.array(js_vector)
 
 
 def js_specificity_dpm(vector, **kwargs):
     """
     Quantify tissue-specificity as the Dispersion Measure (DPM) [1] computed
     with Jensen-Shannon distance-based specificity [2] values.
```

### Comparing `tspex-0.6.2/tspex.egg-info/PKG-INFO` & `tspex-0.6.3/tspex.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: tspex
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python package for calculating tissue-specificity metrics for gene expression.
 Home-page: https://apcamargo.github.io/tspex/
 Author: Antonio Pedro Camargo
 Author-email: antoniop.camargo@gmail.com
 License: GNU General Public License v3.0
 Description: # tspex
         
+        [![DOI](https://img.shields.io/badge/DOI-10.21203%2Frs.3.rs--51998%2Fv1-red)](https://doi.org/10.21203/rs.3.rs-51998/v1)
+        [![PyPI](https://img.shields.io/pypi/v/tspex.svg?label=PyPI&color=green)](https://pypi.python.org/pypi/tspex)
+        [![Conda](https://img.shields.io/conda/vn/bioconda/tspex.svg?label=Conda&color=green)](https://anaconda.org/bioconda/tspex)
+        [![PyPI downloads](https://img.shields.io/pypi/dm/tspex?label=PyPI%20downloads&color=blue)](https://pypi.python.org/pypi/tspex)
+        [![Conda downloads](https://img.shields.io/conda/dn/bioconda/tspex.svg?label=Conda%20downloads&color=blue)](https://anaconda.org/bioconda/tspex)
         
         - [Overview](#overview)
+        - [Citation](#citation)
         - [Documentation](#documentation)
         - [Installation](#installation)
         - [Python API tutorial](#python-api-tutorial)
         - [Command-line interface](#command-line-interface)
         - [Examples](#examples)
         
         ## Overview
@@ -22,14 +28,21 @@
         
         tspex features include:
           - Twelve different tissue-specificity metrics.
           - Integration with popular data analysis libraries, such as NumPy, SciPy, and pandas.
           - Visualization functions.
           - Support for Jupyter notebooks.
         
+        
+        ## Citation
+        
+        If you use tspex in your research, it would be appreciated if you could cite it.
+        
+        > Camargo, A. P., Vasconcelos, A. A., Fiamenghi, M. B., Pereira, G. A. G. & Carazzolle, M. F.. "[tspex: a tissue-specificity calculator for gene expression data](https://www.researchsquare.com/article/rs-51998/v1)" *Preprint available at Research Square* (2020).
+        
         ## Web version
         
         tspex can be used through a web interface that is freely available online at [https://tspex.lge.ibi.unicamp.br/](https://tspex.lge.ibi.unicamp.br/). The source code of the web app can be found at [https://github.com/apcamargo/tspex-webapp/](https://github.com/apcamargo/tspex-webapp/).
         
         ## Documentation
         
         A complete documentation for tspex can be found at [https://apcamargo.github.io/tspex/](https://apcamargo.github.io/tspex/).
@@ -109,23 +122,14 @@
         
         - Using the `zscore` without transformation to quantify tissue-specificity as the number of standard deviations away from the mean gene expression:
         
         ```
         tspex --disable_transformation gene_expression.tsv tspex_zscore.tsv zscore
         ```
         
-        
-        ## Cite tspex
-        
-        If you use tspex in your research, it would be appreciated if you could cite it.
-        
-        [![DOI](https://zenodo.org/badge/172384291.svg)](https://zenodo.org/badge/latestdoi/172384291)
-        
-        > Camargo, Antonio P., "*tspex: tissue-specificity calculator*" (2019). doi:10.5281/zenodo.3558708
-        
 Keywords: bioinformatics,gene expression,tissue-specificity,transcriptomics
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

