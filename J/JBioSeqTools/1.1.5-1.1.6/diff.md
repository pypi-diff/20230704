# Comparing `tmp/JBioSeqTools-1.1.5.tar.gz` & `tmp/JBioSeqTools-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-1.1.5.tar", last modified: Tue Jul  4 10:20:12 2023, max compression
+gzip compressed data, was "JBioSeqTools-1.1.6.tar", last modified: Tue Jul  4 12:41:46 2023, max compression
```

## Comparing `JBioSeqTools-1.1.5.tar` & `JBioSeqTools-1.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.332359 JBioSeqTools-1.1.5/JBioSeqTools/
--rw-rw-rw-   0        0        0      343 2023-07-04 10:19:10.000000 JBioSeqTools-1.1.5/JBioSeqTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.341772 JBioSeqTools-1.1.5/JBioSeqTools/api_elements/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/api_elements/__init__.py
--rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.5/JBioSeqTools/api_elements/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.348298 JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/__init__.py
--rw-rw-rw-   0        0        0    18698 2023-07-04 10:17:29.000000 JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/seq_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.348298 JBioSeqTools-1.1.5/JBioSeqTools/vector_build/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_build/__init__.py
--rw-rw-rw-   0        0        0    47188 2023-07-04 10:18:13.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_build/vector_build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.348298 JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/graph_plot.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.341772 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1000 2023-07-04 10:20:11.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-07-04 10:20:12.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:20:11.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-04 10:20:12.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 10:20:12.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1000 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/data/
--rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.5/data/backbone.xlsx
--rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.5/data/codons.xlsx
--rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.5/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.5/data/linkers.xlsx
--rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.5/data/promoters.xlsx
--rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.5/data/regulators.xlsx
--rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.5/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.5/data/vectors.xlsx
--rw-rw-rw-   0        0        0       42 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1421 2023-07-04 10:18:52.000000 JBioSeqTools-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.816467 JBioSeqTools-1.1.6/
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.772374 JBioSeqTools-1.1.6/JBioSeqTools/
+-rw-rw-rw-   0        0        0      343 2023-07-04 12:38:01.000000 JBioSeqTools-1.1.6/JBioSeqTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.783883 JBioSeqTools-1.1.6/JBioSeqTools/api_elements/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.6/JBioSeqTools/api_elements/__init__.py
+-rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.6/JBioSeqTools/api_elements/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.789903 JBioSeqTools-1.1.6/JBioSeqTools/seq_tools/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.6/JBioSeqTools/seq_tools/__init__.py
+-rw-rw-rw-   0        0        0    18704 2023-07-04 12:39:40.000000 JBioSeqTools-1.1.6/JBioSeqTools/seq_tools/seq_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.796390 JBioSeqTools-1.1.6/JBioSeqTools/vector_build/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.6/JBioSeqTools/vector_build/__init__.py
+-rw-rw-rw-   0        0        0    47212 2023-07-04 12:40:31.000000 JBioSeqTools-1.1.6/JBioSeqTools/vector_build/vector_build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.801762 JBioSeqTools-1.1.6/JBioSeqTools/vector_graph/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.6/JBioSeqTools/vector_graph/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.6/JBioSeqTools/vector_graph/graph_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.778902 JBioSeqTools-1.1.6/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1000 2023-07-04 12:41:46.000000 JBioSeqTools-1.1.6/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-07-04 12:41:46.000000 JBioSeqTools-1.1.6/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 12:41:46.000000 JBioSeqTools-1.1.6/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-04 12:41:46.000000 JBioSeqTools-1.1.6/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 12:41:46.000000 JBioSeqTools-1.1.6/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1000 2023-07-04 12:41:46.815466 JBioSeqTools-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 12:41:46.814454 JBioSeqTools-1.1.6/data/
+-rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.6/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.6/data/codons.xlsx
+-rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.6/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.6/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.6/data/promoters.xlsx
+-rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.6/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.6/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.6/data/vectors.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-04 12:41:46.816467 JBioSeqTools-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2023-07-04 12:37:48.000000 JBioSeqTools-1.1.6/setup.py
```

### Comparing `JBioSeqTools-1.1.5/JBioSeqTools/api_elements/api.py` & `JBioSeqTools-1.1.6/JBioSeqTools/api_elements/api.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/seq_tools.py` & `JBioSeqTools-1.1.6/JBioSeqTools/seq_tools/seq_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 pd.options.mode.chained_assignment = None
 import numpy as np
 from tqdm import tqdm
 
 
 
-def load_metadata(codons:str() = '../data/codons.xlsx', restriction:str() = '../data/restriction_enzymes.xlsx'):
+def load_metadata(codons:str() = '../../data/codons.xlsx', restriction:str() = '../../data/restriction_enzymes.xlsx'):
     codons = pd.read_excel(codons)
     restriction = pd.read_excel(restriction)
     
     metadata = {'codons':codons,'restriction':restriction}
 
     return metadata
```

### Comparing `JBioSeqTools-1.1.5/JBioSeqTools/vector_build/vector_build.py` & `JBioSeqTools-1.1.6/JBioSeqTools/vector_build/vector_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tqdm import tqdm
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 
 
 
-def load_metadata(codons:str() = '../data/codons.xlsx', vectors:str() = '../data/vectors.xlsx', linkers:str() = '../data/linkers.xlsx', regulators:str() = '../data/regulators.xlsx', fluorescent_tag:str() = '../data/fluorescent_tag.xlsx', backbone:str() = '../data/backbone.xlsx', promoters:str() = '../data/promoters.xlsx', restriction:str() = '../data/restriction_enzymes.xlsx'):
+def load_metadata(codons:str() = '../../data/codons.xlsx', vectors:str() = '../../data/vectors.xlsx', linkers:str() = '../../data/linkers.xlsx', regulators:str() = '../../data/regulators.xlsx', fluorescent_tag:str() = '../../data/fluorescent_tag.xlsx', backbone:str() = '../../data/backbone.xlsx', promoters:str() = '../../data/promoters.xlsx', restriction:str() = '../../data/restriction_enzymes.xlsx'):
     codons = pd.read_excel(codons)
     vectors = pd.read_excel(vectors)
     linkers = pd.read_excel(linkers)
     regulators = pd.read_excel(regulators)
     fluorescent_tag = pd.read_excel(fluorescent_tag)
     backbone = pd.read_excel(backbone)
     promoters = pd.read_excel(promoters)
```

### Comparing `JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/graph_plot.py` & `JBioSeqTools-1.1.6/JBioSeqTools/vector_graph/graph_plot.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-1.1.6/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.5
+Version: 1.1.6
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.5/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-1.1.6/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/LICENSE` & `JBioSeqTools-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/PKG-INFO` & `JBioSeqTools-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.5
+Version: 1.1.6
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.5/README.md` & `JBioSeqTools-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/backbone.xlsx` & `JBioSeqTools-1.1.6/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/codons.xlsx` & `JBioSeqTools-1.1.6/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/fluorescent_tag.xlsx` & `JBioSeqTools-1.1.6/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/linkers.xlsx` & `JBioSeqTools-1.1.6/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/promoters.xlsx` & `JBioSeqTools-1.1.6/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/regulators.xlsx` & `JBioSeqTools-1.1.6/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/restriction_enzymes.xlsx` & `JBioSeqTools-1.1.6/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/data/vectors.xlsx` & `JBioSeqTools-1.1.6/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.5/setup.py` & `JBioSeqTools-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.5' 
+VERSION = '1.1.6' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the python library for biological sequence optimization (GC % content & codon frequency) for better expression of different species cells in vivo. It also allows building AAV vectors with the possibility of choosing sequences between ITRs such as transcript, promoter, enhancer, and molecular fluorescent tag. Finally, the user obtains ready for order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

