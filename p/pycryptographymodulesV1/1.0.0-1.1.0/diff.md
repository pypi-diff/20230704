# Comparing `tmp/pycryptographymodulesV1-1.0.0.tar.gz` & `tmp/pycryptographymodulesV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptographymodulesV1-1.0.0.tar", last modified: Tue Jul  4 09:18:03 2023, max compression
+gzip compressed data, was "pycryptographymodulesV1-1.1.0.tar", last modified: Tue Jul  4 09:20:08 2023, max compression
```

## Comparing `pycryptographymodulesV1-1.0.0.tar` & `pycryptographymodulesV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:18:03.230917 pycryptographymodulesV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-04 09:18:03.230917 pycryptographymodulesV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:18:03.230917 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 09:18:02.000000 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:18:03.230917 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-04 09:18:03.000000 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-07-04 09:18:03.000000 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 09:18:03.000000 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-04 09:18:03.000000 pycryptographymodulesV1-1.0.0/pycryptographymodulesV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 09:18:03.230917 pycryptographymodulesV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      569 2023-07-04 09:18:02.000000 pycryptographymodulesV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:20:08.982488 pycryptographymodulesV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-04 09:20:08.982488 pycryptographymodulesV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:20:08.978488 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-04 09:20:08.000000 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:20:08.982488 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-04 09:20:08.000000 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-07-04 09:20:08.000000 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 09:20:08.000000 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-04 09:20:08.000000 pycryptographymodulesV1-1.1.0/pycryptographymodulesV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 09:20:08.982488 pycryptographymodulesV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      569 2023-07-04 09:20:08.000000 pycryptographymodulesV1-1.1.0/setup.py
```

### Comparing `pycryptographymodulesV1-1.0.0/setup.py` & `pycryptographymodulesV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pycryptographymodulesV1",
     version=VERSION,
```

