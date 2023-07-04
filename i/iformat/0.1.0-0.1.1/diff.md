# Comparing `tmp/iformat-0.1.0.tar.gz` & `tmp/iformat-0.1.1.tar.gz`

## Comparing `iformat-0.1.0.tar` & `iformat-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.1.0/setup.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 iformat-0.1.0/src/iformat/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.1.0/.gitignore
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.1.0/LICENSE
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 iformat-0.1.0/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 iformat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 iformat-0.1.1/setup.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 iformat-0.1.1/src/iformat/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 iformat-0.1.1/.gitignore
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 iformat-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 iformat-0.1.1/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 iformat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 iformat-0.1.1/PKG-INFO
```

### Comparing `iformat-0.1.0/src/iformat/__init__.py` & `iformat-0.1.1/src/iformat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 def _brackets(datatype, newline = False, indentAmount = 0):
     return [("[" if datatype == list else "(" if datatype == tuple else "{" if datatype in [set, dict] else "") + ("\n" if datatype in _iters and newline else "") + (" " * indentAmount), ("\n" if datatype in _iters and newline else "") + (" " * indentAmount) + ("]" if datatype == list else ")" if datatype == tuple else "}" if datatype in [set, dict] else "")]
 
 def _indent(indentLevel, indentDepth):
     return " " * (indentLevel * indentDepth)
 
-def iformat(i, indentLevel = 0, indentDepth = 4, expansionThreshold = 10):
+def iformat(i, indentLevel = 0, indentDepth = 4, expansionThreshold = 0):
     il, id, et = indentLevel, indentDepth, expansionThreshold
     length = _length(i)
     if type(i) in _iters:
         return (_brackets(type(i), True if length > et else False, ((il + 1) * id) if length > et else False)[0]\
             + ((",\n" + _indent(il + 1, id)) if length > et else (", ")).join(\
                     [f"{iformat(k, il + 1, id, et)}: {iformat(v, il + 1, id, et)}" for k, v in i.items()]\
                 if type(i) == dict else\
@@ -49,9 +49,9 @@
             if "iformat" in dir(i):
                 return i.iformat(il, id, et)
             else:
                 return (f"{i.__class__.__name__}({', '.join([f'{k} = {iformat(v, il, id, et)}' for k, v in i.__dict__.items()])})")
         else:
             return str(i)
 
-def iprint(*args, indentDepth = 4, expansionThreshold = 10, sep = " ", end = "\n", file = None, flush = False):
+def iprint(*args, indentDepth = 4, expansionThreshold = 0, sep = " ", end = "\n", file = None, flush = False):
     print(*[iformat(x, 0, indentDepth, expansionThreshold = expansionThreshold) for x in args], sep = sep, end = end, file = file, flush = flush)
```

### Comparing `iformat-0.1.0/.gitignore` & `iformat-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `iformat-0.1.0/LICENSE` & `iformat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iformat-0.1.0/README.md` & `iformat-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iformat-0.1.0/pyproject.toml` & `iformat-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iformat"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Finn Emmerson", email="finne014@gmail.com" },
 ]
 description = "Provides a function that indents and pretty prints data structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iformat-0.1.0/PKG-INFO` & `iformat-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iformat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provides a function that indents and pretty prints data structures
 Project-URL: Homepage, https://github.com/FinnE145/iprint
 Project-URL: Bug Tracker, https://github.com/FinnE145/iprint/issues
 Author-email: Finn Emmerson <finne014@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

