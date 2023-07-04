# Comparing `tmp/tissue-tag-0.1.4.tar.gz` & `tmp/tissue_tag-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-tag-0.1.4.tar", last modified: Tue Jul  4 15:58:45 2023, max compression
+gzip compressed data, was "tissue_tag-0.1.5.tar", last modified: Tue Jul  4 16:03:16 2023, max compression
```

## Comparing `tissue-tag-0.1.4.tar` & `tissue_tag-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.4/LICENSE
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1764 2023-07-04 15:55:26.000000 tissue-tag-0.1.4/README.md
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/setup.cfg
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-04 15:58:37.000000 tissue-tag-0.1.4/setup.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/tissue_tag/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:55:26.000000 tissue-tag-0.1.4/tissue_tag/__init__.py
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)    45249 2023-07-04 15:55:26.000000 tissue-tag-0.1.4/tissue_tag/tissue_tag.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:58:45.584157 tissue-tag-0.1.4/tissue_tag.egg-info/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      243 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/requires.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       11 2023-07-04 15:58:45.000000 tissue-tag-0.1.4/tissue_tag.egg-info/top_level.txt
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 16:03:16.224341 tissue_tag-0.1.5/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue_tag-0.1.5/LICENSE
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 16:03:16.224341 tissue_tag-0.1.5/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1764 2023-07-04 15:55:26.000000 tissue_tag-0.1.5/README.md
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-04 16:03:16.224341 tissue_tag-0.1.5/setup.cfg
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-04 16:02:22.000000 tissue_tag-0.1.5/setup.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 16:03:16.224341 tissue_tag-0.1.5/tissue_tag/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 15:55:26.000000 tissue_tag-0.1.5/tissue_tag/__init__.py
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)    45249 2023-07-04 15:55:26.000000 tissue_tag-0.1.5/tissue_tag/tissue_tag.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-04 16:03:16.224341 tissue_tag-0.1.5/tissue_tag.egg-info/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2148 2023-07-04 16:03:16.000000 tissue_tag-0.1.5/tissue_tag.egg-info/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      243 2023-07-04 16:03:16.000000 tissue_tag-0.1.5/tissue_tag.egg-info/SOURCES.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-04 16:03:16.000000 tissue_tag-0.1.5/tissue_tag.egg-info/dependency_links.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-04 16:03:16.000000 tissue_tag-0.1.5/tissue_tag.egg-info/requires.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       11 2023-07-04 16:03:16.000000 tissue_tag-0.1.5/tissue_tag.egg-info/top_level.txt
```

### Comparing `tissue-tag-0.1.4/LICENSE` & `tissue_tag-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.4/PKG-INFO` & `tissue_tag-0.1.5/tissue_tag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tissue-tag
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `tissue-tag-0.1.4/README.md` & `tissue_tag-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.4/setup.py` & `tissue_tag-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    name='tissue-tag',
-    version='0.1.4',
+    name='tissue_tag',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'opencv-python',
         'Pillow',
         'bokeh',
         'jupyter-bokeh',
         'matplotlib',
```

### Comparing `tissue-tag-0.1.4/tissue_tag/tissue_tag.py` & `tissue_tag-0.1.5/tissue_tag/tissue_tag.py`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.4/tissue_tag.egg-info/PKG-INFO` & `tissue_tag-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tissue-tag
-Version: 0.1.4
+Name: tissue_tag
+Version: 0.1.5
 Summary: Tissue Tag: jupyter image annotator
 Home-page: https://github.com/nadavyayon/TissueTag
 Author: Oren Amsalem, Nadav Yayon
 Author-email: nadav.yayon@mail.huji.ac.il
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

