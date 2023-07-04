# Comparing `tmp/iformat-0.0.3.tar.gz` & `tmp/iformat-0.0.4.tar.gz`

## Comparing `iformat-0.0.3.tar` & `iformat-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.0.3/setup.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 iformat-0.0.3/src/iformat/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.0.3/.gitignore
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.0.3/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 iformat-0.0.3/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 iformat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.0.4/setup.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 iformat-0.0.4/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.0.4/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 iformat-0.0.4/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 iformat-0.0.4/PKG-INFO
```

### Comparing `iformat-0.0.3/src/iformat/__init__.py` & `iformat-0.0.4/src/iformat/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,12 @@
-""" # iformat
+"""iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
 
-iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
+https://github.com/FinnE145/iprint
 
-## Parameters:
-**`indentDepth`:** *(`iprint` and `iformat`)*\
-Specifies how many spaces should be inserted as one indent level. Default `4`.
-
-**`expansionThreshold`**: *(`iprint` and `iformat`)*\
-Specifies how long an object must be when printed before it is shown in a muilti-line format. Default `10`.\
-Ex:
-```py
-iprint([1, 2, 3], expansionThreshold = 10)
-# [1, 2, 3]
-
-iprint([1, 2, 3], expansionThreshold = 8)
-# [
-#   1,
-#   2,
-#   3
-# ]
-```
-
-**`indentLevel`:** *(`iformat` only)*\
-Specifies the indent level of the returned output string. Default `0`. """
+https://pypi.org/project/iformat"""
 
 
 # Copyright (C) 2023  Finn Emmerson
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published
 # by the Free Software Foundation, either version 3 of the License, or
```

### Comparing `iformat-0.0.3/.gitignore` & `iformat-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `iformat-0.0.3/LICENSE` & `iformat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.0.3/README.md` & `iformat-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,7 +19,10 @@
 #   2,
 #   3
 # ]
 ```
 
 **`indentLevel`:** *(`iformat` only)*\
 Specifies the indent level of the returned output string. Default `0`.
+
+https://github.com/FinnE145/iprint
+https://pypi.org/project/iformat
```

### Comparing `iformat-0.0.3/pyproject.toml` & `iformat-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Provides a function that indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.0.3/PKG-INFO` & `iformat-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides a function that indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -33,7 +33,10 @@
 #   2,
 #   3
 # ]
 ```
 
 **`indentLevel`:** *(`iformat` only)*\
 Specifies the indent level of the returned output string. Default `0`.
+
+https://github.com/FinnE145/iprint
+https://pypi.org/project/iformat
```

