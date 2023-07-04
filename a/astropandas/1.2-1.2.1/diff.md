# Comparing `tmp/astropandas-1.2.tar.gz` & `tmp/astropandas-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropandas-1.2.tar", last modified: Mon Jun 26 14:58:56 2023, max compression
+gzip compressed data, was "astropandas-1.2.1.tar", last modified: Tue Jul  4 09:32:36 2023, max compression
```

## Comparing `astropandas-1.2.tar` & `astropandas-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:58:56.237604 astropandas-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-26 14:58:44.000000 astropandas-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 14:58:56.237604 astropandas-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 14:58:44.000000 astropandas-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:58:56.237604 astropandas-1.2/astropandas/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 14:58:44.000000 astropandas-1.2/astropandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-26 14:58:44.000000 astropandas-1.2/astropandas/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-06-26 14:58:44.000000 astropandas-1.2/astropandas/match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:58:56.237604 astropandas-1.2/astropandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 14:58:56.000000 astropandas-1.2/astropandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 14:58:44.000000 astropandas-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 14:58:56.237604 astropandas-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:58:44.000000 astropandas-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:32:36.024808 astropandas-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-04 09:32:21.000000 astropandas-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 09:32:36.024808 astropandas-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 09:32:21.000000 astropandas-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:32:36.024808 astropandas-1.2.1/astropandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 09:32:21.000000 astropandas-1.2.1/astropandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-04 09:32:21.000000 astropandas-1.2.1/astropandas/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-07-04 09:32:21.000000 astropandas-1.2.1/astropandas/match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:32:36.024808 astropandas-1.2.1/astropandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 09:32:21.000000 astropandas-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 09:32:36.028807 astropandas-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 09:32:21.000000 astropandas-1.2.1/setup.py
```

### Comparing `astropandas-1.2/LICENSE` & `astropandas-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astropandas-1.2/PKG-INFO` & `astropandas-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropandas
-Version: 1.2
+Version: 1.2.1
 Summary: Tools to expand on pandas functionality for astronomical operations.
 Author: Jan Luca van den Busch
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `astropandas-1.2/README.md` & `astropandas-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `astropandas-1.2/astropandas/io.py` & `astropandas-1.2.1/astropandas/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,25 +138,26 @@
             dataframe[colname] = values.astype("|S")
     return dataframe
 
 
 def read_auto(
     fpath: str,
     columns: Sequence[str] | None = None,
+    ext: str | None = None,
     **kwargs
 ) -> pd.DataFrame:
     """
     Read a file by guessing its type from the extension. Standard parameters
     are used for the pandas.read_xxx() method.
 
     Parameters:
     -----------
     fpath : str
         Path to the FITS file.
-    ext : str
+    ext : str (optional)
         Manual overwrite for the file extension.
     columns : list of str (optional)
         Subset of columns to read from the table (if supported), defaults to
         all.
     **kwargs
         Passed on to the pandas.read_xxx() method.
```

### Comparing `astropandas-1.2/astropandas/match.py` & `astropandas-1.2.1/astropandas/match.py`

 * *Files identical despite different names*

### Comparing `astropandas-1.2/astropandas.egg-info/PKG-INFO` & `astropandas-1.2.1/astropandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropandas
-Version: 1.2
+Version: 1.2.1
 Summary: Tools to expand on pandas functionality for astronomical operations.
 Author: Jan Luca van den Busch
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `astropandas-1.2/setup.cfg` & `astropandas-1.2.1/setup.cfg`

 * *Files identical despite different names*

