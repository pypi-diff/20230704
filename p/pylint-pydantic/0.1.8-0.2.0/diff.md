# Comparing `tmp/pylint_pydantic-0.1.8-py3-none-any.whl.zip` & `tmp/pylint_pydantic-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14860 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1864 b- defN 23-Mar-14 03:15 pylint_pydantic/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Mar-14 03:15 pylint_pydantic-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1770 b- defN 23-Mar-14 03:15 pylint_pydantic-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 03:15 pylint_pydantic-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-14 03:15 pylint_pydantic-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      511 b- defN 23-Mar-14 03:15 pylint_pydantic-0.1.8.dist-info/RECORD
-6 files, 39402 bytes uncompressed, 13930 bytes compressed:  64.6%
+Zip file size: 14910 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1857 b- defN 23-Jul-04 03:46 pylint_pydantic/__init__.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1833 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      511 b- defN 23-Jul-04 03:46 pylint_pydantic-0.2.0.dist-info/RECORD
+6 files, 39458 bytes uncompressed, 13980 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pylint_pydantic/__init__.py
 Comment: 
 
-Filename: pylint_pydantic-0.1.8.dist-info/LICENSE
+Filename: pylint_pydantic-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pylint_pydantic-0.1.8.dist-info/METADATA
+Filename: pylint_pydantic-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pylint_pydantic-0.1.8.dist-info/WHEEL
+Filename: pylint_pydantic-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pylint_pydantic-0.1.8.dist-info/top_level.txt
+Filename: pylint_pydantic-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pylint_pydantic-0.1.8.dist-info/RECORD
+Filename: pylint_pydantic-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylint_pydantic/__init__.py

```diff
@@ -1,34 +1,32 @@
 import astroid
 from astroid import (MANAGER, Attribute, Call, ClassDef, FunctionDef, Name, nodes)
 from pylint.checkers.design_analysis import MisdesignChecker
 from pylint_plugin_utils import suppress_message
 
+VALIDATOR_METHOD_NAMES = {"validator", "root_validator", "field_validator"}
+
 
 def is_validator_method(node: FunctionDef):
-    validator_method_names = {
-        "validator",
-        "root_validator",
-    }
 
     if not node.decorators:
         return False
 
     for decorator in node.decorators.get_children():
         # @validator(pre=True)
         if isinstance(decorator, Call):
             # transform to @validator case
             decorator = decorator.func
 
         # @validator
-        if (isinstance(decorator, Name) and decorator.name in validator_method_names):
+        if (isinstance(decorator, Name) and decorator.name in VALIDATOR_METHOD_NAMES):
             return True
 
         # @pydantic.validator
-        if (isinstance(decorator, Attribute) and decorator.attrname in validator_method_names):
+        if (isinstance(decorator, Attribute) and decorator.attrname in VALIDATOR_METHOD_NAMES):
             return True
 
     return False
 
 
 def transform(node: FunctionDef):
     if is_validator_method(node):
```

## Comparing `pylint_pydantic-0.1.8.dist-info/LICENSE` & `pylint_pydantic-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylint_pydantic-0.1.8.dist-info/METADATA` & `pylint_pydantic-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-pydantic
-Version: 0.1.8
+Version: 0.2.0
 Summary: A Pylint plugin to help Pylint understand the Pydantic
 Home-page: https://github.com/fcfangcc/pylint-pydantic
 Author: fcfangcc
 Author-email: swjfc22@163.com
 License: GPLv3
 Keywords: pylint,pydantic
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: pylint (<3.0,>2.0)
-Requires-Dist: pydantic (<2.0)
+Requires-Dist: pydantic (<3.0)
 Requires-Dist: pylint-plugin-utils
 
 pylint-pydantic
 ================
 A Pylint plugin to help Pylint understand the Pydantic
 
 How to use
@@ -61,8 +61,12 @@
 
 Other
 =====================
 If you have any questions, please create a issue.
 https://github.com/fcfangcc/pylint-pydantic/issues
 
 
+Changelog
+=====================
+- v0.2.0: support Pydantic V2
+
```

