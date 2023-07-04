# Comparing `tmp/dk-1.2.0.tar.gz` & `tmp/dk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dk-1.2.0.tar", last modified: Wed Jan 18 12:52:38 2023, max compression
+gzip compressed data, was "dk-1.2.1.tar", last modified: Tue Jul  4 12:58:11 2023, max compression
```

## Comparing `dk-1.2.0.tar` & `dk-1.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:38.657216 dk-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-01-18 12:52:26.000000 dk-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:26.000000 dk-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-18 12:52:38.657216 dk-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-18 12:52:26.000000 dk-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:38.653216 dk-1.2.0/dk/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-18 12:52:26.000000 dk-1.2.0/dk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-01-18 12:52:26.000000 dk-1.2.0/dk/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-18 12:52:26.000000 dk-1.2.0/dk/asciify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:38.657216 dk-1.2.0/dk/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/OrderedSet.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/invdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/mmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/pset.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/sdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-18 12:52:26.000000 dk-1.2.0/dk/collections/xmlrec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-18 12:52:26.000000 dk-1.2.0/dk/dkimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-01-18 12:52:26.000000 dk-1.2.0/dk/dklogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-01-18 12:52:26.000000 dk-1.2.0/dk/fstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-01-18 12:52:26.000000 dk-1.2.0/dk/gchart.py
--rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-01-18 12:52:26.000000 dk-1.2.0/dk/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:38.657216 dk-1.2.0/dk/html/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-18 12:52:26.000000 dk-1.2.0/dk/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-18 12:52:26.000000 dk-1.2.0/dk/html/css.py
--rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-01-18 12:52:26.000000 dk-1.2.0/dk/html/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-01-18 12:52:26.000000 dk-1.2.0/dk/html/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-01-18 12:52:26.000000 dk-1.2.0/dk/html/uhtml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-01-18 12:52:26.000000 dk-1.2.0/dk/iplist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:38.657216 dk-1.2.0/dk/js/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-18 12:52:26.000000 dk-1.2.0/dk/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-18 12:52:26.000000 dk-1.2.0/dk/js/js.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-01-18 12:52:26.000000 dk-1.2.0/dk/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-18 12:52:26.000000 dk-1.2.0/dk/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-01-18 12:52:26.000000 dk-1.2.0/dk/utidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-01-18 12:52:26.000000 dk-1.2.0/dk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:52:38.653216 dk-1.2.0/dk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-18 12:52:38.000000 dk-1.2.0/dk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-18 12:52:38.000000 dk-1.2.0/dk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 12:52:38.000000 dk-1.2.0/dk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 12:52:38.000000 dk-1.2.0/dk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-18 12:52:38.000000 dk-1.2.0/dk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-18 12:52:38.000000 dk-1.2.0/dk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-18 12:52:38.657216 dk-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-18 12:52:26.000000 dk-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:11.522103 dk-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-04 12:57:56.000000 dk-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:57:56.000000 dk-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-04 12:58:11.522103 dk-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-04 12:57:56.000000 dk-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:11.522103 dk-1.2.1/dk/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-04 12:57:56.000000 dk-1.2.1/dk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-04 12:57:56.000000 dk-1.2.1/dk/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-04 12:57:56.000000 dk-1.2.1/dk/asciify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:11.522103 dk-1.2.1/dk/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/OrderedSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/invdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/pset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/sdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-04 12:57:56.000000 dk-1.2.1/dk/collections/xmlrec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-04 12:57:56.000000 dk-1.2.1/dk/dkimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-04 12:57:56.000000 dk-1.2.1/dk/dklogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-04 12:57:56.000000 dk-1.2.1/dk/fstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-04 12:57:56.000000 dk-1.2.1/dk/gchart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-04 12:57:56.000000 dk-1.2.1/dk/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:11.522103 dk-1.2.1/dk/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-04 12:57:56.000000 dk-1.2.1/dk/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-04 12:57:56.000000 dk-1.2.1/dk/html/css.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-07-04 12:57:56.000000 dk-1.2.1/dk/html/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-04 12:57:56.000000 dk-1.2.1/dk/html/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-07-04 12:57:56.000000 dk-1.2.1/dk/html/uhtml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-04 12:57:56.000000 dk-1.2.1/dk/iplist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:11.522103 dk-1.2.1/dk/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 12:57:56.000000 dk-1.2.1/dk/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-04 12:57:56.000000 dk-1.2.1/dk/js/js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-04 12:57:56.000000 dk-1.2.1/dk/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 12:57:56.000000 dk-1.2.1/dk/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-07-04 12:57:56.000000 dk-1.2.1/dk/utidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-04 12:57:56.000000 dk-1.2.1/dk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:11.522103 dk-1.2.1/dk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-04 12:58:11.000000 dk-1.2.1/dk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-04 12:58:11.000000 dk-1.2.1/dk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:58:11.000000 dk-1.2.1/dk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:58:11.000000 dk-1.2.1/dk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 12:58:11.000000 dk-1.2.1/dk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-04 12:58:11.000000 dk-1.2.1/dk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 12:58:11.522103 dk-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 12:57:56.000000 dk-1.2.1/setup.py
```

### Comparing `dk-1.2.0/LICENSE.txt` & `dk-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/PKG-INFO` & `dk-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dk
-Version: 1.2.0
+Version: 1.2.1
 Summary: The Datakortet Basic utilities package: `dk`.
 Home-page: http://www.github.com/datakortet/dk/
 Author: Bjorn Pettersen
 Author-email: bp@datakortet.no
 License: LGPL
 Download-URL: https://www.github.com/datakortet/dk
 Description:
```

### Comparing `dk-1.2.0/README.rst` & `dk-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/age.py` & `dk-1.2.1/dk/age.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/asciify.py` & `dk-1.2.1/dk/asciify.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/collections/OrderedSet.py` & `dk-1.2.1/dk/collections/OrderedSet.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/collections/mmap.py` & `dk-1.2.1/dk/collections/mmap.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/collections/pset.py` & `dk-1.2.1/dk/collections/pset.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/collections/sdict.py` & `dk-1.2.1/dk/collections/sdict.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/collections/xmlrec.py` & `dk-1.2.1/dk/collections/xmlrec.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/dkimport.py` & `dk-1.2.1/dk/dkimport.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/dklogger.py` & `dk-1.2.1/dk/dklogger.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/fstr.py` & `dk-1.2.1/dk/fstr.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/gchart.py` & `dk-1.2.1/dk/gchart.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/grid.py` & `dk-1.2.1/dk/grid.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/html/css.py` & `dk-1.2.1/dk/html/css.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/html/html.py` & `dk-1.2.1/dk/html/html.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/html/theme.py` & `dk-1.2.1/dk/html/theme.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/html/uhtml.py` & `dk-1.2.1/dk/html/uhtml.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/iplist.py` & `dk-1.2.1/dk/iplist.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/js/js.py` & `dk-1.2.1/dk/js/js.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/proxy.py` & `dk-1.2.1/dk/proxy.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/text.py` & `dk-1.2.1/dk/text.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/utidy.py` & `dk-1.2.1/dk/utidy.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk/utils.py` & `dk-1.2.1/dk/utils.py`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/dk.egg-info/PKG-INFO` & `dk-1.2.1/dk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dk
-Version: 1.2.0
+Version: 1.2.1
 Summary: The Datakortet Basic utilities package: `dk`.
 Home-page: http://www.github.com/datakortet/dk/
 Author: Bjorn Pettersen
 Author-email: bp@datakortet.no
 License: LGPL
 Download-URL: https://www.github.com/datakortet/dk
 Description:
```

### Comparing `dk-1.2.0/dk.egg-info/SOURCES.txt` & `dk-1.2.1/dk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dk-1.2.0/setup.py` & `dk-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Programming Language :: Python
 Programming Language :: Python :: 3
 Topic :: Software Development :: Libraries
 """
 
 import setuptools
 
-version = '1.2.0'
+version = '1.2.1'
 
 
 setuptools.setup(
     name='dk',
     version=version,
     requires=[],
     install_requires=[
```

