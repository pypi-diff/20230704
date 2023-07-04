# Comparing `tmp/sacc-0.8.1.tar.gz` & `tmp/sacc-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sacc-0.8.1.tar", last modified: Wed May 10 16:00:52 2023, max compression
+gzip compressed data, was "sacc-0.9.tar", last modified: Tue Jul  4 14:04:36 2023, max compression
```

## Comparing `sacc-0.8.1.tar` & `sacc-0.9.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.766541 sacc-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 16:00:48.000000 sacc-0.8.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 16:00:48.000000 sacc-0.8.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.758541 sacc-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.758541 sacc-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-10 16:00:48.000000 sacc-0.8.1/.github/workflows/desc-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 16:00:48.000000 sacc-0.8.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 16:00:48.000000 sacc-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-10 16:00:48.000000 sacc-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-10 16:00:48.000000 sacc-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:00:48.000000 sacc-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-10 16:00:52.766541 sacc-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-10 16:00:48.000000 sacc-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.758541 sacc-0.8.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/format.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/covariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/data_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/sacc.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/tracers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/windows.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   102753 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/CMB_LSS_read.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   120842 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/CMB_LSS_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Convert_DES_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Convert_KIDS_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Create_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42715 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Create_cluster_count_SACC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/SACC_for_clusters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   154105 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/SACC_read.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/SACC_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20744 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/example-txpipe-sacc1.sacc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 16:00:48.000000 sacc-0.8.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/sacc/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16583 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    49485 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/sacc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27599 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/tracers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/sacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:00:52.766541 sacc-0.8.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-05-10 16:00:48.000000 sacc-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.766541 sacc-0.8.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.766541 sacc-0.8.1/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 16:00:48.000000 sacc-0.8.1/test/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-10 16:00:48.000000 sacc-0.8.1/test/make_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28004 2023-05-10 16:00:48.000000 sacc-0.8.1/test/test_sacc2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.943671 sacc-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 14:04:31.000000 sacc-0.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-04 14:04:31.000000 sacc-0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.935670 sacc-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.935670 sacc-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 14:04:31.000000 sacc-0.9/.github/workflows/desc-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 14:04:31.000000 sacc-0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 14:04:31.000000 sacc-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 14:04:31.000000 sacc-0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-04 14:04:31.000000 sacc-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 14:04:31.000000 sacc-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-04 14:04:36.943671 sacc-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-04 14:04:31.000000 sacc-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.935670 sacc-0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 14:04:31.000000 sacc-0.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-04 14:04:31.000000 sacc-0.9/doc/format.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.939671 sacc-0.9/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/covariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/data_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/sacc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/tracers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 14:04:31.000000 sacc-0.9/doc/source/windows.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.939671 sacc-0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 14:04:31.000000 sacc-0.9/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   102753 2023-07-04 14:04:31.000000 sacc-0.9/examples/CMB_LSS_read.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   120842 2023-07-04 14:04:31.000000 sacc-0.9/examples/CMB_LSS_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-04 14:04:31.000000 sacc-0.9/examples/Convert_DES_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-04 14:04:31.000000 sacc-0.9/examples/Convert_KIDS_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-07-04 14:04:31.000000 sacc-0.9/examples/Create_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 14:04:31.000000 sacc-0.9/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-07-04 14:04:31.000000 sacc-0.9/examples/SACC_for_clusters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   154105 2023-07-04 14:04:31.000000 sacc-0.9/examples/SACC_read.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-07-04 14:04:31.000000 sacc-0.9/examples/SACC_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-07-04 14:04:31.000000 sacc-0.9/examples/demo_sacc_for_clusters_N+M.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20744 2023-07-04 14:04:31.000000 sacc-0.9/examples/example-txpipe-sacc1.sacc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 14:04:31.000000 sacc-0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.943671 sacc-0.9/sacc/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-04 14:04:31.000000 sacc-0.9/sacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-07-04 14:04:31.000000 sacc-0.9/sacc/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-07-04 14:04:31.000000 sacc-0.9/sacc/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49485 2023-07-04 14:04:31.000000 sacc-0.9/sacc/sacc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38577 2023-07-04 14:04:31.000000 sacc-0.9/sacc/tracers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-04 14:04:31.000000 sacc-0.9/sacc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-04 14:04:31.000000 sacc-0.9/sacc/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.943671 sacc-0.9/sacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-04 14:04:36.000000 sacc-0.9/sacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 14:04:36.000000 sacc-0.9/sacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:04:36.000000 sacc-0.9/sacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 14:04:36.000000 sacc-0.9/sacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 14:04:36.000000 sacc-0.9/sacc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:04:36.943671 sacc-0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-07-04 14:04:31.000000 sacc-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.943671 sacc-0.9/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:04:36.943671 sacc-0.9/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 14:04:31.000000 sacc-0.9/test/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 14:04:31.000000 sacc-0.9/test/make_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-07-04 14:04:31.000000 sacc-0.9/test/test_cluster_data_tracers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28004 2023-07-04 14:04:31.000000 sacc-0.9/test/test_sacc2.py
```

### Comparing `sacc-0.8.1/.github/workflows/desc-ci.yml` & `sacc-0.9/.github/workflows/desc-ci.yml`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/.gitignore` & `sacc-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/LICENSE` & `sacc-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/PKG-INFO` & `sacc-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sacc
-Version: 0.8.1
+Version: 0.9
 Summary: SACC - the LSST/DESC summary statistic data format library
 Home-page: https://github.com/LSSTDESC/sacc
 Author: LSST DESC
 Author-email: joezuntz@googlemail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sacc-0.8.1/README.md` & `sacc-0.9/README.md`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/doc/Makefile` & `sacc-0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/doc/format.md` & `sacc-0.9/doc/format.md`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/doc/source/Makefile` & `sacc-0.9/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/doc/source/conf.py` & `sacc-0.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/doc/source/intro.rst` & `sacc-0.9/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/CMB_LSS_read.ipynb` & `sacc-0.9/examples/CMB_LSS_read.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/CMB_LSS_write.ipynb` & `sacc-0.9/examples/CMB_LSS_write.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/Convert_DES_Sacc.ipynb` & `sacc-0.9/examples/Convert_DES_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/Convert_KIDS_Sacc.ipynb` & `sacc-0.9/examples/Convert_KIDS_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/Create_Sacc.ipynb` & `sacc-0.9/examples/Create_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/SACC_for_clusters.ipynb` & `sacc-0.9/examples/SACC_for_clusters.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/SACC_read.ipynb` & `sacc-0.9/examples/SACC_read.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/SACC_write.ipynb` & `sacc-0.9/examples/SACC_write.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/examples/example-txpipe-sacc1.sacc` & `sacc-0.9/examples/example-txpipe-sacc1.sacc`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/sacc/covariance.py` & `sacc-0.9/sacc/covariance.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/sacc/data_types.py` & `sacc-0.9/sacc/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,18 @@
     "xi_0b": ['theta'],
     "xi_e0": ['theta'],
     "xi_b0": ['theta'],
     "xi_plus_re": ['theta'],
     "xi_plus_im": ['theta'],
     "xi_minus_re": ['theta'],
     "xi_minus_im": ['theta'],
-    "count": []
+    "count": [],
+    "cluster_counts": [],
+    "cluster_mean_log_mass": [],
+    "cluster_shear": ["radius_bin"]
 }
 
 required_tags_verbose = {
     "clusterGalaxy_densityConvergence_cl": ['ell'],
     "clusterGalaxy_densityConvergence_xi": ['theta'],
     "clusterGalaxy_densityShear_cl_b": ['ell'],
     "clusterGalaxy_densityShear_cl_e": ['ell'],
```

### Comparing `sacc-0.8.1/sacc/sacc.py` & `sacc-0.9/sacc/sacc.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/sacc/tracers.py` & `sacc-0.9/sacc/tracers.py`

 * *Files 24% similar despite different names*

```diff
@@ -704,42 +704,42 @@
         -------
         tables: list
             List of astropy tables
         """
         from tables_io.convUtils import convertToApTables
 
         tables = []
-        
+
         for tracer in instance_list:
             table_dict = tracer.ensemble.build_tables()
             ap_tables = convertToApTables(table_dict)
             data_table = ap_tables['data']
             meta_table = ap_tables['meta']
             ancil_table = ap_tables.get('ancil', None)
             meta_table.meta['SACCTYPE'] = 'tracer'
             meta_table.meta['SACCCLSS'] = cls.tracer_type
             meta_table.meta['SACCNAME'] = tracer.name
-            meta_table.meta['SACCQTTY'] = tracer.quantity            
+            meta_table.meta['SACCQTTY'] = tracer.quantity
             meta_table.meta['EXTNAME'] = f'tracer:{cls.tracer_type}:{tracer.name}:meta'
 
             data_table.meta['SACCTYPE'] = 'tracer'
             data_table.meta['SACCCLSS'] = cls.tracer_type
             data_table.meta['SACCNAME'] = tracer.name
-            data_table.meta['SACCQTTY'] = tracer.quantity            
+            data_table.meta['SACCQTTY'] = tracer.quantity
             data_table.meta['EXTNAME'] = f'tracer:{cls.tracer_type}:{tracer.name}:data'
 
             for kk, vv in tracer.metadata.items():
                 meta_table.meta['META_'+kk] = vv
             tables.append(data_table)
             tables.append(meta_table)
             if ancil_table:
                 ancil_table.meta['SACCTYPE'] = 'tracer'
                 ancil_table.meta['SACCCLSS'] = cls.tracer_type
                 ancil_table.meta['SACCNAME'] = tracer.name
-                ancil_table.meta['SACCQTTY'] = tracer.quantity            
+                ancil_table.meta['SACCQTTY'] = tracer.quantity
                 ancil_table.meta['EXTNAME'] = f'tracer:{cls.tracer_type}:{tracer.name}:ancil'
 
                 tables.append(ancil_table)
         return tables
 
     @classmethod
     def from_tables(cls, table_list):
@@ -764,15 +764,15 @@
         tracers = {}
         sorted_dict = {}
         for table_ in table_list:
             tokens = table_.meta['EXTNAME'].split(':')
             table_key = f'{tokens[0]}:{tokens[1]}:{tokens[2]}'
             table_type = f'{tokens[3]}'
             if table_key not in sorted_dict:
-                sorted_dict[table_key] = {table_type:table_}
+                sorted_dict[table_key] = {table_type: table_}
             else:
                 sorted_dict[table_key][table_type] = table_
 
         for key, val in sorted_dict.items():
             meta_table = val['meta']
             ensemble = qp.from_tables(val)
             name = meta_table.meta['SACCNAME']
@@ -782,7 +782,318 @@
             for key, value in meta_table.meta.items():
                 if key.startswith("META_"):
                     metadata[key[5:]] = value
             tracers[name] = cls(name, ensemble,
                                 quantity=quantity,
                                 metadata=metadata)
         return tracers
+
+
+class BinZTracer(BaseTracer, tracer_type="bin_z"):  # type: ignore
+    """A tracer for a single redshift bin. The tracer shall
+    be used for binned data where we want a desired quantity
+    per interval of redshift, such that we only need the data
+    for a given interval instead of at individual redshifts."""
+
+    def __init__(self, name: str, lower: float, upper: float, **kwargs):
+        """
+        Create a tracer corresponding to a single redshift bin.
+
+        :param name: The name of the tracer
+        :param lower: The lower bound of the redshift bin
+        :param upper: The upper bound of the redshift bin
+        """
+        super().__init__(name, **kwargs)
+        self.lower = lower
+        self.upper = upper
+
+    def __eq__(self, other) -> bool:
+        """Test for equality.  If :python:`other` is not a
+        :python:`BinZTracer`, then it is not equal to :python:`self`.
+        Otherwise, they are equal if names, and the z-range of the bins,
+        are equal."""
+        if not isinstance(other, BinZTracer):
+            return False
+        return (
+            self.name == other.name
+            and self.lower == other.lower
+            and self.upper == other.upper
+        )
+
+    @classmethod
+    def to_tables(cls, instance_list):
+        """Convert a list of BinZTracers to a single astropy table
+
+        This is used when saving data to a file.
+        One table is generated with the information for all the tracers.
+
+        :param instance_list: List of tracer instances
+        :return: List with a single astropy table
+        """
+
+        names = ["name", "quantity", "lower", "upper"]
+
+        cols = [
+            [obj.name for obj in instance_list],
+            [obj.quantity for obj in instance_list],
+            [obj.lower for obj in instance_list],
+            [obj.upper for obj in instance_list],
+        ]
+
+        table = Table(data=cols, names=names)
+        table.meta["SACCTYPE"] = "tracer"
+        table.meta["SACCCLSS"] = cls.tracer_type
+        table.meta["EXTNAME"] = f"tracer:{cls.tracer_type}"
+        return [table]
+
+    @classmethod
+    def from_tables(cls, table_list):
+        """Convert an astropy table into a dictionary of tracers
+
+        This is used when loading data from a file.
+        One tracer object is created for each "row" in each table.
+
+        :param table_list: List of astropy tables
+        :return: Dictionary of tracers
+        """
+        tracers = {}
+
+        for table in table_list:
+            for row in table:
+                name = row["name"]
+                quantity = row["quantity"]
+                lower = row["lower"]
+                upper = row["upper"]
+                tracers[name] = cls(name, quantity=quantity, lower=lower, upper=upper)
+        return tracers
+
+class BinLogMTracer(BaseTracer, tracer_type="bin_logM"):  # type: ignore
+    """A tracer for a single log-mass bin. The tracer shall
+    be used for binned data where we want a desired quantity
+    per interval of log(mass), such that we only need the data
+    for a given interval instead of at individual masses."""
+
+    def __init__(self, name: str, lower: float, upper: float, **kwargs):
+        """
+        Create a tracer corresponding to a single log-mass bin.
+
+        :param name: The name of the tracer
+        :param lower: The lower bound of the log-mass bin
+        :param upper: The upper bound of the log-mass bin
+        """
+        super().__init__(name, **kwargs)
+        self.lower = lower
+        self.upper = upper
+
+    def __eq__(self, other) -> bool:
+        """Test for equality.  If :python:`other` is not a
+        :python:`BinLogMTracer`, then it is not equal to :python:`self`.
+        Otherwise, they are equal if names, and the z-range of the bins,
+        are equal."""
+        if not isinstance(other, BinLogMTracer):
+            return False
+        return (
+            self.name == other.name
+            and self.lower == other.lower
+            and self.upper == other.upper
+        )
+
+    @classmethod
+    def to_tables(cls, instance_list):
+        """Convert a list of BinLogMTracers to a single astropy table
+
+        This is used when saving data to a file.
+        One table is generated with the information for all the tracers.
+
+        :param instance_list: List of tracer instances
+        :return: List with a single astropy table
+        """
+
+        names = ["name", "quantity", "lower", "upper"]
+
+        cols = [
+            [obj.name for obj in instance_list],
+            [obj.quantity for obj in instance_list],
+            [obj.lower for obj in instance_list],
+            [obj.upper for obj in instance_list],
+        ]
+        table = Table(data=cols, names=names)
+        table.meta["SACCTYPE"] = "tracer"
+        table.meta["SACCCLSS"] = cls.tracer_type
+        table.meta["EXTNAME"] = f"tracer:{cls.tracer_type}"
+        return [table]
+
+    @classmethod
+    def from_tables(cls, table_list):
+        """Convert an astropy table into a dictionary of tracers
+
+        This is used when loading data from a file.
+        One tracer object is created for each "row" in each table.
+
+        :param table_list: List of astropy tables
+        :return: Dictionary of tracers
+        """
+        tracers = {}
+
+        for table in table_list:
+            for row in table:
+                name = row["name"]
+                quantity = row["quantity"]
+                lower = row["lower"]
+                upper = row["upper"]
+                tracers[name] = cls(name, quantity=quantity, lower=lower, upper=upper)
+        return tracers
+
+         
+class BinRichnessTracer(BaseTracer, tracer_type="bin_richness"):  # type: ignore
+    """A tracer for a single richness bin. The tracer shall
+    be used for binned data where we want a desired quantity
+    per interval of log(richness), such that we only need the data
+    for a given interval instead of at individual richness."""
+
+    def __eq__(self, other) -> bool:
+        """Test for equality. If :python:`other` is not a
+        :python:`BinRichnessTracer`, then it is not equal to :python:`self`.
+        Otherwise, they are equal if names and the richness-range of the
+        bins, are equal."""
+        if not isinstance(other, BinRichnessTracer):
+            return False
+        return (
+            self.name == other.name
+            and self.lower == other.lower
+            and self.upper == other.upper
+        )
+
+    def __init__(self, name: str, lower: float, upper: float, **kwargs):
+        """
+        Create a tracer corresponding to a single richness bin.
+
+        :param name: The name of the tracer
+        :param lower: The lower bound of the richness bin in log10.
+        :param upper: The upper bound of the richness bin in log10.
+        """
+        super().__init__(name, **kwargs)
+        self.lower = lower
+        self.upper = upper
+
+    @classmethod
+    def to_tables(cls, instance_list):
+        """Convert a list of BinZTracers to a list of astropy tables
+
+        This is used when saving data to a file.
+        One table is generated with the information for all the tracers.
+
+        :param instance_list: List of tracer instances
+        :return: List with a single astropy table
+        """
+        names = ["name", "quantity", "lower", "upper"]
+
+        cols = [
+            [obj.name for obj in instance_list],
+            [obj.quantity for obj in instance_list],
+            [obj.lower for obj in instance_list],
+            [obj.upper for obj in instance_list],
+        ]
+
+        table = Table(data=cols, names=names)
+        table.meta["SACCTYPE"] = "tracer"
+        table.meta["SACCCLSS"] = cls.tracer_type
+        table.meta["EXTNAME"] = f"tracer:{cls.tracer_type}"
+        return [table]
+
+    @classmethod
+    def from_tables(cls, table_list):
+        """Convert an astropy table into a dictionary of tracers
+
+        This is used when loading data from a file.
+        One tracer object is created for each "row" in each table.
+
+        :param table_list: List of astropy tables
+        :return: Dictionary of tracers
+        """
+        tracers = {}
+
+        for table in table_list:
+            for row in table:
+                name = row["name"]
+                quantity = row["quantity"]
+                lower = row["lower"]
+                upper = row["upper"]
+                tracers[name] = cls(
+                    name,
+                    quantity=quantity,
+                    lower=lower,
+                    upper=upper,
+                )
+        return tracers
+
+
+class SurveyTracer(BaseTracer, tracer_type="survey"):  # type: ignore
+    """A tracer for the survey definition. It shall 
+    be used to filter data related to a given survey
+    and to provide the survey sky-area of analysis."""
+
+    def __eq__(self, other) -> bool:
+        """Test for equality. If :python:`other` is not a
+        :python:`SurveyTracer`, then it is not equal to :python:`self`.
+        Otherwise, they are equal if names and the sky-areas are equal."""
+        if not isinstance(other, SurveyTracer):
+            return False
+        return self.name == other.name and self.sky_area == other.sky_area
+
+    def __init__(self, name: str, sky_area: float, **kwargs):
+        """
+        Create a tracer corresponding to the survey definition.
+
+        :param name: The name of the tracer
+        :param sky_area: The survey's sky area in square degrees
+        """
+        super().__init__(name, **kwargs)
+        self.sky_area = sky_area
+
+    @classmethod
+    def to_tables(cls, instance_list):
+        """Convert a list of SurveyTracer to a list of astropy tables
+
+        This is used when saving data to a file.
+        One table is generated with the information for all the tracers.
+
+        :param instance_list: List of tracer instances
+        :return: List of astropy tables with one table
+        """
+        names = ["name", "quantity", "sky_area"]
+
+        cols = [
+            [obj.name for obj in instance_list],
+            [obj.quantity for obj in instance_list],
+            [obj.sky_area for obj in instance_list],
+        ]
+
+        table = Table(data=cols, names=names)
+        table.meta["SACCTYPE"] = "tracer"
+        table.meta["SACCCLSS"] = cls.tracer_type
+        table.meta["EXTNAME"] = f"tracer:{cls.tracer_type}"
+        return [table]
+
+    @classmethod
+    def from_tables(cls, table_list):
+        """Convert an astropy table into a dictionary of tracers
+
+        This is used when loading data from a file.
+        One tracer object is created for each "row" in each table.
+
+        :param table_list: List of astropy tables
+        :return: Dictionary of tracers
+        """
+        tracers = {}
+
+        for table in table_list:
+            for row in table:
+                name = row["name"]
+                quantity = row["quantity"]
+                sky_area = row["sky_area"]
+                tracers[name] = cls(
+                    name,
+                    quantity=quantity,
+                    sky_area=sky_area,
+                )
+        return tracers
```

### Comparing `sacc-0.8.1/sacc/utils.py` & `sacc-0.9/sacc/utils.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/sacc/windows.py` & `sacc-0.9/sacc/windows.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/sacc.egg-info/PKG-INFO` & `sacc-0.9/sacc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sacc
-Version: 0.8.1
+Version: 0.9
 Summary: SACC - the LSST/DESC summary statistic data format library
 Home-page: https://github.com/LSSTDESC/sacc
 Author: LSST DESC
 Author-email: joezuntz@googlemail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sacc-0.8.1/sacc.egg-info/SOURCES.txt` & `sacc-0.9/sacc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 doc/source/windows.rst
 examples/.gitignore
 examples/CMB_LSS_read.ipynb
 examples/CMB_LSS_write.ipynb
 examples/Convert_DES_Sacc.ipynb
 examples/Convert_KIDS_Sacc.ipynb
 examples/Create_Sacc.ipynb
-examples/Create_cluster_count_SACC.ipynb
 examples/README.md
 examples/SACC_for_clusters.ipynb
 examples/SACC_read.ipynb
 examples/SACC_write.ipynb
+examples/demo_sacc_for_clusters_N+M.ipynb
 examples/example-txpipe-sacc1.sacc
 sacc/__init__.py
 sacc/covariance.py
 sacc/data_types.py
 sacc/sacc.py
 sacc/tracers.py
 sacc/utils.py
 sacc/windows.py
 sacc.egg-info/PKG-INFO
 sacc.egg-info/SOURCES.txt
 sacc.egg-info/dependency_links.txt
 sacc.egg-info/requires.txt
 sacc.egg-info/top_level.txt
 test/make_test_data.py
+test/test_cluster_data_tracers.py
 test/test_sacc2.py
 test/data/.gitignore
```

### Comparing `sacc-0.8.1/setup.py` & `sacc-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/test/make_test_data.py` & `sacc-0.9/test/make_test_data.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8.1/test/test_sacc2.py` & `sacc-0.9/test/test_sacc2.py`

 * *Files identical despite different names*

