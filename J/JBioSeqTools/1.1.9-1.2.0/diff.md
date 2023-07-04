# Comparing `tmp/JBioSeqTools-1.1.9.tar.gz` & `tmp/JBioSeqTools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-1.1.9.tar", last modified: Tue Jul  4 13:14:27 2023, max compression
+gzip compressed data, was "JBioSeqTools-1.2.0.tar", last modified: Tue Jul  4 13:17:03 2023, max compression
```

## Comparing `JBioSeqTools-1.1.9.tar` & `JBioSeqTools-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.141854 JBioSeqTools-1.1.9/
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.115567 JBioSeqTools-1.1.9/JBioSeqTools/
--rw-rw-rw-   0        0        0      343 2023-07-04 13:13:50.000000 JBioSeqTools-1.1.9/JBioSeqTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.124101 JBioSeqTools-1.1.9/JBioSeqTools/api_elements/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.9/JBioSeqTools/api_elements/__init__.py
--rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.9/JBioSeqTools/api_elements/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.126108 JBioSeqTools-1.1.9/JBioSeqTools/seq_tools/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.9/JBioSeqTools/seq_tools/__init__.py
--rw-rw-rw-   0        0        0    18804 2023-07-04 13:07:41.000000 JBioSeqTools-1.1.9/JBioSeqTools/seq_tools/seq_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.127099 JBioSeqTools-1.1.9/JBioSeqTools/vector_build/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.9/JBioSeqTools/vector_build/__init__.py
--rw-rw-rw-   0        0        0    47553 2023-07-04 13:07:18.000000 JBioSeqTools-1.1.9/JBioSeqTools/vector_build/vector_build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.129563 JBioSeqTools-1.1.9/JBioSeqTools/vector_graph/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.9/JBioSeqTools/vector_graph/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.9/JBioSeqTools/vector_graph/graph_plot.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.120994 JBioSeqTools-1.1.9/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1000 2023-07-04 13:14:26.000000 JBioSeqTools-1.1.9/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-07-04 13:14:26.000000 JBioSeqTools-1.1.9/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:14:26.000000 JBioSeqTools-1.1.9/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-04 13:14:26.000000 JBioSeqTools-1.1.9/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 13:14:26.000000 JBioSeqTools-1.1.9/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.9/LICENSE
--rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1000 2023-07-04 13:14:27.140830 JBioSeqTools-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 13:14:27.139459 JBioSeqTools-1.1.9/data/
--rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.9/data/backbone.xlsx
--rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.9/data/codons.xlsx
--rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.9/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.9/data/linkers.xlsx
--rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.9/data/promoters.xlsx
--rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.9/data/regulators.xlsx
--rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.9/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.9/data/vectors.xlsx
--rw-rw-rw-   0        0        0       42 2023-07-04 13:14:27.141854 JBioSeqTools-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1457 2023-07-04 13:13:46.000000 JBioSeqTools-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.898547 JBioSeqTools-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.872925 JBioSeqTools-1.2.0/JBioSeqTools/
+-rw-rw-rw-   0        0        0      343 2023-07-04 13:16:57.000000 JBioSeqTools-1.2.0/JBioSeqTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.872925 JBioSeqTools-1.2.0/JBioSeqTools/api_elements/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.0/JBioSeqTools/api_elements/__init__.py
+-rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.2.0/JBioSeqTools/api_elements/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.872925 JBioSeqTools-1.2.0/JBioSeqTools/seq_tools/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.0/JBioSeqTools/seq_tools/__init__.py
+-rw-rw-rw-   0        0        0    18804 2023-07-04 13:07:41.000000 JBioSeqTools-1.2.0/JBioSeqTools/seq_tools/seq_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.872925 JBioSeqTools-1.2.0/JBioSeqTools/vector_build/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.0/JBioSeqTools/vector_build/__init__.py
+-rw-rw-rw-   0        0        0    47542 2023-07-04 13:16:14.000000 JBioSeqTools-1.2.0/JBioSeqTools/vector_build/vector_build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.885938 JBioSeqTools-1.2.0/JBioSeqTools/vector_graph/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.2.0/JBioSeqTools/vector_graph/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.2.0/JBioSeqTools/vector_graph/graph_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.872925 JBioSeqTools-1.2.0/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1000 2023-07-04 13:17:03.000000 JBioSeqTools-1.2.0/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-07-04 13:17:03.000000 JBioSeqTools-1.2.0/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:17:03.000000 JBioSeqTools-1.2.0/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-04 13:17:03.000000 JBioSeqTools-1.2.0/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 13:17:03.000000 JBioSeqTools-1.2.0/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1000 2023-07-04 13:17:03.898547 JBioSeqTools-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 13:17:03.897231 JBioSeqTools-1.2.0/data/
+-rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.2.0/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.2.0/data/codons.xlsx
+-rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.2.0/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.2.0/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.2.0/data/promoters.xlsx
+-rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.2.0/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.2.0/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.2.0/data/vectors.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-04 13:17:03.898547 JBioSeqTools-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1457 2023-07-04 13:16:52.000000 JBioSeqTools-1.2.0/setup.py
```

### Comparing `JBioSeqTools-1.1.9/JBioSeqTools/api_elements/api.py` & `JBioSeqTools-1.2.0/JBioSeqTools/api_elements/api.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/JBioSeqTools/seq_tools/seq_tools.py` & `JBioSeqTools-1.2.0/JBioSeqTools/seq_tools/seq_tools.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/JBioSeqTools/vector_build/vector_build.py` & `JBioSeqTools-1.2.0/JBioSeqTools/vector_build/vector_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 import pkg_resources
 
 
 
 
-def load_metadata(codons:str() = pkg_resources.resource_filename('JBioSeqTools', '../../data/codons.xlsx'), vectors:str() = pkg_resources.resource_filename('JBioSeqTools', 'vectors.xlsx'), linkers:str() = pkg_resources.resource_filename('JBioSeqTools',  'linkers.xlsx'), regulators:str() = pkg_resources.resource_filename('JBioSeqTools', 'regulators.xlsx'), fluorescent_tag:str() = pkg_resources.resource_filename('JBioSeqTools',  'fluorescent_tag.xlsx'), backbone:str() = pkg_resources.resource_filename('JBioSeqTools', 'backbone.xlsx'), promoters:str() = pkg_resources.resource_filename('JBioSeqTools', 'promoters.xlsx'), restriction:str() = pkg_resources.resource_filename('JBioSeqTools', 'restriction_enzymes.xlsx')):
+def load_metadata(codons:str() = pkg_resources.resource_filename('JBioSeqTools', 'codons.xlsx'), vectors:str() = pkg_resources.resource_filename('JBioSeqTools', 'vectors.xlsx'), linkers:str() = pkg_resources.resource_filename('JBioSeqTools',  'linkers.xlsx'), regulators:str() = pkg_resources.resource_filename('JBioSeqTools', 'regulators.xlsx'), fluorescent_tag:str() = pkg_resources.resource_filename('JBioSeqTools',  'fluorescent_tag.xlsx'), backbone:str() = pkg_resources.resource_filename('JBioSeqTools', 'backbone.xlsx'), promoters:str() = pkg_resources.resource_filename('JBioSeqTools', 'promoters.xlsx'), restriction:str() = pkg_resources.resource_filename('JBioSeqTools', 'restriction_enzymes.xlsx')):
     codons = pd.read_excel(codons)
     vectors = pd.read_excel(vectors)
     linkers = pd.read_excel(linkers)
     regulators = pd.read_excel(regulators)
     fluorescent_tag = pd.read_excel(fluorescent_tag)
     backbone = pd.read_excel(backbone)
     promoters = pd.read_excel(promoters)
```

### Comparing `JBioSeqTools-1.1.9/JBioSeqTools/vector_graph/graph_plot.py` & `JBioSeqTools-1.2.0/JBioSeqTools/vector_graph/graph_plot.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-1.2.0/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.9
+Version: 1.2.0
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.9/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-1.2.0/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/LICENSE` & `JBioSeqTools-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/PKG-INFO` & `JBioSeqTools-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.9
+Version: 1.2.0
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.9/README.md` & `JBioSeqTools-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/backbone.xlsx` & `JBioSeqTools-1.2.0/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/codons.xlsx` & `JBioSeqTools-1.2.0/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/fluorescent_tag.xlsx` & `JBioSeqTools-1.2.0/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/linkers.xlsx` & `JBioSeqTools-1.2.0/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/promoters.xlsx` & `JBioSeqTools-1.2.0/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/regulators.xlsx` & `JBioSeqTools-1.2.0/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/restriction_enzymes.xlsx` & `JBioSeqTools-1.2.0/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/data/vectors.xlsx` & `JBioSeqTools-1.2.0/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.9/setup.py` & `JBioSeqTools-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.9' 
+VERSION = '1.2.0' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the python library for biological sequence optimization (GC % content & codon frequency) for better expression of different species cells in vivo. It also allows building AAV vectors with the possibility of choosing sequences between ITRs such as transcript, promoter, enhancer, and molecular fluorescent tag. Finally, the user obtains ready for order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

