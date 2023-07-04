# Comparing `tmp/grassmanntn-1.1.0.tar.gz` & `tmp/grassmanntn-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.0.tar", last modified: Tue Jul  4 06:40:09 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.1.tar", last modified: Tue Jul  4 06:44:09 2023, max compression
```

## Comparing `grassmanntn-1.1.0.tar` & `grassmanntn-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:40:09.124754 grassmanntn-1.1.0/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.0/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-04 06:40:09.124754 grassmanntn-1.1.0/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.0/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:40:09.124754 grassmanntn-1.1.0/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109377 2023-07-04 06:29:26.000000 grassmanntn-1.1.0/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132612 2023-06-26 03:15:27.000000 grassmanntn-1.1.0/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.0/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:40:09.124754 grassmanntn-1.1.0/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-04 06:40:09.000000 grassmanntn-1.1.0/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      282 2023-07-04 06:40:09.000000 grassmanntn-1.1.0/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-04 06:40:09.000000 grassmanntn-1.1.0/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-04 06:40:09.000000 grassmanntn-1.1.0/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-04 06:40:09.000000 grassmanntn-1.1.0/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-04 06:40:09.124754 grassmanntn-1.1.0/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-04 06:30:53.000000 grassmanntn-1.1.0/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:44:09.121746 grassmanntn-1.1.1/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.1/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-04 06:44:09.121746 grassmanntn-1.1.1/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.1/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:44:09.121746 grassmanntn-1.1.1/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109338 2023-07-04 06:41:05.000000 grassmanntn-1.1.1/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132591 2023-07-04 06:41:43.000000 grassmanntn-1.1.1/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.1/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:44:09.121746 grassmanntn-1.1.1/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-04 06:44:09.000000 grassmanntn-1.1.1/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      282 2023-07-04 06:44:09.000000 grassmanntn-1.1.1/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-04 06:44:09.000000 grassmanntn-1.1.1/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-04 06:44:09.000000 grassmanntn-1.1.1/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-04 06:44:09.000000 grassmanntn-1.1.1/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-04 06:44:09.121746 grassmanntn-1.1.1/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-04 06:42:19.000000 grassmanntn-1.1.1/setup.py
```

### Comparing `grassmanntn-1.1.0/LICENSE.txt` & `grassmanntn-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.0/PKG-INFO` & `grassmanntn-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.0
+Version: 1.1.1
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_110.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_111.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.0/README.md` & `grassmanntn-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.0/grassmanntn/__init__.py` & `grassmanntn-1.1.1/grassmanntn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from grassmanntn.grassmanntn import *
 from grassmanntn.param import *
 from grassmanntn.gauge2d import *
 
 import numpy as np
 import math
 from grassmanntn import param
 import sparse as sp
```

### Comparing `grassmanntn-1.1.0/grassmanntn/gauge2d.py` & `grassmanntn-1.1.1/grassmanntn/gauge2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import math
-from grassmanntn import grassmanntn as gtn
-from grassmanntn import param
+import grassmanntn as gtn
+import gtn.param as param
 import sparse as sp
 import opt_einsum as oe
 import time
 import sys
 import gc
 import tracemalloc
 import os
```

### Comparing `grassmanntn-1.1.0/grassmanntn/param.py` & `grassmanntn-1.1.1/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.0/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.1/grassmanntn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.0
+Version: 1.1.1
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_110.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_111.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.0/setup.py` & `grassmanntn-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.0',      # Start with a small number and increase it with every change you make
+  version = '1.1.1',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_110.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_111.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

