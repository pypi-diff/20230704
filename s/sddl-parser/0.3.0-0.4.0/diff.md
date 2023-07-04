# Comparing `tmp/sddl_parser-0.3.0.tar.gz` & `tmp/sddl_parser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddl_parser-0.3.0.tar", max compression
+gzip compressed data, was "sddl_parser-0.4.0.tar", max compression
```

## Comparing `sddl_parser-0.3.0.tar` & `sddl_parser-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      455 2023-06-30 23:54:30.580370 sddl_parser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3782 2023-06-30 23:55:19.526760 sddl_parser-0.3.0/README.md
--rw-r--r--   0        0        0       75 2023-06-30 20:12:20.818217 sddl_parser-0.3.0/sddl_parser/__init__.py
--rw-r--r--   0        0        0    50688 2023-06-30 17:28:00.851573 sddl_parser-0.3.0/sddl_parser/ace_rights_enums.py
--rw-r--r--   0        0        0     1526 2023-06-30 23:47:30.535387 sddl_parser-0.3.0/sddl_parser/api.py
--rw-r--r--   0        0        0     1257 2023-06-30 22:00:15.446960 sddl_parser-0.3.0/sddl_parser/enums.py
--rw-r--r--   0        0        0     5295 2023-06-30 23:27:33.678123 sddl_parser-0.3.0/sddl_parser/parser.py
--rw-r--r--   0        0        0     2845 2023-06-30 21:01:35.039016 sddl_parser-0.3.0/sddl_parser/sid_enum.py
--rw-r--r--   0        0        0     2647 2023-06-30 23:41:53.672836 sddl_parser-0.3.0/sddl_parser/types.py
--rw-r--r--   0        0        0     5410 2023-06-30 23:09:49.290197 sddl_parser-0.3.0/sddl_parser/well_known_dictionary.py
--rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 sddl_parser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      455 2023-07-04 16:43:56.109957 sddl_parser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4164 2023-07-04 16:44:19.894549 sddl_parser-0.4.0/README.md
+-rw-r--r--   0        0        0     1502 2023-07-04 16:43:29.936209 sddl_parser-0.4.0/sddl_parser/__init__.py
+-rw-r--r--   0        0        0    50688 2023-06-30 17:28:00.851573 sddl_parser-0.4.0/sddl_parser/ace_rights_enums.py
+-rw-r--r--   0        0        0     1526 2023-06-30 23:47:30.535387 sddl_parser-0.4.0/sddl_parser/api.py
+-rw-r--r--   0        0        0     1257 2023-06-30 22:00:15.446960 sddl_parser-0.4.0/sddl_parser/enums.py
+-rw-r--r--   0        0        0     5295 2023-06-30 23:27:33.678123 sddl_parser-0.4.0/sddl_parser/parser.py
+-rw-r--r--   0        0        0     2845 2023-06-30 21:01:35.039016 sddl_parser-0.4.0/sddl_parser/sid_enum.py
+-rw-r--r--   0        0        0     2647 2023-06-30 23:41:53.672836 sddl_parser-0.4.0/sddl_parser/types.py
+-rw-r--r--   0        0        0     5410 2023-06-30 23:09:49.290197 sddl_parser-0.4.0/sddl_parser/well_known_dictionary.py
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 sddl_parser-0.4.0/PKG-INFO
```

### Comparing `sddl_parser-0.3.0/README.md` & `sddl_parser-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -80,14 +80,29 @@
         FileAccessRights.FILE_GENERIC_READ,
     },
 )
 ```
 
 All rights are IntEnums, so if you want to check for generic rights, `FileAccessRights.DELETE` is equivalent to `GenericAccessRights.DELETE`
 
+If you want to map SIDs to strings, you can pass in `sidmap`:
+
+```py
+>>> from sddl_parser import api
+>>> test = "O:S-1-20-20-20G:SYD:"
+>>> sidmap = {"S-1-20-20-20": "DOMAIN\\user"}
+>>> api.parse_sddl(test, sidmap=sidmap)
+SDDL(
+    owner="DOMAIN\\user",
+    group=SIDEnum.LOCAL_SYSTEM,
+    dacl=ACL(flags={SDDLFlags.NO_ACCESS_CONTROL}, aces=[]),
+    sacl=None,
+)
+```
+
 # Access Rights Available
 
 All right enums are given here
 
 ```
 >> from sddl_parser import rights_enums
 >> for x in dir(rights_enums):
```

### Comparing `sddl_parser-0.3.0/sddl_parser/ace_rights_enums.py` & `sddl_parser-0.4.0/sddl_parser/ace_rights_enums.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/sddl_parser/api.py` & `sddl_parser-0.4.0/sddl_parser/api.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/sddl_parser/enums.py` & `sddl_parser-0.4.0/sddl_parser/enums.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/sddl_parser/parser.py` & `sddl_parser-0.4.0/sddl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/sddl_parser/sid_enum.py` & `sddl_parser-0.4.0/sddl_parser/sid_enum.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/sddl_parser/types.py` & `sddl_parser-0.4.0/sddl_parser/types.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/sddl_parser/well_known_dictionary.py` & `sddl_parser-0.4.0/sddl_parser/well_known_dictionary.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.3.0/PKG-INFO` & `sddl_parser-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sddl-parser
-Version: 0.3.0
+Version: 0.4.0
 Summary: Parse SDDL strings
 Author: Max Harley
 Author-email: maxh@maxh.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -93,14 +93,29 @@
         FileAccessRights.FILE_GENERIC_READ,
     },
 )
 ```
 
 All rights are IntEnums, so if you want to check for generic rights, `FileAccessRights.DELETE` is equivalent to `GenericAccessRights.DELETE`
 
+If you want to map SIDs to strings, you can pass in `sidmap`:
+
+```py
+>>> from sddl_parser import api
+>>> test = "O:S-1-20-20-20G:SYD:"
+>>> sidmap = {"S-1-20-20-20": "DOMAIN\\user"}
+>>> api.parse_sddl(test, sidmap=sidmap)
+SDDL(
+    owner="DOMAIN\\user",
+    group=SIDEnum.LOCAL_SYSTEM,
+    dacl=ACL(flags={SDDLFlags.NO_ACCESS_CONTROL}, aces=[]),
+    sacl=None,
+)
+```
+
 # Access Rights Available
 
 All right enums are given here
 
 ```
 >> from sddl_parser import rights_enums
 >> for x in dir(rights_enums):
```

