# Comparing `tmp/iformat-0.0.1.tar.gz` & `tmp/iformat-0.0.2.tar.gz`

## Comparing `iformat-0.0.1.tar` & `iformat-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.0.1/setup.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 iformat-0.0.1/src/iprint/__init__.py
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.0.1/LICENSE
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 iformat-0.0.1/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 iformat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.0.2/setup.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 iformat-0.0.2/src/iformat/__init__.py
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 iformat-0.0.2/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 iformat-0.0.2/PKG-INFO
```

### Comparing `iformat-0.0.1/src/iprint/__init__.py` & `iformat-0.0.2/src/iformat/__init__.py`

 * *Files identical despite different names*

### Comparing `iformat-0.0.1/LICENSE` & `iformat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.0.1/README.md` & `iformat-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# iprint
+# iformat
 
-iprint is a simple package that prints basic data structures in an indented and readable way. It supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
+iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
 
 ## Parameters:
-**`indentDepth`:**\
+**`indentDepth`:** *(`iprint` and `iformat`)*\
 Specifies how many spaces should be inserted as one indent level. Default `4`.
 
-**`expansionThreshold`**:\
+**`expansionThreshold`**: *(`iprint` and `iformat`)*\
 Specifies how long an object must be when printed before it is shown in a muilti-line format. Default `10`.\
 Ex:
 ```py
 iprint([1, 2, 3], expansionThreshold = 10)
 # [1, 2, 3]
 
 iprint([1, 2, 3], expansionThreshold = 8)
@@ -18,8 +18,8 @@
 #   1,
 #   2,
 #   3
 # ]
 ```
 
 **`indentLevel`:** *(`iformat` only)*\
-Specifies the indent level of the returned output string. Default `0`.
+Specifies the indent level of the returned output string. Default `0`.
```

### Comparing `iformat-0.0.1/pyproject.toml` & `iformat-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Provides a function that indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.0.1/PKG-INFO` & `iformat-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provides a function that indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# iprint
+# iformat
 
-iprint is a simple package that prints basic data structures in an indented and readable way. It supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
+iformat is a simple package that prints basic data structures in an indented and readable way. The main `iprint` function supports changing the indent size and expansion threshold, as well as all vanilla `print` arguments. The included `iformat` function provides more customization, and returns a string that has been indented and formatted. An `.iformat` method (returning a string) can be added to any class for that class to be printed with custom formatting.
 
 ## Parameters:
-**`indentDepth`:**\
+**`indentDepth`:** *(`iprint` and `iformat`)*\
 Specifies how many spaces should be inserted as one indent level. Default `4`.
 
-**`expansionThreshold`**:\
+**`expansionThreshold`**: *(`iprint` and `iformat`)*\
 Specifies how long an object must be when printed before it is shown in a muilti-line format. Default `10`.\
 Ex:
 ```py
 iprint([1, 2, 3], expansionThreshold = 10)
 # [1, 2, 3]
 
 iprint([1, 2, 3], expansionThreshold = 8)
@@ -32,8 +32,8 @@
 #   1,
 #   2,
 #   3
 # ]
 ```
 
 **`indentLevel`:** *(`iformat` only)*\
-Specifies the indent level of the returned output string. Default `0`.
+Specifies the indent level of the returned output string. Default `0`.
```

