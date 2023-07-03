# Comparing `tmp/stegoveritas-1.8.tar.gz` & `tmp/stegoveritas-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stegoveritas-1.8.tar", last modified: Mon Jul  6 15:56:26 2020, max compression
+gzip compressed data, was "stegoveritas-1.9.tar", last modified: Mon Jul 19 21:35:19 2021, max compression
```

## Comparing `stegoveritas-1.8.tar` & `stegoveritas-1.9.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/
--rw-rw-r--   0 user      (1000) user      (1000)      624 2020-07-06 15:56:26.000000 stegoveritas-1.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       38 2020-07-06 15:56:26.000000 stegoveritas-1.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2231 2020-01-03 03:28:04.000000 stegoveritas-1.8/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      624 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       13 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      275 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1211 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)      175 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3163 2020-04-06 21:45:23.000000 stegoveritas-1.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas/
--rwxrwxr-x   0 user      (1000) user      (1000)    11975 2020-06-29 21:26:42.000000 stegoveritas-1.8/stegoveritas/stegoveritas.py
--rwxrwxr-x   0 user      (1000) user      (1000)     3655 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/hide_lsb.py
--rw-rw-r--   0 user      (1000) user      (1000)       90 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3831 2020-04-07 20:05:40.000000 stegoveritas-1.8/stegoveritas/Colorer.py
--rw-rw-r--   0 user      (1000) user      (1000)       16 2020-07-06 15:54:51.000000 stegoveritas-1.8/stegoveritas/version.py
--rw-rw-r--   0 user      (1000) user      (1000)      990 2020-04-07 20:47:44.000000 stegoveritas-1.8/stegoveritas/helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     1770 2020-04-10 18:09:16.000000 stegoveritas-1.8/stegoveritas/install_deps.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas/modules/
--rw-rw-r--   0 user      (1000) user      (1000)     2104 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas/modules/image/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/
--rw-rw-r--   0 user      (1000) user      (1000)     7903 2020-04-07 22:04:58.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/filters.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1092 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/extractLSB.py
--rw-rw-r--   0 user      (1000) user      (1000)     5496 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/extract_frames.py
--rw-rw-r--   0 user      (1000) user      (1000)     2925 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/meta.py
--rw-rw-r--   0 user      (1000) user      (1000)     2853 2020-04-07 20:39:16.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/brute_lsb.py
--rw-rw-r--   0 user      (1000) user      (1000)     6679 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/trailing.py
--rw-rw-r--   0 user      (1000) user      (1000)     1998 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/colormap.py
--rw-rw-r--   0 user      (1000) user      (1000)     1459 2020-01-03 05:03:10.000000 stegoveritas-1.8/stegoveritas/modules/image/analysis/steghide.py
--rw-rw-r--   0 user      (1000) user      (1000)   155813 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/png.py
--rw-rw-r--   0 user      (1000) user      (1000)     6399 2020-04-07 20:26:46.000000 stegoveritas-1.8/stegoveritas/modules/image/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     8891 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/image/gif.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas/modules/multi/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-07-06 15:56:26.000000 stegoveritas-1.8/stegoveritas/modules/multi/analysis/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/multi/analysis/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1500 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/multi/analysis/xmp.py
--rw-rw-r--   0 user      (1000) user      (1000)      640 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/multi/analysis/carve.py
--rw-rw-r--   0 user      (1000) user      (1000)     1734 2020-04-07 17:57:45.000000 stegoveritas-1.8/stegoveritas/modules/multi/analysis/exif.py
--rw-rw-r--   0 user      (1000) user      (1000)      818 2020-01-03 03:28:04.000000 stegoveritas-1.8/stegoveritas/modules/multi/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.693068 stegoveritas-1.9/
+-rw-rw-r--   0 user      (1000) user      (1000)      624 2021-07-19 21:35:19.693068 stegoveritas-1.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3594 2021-07-19 21:26:38.000000 stegoveritas-1.9/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2021-07-19 21:35:19.693068 stegoveritas-1.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2244 2021-07-19 21:26:38.000000 stegoveritas-1.9/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.689068 stegoveritas-1.9/stegoveritas/
+-rw-rw-r--   0 user      (1000) user      (1000)     3831 2021-07-19 18:08:05.000000 stegoveritas-1.9/stegoveritas/Colorer.py
+-rw-rw-r--   0 user      (1000) user      (1000)       90 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      990 2021-07-19 18:08:05.000000 stegoveritas-1.9/stegoveritas/helpers.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     3655 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/hide_lsb.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.689068 stegoveritas-1.9/stegoveritas/modules/
+-rw-rw-r--   0 user      (1000) user      (1000)     2104 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.689068 stegoveritas-1.9/stegoveritas/modules/image/
+-rw-rw-r--   0 user      (1000) user      (1000)     6399 2021-07-19 18:08:05.000000 stegoveritas-1.9/stegoveritas/modules/image/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.693068 stegoveritas-1.9/stegoveritas/modules/image/analysis/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2915 2021-07-19 18:08:05.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/brute_lsb.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1998 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/colormap.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1092 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/extractLSB.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5496 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/extract_frames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7903 2021-07-19 18:08:05.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/filters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2925 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/meta.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1459 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/steghide.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6679 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/analysis/trailing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8891 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/gif.py
+-rw-rw-r--   0 user      (1000) user      (1000)   155813 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/image/png.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.693068 stegoveritas-1.9/stegoveritas/modules/multi/
+-rw-rw-r--   0 user      (1000) user      (1000)      818 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/multi/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.693068 stegoveritas-1.9/stegoveritas/modules/multi/analysis/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/multi/analysis/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      640 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/multi/analysis/carve.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1734 2021-07-19 18:08:05.000000 stegoveritas-1.9/stegoveritas/modules/multi/analysis/exif.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1500 2021-04-17 02:41:30.000000 stegoveritas-1.9/stegoveritas/modules/multi/analysis/xmp.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    12009 2021-07-19 21:26:38.000000 stegoveritas-1.9/stegoveritas/stegoveritas.py
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2021-07-19 21:33:29.000000 stegoveritas-1.9/stegoveritas/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.689068 stegoveritas-1.9/stegoveritas.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      624 2021-07-19 21:35:19.000000 stegoveritas-1.9/stegoveritas.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1299 2021-07-19 21:35:19.000000 stegoveritas-1.9/stegoveritas.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2021-07-19 21:35:19.000000 stegoveritas-1.9/stegoveritas.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      188 2021-07-19 21:35:19.000000 stegoveritas-1.9/stegoveritas.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      275 2021-07-19 21:35:19.000000 stegoveritas-1.9/stegoveritas.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2021-07-19 21:35:19.000000 stegoveritas-1.9/stegoveritas.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-07-19 21:35:19.693068 stegoveritas-1.9/stegoveritas_install_deps/
+-rw-rw-r--   0 user      (1000) user      (1000)     3831 2021-07-19 21:26:38.000000 stegoveritas-1.9/stegoveritas_install_deps/Colorer.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-07-19 21:26:38.000000 stegoveritas-1.9/stegoveritas_install_deps/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1862 2021-07-19 21:26:38.000000 stegoveritas-1.9/stegoveritas_install_deps/install_deps.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stegoveritas-1.8/PKG-INFO` & `stegoveritas-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stegoveritas
-Version: 1.8
+Version: 1.9
 Summary: General Steganography detection tool.
 Home-page: https://github.com/bannsec/stegoVeritas
 Author: Michael Bann
 Author-email: self@bannsecurity.com
 License: MIT
 Description: See website for more info.
 Keywords: steg stego steganography stegoveritas
```

### Comparing `stegoveritas-1.8/setup.py` & `stegoveritas-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,13 +38,13 @@
     install_requires=['pillow', 'numpy', 'python-magic', 'prettytable', 'exifread', 'python-xmp-toolkit', 'stegoveritas-binwalk', 'pypng', 'apng', 'stegoveritas-pfp', 'distro'],
     extras_require={
         'dev': ['ipython','twine','pytest','python-coveralls','coverage','pytest-cov','pytest-xdist','sphinxcontrib-napoleon', 'sphinx_rtd_theme','sphinx-autodoc-typehints', 'pyOpenSSL'],
     },
     entry_points={
         'console_scripts': [
             'stegoveritas = stegoveritas.stegoveritas:main',
-            'stegoveritas_install_deps = stegoveritas.install_deps:main',
+            'stegoveritas_install_deps = stegoveritas_install_deps.install_deps:main',
             'stegoveritas_hide_lsb = stegoveritas.hide_lsb:main',
         ],
     },
 )
```

### Comparing `stegoveritas-1.8/stegoveritas.egg-info/PKG-INFO` & `stegoveritas-1.9/stegoveritas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stegoveritas
-Version: 1.8
+Version: 1.9
 Summary: General Steganography detection tool.
 Home-page: https://github.com/bannsec/stegoVeritas
 Author: Michael Bann
 Author-email: self@bannsecurity.com
 License: MIT
 Description: See website for more info.
 Keywords: steg stego steganography stegoveritas
```

### Comparing `stegoveritas-1.8/stegoveritas.egg-info/SOURCES.txt` & `stegoveritas-1.9/stegoveritas.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 setup.py
 stegoveritas/Colorer.py
 stegoveritas/__init__.py
 stegoveritas/helpers.py
 stegoveritas/hide_lsb.py
-stegoveritas/install_deps.py
 stegoveritas/stegoveritas.py
 stegoveritas/version.py
 stegoveritas.egg-info/PKG-INFO
 stegoveritas.egg-info/SOURCES.txt
 stegoveritas.egg-info/dependency_links.txt
 stegoveritas.egg-info/entry_points.txt
 stegoveritas.egg-info/requires.txt
@@ -26,8 +25,11 @@
 stegoveritas/modules/image/analysis/meta.py
 stegoveritas/modules/image/analysis/steghide.py
 stegoveritas/modules/image/analysis/trailing.py
 stegoveritas/modules/multi/__init__.py
 stegoveritas/modules/multi/analysis/__init__.py
 stegoveritas/modules/multi/analysis/carve.py
 stegoveritas/modules/multi/analysis/exif.py
-stegoveritas/modules/multi/analysis/xmp.py
+stegoveritas/modules/multi/analysis/xmp.py
+stegoveritas_install_deps/Colorer.py
+stegoveritas_install_deps/__init__.py
+stegoveritas_install_deps/install_deps.py
```

### Comparing `stegoveritas-1.8/README.md` & `stegoveritas-1.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://travis-ci.org/bannsec/stegoVeritas.svg?branch=master)](https://travis-ci.org/bannsec/stegoVeritas)
+[![Unit Tests](https://github.com/bannsec/stegoVeritas/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/bannsec/stegoVeritas/actions/workflows/unit_tests.yml)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/stegoveritas.svg)](https://pypistats.org/packages/stegoveritas)
 [![Latest Release](https://img.shields.io/pypi/v/stegoveritas.svg)](https://pypi.python.org/pypi/stegoveritas/)
 
 # StegoVeritas
 Yet another Stego Tool
 
 # Quick Start
@@ -38,51 +38,58 @@
 
 `stegoveritas <file>`
 
 If you want to do something specific, you can check out the help:
 
 ```
 stegoveritas -h
-usage: stegoveritas [-h] [-out dir] [-debug] [-meta] [-imageTransform]
+usage: stegoveritas [-h] [-out dir] [-debug] [-password PASSWORD]
+                    [-wordlist WORDLIST] [-meta] [-imageTransform]
                     [-bruteLSB] [-colorMap [N [N ...]]]
                     [-colorMapRange Start End] [-extractLSB]
                     [-red index [index ...]] [-green index [index ...]]
                     [-blue index [index ...]] [-alpha index [index ...]]
-                    [-extract_frames] [-trailing] [-exif] [-xmp] [-carve]
+                    [-extract_frames] [-trailing] [-steghide] [-exif]
+                    [-xmp] [-carve] [-steghide]
                     file
 
 Yet another Stego tool
 
 positional arguments:
   file                  The file to analyze
 
 optional arguments:
   -h, --help            show this help message and exit
   -out dir              Directory to place output in. Defaults to ./results
   -debug                Enable debugging logging.
+  -password PASSWORD    When applicable, attempt to use this password to
+                        extract data.
+  -wordlist WORDLIST    When applicable, attempt to brute force with this
+                        wordlist.
 
 image options:
   -meta                 Check file for metadata information
   -imageTransform       Perform various image transformations on the input
                         image and save them to the output directory
-  -bruteLSB             Attempt to brute force any LSB related stegonography.
+  -bruteLSB             Attempt to brute force any LSB related steganography.
   -colorMap [N [N ...]]
                         Analyze a color map. Optional arguments are colormap
                         indexes to save while searching
   -colorMapRange Start End
                         Analyze a color map. Same as colorMap but implies a
                         range of colorMap values to keep
   -extractLSB           Extract a specific LSB RGB from the image. Use with
                         -red, -green, -blue, and -alpha
   -red index [index ...]
   -green index [index ...]
   -blue index [index ...]
   -alpha index [index ...]
   -extract_frames       Split up an animated gif into individual frames.
   -trailing             Check for trailing data on the given file
+  -steghide             Check for StegHide hidden info.
 
 multi options:
   -exif                 Check this file for exif information.
   -xmp                  Check this file for XMP information.
   -carve                Attempt to carve/extract things from this file.
 
 Have a good example? Wish it did something more? Submit a ticket:
```

### Comparing `stegoveritas-1.8/stegoveritas/stegoveritas.py` & `stegoveritas-1.9/stegoveritas/stegoveritas.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .version import version
 
 import magic
 import time
 import shutil
 from copy import copy
 
-from .install_deps import required_packages
+from stegoveritas_install_deps.install_deps import required_packages
 
 import binwalk
 import tempfile
 import hashlib
 import random
 
 from .helpers import generate_nonce
@@ -123,30 +123,30 @@
             if keepers != []:
                 print(table)
 
                 for keeper in keepers:
                     keeper_dst = os.path.join(self._keeper_directory, os.path.basename(keeper))
 
                     if os.path.exists(keeper_dst):
-                        logger.warn('Keeper name already exists, modifying.')
+                        logger.warning('Keeper name already exists, modifying.')
                         keeper_dst += '_' + generate_nonce()
 
                     # When binwalk hits a gzip (and likely bz2/xz/etc), with the extract flag it will actually
                     # run the uncompressor on it, thus removing the original compressed file.
                     # This is a simple heuristic for this situation
                     if not os.path.isfile(keeper):
 
                         # If there is another file, just with the extention removed, let's assume this is the uncompressed version
                         keeper_minus_extension = ".".join(keeper.split(".")[:-1])
                         if keeper_minus_extension in keepers:
                             # This is fine. We may be missing info unfortunately.
-                            logger.warn("Looks like binwalk removed this file during extraction %s", keeper)
+                            logger.warning("Looks like binwalk removed this file during extraction %s", keeper)
                             continue
 
-                        logger.warn("Couldn't find extracted file named %s", keeper)
+                        logger.warning("Couldn't find extracted file named %s", keeper)
                         continue
 
                     shutil.move(keeper, keeper_dst)
 
             os.chdir(saved_dir)
 
         # TODO: Check if strings of output contain a known word, save if so.
@@ -181,15 +181,15 @@
         parser.add_argument('-wordlist', type=str, default=None, help='When applicable, attempt to brute force with this wordlist.')
         parser.add_argument('file_name', metavar='file', type=str, default=False, help='The file to analyze')
 
         # Image Options
         image = parser.add_argument_group('image options')
         image.add_argument('-meta', action='store_true', help='Check file for metadata information')
         image.add_argument('-imageTransform', action='store_true', help='Perform various image transformations on the input image and save them to the output directory')
-        image.add_argument('-bruteLSB', action='store_true', help='Attempt to brute force any LSB related stegonography.')
+        image.add_argument('-bruteLSB', action='store_true', help='Attempt to brute force any LSB related steganography.')
         image.add_argument('-colorMap', nargs="*", metavar='N', type=int, default=None, help='Analyze a color map. Optional arguments are colormap indexes to save while searching')
         image.add_argument('-colorMapRange', nargs=2, metavar=('Start', 'End'), type=int, default=None, help='Analyze a color map. Same as colorMap but implies a range of colorMap values to keep')
         image.add_argument('-extractLSB', action='store_true', help='Extract a specific LSB RGB from the image. Use with -red, -green, -blue, and -alpha')
         image.add_argument('-red', nargs='+', metavar='index', type=int)
         image.add_argument('-green', nargs='+', metavar='index', type=int)
         image.add_argument('-blue', nargs='+', metavar='index', type=int)
         image.add_argument('-alpha', nargs='+', metavar='index', type=int)
```

### Comparing `stegoveritas-1.8/stegoveritas/hide_lsb.py` & `stegoveritas-1.9/stegoveritas/hide_lsb.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/Colorer.py` & `stegoveritas-1.9/stegoveritas/Colorer.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/helpers.py` & `stegoveritas-1.9/stegoveritas/helpers.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/install_deps.py` & `stegoveritas-1.9/stegoveritas_install_deps/install_deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 # What is required by stegoveritas?
 required_packages = ['exiftool', '7z', 'foremost']
 
 def main():
 
     dist_name = distro.name().lower()
-    
-    if dist_name in ['ubuntu', 'debian', 'kali', 'debian gnu/linux', 'kali gnu/linux']:
+
+    if dist_name in ['ubuntu', 'debian', 'kali', 'debian gnu/linux', 'kali gnu/linux', 'pop!_os', 'elementary os',
+                     'deepin', 'pureos', 'linux mint']:
         debian()
 
     elif dist_name == 'fedora':
         fedora()
 
     elif dist_name in ['archlinux', 'arch', 'arch linux', 'manjaro', 'manjaro linux']:
         archlinux()
@@ -30,15 +31,15 @@
     else:
         logger.error('Unhandled distribution to install deps: {}'.format(dist_name))
         logger.error('Please poke me or submit a PR.')
         return
 
 def debian():
 
-    packages = ['libimage-exiftool-perl', 'libexempi*', 'p7zip-full', 'foremost', 'steghide']
+    packages = ['libimage-exiftool-perl', 'libexempi*', 'p7zip-full', 'foremost', 'steghide', 'libmagic1']
 
     subprocess.run(command_start + ['apt-get','update'])
     subprocess.run(command_start + ['apt-get','install','-y'] + packages)
 
 def fedora():
 
     packages = ['perl-Image-ExifTool', 'exempi', 'p7zip-plugins', 'foremost', 'steghide']
```

### Comparing `stegoveritas-1.8/stegoveritas/modules/__init__.py` & `stegoveritas-1.9/stegoveritas/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/filters.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/filters.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/extractLSB.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/extractLSB.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/extract_frames.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/extract_frames.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/meta.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/meta.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/brute_lsb.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/brute_lsb.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 logger = logging.getLogger('StegoVeritas:Modules:Image:Analysis:BruteLSB')
 
 import os
 import shutil
 import multiprocessing
 from ....helpers import print_error
 
-def run_dump(image, red_index=None, green_index=None, blue_index=None):
-    logger.debug("Trying red={0} green={0} blue={0}".format(red_index, green_index, blue_index))
-    o = image.dumpLSBRGBA(red_index=red_index, green_index=green_index, blue_index=blue_index)
+def run_dump(image, red_index=None, green_index=None, blue_index=None, alpha_index=None):
+    logger.debug("Trying red={} green={} blue={} alpha={}".format(red_index, green_index, blue_index, alpha_index))
+    o = image.dumpLSBRGBA(red_index=red_index, green_index=green_index, blue_index=blue_index, alpha_index=alpha_index)
     image.veritas.test_output(o)
 
 def run(image):
     """Attempts to brute force out any LSB stego.
 
     Args:
         image: SVImage class instance
```

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/trailing.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/trailing.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/colormap.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/colormap.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/analysis/steghide.py` & `stegoveritas-1.9/stegoveritas/modules/image/analysis/steghide.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/png.py` & `stegoveritas-1.9/stegoveritas/modules/image/png.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/__init__.py` & `stegoveritas-1.9/stegoveritas/modules/image/__init__.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/image/gif.py` & `stegoveritas-1.9/stegoveritas/modules/image/gif.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/multi/analysis/xmp.py` & `stegoveritas-1.9/stegoveritas/modules/multi/analysis/xmp.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/multi/analysis/carve.py` & `stegoveritas-1.9/stegoveritas/modules/multi/analysis/carve.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/multi/analysis/exif.py` & `stegoveritas-1.9/stegoveritas/modules/multi/analysis/exif.py`

 * *Files identical despite different names*

### Comparing `stegoveritas-1.8/stegoveritas/modules/multi/__init__.py` & `stegoveritas-1.9/stegoveritas/modules/multi/__init__.py`

 * *Files identical despite different names*

