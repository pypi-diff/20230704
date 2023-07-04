# Comparing `tmp/tissue-tag-0.1.2.tar.gz` & `tmp/tissue-tag-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-tag-0.1.2.tar", last modified: Sat Jul  1 12:01:01 2023, max compression
+gzip compressed data, was "tissue-tag-0.1.3.tar", last modified: Tue Jul  4 15:50:02 2023, max compression
```

## Comparing `tissue-tag-0.1.2.tar` & `tissue-tag-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.2/LICENSE
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      650 2023-07-01 12:00:11.000000 tissue-tag-0.1.2/README.md
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/setup.cfg
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-01 11:59:22.000000 tissue-tag-0.1.2/setup.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/tissue_tag.egg-info/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      195 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/requires.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/top_level.txt
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.3/LICENSE
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      650 2023-07-01 12:02:23.000000 tissue-tag-0.1.3/README.md
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/setup.cfg
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-04 15:49:38.000000 tissue-tag-0.1.3/setup.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:50:02.023293 tissue-tag-0.1.3/tissue-tag/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:49:10.000000 tissue-tag-0.1.3/tissue-tag/__init__.py
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)    42646 2023-07-01 11:59:22.000000 tissue-tag-0.1.3/tissue-tag/tissue_tag.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:50:02.027293 tissue-tag-0.1.3/tissue_tag.egg-info/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      243 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/SOURCES.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/dependency_links.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/requires.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       11 2023-07-04 15:50:02.000000 tissue-tag-0.1.3/tissue_tag.egg-info/top_level.txt
```

### Comparing `tissue-tag-0.1.2/LICENSE` & `tissue-tag-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.2/PKG-INFO` & `tissue-tag-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPN554AA2TCXSAP6JLSZFACQRQ" width="300" >
+	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPMPLHBMH5KAQK74NAYZFACXRA" width="300" >
 </p>
 
 # Tissue Tag jupyter image annotator
 ??? What does it do, small intro ???
 
 
 ## Installation
```

### Comparing `tissue-tag-0.1.2/README.md` & `tissue-tag-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPN554AA2TCXSAP6JLSZFACQRQ" width="300" >
+	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPMPLHBMH5KAQK74NAYZFACXRA" width="300" >
 </p>
 
 # Tissue Tag jupyter image annotator
 ??? What does it do, small intro ???
 
 
 ## Installation
```

### Comparing `tissue-tag-0.1.2/setup.py` & `tissue-tag-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tissue-tag',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'opencv-python',
         'Pillow',
         'bokeh',
         'jupyter-bokeh',
         'matplotlib',
```

### Comparing `tissue-tag-0.1.2/tissue_tag.egg-info/PKG-INFO` & `tissue-tag-0.1.3/tissue_tag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPN554AA2TCXSAP6JLSZFACQRQ" width="300" >
+	<img src="https://raw.githubusercontent.com/nadavyayon/TissueTag/main/tissueTag_logo.png?token=GHSAT0AAAAAACEBVMPMPLHBMH5KAQK74NAYZFACXRA" width="300" >
 </p>
 
 # Tissue Tag jupyter image annotator
 ??? What does it do, small intro ???
 
 
 ## Installation
```

