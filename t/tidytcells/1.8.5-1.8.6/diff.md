# Comparing `tmp/tidytcells-1.8.5.tar.gz` & `tmp/tidytcells-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.8.5.tar", last modified: Sun Jun  4 14:01:03 2023, max compression
+gzip compressed data, was "tidytcells-1.8.6.tar", last modified: Tue Jul  4 15:19:24 2023, max compression
```

## Comparing `tidytcells-1.8.5.tar` & `tidytcells-1.8.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.990591 tidytcells-1.8.5/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.8.5/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.8.5/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 14:01:03.990591 tidytcells-1.8.5/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-04 13:01:59.000000 tidytcells-1.8.5/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-04 13:54:37.000000 tidytcells-1.8.5/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-04 14:01:03.990591 tidytcells-1.8.5/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-04 13:01:59.000000 tidytcells-1.8.5/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.982591 tidytcells-1.8.5/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.983591 tidytcells-1.8.5/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-04 13:01:43.000000 tidytcells-1.8.5/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.986591 tidytcells-1.8.5/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-06-04 13:01:15.000000 tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-06-04 13:01:15.000000 tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.987591 tidytcells-1.8.5/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4921 2023-06-04 13:51:59.000000 tidytcells-1.8.5/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-06-04 13:01:37.000000 tidytcells-1.8.5/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_utils/gene_standardizers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.988592 tidytcells-1.8.5/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1607 2023-06-04 13:02:14.000000 tidytcells-1.8.5/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.988592 tidytcells-1.8.5/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3139 2023-06-04 13:52:39.000000 tidytcells-1.8.5/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.988592 tidytcells-1.8.5/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10549 2023-06-04 13:02:14.000000 tidytcells-1.8.5/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.989591 tidytcells-1.8.5/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8842 2023-06-04 13:02:14.000000 tidytcells-1.8.5/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.984591 tidytcells-1.8.5/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.990591 tidytcells-1.8.5/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1400 2023-06-04 13:52:56.000000 tidytcells-1.8.5/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2193 2023-06-04 13:53:42.000000 tidytcells-1.8.5/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9326 2023-06-04 13:02:14.000000 tidytcells-1.8.5/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8620 2023-06-04 13:02:14.000000 tidytcells-1.8.5/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.299523 tidytcells-1.8.6/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-12-06 13:03:03.000000 tidytcells-1.8.6/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-12-06 13:03:03.000000 tidytcells-1.8.6/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-07-04 15:19:24.299523 tidytcells-1.8.6/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-21 13:44:44.000000 tidytcells-1.8.6/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-07-04 15:11:39.000000 tidytcells-1.8.6/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-07-04 15:19:24.299523 tidytcells-1.8.6/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-21 13:44:44.000000 tidytcells-1.8.6/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.292523 tidytcells-1.8.6/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.293523 tidytcells-1.8.6/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-02 16:02:49.000000 tidytcells-1.8.6/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.296523 tidytcells-1.8.6/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-07-04 15:09:36.000000 tidytcells-1.8.6/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.297523 tidytcells-1.8.6/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-02 13:53:55.000000 tidytcells-1.8.6/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4921 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3083 2023-07-04 15:01:37.000000 tidytcells-1.8.6/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/_utils/gene_standardizers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.297523 tidytcells-1.8.6/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1596 2023-07-04 14:57:09.000000 tidytcells-1.8.6/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.297523 tidytcells-1.8.6/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3156 2023-07-04 14:57:09.000000 tidytcells-1.8.6/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.298523 tidytcells-1.8.6/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      692 2023-07-04 14:57:09.000000 tidytcells-1.8.6/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10708 2023-07-04 14:57:09.000000 tidytcells-1.8.6/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.298523 tidytcells-1.8.6/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-21 13:44:44.000000 tidytcells-1.8.6/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8913 2023-07-04 14:57:09.000000 tidytcells-1.8.6/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.293523 tidytcells-1.8.6/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-07-04 15:19:24.000000 tidytcells-1.8.6/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-07-04 15:19:24.000000 tidytcells-1.8.6/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-07-04 15:19:24.000000 tidytcells-1.8.6/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-07-04 15:19:24.000000 tidytcells-1.8.6/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-07-04 15:19:24.000000 tidytcells-1.8.6/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-07-04 15:19:24.298523 tidytcells-1.8.6/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1400 2023-06-21 13:44:44.000000 tidytcells-1.8.6/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2193 2023-06-21 13:44:44.000000 tidytcells-1.8.6/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9326 2023-06-21 13:44:44.000000 tidytcells-1.8.6/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8687 2023-07-04 15:04:16.000000 tidytcells-1.8.6/tests/test_tcr.py
```

### Comparing `tidytcells-1.8.5/LICENSE.txt` & `tidytcells-1.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/PKG-INFO` & `tidytcells-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.5
+Version: 1.8.6
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.5/README.md` & `tidytcells-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/setup.py` & `tidytcells-1.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/__init__.py` & `tidytcells-1.8.6/src/tidytcells/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json` & `tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.6/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.6/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.6/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.6/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.6/src/tidytcells/_utils/abstract_functions.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.6/src/tidytcells/_utils/gene_query_engines.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     functionality == "any"
                     or (
                         functionality in ("F", "P", "ORF")
                         and functionality in cls.ref_dict[gene].values()
                     )
                     or (
                         functionality == "NF"
-                        and {"P", "ORF"}.intersection(cls.ref_dict[gene].values)
+                        and {"P", "ORF"}.intersection(cls.ref_dict[gene].values())
                     )
                 ):
                     tcrs.append(gene)
 
                 continue
 
             for d in cls.ref_dict[gene]:
```

### Comparing `tidytcells-1.8.5/src/tidytcells/_utils/gene_standardizers.py` & `tidytcells-1.8.6/src/tidytcells/_utils/gene_standardizers.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/src/tidytcells/aa/_main.py` & `tidytcells-1.8.6/src/tidytcells/aa/_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         bool
 
     :return:
         Capitalised version of ``seq``, if seq is a valid amino acid sequence.
-        Otherwise the input is rejected and ``None`` is returned.
+        Otherwise follow behaviour set by ``on_fail``.
     :rtype:
         Union[str, None]
 
     .. topic:: Example usage
 
         Strings that look like amino acid sequences will be accepted, and returned in capitalised form.
```

### Comparing `tidytcells-1.8.5/src/tidytcells/junction/_main.py` & `tidytcells-1.8.6/src/tidytcells/junction/_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         bool
 
     :return:
         If possible, a standardized version of the input string is returned.
-        If the input string cannot be standardized, it is rejected and ``None`` is returned.
+        If the input string cannot be standardized, the function follows the behaviour as set by ``on_fail``.
     :rtype:
         Union[str, None]
 
     .. topic:: Example usage
 
         Strings that look like junction sequences will be accepted, and returned in capitalised form.
```

### Comparing `tidytcells-1.8.5/src/tidytcells/mhc/__init__.py` & `tidytcells-1.8.6/src/tidytcells/mhc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     Alias for :py:func:`tidytcells.mhc.standardize`.
     """
     return standardize(*args, **kwargs)
 
 
 def classify(*args, **kwargs):
     """
-    Alias for :py:func:`tidytcells.mhc.get_class`. This will be deprecated soon.
+    .. caution:: This will be deprecated soon in favour of :py:func:`tidytcells.mhc.get_class`.
+
+    Alias for :py:func:`tidytcells.mhc.get_class`.
     """
     _warn(
         '"mhc.classify" as an alias will be deprecated in the near future. Please switch to using "mhc.get_class".',
         FutureWarning,
     )
     return get_class(*args, **kwargs)
```

### Comparing `tidytcells-1.8.5/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.6/src/tidytcells/mhc/_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,24 @@
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         bool
 
     :param gene_name:
-        Alias for the parameter ``gene``. This will be deprecated soon.
+        Alias for the parameter ``gene``.
+
+        .. caution:: This will be deprecated soon in favour of ``gene``.
     :type gene_name:
         str
 
     :return:
         If the specified ``species`` is supported, and ``gene`` could be standardized, then return the standardized gene name.
         If ``species`` is unsupported, then the function does not attempt to standardize, and returns the unaltered ``gene`` string.
-        Else returns ``None``.
+        Else follows the behvaiour as set by ``on_fail``.
     :rtype:
         Union[str, None]
 
     .. topic:: Example usage
 
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
@@ -218,15 +220,17 @@
     :param suppress_warnings:
         Disable warnings that are usually emitted when chain classification fails.
         Defaults to ``False``.
     :type suppress_warnings:
         bool
 
     :param gene_name:
-        Alias for the parameter ``gene``. This will be deprecated soon.
+        Alias for the parameter ``gene``.
+
+        .. caution:: This will be deprecated soon in favour of ``gene``.
     :type gene_name:
         str
 
     :return:
         ``'alpha'`` or ``'beta'`` if ``gene`` is recognised and its chain is known, else ``None``.
     :rtype:
         Union[str, None]
@@ -290,15 +294,17 @@
     :param suppress_warnings:
         Disable warnings that are usually emitted when classification fails.
         Defaults to ``False``.
     :type suppress_warnings:
         bool
 
     :param gene_name:
-        Alias for the parameter ``gene``. This will be deprecated soon.
+        Alias for the parameter ``gene``.
+
+        .. caution:: This will be deprecated soon in favour of ``gene``.
     :type gene_name:
         str
 
     :return:
         ``1`` or ``2`` if ``gene`` is recognised and its class is known, else ``None``.
     :rtype:
         Union[int, None]
```

### Comparing `tidytcells-1.8.5/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.6/src/tidytcells/tcr/_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,24 @@
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
         bool
 
     :param gene_name:
-        Alias for the parameter ``gene``. This will be deprecated soon.
+        Alias for the parameter ``gene``.
+
+        .. caution:: This will be deprecated soon in favour of ``gene``.
     :type gene_name:
         str
 
     :return:
         If the specified ``species`` is supported, and ``gene`` could be standardized, then return the standardized gene name.
         If ``species`` is unsupported, then the function does not attempt to standardize , and returns the unaltered ``gene`` string.
-        Else returns ``None``.
+        Else follows the behaviour as set by ``on_fail``.
     :rtype:
         Union[str, None]
 
     .. topic:: Example usage
 
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
```

### Comparing `tidytcells-1.8.5/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.6/src/tidytcells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.5
+Version: 1.8.6
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.5/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.6/src/tidytcells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/tests/test_aa.py` & `tidytcells-1.8.6/tests/test_aa.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/tests/test_junction.py` & `tidytcells-1.8.6/tests/test_junction.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/tests/test_mhc.py` & `tidytcells-1.8.6/tests/test_mhc.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.5/tests/test_tcr.py` & `tidytcells-1.8.6/tests/test_tcr.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
             "expected_len",
             "expected_in",
             "expected_not_in",
         ),
         (
             ("homosapiens", "gene", "F", 186, "TRBJ2-7", "TRBV12-2"),
             ("homosapiens", "allele", "NF", 105, "TRAV35*03", "TRAV35*01"),
+            ("homosapiens", "gene", "NF", 74, "TRAV35", "TRAJ30"),
             ("musmusculus", "gene", "P", 59, "TRGC3", "TRDV5"),
             ("musmusculus", "allele", "ORF", 24, "TRBV24*03", "TRBV24*01"),
         ),
     )
     def test_query_functionality(
         self,
         species,
```

