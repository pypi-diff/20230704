# Comparing `tmp/AlphaPeel-1.1.1.tar.gz` & `tmp/AlphaPeel-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlphaPeel-1.1.1.tar", last modified: Thu Jun 29 11:43:00 2023, max compression
+gzip compressed data, was "AlphaPeel-1.1.2.tar", last modified: Tue Jul  4 09:44:40 2023, max compression
```

## Comparing `AlphaPeel-1.1.1.tar` & `AlphaPeel-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:43:00.577410 AlphaPeel-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/MIT_License.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-29 11:43:00.577410 AlphaPeel-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:43:00.577410 AlphaPeel-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:43:00.573409 AlphaPeel-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:43:00.573409 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-29 11:43:00.000000 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-29 11:43:00.000000 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:43:00.000000 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 11:43:00.000000 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 11:43:00.000000 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 11:43:00.000000 AlphaPeel-1.1.1/src/AlphaPeel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:43:00.573409 AlphaPeel-1.1.1/src/tinypeel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:43:00.577410 AlphaPeel-1.1.1/src/tinypeel/Peeling/
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/src/tinypeel/Peeling/Peeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/src/tinypeel/Peeling/PeelingIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/src/tinypeel/Peeling/PeelingInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/src/tinypeel/Peeling/PeelingUpdates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-06-29 11:42:48.000000 AlphaPeel-1.1.1/src/tinypeel/tinypeel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:44:40.248363 AlphaPeel-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/MIT_License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-04 09:44:40.248363 AlphaPeel-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:44:40.248363 AlphaPeel-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:44:40.236363 AlphaPeel-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:44:40.240363 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-04 09:44:40.000000 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-04 09:44:40.000000 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:44:40.000000 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 09:44:40.000000 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 09:44:40.000000 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 09:44:40.000000 AlphaPeel-1.1.2/src/AlphaPeel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:44:40.240363 AlphaPeel-1.1.2/src/tinypeel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:44:40.244363 AlphaPeel-1.1.2/src/tinypeel/Peeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/src/tinypeel/Peeling/Peeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/src/tinypeel/Peeling/PeelingIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/src/tinypeel/Peeling/PeelingInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/src/tinypeel/Peeling/PeelingUpdates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:44:40.248363 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/BurrowsWheelerLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27139 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/CombinedHMM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/DiploidHMM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/HaploidHMM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16124 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/HaplotypeLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/HaplotypeOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/InputOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/MultiThreadIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/NumbaUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38012 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/Pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/ProbMath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 09:44:29.000000 AlphaPeel-1.1.2/src/tinypeel/tinyhouse/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-04 09:44:22.000000 AlphaPeel-1.1.2/src/tinypeel/tinypeel.py
```

### Comparing `AlphaPeel-1.1.1/MIT_License.txt` & `AlphaPeel-1.1.2/MIT_License.txt`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/PKG-INFO` & `AlphaPeel-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlphaPeel
-Version: 1.1.1
+Version: 1.1.2
 Summary: Multilocus and hybrid peeling
 Author: Andrew Whalen
 Author-email: Andrew Whalen <awhalen@roslin.ed.ac.uk>
 License: Copyright (C) 2020 University of Edinburgh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AlphaPeel Version: 1.1.1 Summary: Multilocus and
+Metadata-Version: 2.1 Name: AlphaPeel Version: 1.1.2 Summary: Multilocus and
 hybrid peeling Author: Andrew Whalen Author-email: Andrew Whalen
 roslin.ed.ac.uk> License: Copyright (C) 2020 University of Edinburgh Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `AlphaPeel-1.1.1/README.md` & `AlphaPeel-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/pyproject.toml` & `AlphaPeel-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AlphaPeel"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Andrew Whalen", email="awhalen@roslin.ed.ac.uk" },
 ]
 description = "Multilocus and hybrid peeling"
 # readme corresponds to the long_description
 # "*.md" specifies the long_description_content_type
 readme = "README.md"
@@ -29,8 +29,8 @@
 
 [project.urls]
 "Homepage" = "https://github.com/AlphaGenes/AlphaPeel"
 "Bug Tracker" = "https://github.com/AlphaGenes/AlphaPeel/issues"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
-packages = ["tinypeel", "tinypeel.Peeling"]
+packages = ["tinypeel", "tinypeel.tinyhouse", "tinypeel.Peeling"]
```

### Comparing `AlphaPeel-1.1.1/setup.py` & `AlphaPeel-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/src/AlphaPeel.egg-info/PKG-INFO` & `AlphaPeel-1.1.2/src/AlphaPeel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlphaPeel
-Version: 1.1.1
+Version: 1.1.2
 Summary: Multilocus and hybrid peeling
 Author: Andrew Whalen
 Author-email: Andrew Whalen <awhalen@roslin.ed.ac.uk>
 License: Copyright (C) 2020 University of Edinburgh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AlphaPeel Version: 1.1.1 Summary: Multilocus and
+Metadata-Version: 2.1 Name: AlphaPeel Version: 1.1.2 Summary: Multilocus and
 hybrid peeling Author: Andrew Whalen Author-email: Andrew Whalen
 roslin.ed.ac.uk> License: Copyright (C) 2020 University of Edinburgh Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `AlphaPeel-1.1.1/src/tinypeel/Peeling/Peeling.py` & `AlphaPeel-1.1.2/src/tinypeel/Peeling/Peeling.py`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/src/tinypeel/Peeling/PeelingIO.py` & `AlphaPeel-1.1.2/src/tinypeel/Peeling/PeelingIO.py`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/src/tinypeel/Peeling/PeelingInfo.py` & `AlphaPeel-1.1.2/src/tinypeel/Peeling/PeelingInfo.py`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/src/tinypeel/Peeling/PeelingUpdates.py` & `AlphaPeel-1.1.2/src/tinypeel/Peeling/PeelingUpdates.py`

 * *Files identical despite different names*

### Comparing `AlphaPeel-1.1.1/src/tinypeel/tinypeel.py` & `AlphaPeel-1.1.2/src/tinypeel/tinypeel.py`

 * *Files identical despite different names*

