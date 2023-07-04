# Comparing `tmp/sccd45ra-0.2.1.tar.gz` & `tmp/sccd45ra-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccd45ra-0.2.1.tar", last modified: Tue Jul  4 00:53:10 2023, max compression
+gzip compressed data, was "sccd45ra-0.3.tar", last modified: Tue Jul  4 00:56:06 2023, max compression
```

## Comparing `sccd45ra-0.2.1.tar` & `sccd45ra-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:10.454066 sccd45ra-0.2.1/
--rw-rw-rw-   0        0        0       55 2023-07-04 00:53:10.454066 sccd45ra-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:10.443098 sccd45ra-0.2.1/sccd45ra/
--rw-rw-rw-   0        0        0       38 2023-05-22 18:45:19.000000 sccd45ra-0.2.1/sccd45ra/__init__.py
--rw-rw-rw-   0        0        0     1038 2023-05-22 19:24:57.000000 sccd45ra-0.2.1/sccd45ra/cd45ra_infer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:10.448083 sccd45ra-0.2.1/sccd45ra/feature/
--rw-rw-rw-   0        0        0   148483 2023-07-04 00:50:28.000000 sccd45ra-0.2.1/sccd45ra/feature/Supplement Tables.xlsx
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:10.451075 sccd45ra-0.2.1/sccd45ra/model/
--rw-rw-rw-   0        0        0  1823659 2023-07-04 00:50:50.000000 sccd45ra-0.2.1/sccd45ra/model/best_rbf_svm.joblib
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:10.447057 sccd45ra-0.2.1/sccd45ra.egg-info/
--rw-rw-rw-   0        0        0       55 2023-07-04 00:53:10.000000 sccd45ra-0.2.1/sccd45ra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-07-04 00:53:10.000000 sccd45ra-0.2.1/sccd45ra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:53:10.000000 sccd45ra-0.2.1/sccd45ra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-04 00:53:10.000000 sccd45ra-0.2.1/sccd45ra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 00:53:10.000000 sccd45ra-0.2.1/sccd45ra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 00:53:10.454066 sccd45ra-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      314 2023-07-04 00:53:00.000000 sccd45ra-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.751240 sccd45ra-0.3/
+-rw-rw-rw-   0        0        0       53 2023-07-04 00:56:06.751240 sccd45ra-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.740619 sccd45ra-0.3/sccd45ra/
+-rw-rw-rw-   0        0        0       38 2023-05-22 18:45:19.000000 sccd45ra-0.3/sccd45ra/__init__.py
+-rw-rw-rw-   0        0        0     1038 2023-05-22 19:24:57.000000 sccd45ra-0.3/sccd45ra/cd45ra_infer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.746224 sccd45ra-0.3/sccd45ra/feature/
+-rw-rw-rw-   0        0        0   148483 2023-07-04 00:50:28.000000 sccd45ra-0.3/sccd45ra/feature/Supplement Tables.xlsx
+drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.748223 sccd45ra-0.3/sccd45ra/model/
+-rw-rw-rw-   0        0        0  1823659 2023-07-04 00:50:50.000000 sccd45ra-0.3/sccd45ra/model/best_rbf_svm.joblib
+drwxrwxrwx   0        0        0        0 2023-07-04 00:56:06.745255 sccd45ra-0.3/sccd45ra.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 00:56:06.000000 sccd45ra-0.3/sccd45ra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 00:56:06.751240 sccd45ra-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-07-04 00:55:46.000000 sccd45ra-0.3/setup.py
```

### Comparing `sccd45ra-0.2.1/sccd45ra/cd45ra_infer.py` & `sccd45ra-0.3/sccd45ra/cd45ra_infer.py`

 * *Files identical despite different names*

### Comparing `sccd45ra-0.2.1/sccd45ra/feature/Supplement Tables.xlsx` & `sccd45ra-0.3/sccd45ra/feature/Supplement Tables.xlsx`

 * *Files identical despite different names*

### Comparing `sccd45ra-0.2.1/sccd45ra/model/best_rbf_svm.joblib` & `sccd45ra-0.3/sccd45ra/model/best_rbf_svm.joblib`

 * *Files identical despite different names*

