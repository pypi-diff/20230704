# Comparing `tmp/IsoScore-1.0.tar.gz` & `tmp/IsoScore-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IsoScore-1.0.tar", last modified: Fri Jul 30 15:41:04 2021, max compression
+gzip compressed data, was "IsoScore-2.0.0.tar", last modified: Tue Jul  4 01:01:26 2023, max compression
```

## Comparing `IsoScore-1.0.tar` & `IsoScore-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2021-07-30 15:41:04.649607 IsoScore-1.0/
--rw-r--r--   0 nate       (501) staff       (20)     1116 2021-07-30 15:39:24.000000 IsoScore-1.0/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     1658 2021-07-30 15:41:04.649680 IsoScore-1.0/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1149 2021-07-30 15:39:28.000000 IsoScore-1.0/README.md
--rw-r--r--   0 nate       (501) staff       (20)      103 2021-07-30 15:39:26.000000 IsoScore-1.0/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)      592 2021-07-30 15:41:04.650023 IsoScore-1.0/setup.cfg
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2021-07-30 15:41:04.647995 IsoScore-1.0/src/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2021-07-30 15:41:04.649042 IsoScore-1.0/src/IsoScore/
--rw-rw-r--   0 nate       (501) staff       (20)     2439 2021-07-30 15:40:07.000000 IsoScore-1.0/src/IsoScore/IsoScore.py
--rw-r--r--   0 nate       (501) staff       (20)       96 2021-05-13 14:36:14.000000 IsoScore-1.0/src/IsoScore/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2021-07-30 15:41:04.649502 IsoScore-1.0/src/IsoScore.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     1658 2021-07-30 15:41:04.000000 IsoScore-1.0/src/IsoScore.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      236 2021-07-30 15:41:04.000000 IsoScore-1.0/src/IsoScore.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2021-07-30 15:41:04.000000 IsoScore-1.0/src/IsoScore.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        9 2021-07-30 15:41:04.000000 IsoScore-1.0/src/IsoScore.egg-info/top_level.txt
+drwxr-xr-x   0 wrudman    (502) staff       (20)        0 2023-07-04 01:01:26.729599 IsoScore-2.0.0/
+-rw-r--r--   0 wrudman    (502) staff       (20)     1116 2021-07-30 15:39:24.000000 IsoScore-2.0.0/LICENSE
+-rw-r--r--   0 wrudman    (502) staff       (20)     1490 2023-07-04 01:01:26.729646 IsoScore-2.0.0/PKG-INFO
+-rw-r--r--   0 wrudman    (502) staff       (20)      967 2023-07-04 00:56:28.000000 IsoScore-2.0.0/README.md
+-rw-r--r--   0 wrudman    (502) staff       (20)      103 2021-07-30 15:39:26.000000 IsoScore-2.0.0/pyproject.toml
+-rw-r--r--   0 wrudman    (502) staff       (20)      643 2023-07-04 01:01:26.729858 IsoScore-2.0.0/setup.cfg
+drwxr-xr-x   0 wrudman    (502) staff       (20)        0 2023-07-04 01:01:26.727878 IsoScore-2.0.0/src/
+drwxr-xr-x   0 wrudman    (502) staff       (20)        0 2023-07-04 01:01:26.728922 IsoScore-2.0.0/src/IsoScore/
+-rw-r--r--   0 wrudman    (502) staff       (20)     6755 2023-07-04 00:20:34.000000 IsoScore-2.0.0/src/IsoScore/IsoScore.py
+-rw-r--r--   0 wrudman    (502) staff       (20)       96 2021-05-13 14:36:14.000000 IsoScore-2.0.0/src/IsoScore/__init__.py
+drwxr-xr-x   0 wrudman    (502) staff       (20)        0 2023-07-04 01:01:26.729476 IsoScore-2.0.0/src/IsoScore.egg-info/
+-rw-r--r--   0 wrudman    (502) staff       (20)     1490 2023-07-04 01:01:26.000000 IsoScore-2.0.0/src/IsoScore.egg-info/PKG-INFO
+-rw-r--r--   0 wrudman    (502) staff       (20)      236 2023-07-04 01:01:26.000000 IsoScore-2.0.0/src/IsoScore.egg-info/SOURCES.txt
+-rw-r--r--   0 wrudman    (502) staff       (20)        1 2023-07-04 01:01:26.000000 IsoScore-2.0.0/src/IsoScore.egg-info/dependency_links.txt
+-rw-r--r--   0 wrudman    (502) staff       (20)        9 2023-07-04 01:01:26.000000 IsoScore-2.0.0/src/IsoScore.egg-info/top_level.txt
```

### Comparing `IsoScore-1.0/LICENSE` & `IsoScore-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IsoScore-1.0/setup.cfg` & `IsoScore-2.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = IsoScore
-version = 1.0
-author = Nate Gillman
-author_email = ngillman@brown.edu
-description = IsoScore measures uniformity of spatial utilization of point clouds
+version = 2.0.0
+author = William Rudman
+author_email = william_rudman@brown.edu
+description = IsoScore is the first tool available in the literature that accurately measures isotropy in embedding space.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bcbi-edu/p_eickhoff_isoscore
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

