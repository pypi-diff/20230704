# Comparing `tmp/sccd45ra-0.1.tar.gz` & `tmp/sccd45ra-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sccd45ra-0.1.tar", last modified: Mon May 22 19:28:24 2023, max compression
+gzip compressed data, was "sccd45ra-0.2.tar", last modified: Tue Jul  4 00:31:37 2023, max compression
```

## Comparing `sccd45ra-0.1.tar` & `sccd45ra-0.2.tar`

### file list

```diff
@@ -1,18 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:28:24.845417 sccd45ra-0.1/
--rw-rw-rw-   0        0        0       53 2023-05-22 19:28:24.844962 sccd45ra-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-22 18:45:48.000000 sccd45ra-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 19:28:24.834172 sccd45ra-0.1/sccd45ra/
--rw-rw-rw-   0        0        0       38 2023-05-22 18:45:19.000000 sccd45ra-0.1/sccd45ra/__init__.py
--rw-rw-rw-   0        0        0     1038 2023-05-22 19:24:57.000000 sccd45ra-0.1/sccd45ra/cd45ra_infer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:28:24.840069 sccd45ra-0.1/sccd45ra/feature/
--rw-rw-rw-   0        0        0   148483 2023-05-05 17:32:21.000000 sccd45ra-0.1/sccd45ra/feature/Supplement Tables.xlsx
-drwxrwxrwx   0        0        0        0 2023-05-22 19:28:24.841969 sccd45ra-0.1/sccd45ra/model/
--rw-rw-rw-   0        0        0  1823659 2023-04-27 07:52:39.000000 sccd45ra-0.1/sccd45ra/model/best_rbf_svm.joblib
-drwxrwxrwx   0        0        0        0 2023-05-22 19:28:24.839072 sccd45ra-0.1/sccd45ra.egg-info/
--rw-rw-rw-   0        0        0       53 2023-05-22 19:28:24.000000 sccd45ra-0.1/sccd45ra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-22 19:28:24.000000 sccd45ra-0.1/sccd45ra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:28:24.000000 sccd45ra-0.1/sccd45ra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-05-22 19:28:24.000000 sccd45ra-0.1/sccd45ra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 19:28:24.000000 sccd45ra-0.1/sccd45ra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 19:28:24.845417 sccd45ra-0.1/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-05-22 19:12:17.000000 sccd45ra-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:31:37.060912 sccd45ra-0.2/
+-rw-rw-rw-   0        0        0       53 2023-07-04 00:31:36.983059 sccd45ra-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 00:31:36.978073 sccd45ra-0.2/sccd45ra/
+-rw-rw-rw-   0        0        0       38 2023-05-22 18:45:19.000000 sccd45ra-0.2/sccd45ra/__init__.py
+-rw-rw-rw-   0        0        0     1038 2023-05-22 19:24:57.000000 sccd45ra-0.2/sccd45ra/cd45ra_infer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:31:36.982062 sccd45ra-0.2/sccd45ra.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-07-04 00:31:36.000000 sccd45ra-0.2/sccd45ra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-07-04 00:31:36.000000 sccd45ra-0.2/sccd45ra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:31:36.000000 sccd45ra-0.2/sccd45ra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-04 00:31:36.000000 sccd45ra-0.2/sccd45ra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 00:31:36.000000 sccd45ra-0.2/sccd45ra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 00:31:37.060912 sccd45ra-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-07-04 00:31:30.000000 sccd45ra-0.2/setup.py
```

### Comparing `sccd45ra-0.1/sccd45ra/cd45ra_infer.py` & `sccd45ra-0.2/sccd45ra/cd45ra_infer.py`

 * *Files identical despite different names*

