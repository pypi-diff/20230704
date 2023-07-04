# Comparing `tmp/JBioSeqTools-1.1.4.tar.gz` & `tmp/JBioSeqTools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-1.1.4.tar", last modified: Tue Jul  4 09:43:22 2023, max compression
+gzip compressed data, was "JBioSeqTools-1.1.5.tar", last modified: Tue Jul  4 10:20:12 2023, max compression
```

## Comparing `JBioSeqTools-1.1.4.tar` & `JBioSeqTools-1.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.971984 JBioSeqTools-1.1.4/JBioSeqTools/
--rw-rw-rw-   0        0        0      344 2022-12-15 18:39:54.000000 JBioSeqTools-1.1.4/JBioSeqTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/api_elements/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/api_elements/__init__.py
--rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.4/JBioSeqTools/api_elements/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/__init__.py
--rw-rw-rw-   0        0        0    18682 2023-07-04 08:31:50.000000 JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/seq_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/vector_build/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_build/__init__.py
--rw-rw-rw-   0        0        0    47172 2023-07-04 08:30:28.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_build/vector_build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.985047 JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/graph_plot.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.971984 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1000 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 09:43:22.000000 JBioSeqTools-1.1.4/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1000 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/data/
--rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.4/data/backbone.xlsx
--rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.4/data/codons.xlsx
--rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.4/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.4/data/linkers.xlsx
--rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.4/data/promoters.xlsx
--rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.4/data/regulators.xlsx
--rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.4/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.4/data/vectors.xlsx
--rw-rw-rw-   0        0        0       42 2023-07-04 09:43:22.999003 JBioSeqTools-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1421 2023-07-04 08:37:40.000000 JBioSeqTools-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.332359 JBioSeqTools-1.1.5/JBioSeqTools/
+-rw-rw-rw-   0        0        0      343 2023-07-04 10:19:10.000000 JBioSeqTools-1.1.5/JBioSeqTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.341772 JBioSeqTools-1.1.5/JBioSeqTools/api_elements/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/api_elements/__init__.py
+-rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.5/JBioSeqTools/api_elements/api.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.348298 JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/__init__.py
+-rw-rw-rw-   0        0        0    18698 2023-07-04 10:17:29.000000 JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/seq_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.348298 JBioSeqTools-1.1.5/JBioSeqTools/vector_build/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_build/__init__.py
+-rw-rw-rw-   0        0        0    47188 2023-07-04 10:18:13.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_build/vector_build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.348298 JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/
+-rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/graph_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.341772 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1000 2023-07-04 10:20:11.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-07-04 10:20:12.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 10:20:11.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-04 10:20:12.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 10:20:12.000000 JBioSeqTools-1.1.5/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1000 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/data/
+-rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.5/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.5/data/codons.xlsx
+-rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.5/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.5/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.5/data/promoters.xlsx
+-rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.5/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.5/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.5/data/vectors.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-04 10:20:12.353170 JBioSeqTools-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2023-07-04 10:18:52.000000 JBioSeqTools-1.1.5/setup.py
```

### Comparing `JBioSeqTools-1.1.4/JBioSeqTools/api_elements/api.py` & `JBioSeqTools-1.1.5/JBioSeqTools/api_elements/api.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/JBioSeqTools/seq_tools/seq_tools.py` & `JBioSeqTools-1.1.5/JBioSeqTools/seq_tools/seq_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     return sequence  
                 
 
 
 
 
 def codon_otymization(sequence:str(), codons:pd.DataFrame, species:str()):
-    codons = codons[codons['Species'] == species]
+    codons = codons[codons['Species'] == species.lower()]
     seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
     seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq_codon]
     seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
     
     seq_codon_mean = ''.join(seq_codon).count('C')
     seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
     seq_aa = []
@@ -248,15 +248,15 @@
 
 
 
 
 def repair_sequence(sequence:str(), codons:pd.DataFrame, restriction_df:pd.DataFrame(), restriction:pd.DataFrame(), enzyme_list:list(), species:str()):
     if len(restriction_df) != 0:
         not_repaired = []
-        codons = codons[codons['Species'] == species]
+        codons = codons[codons['Species'] == species.lower()]
         seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
         seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq][codons['Fraction'][codons['Triplet'] == seq].index[0]] for seq in seq_codon]
         seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
         seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
         
         seq_aa = []
         for element in seq_codon:
```

### Comparing `JBioSeqTools-1.1.4/JBioSeqTools/vector_build/vector_build.py` & `JBioSeqTools-1.1.5/JBioSeqTools/vector_build/vector_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
     return project
 
 
 
 
 def codon_otymization(sequence:str(), codons:pd.DataFrame, species:str()):
-    codons = codons[codons['Species'] == species]
+    codons = codons[codons['Species'] == species.lower()]
     seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
     seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq.upper()][codons['Fraction'][codons['Triplet'] == seq.upper()].index[0]] for seq in seq_codon]
     seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
     
     seq_codon_mean = ''.join(seq_codon).count('C')
     seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
     seq_aa = []
@@ -582,15 +582,15 @@
 
 
 
 
 def repair_sequences(sequence:str(), codons:pd.DataFrame, restriction_df:pd.DataFrame(), restriction:pd.DataFrame(), enzyme_list:list(), species:str()):
     if len(restriction_df) != 0:
         not_repaired = []
-        codons = codons[codons['Species'] == species]
+        codons = codons[codons['Species'] == species.lower()]
         seq_codon = [sequence[y:y+3].upper() for y in range(0, len(sequence), 3)]
         seq_codon_fr = [codons['Fraction'][codons['Triplet'] == seq.upper()][codons['Fraction'][codons['Triplet'] == seq.upper()].index[0]] for seq in seq_codon]
         seq_codon_fr = round(sum(seq_codon_fr) / len(seq_codon_fr),2)
         seq_codon_GC = (''.join(seq_codon).count('C') + ''.join(seq_codon).count('G')) / len(''.join(seq_codon)) * 100
         
         seq_aa = []
         for element in seq_codon:
```

### Comparing `JBioSeqTools-1.1.4/JBioSeqTools/vector_graph/graph_plot.py` & `JBioSeqTools-1.1.5/JBioSeqTools/vector_graph/graph_plot.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-1.1.5/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.4
+Version: 1.1.5
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.4/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-1.1.5/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/LICENSE` & `JBioSeqTools-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/PKG-INFO` & `JBioSeqTools-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.4
+Version: 1.1.5
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.4/README.md` & `JBioSeqTools-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/backbone.xlsx` & `JBioSeqTools-1.1.5/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/codons.xlsx` & `JBioSeqTools-1.1.5/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/fluorescent_tag.xlsx` & `JBioSeqTools-1.1.5/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/linkers.xlsx` & `JBioSeqTools-1.1.5/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/promoters.xlsx` & `JBioSeqTools-1.1.5/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/regulators.xlsx` & `JBioSeqTools-1.1.5/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/restriction_enzymes.xlsx` & `JBioSeqTools-1.1.5/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/data/vectors.xlsx` & `JBioSeqTools-1.1.5/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.4/setup.py` & `JBioSeqTools-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.4' 
+VERSION = '1.1.5' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the python library for biological sequence optimization (GC % content & codon frequency) for better expression of different species cells in vivo. It also allows building AAV vectors with the possibility of choosing sequences between ITRs such as transcript, promoter, enhancer, and molecular fluorescent tag. Finally, the user obtains ready for order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

