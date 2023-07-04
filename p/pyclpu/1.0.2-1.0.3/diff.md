# Comparing `tmp/pyclpu-1.0.2.tar.gz` & `tmp/pyclpu-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclpu-1.0.2.tar", last modified: Fri Jun  9 10:22:21 2023, max compression
+gzip compressed data, was "pyclpu-1.0.3.tar", last modified: Tue Jul  4 13:46:12 2023, max compression
```

## Comparing `pyclpu-1.0.2.tar` & `pyclpu-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 10:22:21.369091 pyclpu-1.0.2/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-09 10:22:21.369091 pyclpu-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7615 2023-06-09 10:09:34.000000 pyclpu-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 10:22:21.356586 pyclpu-1.0.2/pyclpu/
--rw-rw-rw-   0        0        0      629 2023-06-09 10:21:06.000000 pyclpu-1.0.2/pyclpu/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.0.2/pyclpu/constants.py
--rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-1.0.2/pyclpu/formats.py
--rw-rw-rw-   0        0        0    20857 2023-06-09 10:12:34.000000 pyclpu-1.0.2/pyclpu/image.py
--rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.0.2/pyclpu/main.py
--rw-rw-rw-   0        0        0    16301 2023-06-09 09:57:04.000000 pyclpu-1.0.2/pyclpu/manager.py
--rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.0.2/pyclpu/s33293804.py
-drwxrwxrwx   0        0        0        0 2023-06-09 10:22:21.367505 pyclpu-1.0.2/pyclpu.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-06-09 10:22:21.369091 pyclpu-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2295 2023-06-06 23:27:35.000000 pyclpu-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:46:12.187727 pyclpu-1.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-07-04 13:46:12.187727 pyclpu-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7615 2023-06-09 10:25:56.000000 pyclpu-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 13:46:12.179845 pyclpu-1.0.3/pyclpu/
+-rw-rw-rw-   0        0        0      629 2023-07-04 13:44:19.000000 pyclpu-1.0.3/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.0.3/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-1.0.3/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    20857 2023-06-09 10:25:56.000000 pyclpu-1.0.3/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.0.3/pyclpu/main.py
+-rw-rw-rw-   0        0        0    16301 2023-06-09 10:25:56.000000 pyclpu-1.0.3/pyclpu/manager.py
+-rw-rw-rw-   0        0        0    16933 2023-07-04 13:42:30.000000 pyclpu-1.0.3/pyclpu/metrology.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.0.3/pyclpu/s33293804.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:46:12.187352 pyclpu-1.0.3/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-07-04 13:46:11.000000 pyclpu-1.0.3/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-04 13:46:11.000000 pyclpu-1.0.3/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:46:11.000000 pyclpu-1.0.3/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-04 13:46:11.000000 pyclpu-1.0.3/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 13:46:11.000000 pyclpu-1.0.3/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-07-04 13:46:12.189437 pyclpu-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2305 2023-07-04 13:39:23.000000 pyclpu-1.0.3/setup.py
```

### Comparing `pyclpu-1.0.2/LICENSE` & `pyclpu-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/PKG-INFO` & `pyclpu-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.0.2
+Version: 1.0.3
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyclpu-1.0.2/README.md` & `pyclpu-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu/__init__.py` & `pyclpu-1.0.3/pyclpu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-1.0.2/pyclpu/constants.py` & `pyclpu-1.0.3/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu/formats.py` & `pyclpu-1.0.3/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu/image.py` & `pyclpu-1.0.3/pyclpu/image.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu/main.py` & `pyclpu-1.0.3/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu/manager.py` & `pyclpu-1.0.3/pyclpu/manager.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu/s33293804.py` & `pyclpu-1.0.3/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.2/pyclpu.egg-info/PKG-INFO` & `pyclpu-1.0.3/pyclpu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.0.2
+Version: 1.0.3
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyclpu-1.0.2/setup.py` & `pyclpu-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     author_email='mehret@clpu.es',\
     url='https://git.clpu.es/mehret/pyclpu',\
     license='MIT',\
     packages=['pyclpu'],
     scripts=glob.glob("pyclpu/*.py"),
     install_requires=[\
         'numpy','scipy','opencv-python','cython','pillow',\
-        'matplotlib',\
+        'matplotlib','tkinter',\
     ],\
     # and build in modules cython, importlib.reload, inspect.getsourcefile, glob, math, opencv, pillow, os, sys, time
     classifiers=[\
         'Development Status :: 1 - Planning',\
         'Intended Audience :: Science/Research',\
         'Programming Language :: Python :: 3.11',\
     ],\
```

