# Comparing `tmp/bstk_datatables-0.1.5.tar.gz` & `tmp/bstk_datatables-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.1.5.tar", max compression
+gzip compressed data, was "bstk_datatables-0.1.6.tar", max compression
```

## Comparing `bstk_datatables-0.1.5.tar` & `bstk_datatables-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4244 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/README.md
--rw-r--r--   0        0        0     2319 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3248 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/merge.py
--rw-r--r--   0        0        0     6968 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-05-23 02:17:01.871551 bstk_datatables-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/README.md
+-rw-r--r--   0        0        0     2358 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3248 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     6968 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/table.py
+-rw-r--r--   0        0        0      669 2023-07-04 06:49:21.782220 bstk_datatables-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.6/PKG-INFO
```

### Comparing `bstk_datatables-0.1.5/README.md` & `bstk_datatables-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.5/bstk_datatables/__init__.py` & `bstk_datatables-0.1.6/bstk_datatables/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "email": marshmallow_fields.Email,
     "enum": marshmallow_fields.Enum,
     "ip": marshmallow_fields.IPInterface,
     "mac_address": marshmallow_fields.String,
     "number": marshmallow_fields.Number,
     "phone": marshmallow_fields.String,
     "text": marshmallow_fields.String,
+    "blob": marshmallow_fields.String,
     "url": marshmallow_fields.Url,
 }
 
 """
 Any "default" params that should be injected into the marshmallow field constructor
 """
 SCHEMAFIELD_EXTATTR: typing.Dict[
```

### Comparing `bstk_datatables-0.1.5/bstk_datatables/entry.py` & `bstk_datatables-0.1.6/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.5/bstk_datatables/enum.py` & `bstk_datatables-0.1.6/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.5/bstk_datatables/merge.py` & `bstk_datatables-0.1.6/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.5/bstk_datatables/schema.py` & `bstk_datatables-0.1.6/bstk_datatables/schema.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.5/bstk_datatables/table.py` & `bstk_datatables-0.1.6/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.5/pyproject.toml` & `bstk_datatables-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.1.5"
+version = "0.1.6"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.1.5/PKG-INFO` & `bstk_datatables-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.1.5
+Version: 0.1.6
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

