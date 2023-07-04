# Comparing `tmp/cjm-psl-utils-0.0.2.tar.gz` & `tmp/cjm-psl-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-psl-utils-0.0.2.tar", last modified: Wed Feb  8 19:16:52 2023, max compression
+gzip compressed data, was "cjm-psl-utils-0.0.4.tar", last modified: Tue Jul  4 21:27:56 2023, max compression
```

## Comparing `cjm-psl-utils-0.0.2.tar` & `cjm-psl-utils-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-02-08 19:16:52.900790 cjm-psl-utils-0.0.2/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-02-08 02:20:00.000000 cjm-psl-utils-0.0.2/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-01-20 02:50:04.000000 cjm-psl-utils-0.0.2/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3105 2023-02-08 19:16:52.900616 cjm-psl-utils-0.0.2/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2298 2023-02-08 19:16:43.000000 cjm-psl-utils-0.0.2/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-02-08 19:16:52.898136 cjm-psl-utils-0.0.2/cjm_psl_utils/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-02-08 19:16:42.000000 cjm-psl-utils-0.0.2/cjm_psl_utils/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      545 2023-02-08 19:16:42.000000 cjm-psl-utils-0.0.2/cjm_psl_utils/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2773 2023-02-08 19:16:42.000000 cjm-psl-utils-0.0.2/cjm_psl_utils/core.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-02-08 19:16:52.900280 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3105 2023-02-08 19:16:52.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      384 2023-02-08 19:16:52.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-02-08 19:16:52.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       48 2023-02-08 19:16:52.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-02-08 03:09:09.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        7 2023-02-08 19:16:52.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       14 2023-02-08 19:16:52.000000 cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      963 2023-02-08 19:16:33.000000 cjm-psl-utils-0.0.2/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-02-08 19:16:52.900844 cjm-psl-utils-0.0.2/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2560 2023-01-20 02:50:04.000000 cjm-psl-utils-0.0.2/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-04 21:27:56.026051 cjm-psl-utils-0.0.4/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-02-08 02:20:00.000000 cjm-psl-utils-0.0.4/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-01-20 02:50:04.000000 cjm-psl-utils-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3008 2023-07-04 21:27:56.025887 cjm-psl-utils-0.0.4/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2301 2023-07-04 21:13:06.000000 cjm-psl-utils-0.0.4/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-04 21:27:56.023316 cjm-psl-utils-0.0.4/cjm_psl_utils/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-04 21:23:28.000000 cjm-psl-utils-0.0.4/cjm_psl_utils/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      671 2023-07-04 21:23:28.000000 cjm-psl-utils-0.0.4/cjm_psl_utils/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     5046 2023-07-04 21:23:28.000000 cjm-psl-utils-0.0.4/cjm_psl_utils/core.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-04 21:27:56.025560 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3008 2023-07-04 21:27:55.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      384 2023-07-04 21:27:55.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-04 21:27:55.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       48 2023-07-04 21:27:55.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-02-08 03:09:09.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       12 2023-07-04 21:27:55.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       14 2023-07-04 21:27:55.000000 cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      950 2023-07-04 21:23:09.000000 cjm-psl-utils-0.0.4/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-04 21:27:56.026100 cjm-psl-utils-0.0.4/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2560 2023-01-20 02:50:04.000000 cjm-psl-utils-0.0.4/setup.py
```

### Comparing `cjm-psl-utils-0.0.2/LICENSE` & `cjm-psl-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-psl-utils-0.0.2/PKG-INFO` & `cjm-psl-utils-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: cjm-psl-utils
-Version: 0.0.2
+Version: 0.0.4
 Summary: Some utility functions using the Python Standard Library.
 Home-page: https://github.com/cj-mills/cjm-psl-utils
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-cjm-psl-utils
-================
+# cjm-psl-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
@@ -85,14 +82,16 @@
         except NameError:
             # If not in Jupyter Notebook, do nothing
             pass
     # Return the formatted source code
     return source
 ```
 
+### file_extract
+
 ``` python
 from cjm_psl_utils.core import file_extract
 from pathlib import Path
 ```
 
 ``` python
 fname = "../images/images.zip"
```

### Comparing `cjm-psl-utils-0.0.2/README.md` & `cjm-psl-utils-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-cjm-psl-utils
-================
+# cjm-psl-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
@@ -63,14 +62,16 @@
         except NameError:
             # If not in Jupyter Notebook, do nothing
             pass
     # Return the formatted source code
     return source
 ```
 
+### file_extract
+
 ``` python
 from cjm_psl_utils.core import file_extract
 from pathlib import Path
 ```
 
 ``` python
 fname = "../images/images.zip"
```

### Comparing `cjm-psl-utils-0.0.2/cjm_psl_utils.egg-info/PKG-INFO` & `cjm-psl-utils-0.0.4/cjm_psl_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: cjm-psl-utils
-Version: 0.0.2
+Version: 0.0.4
 Summary: Some utility functions using the Python Standard Library.
 Home-page: https://github.com/cj-mills/cjm-psl-utils
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-cjm-psl-utils
-================
+# cjm-psl-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
@@ -85,14 +82,16 @@
         except NameError:
             # If not in Jupyter Notebook, do nothing
             pass
     # Return the formatted source code
     return source
 ```
 
+### file_extract
+
 ``` python
 from cjm_psl_utils.core import file_extract
 from pathlib import Path
 ```
 
 ``` python
 fname = "../images/images.zip"
```

### Comparing `cjm-psl-utils-0.0.2/settings.ini` & `cjm-psl-utils-0.0.4/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-psl-utils
 lib_name = %(repo)s
-version = 0.0.2
-min_python = 3.7
+version = 0.0.4
+min_python = 3.9
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_psl_utils
 nbs_path = nbs
 recursive = True
@@ -33,10 +33,10 @@
 description = Some utility functions using the Python Standard Library.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = cj-mills
 
 ### Optional ###
-# requirements = fastcore pandas
+requirements = tqdm
 # dev_requirements = 
 # console_scripts =
```

### Comparing `cjm-psl-utils-0.0.2/setup.py` & `cjm-psl-utils-0.0.4/setup.py`

 * *Files identical despite different names*

