# Comparing `tmp/JBioSeqTools-1.1.7.tar.gz` & `tmp/JBioSeqTools-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-1.1.7.tar", last modified: Tue Jul  4 12:50:43 2023, max compression
+gzip compressed data, was "JBioSeqTools-1.1.8.tar", last modified: Tue Jul  4 13:09:06 2023, max compression
```

## Comparing `JBioSeqTools-1.1.7.tar` & `JBioSeqTools-1.1.8.tar`

### file list

```diff
@@ -1,36 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.170467 JBioSeqTools-1.1.7/
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.153339 JBioSeqTools-1.1.7/JBioSeqTools/
--rw-rw-rw-   0        0        0      343 2023-07-04 12:49:57.000000 JBioSeqTools-1.1.7/JBioSeqTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.153339 JBioSeqTools-1.1.7/JBioSeqTools/api_elements/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.7/JBioSeqTools/api_elements/__init__.py
--rw-rw-rw-   0        0        0     6152 2022-12-15 18:39:44.000000 JBioSeqTools-1.1.7/JBioSeqTools/api_elements/api.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.153339 JBioSeqTools-1.1.7/JBioSeqTools/seq_tools/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.7/JBioSeqTools/seq_tools/__init__.py
--rw-rw-rw-   0        0        0    18704 2023-07-04 12:39:40.000000 JBioSeqTools-1.1.7/JBioSeqTools/seq_tools/seq_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.168824 JBioSeqTools-1.1.7/JBioSeqTools/vector_build/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.7/JBioSeqTools/vector_build/__init__.py
--rw-rw-rw-   0        0        0    47212 2023-07-04 12:40:31.000000 JBioSeqTools-1.1.7/JBioSeqTools/vector_build/vector_build.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.170467 JBioSeqTools-1.1.7/JBioSeqTools/vector_graph/
--rw-rw-rw-   0        0        0        0 2022-01-10 01:41:35.000000 JBioSeqTools-1.1.7/JBioSeqTools/vector_graph/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-07-04 08:33:55.000000 JBioSeqTools-1.1.7/JBioSeqTools/vector_graph/graph_plot.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.153339 JBioSeqTools-1.1.7/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1000 2023-07-04 12:50:42.000000 JBioSeqTools-1.1.7/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      711 2023-07-04 12:50:42.000000 JBioSeqTools-1.1.7/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 12:50:42.000000 JBioSeqTools-1.1.7/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-04 12:50:42.000000 JBioSeqTools-1.1.7/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 12:50:42.000000 JBioSeqTools-1.1.7/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.7/LICENSE
--rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1000 2023-07-04 12:50:43.170467 JBioSeqTools-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 12:50:43.170467 JBioSeqTools-1.1.7/data/
--rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.7/data/backbone.xlsx
--rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.7/data/codons.xlsx
--rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.7/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.7/data/linkers.xlsx
--rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.7/data/promoters.xlsx
--rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.7/data/regulators.xlsx
--rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.7/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.7/data/vectors.xlsx
--rw-rw-rw-   0        0        0       42 2023-07-04 12:50:43.170467 JBioSeqTools-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1457 2023-07-04 12:49:18.000000 JBioSeqTools-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:09:06.557806 JBioSeqTools-1.1.8/
+drwxrwxrwx   0        0        0        0 2023-07-04 13:09:06.543903 JBioSeqTools-1.1.8/JBioSeqTools/
+-rw-rw-rw-   0        0        0      343 2023-07-04 13:08:29.000000 JBioSeqTools-1.1.8/JBioSeqTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:09:06.549154 JBioSeqTools-1.1.8/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1000 2023-07-04 13:09:05.000000 JBioSeqTools-1.1.8/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-04 13:09:06.000000 JBioSeqTools-1.1.8/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:09:05.000000 JBioSeqTools-1.1.8/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-04 13:09:06.000000 JBioSeqTools-1.1.8/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 13:09:06.000000 JBioSeqTools-1.1.8/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-04 07:17:12.000000 JBioSeqTools-1.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1000 2023-07-04 13:09:06.557806 JBioSeqTools-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8666 2022-12-12 11:02:45.000000 JBioSeqTools-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 13:09:06.556720 JBioSeqTools-1.1.8/data/
+-rw-rw-rw-   0        0        0     8832 2022-12-11 22:51:54.000000 JBioSeqTools-1.1.8/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    12304 2022-11-14 12:08:41.000000 JBioSeqTools-1.1.8/data/codons.xlsx
+-rw-rw-rw-   0        0        0    10901 2022-11-07 22:29:27.000000 JBioSeqTools-1.1.8/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2022-11-07 21:42:47.000000 JBioSeqTools-1.1.8/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    63680 2022-11-13 21:43:05.000000 JBioSeqTools-1.1.8/data/promoters.xlsx
+-rw-rw-rw-   0        0        0     9642 2022-11-07 21:30:01.000000 JBioSeqTools-1.1.8/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   254880 2022-12-05 10:11:38.000000 JBioSeqTools-1.1.8/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0    10149 2022-11-09 17:19:49.000000 JBioSeqTools-1.1.8/data/vectors.xlsx
+-rw-rw-rw-   0        0        0       42 2023-07-04 13:09:06.557806 JBioSeqTools-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1458 2023-07-04 13:08:23.000000 JBioSeqTools-1.1.8/setup.py
```

### Comparing `JBioSeqTools-1.1.7/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-1.1.8/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.7
+Version: 1.1.8
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.7/LICENSE` & `JBioSeqTools-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/PKG-INFO` & `JBioSeqTools-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 1.1.7
+Version: 1.1.8
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-1.1.7/README.md` & `JBioSeqTools-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/backbone.xlsx` & `JBioSeqTools-1.1.8/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/codons.xlsx` & `JBioSeqTools-1.1.8/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/fluorescent_tag.xlsx` & `JBioSeqTools-1.1.8/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/linkers.xlsx` & `JBioSeqTools-1.1.8/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/promoters.xlsx` & `JBioSeqTools-1.1.8/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/regulators.xlsx` & `JBioSeqTools-1.1.8/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/restriction_enzymes.xlsx` & `JBioSeqTools-1.1.8/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/data/vectors.xlsx` & `JBioSeqTools-1.1.8/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-1.1.7/setup.py` & `JBioSeqTools-1.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.7' 
+VERSION = '1.1.8' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the python library for biological sequence optimization (GC % content & codon frequency) for better expression of different species cells in vivo. It also allows building AAV vectors with the possibility of choosing sequences between ITRs such as transcript, promoter, enhancer, and molecular fluorescent tag. Finally, the user obtains ready for order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
         author="Jakub Kubis",
         author_email="jbiosystem@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
-        packages=find_packages(),
+        packages=['JBioSeqTools'],
         include_package_data=True,
         install_requires=['pandas', 'tqdm', 'matplotlib', 'numpy', 'requests'],       
         keywords=['sequence', 'optimization', 'vectors', 'AAV', 'GC', 'restriction enzyme'],
         license = 'MIT',
         classifiers = [
             "Development Status :: 3 - Alpha",
             "Programming Language :: Python :: 3",
```

