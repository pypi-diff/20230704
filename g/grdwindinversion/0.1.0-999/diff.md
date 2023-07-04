# Comparing `tmp/grdwindinversion-0.1.0.tar.gz` & `tmp/grdwindinversion-999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grdwindinversion-0.1.0.tar", last modified: Fri Jun 30 14:11:12 2023, max compression
+gzip compressed data, was "grdwindinversion-999.tar", last modified: Tue Jul  4 08:52:28 2023, max compression
```

## Comparing `grdwindinversion-0.1.0.tar` & `grdwindinversion-999.tar`

### file list

```diff
@@ -1,63 +1,39 @@
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      292 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/.editorconfig
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1772 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/.gitignore
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      218 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/AUTHORS.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     3632 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       89 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/HISTORY.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1075 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/LICENSE
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      262 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/MANIFEST.in
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2331 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/Makefile
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1830 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      984 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/README.rst
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/docs/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      657 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/Makefile
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.578970 grdwindinversion-0.1.0/docs/_build/
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.578970 grdwindinversion-0.1.0/docs/_build/html/
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/docs/_build/html/_static/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      286 2023-05-26 12:27:18.000000 grdwindinversion-0.1.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       90 2023-05-26 12:27:18.000000 grdwindinversion-0.1.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       90 2023-05-26 12:27:18.000000 grdwindinversion-0.1.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       50 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/algorithm.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       28 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/docs/authors.rst
--rwxrwxr-x   0 antoine   (1000) antoine   (1000)     5704 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/conf.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       33 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/docs/contributing.rst
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/docs/examples/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     4190 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/examples/wind-inversion-from-grd.ipynb
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       28 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/docs/history.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      722 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/index.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1186 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/docs/installation.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      814 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/docs/make.bat
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      504 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/modules.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       27 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/docs/readme.rst
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      352 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/docs/usage.rst
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/grdwindinversion/
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/grdwindinversion/.github/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      327 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1204 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/.gitignore
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      694 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/.travis.yml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      205 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/grdwindinversion/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       86 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/config_RCM.yaml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       88 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/config_RS2.yaml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      173 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/config_S1.yaml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      344 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/config_hy2b.yaml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      349 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/config_prod.yaml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     3240 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/grdwindinversion/degrade.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    20626 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/grdwindinversion/inversion.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      692 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/grdwindinversion/load_config.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      702 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/main.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     5364 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/grdwindinversion/main_plot.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/grdwindinversion.egg-info/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1830 2023-06-30 14:11:12.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1271 2023-06-30 14:11:12.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-06-30 14:11:12.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       63 2023-06-30 14:11:12.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/entry_points.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-06-29 13:33:50.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/not-zip-safe
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       39 2023-06-30 14:11:12.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       17 2023-06-30 14:11:12.000000 grdwindinversion-0.1.0/grdwindinversion.egg-info/top_level.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      136 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/requirements_dev.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      388 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/setup.cfg
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1545 2023-06-30 14:08:37.000000 grdwindinversion-0.1.0/setup.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-30 14:11:12.582970 grdwindinversion-0.1.0/tests/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       46 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/tests/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      432 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/tests/test_grdwindinversion.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      277 2023-06-29 13:14:41.000000 grdwindinversion-0.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:52:28.002055 grdwindinversion-999/
+-rw-rw-r--   0 root         (0) root         (0)      218 2023-07-04 08:50:02.000000 grdwindinversion-999/AUTHORS.rst
+-rw-rw-r--   0 root         (0) root         (0)     3632 2023-07-04 08:50:02.000000 grdwindinversion-999/CONTRIBUTING.rst
+-rw-rw-r--   0 root         (0) root         (0)       89 2023-07-04 08:50:02.000000 grdwindinversion-999/HISTORY.rst
+-rw-rw-r--   0 root         (0) root         (0)     1075 2023-07-04 08:50:02.000000 grdwindinversion-999/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      262 2023-07-04 08:50:02.000000 grdwindinversion-999/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-07-04 08:52:28.002055 grdwindinversion-999/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      984 2023-07-04 08:50:02.000000 grdwindinversion-999/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:52:27.998055 grdwindinversion-999/docs/
+-rw-rw-r--   0 root         (0) root         (0)      657 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/Makefile
+-rw-rw-r--   0 root         (0) root         (0)       50 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/algorithm.rst
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/authors.rst
+-rwxrwxr-x   0 root         (0) root         (0)     5704 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/conf.py
+-rw-rw-r--   0 root         (0) root         (0)       33 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/contributing.rst
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/history.rst
+-rw-rw-r--   0 root         (0) root         (0)      722 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/index.rst
+-rw-rw-r--   0 root         (0) root         (0)     1186 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/installation.rst
+-rw-rw-r--   0 root         (0) root         (0)      814 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/make.bat
+-rw-rw-r--   0 root         (0) root         (0)      504 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/modules.rst
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/readme.rst
+-rw-rw-r--   0 root         (0) root         (0)      352 2023-07-04 08:50:02.000000 grdwindinversion-999/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:52:28.002055 grdwindinversion-999/grdwindinversion/
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-07-04 08:50:02.000000 grdwindinversion-999/grdwindinversion/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-04 08:50:02.000000 grdwindinversion-999/grdwindinversion/degrade.py
+-rw-rw-r--   0 root         (0) root         (0)    20626 2023-07-04 08:50:02.000000 grdwindinversion-999/grdwindinversion/inversion.py
+-rw-rw-r--   0 root         (0) root         (0)      692 2023-07-04 08:50:02.000000 grdwindinversion-999/grdwindinversion/load_config.py
+-rw-rw-r--   0 root         (0) root         (0)      702 2023-07-04 08:50:02.000000 grdwindinversion-999/grdwindinversion/main.py
+-rw-rw-r--   0 root         (0) root         (0)     5364 2023-07-04 08:50:02.000000 grdwindinversion-999/grdwindinversion/main_plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:52:28.002055 grdwindinversion-999/grdwindinversion.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-07-04 08:52:27.000000 grdwindinversion-999/grdwindinversion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-04 08:52:27.000000 grdwindinversion-999/grdwindinversion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 08:52:27.000000 grdwindinversion-999/grdwindinversion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-04 08:52:27.000000 grdwindinversion-999/grdwindinversion.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 08:52:27.000000 grdwindinversion-999/grdwindinversion.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1530 2023-07-04 08:50:02.000000 grdwindinversion-999/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 08:52:28.002055 grdwindinversion-999/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:52:28.002055 grdwindinversion-999/tests/
+-rw-rw-r--   0 root         (0) root         (0)       46 2023-07-04 08:50:02.000000 grdwindinversion-999/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      432 2023-07-04 08:50:02.000000 grdwindinversion-999/tests/test_grdwindinversion.py
```

### Comparing `grdwindinversion-0.1.0/CONTRIBUTING.rst` & `grdwindinversion-999/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/LICENSE` & `grdwindinversion-999/LICENSE`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/PKG-INFO` & `grdwindinversion-999/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grdwindinversion
-Version: 0.1.0
+Version: 999
 Summary: Package to perform Wind inversion from GRD Level-1 SAR images
-Home-page: https://github.com/agrouaze/grdwindinversion
-Author: Antoine Grouazel
-Author-email: antoine.grouazel@ifremer.fr
-License: MIT license
-Keywords: grdwindinversion
+License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ================
 grdwindinversion
 ================
 
@@ -53,17 +53,7 @@
 Credits
 -------
 
 This package was created with Cookiecutter_.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 
-
-
-=======
-History
-=======
-
-0.1.0 (2023-06-26)
-------------------
-
-* First release on PyPI.
```

### Comparing `grdwindinversion-0.1.0/README.rst` & `grdwindinversion-999/README.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/docs/Makefile` & `grdwindinversion-999/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/docs/conf.py` & `grdwindinversion-999/docs/conf.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/docs/index.rst` & `grdwindinversion-999/docs/index.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/docs/installation.rst` & `grdwindinversion-999/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/docs/make.bat` & `grdwindinversion-999/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/grdwindinversion/degrade.py` & `grdwindinversion-999/grdwindinversion/degrade.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/grdwindinversion/inversion.py` & `grdwindinversion-999/grdwindinversion/inversion.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/grdwindinversion/load_config.py` & `grdwindinversion-999/grdwindinversion/load_config.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/grdwindinversion/main.py` & `grdwindinversion-999/grdwindinversion/main.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/grdwindinversion/main_plot.py` & `grdwindinversion-999/grdwindinversion/main_plot.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.1.0/grdwindinversion.egg-info/PKG-INFO` & `grdwindinversion-999/grdwindinversion.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grdwindinversion
-Version: 0.1.0
+Version: 999
 Summary: Package to perform Wind inversion from GRD Level-1 SAR images
-Home-page: https://github.com/agrouaze/grdwindinversion
-Author: Antoine Grouazel
-Author-email: antoine.grouazel@ifremer.fr
-License: MIT license
-Keywords: grdwindinversion
+License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ================
 grdwindinversion
 ================
 
@@ -53,17 +53,7 @@
 Credits
 -------
 
 This package was created with Cookiecutter_.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 
-
-
-=======
-History
-=======
-
-0.1.0 (2023-06-26)
-------------------
-
-* First release on PyPI.
```

### Comparing `grdwindinversion-0.1.0/grdwindinversion.egg-info/SOURCES.txt` & `grdwindinversion-999/grdwindinversion.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,32 @@
-.editorconfig
-.gitignore
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
-requirements_dev.txt
-setup.cfg
-setup.py
-tox.ini
+pyproject.toml
 docs/Makefile
 docs/algorithm.rst
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
-docs/examples/wind-inversion-from-grd.ipynb
-grdwindinversion/.gitignore
-grdwindinversion/.travis.yml
 grdwindinversion/__init__.py
-grdwindinversion/config_RCM.yaml
-grdwindinversion/config_RS2.yaml
-grdwindinversion/config_S1.yaml
-grdwindinversion/config_hy2b.yaml
-grdwindinversion/config_prod.yaml
 grdwindinversion/degrade.py
 grdwindinversion/inversion.py
 grdwindinversion/load_config.py
 grdwindinversion/main.py
 grdwindinversion/main_plot.py
 grdwindinversion.egg-info/PKG-INFO
 grdwindinversion.egg-info/SOURCES.txt
 grdwindinversion.egg-info/dependency_links.txt
-grdwindinversion.egg-info/entry_points.txt
-grdwindinversion.egg-info/not-zip-safe
 grdwindinversion.egg-info/requires.txt
 grdwindinversion.egg-info/top_level.txt
-grdwindinversion/.github/ISSUE_TEMPLATE.md
 tests/__init__.py
 tests/test_grdwindinversion.py
```

### Comparing `grdwindinversion-0.1.0/setup.py` & `grdwindinversion-999/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-#!/usr/bin/env python
+[project]
+name = "grdwindinversion"
+description="Package to perform Wind inversion from GRD Level-1 SAR images"
+readme = "README.rst"
+#long_description='Python library using xarray objects to compute wind speed from SAR observations over ocean'
+#long_description_content_type='text/x-rst'
+#url='https://github.com/agrouaze/grdwindinversion'
+requires-python = ">= 3.9"
+license = {text = "MIT"}
+#author="Antoine Grouazel"
+#author_email='antoine.grouazel@ifremer.fr'
+dependencies = [
+    "xsar",
+    "xsarsea",
+    "xarray",
+    "xarray-datatree",
+    "pyyaml",
+    "numpy",
+    "scipy",
+    "fsspec",
+    "aiohttp",
+]
 
-"""The setup script."""
-
-from setuptools import setup, find_packages
-
-with open('README.rst') as readme_file:
-    readme = readme_file.read()
-
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
-
-requirements = [
-    'xsarsea',
-    'xsar',
-    'pyyaml',
-    'numpy',
-    'xarray',
-    'scipy'
-                ]
-
-test_requirements = [ ]
-
-setup(
-    author="Antoine Grouazel",
-    author_email='antoine.grouazel@ifremer.fr',
-    python_requires='>=3.6',
-    classifiers=[
+dynamic = ["version"]
+classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-    ],
-    description="Package to perform Wind inversion from GRD Level-1 SAR images",
-    entry_points={
-        'console_scripts': [
-            'grdwindinversion=grdwindinversion.cli:main',
-        ],
-    },
-    install_requires=requirements,
-    license="MIT license",
-    long_description=readme + '\n\n' + history,
-    include_package_data=True,
-    keywords='grdwindinversion',
-    name='grdwindinversion',
-    packages=find_packages(include=['grdwindinversion', 'grdwindinversion.*']),
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/agrouaze/grdwindinversion',
-    version='0.1.0',
-    zip_safe=False,
-)
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ]
+
+[build-system]
+requires = ["setuptools>=64.0", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["grdwindinversion"]
+
+[tool.setuptools_scm]
+fallback_version = "999"
+
+[tool.isort]
+profile = "black"
+skip_gitignore = true
+float_to_top = true
+default_section = "THIRDPARTY"
+known_first_party = "grdwindinversion"
```

