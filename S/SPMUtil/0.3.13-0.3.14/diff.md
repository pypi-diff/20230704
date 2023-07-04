# Comparing `tmp/SPMUtil-0.3.13.tar.gz` & `tmp/SPMUtil-0.3.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SPMUtil-0.3.13.tar", last modified: Fri Feb 17 04:51:38 2023, max compression
+gzip compressed data, was "SPMUtil-0.3.14.tar", last modified: Tue Jul  4 05:33:52 2023, max compression
```

## Comparing `SPMUtil-0.3.13.tar` & `SPMUtil-0.3.14.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/
--rw-rw-rw-   0        0        0      388 2022-12-14 07:32:17.000000 SPMUtil-0.3.13/LICENSE.txt
--rw-rw-rw-   0        0        0      184 2022-01-19 07:05:41.000000 SPMUtil-0.3.13/MANIFEST.in
--rw-rw-rw-   0        0        0     1316 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/PKG-INFO
--rw-rw-rw-   0        0        0      997 2022-01-20 07:32:14.000000 SPMUtil-0.3.13/README.MD
--rw-rw-rw-   0        0        0       42 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/setup.cfg
--rw-rw-rw-   0        0        0      723 2023-02-17 04:51:31.000000 SPMUtil-0.3.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/analyzer/
--rw-rw-rw-   0        0        0     1833 2022-01-19 08:17:18.000000 SPMUtil-0.3.13/SPMUtil/analyzer/BaseAnalyzer.py
--rw-rw-rw-   0        0        0     9145 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/analyzer/DulcineaAnalyzer.py
--rw-rw-rw-   0        0        0     5016 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/analyzer/GridAnalyzer.py
--rw-rw-rw-   0        0        0     2040 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/analyzer/SxmAnalyzer.py
--rw-rw-rw-   0        0        0      158 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/analyzer/__init__.py
--rw-rw-rw-   0        0        0     3969 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/converter.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/cython_files/
--rw-rw-rw-   0        0        0   111104 2022-02-07 05:24:14.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_code.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0   434064 2022-02-07 05:24:12.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_pyx_code.c
--rw-rw-rw-   0        0        0     6963 2022-02-07 05:24:07.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_pyx_code.pyx
--rw-rw-rw-   0        0        0      663 2022-01-20 07:16:38.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_setup.py
--rw-rw-rw-   0        0        0   280930 2022-01-22 06:49:13.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_template_matching_code.c
--rw-rw-rw-   0        0        0     1518 2022-01-20 07:00:39.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_template_matching_code.pyx
--rw-rw-rw-   0        0        0    65536 2022-01-22 06:49:16.000000 SPMUtil-0.3.13/SPMUtil/cython_files/cython_tm_code.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0     3503 2022-01-20 07:04:01.000000 SPMUtil-0.3.13/SPMUtil/cython_files/template_matching.c
--rw-rw-rw-   0        0        0      426 2022-01-20 05:50:30.000000 SPMUtil-0.3.13/SPMUtil/cython_files/template_matching.h
--rw-rw-rw-   0        0        0        0 2022-01-20 06:59:45.000000 SPMUtil-0.3.13/SPMUtil/cython_files/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-02-17 04:49:57.000000 SPMUtil-0.3.13/SPMUtil/DataSerializer.py
--rw-rw-rw-   0        0        0     4409 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/DataSerializerPackage.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/filters/
--rw-rw-rw-   0        0        0      738 2022-12-08 06:15:44.000000 SPMUtil-0.3.13/SPMUtil/filters/filter_1d.py
--rw-rw-rw-   0        0        0     5652 2022-10-03 03:23:29.000000 SPMUtil-0.3.13/SPMUtil/filters/filter_2d.py
--rw-rw-rw-   0        0        0     2919 2022-07-27 06:24:39.000000 SPMUtil-0.3.13/SPMUtil/flatten.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/formula/
--rw-rw-rw-   0        0        0     1062 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/formula/_math_formula.py
--rw-rw-rw-   0        0        0     4744 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/formula/_physic_formula.py
--rw-rw-rw-   0        0        0     5420 2022-10-03 03:23:59.000000 SPMUtil-0.3.13/SPMUtil/formula/_spm_common_formula.py
--rw-rw-rw-   0        0        0       96 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/formula/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/gui/
--rw-rw-rw-   0        0        0     6924 2022-07-12 05:09:48.000000 SPMUtil-0.3.13/SPMUtil/gui/JsonEditor.py
--rw-rw-rw-   0        0        0     2294 2022-07-27 06:00:49.000000 SPMUtil-0.3.13/SPMUtil/gui/line_selector.py
--rw-rw-rw-   0        0        0    10550 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/gui/NanonisGridVisualizer.py
--rw-rw-rw-   0        0        0     1560 2022-10-20 07:59:22.000000 SPMUtil-0.3.13/SPMUtil/gui/point_selector.py
--rw-rw-rw-   0        0        0     2009 2022-10-20 07:59:22.000000 SPMUtil-0.3.13/SPMUtil/gui/rect_2d_selector.py
--rw-rw-rw-   0        0        0     5441 2022-07-26 07:11:35.000000 SPMUtil-0.3.13/SPMUtil/gui/tilt_calculator.py
--rw-rw-rw-   0        0        0      333 2022-10-03 03:12:50.000000 SPMUtil-0.3.13/SPMUtil/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil/structures/
--rw-rw-rw-   0        0        0     1042 2022-01-20 10:53:22.000000 SPMUtil-0.3.13/SPMUtil/structures/point.py
--rw-rw-rw-   0        0        0     3057 2022-07-12 04:48:46.000000 SPMUtil-0.3.13/SPMUtil/structures/rect_2d.py
--rw-rw-rw-   0        0        0     5303 2022-10-03 03:14:44.000000 SPMUtil-0.3.13/SPMUtil/structures/scan_data_format.py
--rw-rw-rw-   0        0        0     2179 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/structures/_structures.py
--rw-rw-rw-   0        0        0       57 2021-12-23 07:21:07.000000 SPMUtil-0.3.13/SPMUtil/structures/__init__.py
--rw-rw-rw-   0        0        0      727 2022-10-03 05:44:05.000000 SPMUtil-0.3.13/SPMUtil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil.egg-info/
--rw-rw-rw-   0        0        0        1 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1316 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1490 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-02-17 04:51:38.000000 SPMUtil-0.3.13/SPMUtil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.807753 SPMUtil-0.3.14/
+-rw-rw-rw-   0        0        0      388 2022-12-14 07:32:17.000000 SPMUtil-0.3.14/LICENSE.txt
+-rw-rw-rw-   0        0        0      184 2022-01-19 07:05:41.000000 SPMUtil-0.3.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     1273 2023-07-04 05:33:52.806753 SPMUtil-0.3.14/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2022-01-20 07:32:14.000000 SPMUtil-0.3.14/README.MD
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.706637 SPMUtil-0.3.14/SPMUtil/
+-rw-rw-rw-   0        0        0     4712 2023-02-17 04:49:57.000000 SPMUtil-0.3.14/SPMUtil/DataSerializer.py
+-rw-rw-rw-   0        0        0     4409 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/DataSerializerPackage.py
+-rw-rw-rw-   0        0        0      764 2023-07-04 05:32:48.000000 SPMUtil-0.3.14/SPMUtil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.717636 SPMUtil-0.3.14/SPMUtil/analyzer/
+-rw-rw-rw-   0        0        0     1833 2022-01-19 08:17:18.000000 SPMUtil-0.3.14/SPMUtil/analyzer/BaseAnalyzer.py
+-rw-rw-rw-   0        0        0     9145 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/analyzer/DulcineaAnalyzer.py
+-rw-rw-rw-   0        0        0     5022 2023-07-04 05:32:20.000000 SPMUtil-0.3.14/SPMUtil/analyzer/GridAnalyzer.py
+-rw-rw-rw-   0        0        0     2048 2023-07-04 05:33:13.000000 SPMUtil-0.3.14/SPMUtil/analyzer/SxmAnalyzer.py
+-rw-rw-rw-   0        0        0      158 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     3969 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.763458 SPMUtil-0.3.14/SPMUtil/cython_files/
+-rw-rw-rw-   0        0        0        0 2022-01-20 06:59:45.000000 SPMUtil-0.3.14/SPMUtil/cython_files/__init__.py
+-rw-rw-rw-   0        0        0   111104 2022-02-07 05:24:14.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_code.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0   434064 2022-02-07 05:24:12.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_pyx_code.c
+-rw-rw-rw-   0        0        0     6963 2022-02-07 05:24:07.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_pyx_code.pyx
+-rw-rw-rw-   0        0        0      663 2022-01-20 07:16:38.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_setup.py
+-rw-rw-rw-   0        0        0   280930 2022-01-22 06:49:13.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_template_matching_code.c
+-rw-rw-rw-   0        0        0     1518 2022-01-20 07:00:39.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_template_matching_code.pyx
+-rw-rw-rw-   0        0        0    65536 2022-01-22 06:49:16.000000 SPMUtil-0.3.14/SPMUtil/cython_files/cython_tm_code.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0     3503 2022-01-20 07:04:01.000000 SPMUtil-0.3.14/SPMUtil/cython_files/template_matching.c
+-rw-rw-rw-   0        0        0      426 2022-01-20 05:50:30.000000 SPMUtil-0.3.14/SPMUtil/cython_files/template_matching.h
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.764458 SPMUtil-0.3.14/SPMUtil/filters/
+-rw-rw-rw-   0        0        0      738 2022-12-08 06:15:44.000000 SPMUtil-0.3.14/SPMUtil/filters/filter_1d.py
+-rw-rw-rw-   0        0        0     5652 2022-10-03 03:23:29.000000 SPMUtil-0.3.14/SPMUtil/filters/filter_2d.py
+-rw-rw-rw-   0        0        0     2919 2022-07-27 06:24:39.000000 SPMUtil-0.3.14/SPMUtil/flatten.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.769460 SPMUtil-0.3.14/SPMUtil/formula/
+-rw-rw-rw-   0        0        0       96 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/formula/__init__.py
+-rw-rw-rw-   0        0        0     1062 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/formula/_math_formula.py
+-rw-rw-rw-   0        0        0     4744 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/formula/_physic_formula.py
+-rw-rw-rw-   0        0        0     5420 2023-04-17 07:09:39.000000 SPMUtil-0.3.14/SPMUtil/formula/_spm_common_formula.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.790208 SPMUtil-0.3.14/SPMUtil/gui/
+-rw-rw-rw-   0        0        0     6924 2022-07-12 05:09:48.000000 SPMUtil-0.3.14/SPMUtil/gui/JsonEditor.py
+-rw-rw-rw-   0        0        0    10550 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/gui/NanonisGridVisualizer.py
+-rw-rw-rw-   0        0        0      333 2022-10-03 03:12:50.000000 SPMUtil-0.3.14/SPMUtil/gui/__init__.py
+-rw-rw-rw-   0        0        0     2294 2022-07-27 06:00:49.000000 SPMUtil-0.3.14/SPMUtil/gui/line_selector.py
+-rw-rw-rw-   0        0        0     1560 2022-10-20 07:59:22.000000 SPMUtil-0.3.14/SPMUtil/gui/point_selector.py
+-rw-rw-rw-   0        0        0     2009 2022-10-20 07:59:22.000000 SPMUtil-0.3.14/SPMUtil/gui/rect_2d_selector.py
+-rw-rw-rw-   0        0        0     5441 2022-07-26 07:11:35.000000 SPMUtil-0.3.14/SPMUtil/gui/tilt_calculator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.792177 SPMUtil-0.3.14/SPMUtil/nanonispy/
+-rw-rw-rw-   0        0        0       19 2023-07-04 05:30:02.000000 SPMUtil-0.3.14/SPMUtil/nanonispy/__init__.py
+-rw-rw-rw-   0        0        0      247 2023-07-04 05:30:02.000000 SPMUtil-0.3.14/SPMUtil/nanonispy/constants.py
+-rw-rw-rw-   0        0        0    24582 2023-07-04 05:30:02.000000 SPMUtil-0.3.14/SPMUtil/nanonispy/read.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.806753 SPMUtil-0.3.14/SPMUtil/structures/
+-rw-rw-rw-   0        0        0       57 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/structures/__init__.py
+-rw-rw-rw-   0        0        0     2179 2021-12-23 07:21:07.000000 SPMUtil-0.3.14/SPMUtil/structures/_structures.py
+-rw-rw-rw-   0        0        0     1042 2022-01-20 10:53:22.000000 SPMUtil-0.3.14/SPMUtil/structures/point.py
+-rw-rw-rw-   0        0        0     3294 2023-06-23 05:43:49.000000 SPMUtil-0.3.14/SPMUtil/structures/rect_2d.py
+-rw-rw-rw-   0        0        0     5880 2023-04-10 08:20:26.000000 SPMUtil-0.3.14/SPMUtil/structures/scan_data_format.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:33:52.715636 SPMUtil-0.3.14/SPMUtil.egg-info/
+-rw-rw-rw-   0        0        0     1273 2023-07-04 05:33:52.000000 SPMUtil-0.3.14/SPMUtil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1577 2023-07-04 05:33:52.000000 SPMUtil-0.3.14/SPMUtil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 05:33:52.000000 SPMUtil-0.3.14/SPMUtil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-04 05:33:52.000000 SPMUtil-0.3.14/SPMUtil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 05:33:52.000000 SPMUtil-0.3.14/SPMUtil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 05:33:52.807753 SPMUtil-0.3.14/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-07-04 05:31:49.000000 SPMUtil-0.3.14/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SPMUtil-0.3.13/PKG-INFO` & `SPMUtil-0.3.14/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: SPMUtil
-Version: 0.3.13
+Version: 0.3.14
 Summary: Some Common method for SPM data analysis and realtime data processing.
-Home-page: UNKNOWN
 Author: ZHUO DIAO
 Author-email: enzian0515@gmail.com
 License: LGPL
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 SPMUtil (spmu)
 ===================================
 Some Common method for SPM data analysis and realtime data processing.
 <br>
@@ -55,9 +53,7 @@
 To enable cython script, type this at beginning.
 
 ```python
 import SPMUtil as spmu
 spmu.use_cython = True
 ```
 
-
-
```

### Comparing `SPMUtil-0.3.13/README.MD` & `SPMUtil-0.3.14/README.MD`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/setup.py` & `SPMUtil-0.3.14/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding="utf-8") as f:
     description = f.read()
 
 setuptools.setup(
     name="SPMUtil",
-    version="0.3.13",
+    version="0.3.14",
     description="Some Common method for SPM data analysis and realtime data processing.",
     author="ZHUO DIAO",
     author_email="enzian0515@gmail.com",
     license="LGPL",
     packages=setuptools.find_packages(),
     long_description=description,
     long_description_content_type="text/markdown",
     include_package_data=True,
-    install_requires=["scipy", "matplotlib", "pandas", "nanonispy", "asyncio", "pickle5; python_version < '3.8.3'"]
+    install_requires=["scipy", "matplotlib", "pandas", "asyncio", "pickle5; python_version < '3.8.3'"]
 )
```

### Comparing `SPMUtil-0.3.13/SPMUtil/analyzer/BaseAnalyzer.py` & `SPMUtil-0.3.14/SPMUtil/analyzer/BaseAnalyzer.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/analyzer/DulcineaAnalyzer.py` & `SPMUtil-0.3.14/SPMUtil/analyzer/DulcineaAnalyzer.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/analyzer/GridAnalyzer.py` & `SPMUtil-0.3.14/SPMUtil/analyzer/GridAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import nanonispy as nap
-
+import SPMUtil.nanonispy as nap
 import SPMUtil as spmu
 import SPMUtil.formula as formula
 from SPMUtil.analyzer.BaseAnalyzer import *
 
 
 class GridAnalyzer(BaseAnalyzer):
```

### Comparing `SPMUtil-0.3.13/SPMUtil/analyzer/SxmAnalyzer.py` & `SPMUtil-0.3.14/SPMUtil/analyzer/SxmAnalyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import nanonispy as nap
+import SPMUtil.nanonispy as nap
 
 import SPMUtil as spmu
 from SPMUtil.analyzer.BaseAnalyzer import *
 
 
 class SxmAnalyzer(BaseAnalyzer):
```

### Comparing `SPMUtil-0.3.13/SPMUtil/converter.py` & `SPMUtil-0.3.14/SPMUtil/converter.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/cython_files/cython_pyx_code.c` & `SPMUtil-0.3.14/SPMUtil/cython_files/cython_pyx_code.c`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/cython_files/cython_pyx_code.pyx` & `SPMUtil-0.3.14/SPMUtil/cython_files/cython_pyx_code.pyx`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/cython_files/cython_setup.py` & `SPMUtil-0.3.14/SPMUtil/cython_files/cython_setup.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/cython_files/cython_template_matching_code.c` & `SPMUtil-0.3.14/SPMUtil/cython_files/cython_template_matching_code.c`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/cython_files/cython_template_matching_code.pyx` & `SPMUtil-0.3.14/SPMUtil/cython_files/cython_template_matching_code.pyx`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/cython_files/template_matching.c` & `SPMUtil-0.3.14/SPMUtil/cython_files/template_matching.c`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/DataSerializer.py` & `SPMUtil-0.3.14/SPMUtil/DataSerializer.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/DataSerializerPackage.py` & `SPMUtil-0.3.14/SPMUtil/DataSerializerPackage.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/filters/filter_1d.py` & `SPMUtil-0.3.14/SPMUtil/filters/filter_1d.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/filters/filter_2d.py` & `SPMUtil-0.3.14/SPMUtil/filters/filter_2d.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/flatten.py` & `SPMUtil-0.3.14/SPMUtil/flatten.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/formula/_math_formula.py` & `SPMUtil-0.3.14/SPMUtil/formula/_math_formula.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/formula/_physic_formula.py` & `SPMUtil-0.3.14/SPMUtil/formula/_physic_formula.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/formula/_spm_common_formula.py` & `SPMUtil-0.3.14/SPMUtil/formula/_spm_common_formula.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             array_x[i], array_y[i], _ = np.matmul(rot_matrix, [array_x[i], array_y[i], 1])
         return array_x, array_y
 
 
 def line_proline(map, xy_point_from, xy_point_to):
     length = int(np.hypot(xy_point_to[0] - xy_point_from[0], xy_point_to[1] - xy_point_from[1]))
     x, y = np.linspace(xy_point_from[0], xy_point_to[0], length), np.linspace(xy_point_from[1], xy_point_to[1], length)
-    return map[x.astype(np.int), y.astype(np.int)]
+    return map[y.astype(np.int), x.astype(np.int)]
 
 
 def topo_map_correction(topo_map: np.ndarray, threshold=3):
     mean, std = np.mean(topo_map), np.std(topo_map)
     size = topo_map.shape
     threshold = threshold * std
     topo_map[abs(topo_map - mean) > threshold] = np.nan
```

### Comparing `SPMUtil-0.3.13/SPMUtil/gui/JsonEditor.py` & `SPMUtil-0.3.14/SPMUtil/gui/JsonEditor.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/gui/line_selector.py` & `SPMUtil-0.3.14/SPMUtil/gui/line_selector.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/gui/NanonisGridVisualizer.py` & `SPMUtil-0.3.14/SPMUtil/gui/NanonisGridVisualizer.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/gui/point_selector.py` & `SPMUtil-0.3.14/SPMUtil/gui/point_selector.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/gui/rect_2d_selector.py` & `SPMUtil-0.3.14/SPMUtil/gui/rect_2d_selector.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/gui/tilt_calculator.py` & `SPMUtil-0.3.14/SPMUtil/gui/tilt_calculator.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/structures/point.py` & `SPMUtil-0.3.14/SPMUtil/structures/point.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/structures/rect_2d.py` & `SPMUtil-0.3.14/SPMUtil/structures/rect_2d.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,27 +55,33 @@
         self.points = int(center[0] - self.xbox / 2), int(center[1] - self.ybox / 2)
 
 
     @property
     def center(self):
         return (int(self.points[0] + self.xbox/2), int(self.points[1] + self.ybox/2))
 
+    def hitTestRect(self, pt):
+        px, py = pt
+        return self.points[0] <= px <= self.points[0] + self.xbox \
+            and self.points[1] + self.ybox >= py >= self.points[1]
+
     def extract_2d_map_from_rect(self, map: np.ndarray):
         x_point, y_point = self.points[0], self.points[1]
         return map[y_point:y_point+self.ybox, x_point:x_point+self.xbox]
 
-    def draw_rect_patch_on_matplot(self, ax, c="r"):
-        _rect = Rectangle(self.points, self.xbox, self.ybox, linewidth=1, edgecolor=c, facecolor="none")
+    def draw_rect_patch_on_matplot(self, ax, c="r", linewidth=1, linestyle="-"):
+        _rect = Rectangle(self.points, self.xbox, self.ybox, lw=linewidth, edgecolor=c, facecolor="none", ls=linestyle)
         ax.add_patch(_rect)
 
     @staticmethod
     def get_random_rect(data: np.ndarray, x_box_min, x_box_max, y_box_min, y_box_max, fixed_center=None):
         if len(data.shape) != 2:
             raise ValueError("Wrong Data Shape")
         size = (np.random.uniform(low=x_box_min, high=x_box_max, size=1),
                 np.random.uniform(low=y_box_min, high=y_box_max, size=1))
         if fixed_center is None:
             points = np.random.uniform(low=0, high=data.shape[0]-size[0]), np.random.uniform(low=0, high=data.shape[1]-size[1])
         else:
             points = fixed_center[0] - size[0]/2, fixed_center[1] - size[1]/2
 
         return Rect2D(points, size[0], size[1])
+
```

### Comparing `SPMUtil-0.3.13/SPMUtil/structures/scan_data_format.py` & `SPMUtil-0.3.14/SPMUtil/structures/scan_data_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from SPMUtil import NdarrayEncoder, NdarrayDecoder, DataSerializer
 import json
 from enum import Enum
 from datetime import datetime as dt
+from copy import deepcopy
+from typing import TypeVar
+Cls = TypeVar('Cls')
 
 
 class cache_1d_scope(Enum):
     Output_FW_ZLine = 1
     Output_BW_ZLine = 2
     Output_FW_CurrentLine = 3
     Output_BW_CurrentLine = 4
@@ -53,14 +56,26 @@
     def GetKeyName() -> str:
         raise NotImplementedError
 
     @staticmethod
     def from_dataSerilizer(dataSerilizer: DataSerializer):
         raise NotImplementedError
 
+    @staticmethod
+    def copy_class(cls: Cls) -> Cls:
+        copy_cls = type(f'{cls.__name__}Copy', cls.__bases__, dict(cls.__dict__))
+        for name, attr in cls.__dict__.items():
+            try:
+                hash(attr)
+            except TypeError:
+                # Assume lack of __hash__ implies mutability. This is NOT
+                # a bullet proof assumption but good in many cases.
+                setattr(copy_cls, name, deepcopy(attr))
+        return copy_cls
+
 
 class StageConfigure(JsonStringClass):
 
     def __init__(self):
         super().__init__()
         self.Sample_Bias = 2
         self.Tube_Scanner_Offset_X = 0
@@ -141,14 +156,17 @@
     @staticmethod
     def from_dataSerilizer(dataSerilizer: DataSerializer):
         data = PythonScanParam()
         data.from_json(dataSerilizer.data_dict[data.GetKeyName()])
         return data
 
 
+
+
+
 class ScanDataHeader(JsonStringClass):
     def __init__(self):
         super().__init__()
         self.Date = ""
         self.Time_Start_Scan = ""
         self.Time_End_Scan = ""
         self.Scan_Method = ""
```

### Comparing `SPMUtil-0.3.13/SPMUtil/structures/_structures.py` & `SPMUtil-0.3.14/SPMUtil/structures/_structures.py`

 * *Files identical despite different names*

### Comparing `SPMUtil-0.3.13/SPMUtil/__init__.py` & `SPMUtil-0.3.14/SPMUtil/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import SPMUtil.structures._structures as structures
-
+import SPMUtil.nanonispy as nanonispy
 import SPMUtil.converter as converter
 
 from SPMUtil.DataSerializer import DataSerializer, NdarrayDecoder, NdarrayEncoder
 from SPMUtil.DataSerializerPackage import DataSerializerPackage
 from SPMUtil.structures.rect_2d import Rect2D
 from SPMUtil.structures.scan_data_format import cache_1d_scope, cache_2d_scope, ScanDataHeader, StageConfigure, PythonScanParam
```

### Comparing `SPMUtil-0.3.13/SPMUtil.egg-info/PKG-INFO` & `SPMUtil-0.3.14/SPMUtil.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: SPMUtil
-Version: 0.3.13
+Version: 0.3.14
 Summary: Some Common method for SPM data analysis and realtime data processing.
-Home-page: UNKNOWN
 Author: ZHUO DIAO
 Author-email: enzian0515@gmail.com
 License: LGPL
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 SPMUtil (spmu)
 ===================================
 Some Common method for SPM data analysis and realtime data processing.
 <br>
@@ -55,9 +53,7 @@
 To enable cython script, type this at beginning.
 
 ```python
 import SPMUtil as spmu
 spmu.use_cython = True
 ```
 
-
-
```

### Comparing `SPMUtil-0.3.13/SPMUtil.egg-info/SOURCES.txt` & `SPMUtil-0.3.14/SPMUtil.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,12 +36,15 @@
 SPMUtil/gui/JsonEditor.py
 SPMUtil/gui/NanonisGridVisualizer.py
 SPMUtil/gui/__init__.py
 SPMUtil/gui/line_selector.py
 SPMUtil/gui/point_selector.py
 SPMUtil/gui/rect_2d_selector.py
 SPMUtil/gui/tilt_calculator.py
+SPMUtil/nanonispy/__init__.py
+SPMUtil/nanonispy/constants.py
+SPMUtil/nanonispy/read.py
 SPMUtil/structures/__init__.py
 SPMUtil/structures/_structures.py
 SPMUtil/structures/point.py
 SPMUtil/structures/rect_2d.py
 SPMUtil/structures/scan_data_format.py
```

