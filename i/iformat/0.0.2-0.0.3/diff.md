# Comparing `tmp/iformat-0.0.2.tar.gz` & `tmp/iformat-0.0.3.tar.gz`

## Comparing `iformat-0.0.2.tar` & `iformat-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.0.2/setup.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 iformat-0.0.2/src/iformat/__init__.py
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.0.2/LICENSE
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 iformat-0.0.2/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 iformat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.0.3/setup.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 iformat-0.0.3/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.0.3/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 iformat-0.0.3/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 iformat-0.0.3/PKG-INFO
```

### Comparing `iformat-0.0.2/LICENSE` & `iformat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.0.2/README.md` & `iformat-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iformat-0.0.2/pyproject.toml` & `iformat-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Provides a function that indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.0.2/PKG-INFO` & `iformat-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides a function that indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

