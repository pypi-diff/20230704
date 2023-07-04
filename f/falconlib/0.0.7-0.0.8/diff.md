# Comparing `tmp/falconlib-0.0.7.tar.gz` & `tmp/falconlib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falconlib-0.0.7.tar", last modified: Sat Sep  3 18:35:32 2022, max compression
+gzip compressed data, was "falconlib-0.0.8.tar", last modified: Tue Jul  4 15:32:05 2023, max compression
```

## Comparing `falconlib-0.0.7.tar` & `falconlib-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-09-03 18:35:32.070230 falconlib-0.0.7/
--rw-rw-rw-   0        0        0     1344 2022-08-11 02:42:57.000000 falconlib-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       36 2022-08-13 04:28:04.000000 falconlib-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     9223 2022-09-03 18:35:32.068239 falconlib-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6866 2022-08-28 13:59:07.000000 falconlib-0.0.7/README.md
--rw-rw-rw-   0        0        0     1067 2022-09-03 18:34:36.000000 falconlib-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-03 18:35:32.071258 falconlib-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-03 18:35:31.973628 falconlib-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2022-09-03 18:35:32.007574 falconlib-0.0.7/src/falconlib/
--rw-rw-rw-   0        0        0       42 2022-08-13 20:26:03.000000 falconlib-0.0.7/src/falconlib/conftest.py
--rw-rw-rw-   0        0        0    15800 2022-09-03 18:34:03.000000 falconlib-0.0.7/src/falconlib/falconlib.py
-drwxrwxrwx   0        0        0        0 2022-09-03 18:35:32.061966 falconlib-0.0.7/src/falconlib/tests/
--rw-rw-rw-   0        0        0     6644 2022-08-21 00:33:21.000000 falconlib-0.0.7/src/falconlib/tests/gendoc.py
--rw-rw-rw-   0        0        0     7832 2022-09-03 18:34:19.000000 falconlib-0.0.7/src/falconlib/tests/test_010_lib.py
--rw-rw-rw-   0        0        0        0 2022-08-21 04:34:57.000000 falconlib-0.0.7/src/falconlib/x__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-03 18:35:32.056130 falconlib-0.0.7/src/falconlib.egg-info/
--rw-rw-rw-   0        0        0     9223 2022-09-03 18:35:31.000000 falconlib-0.0.7/src/falconlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-09-03 18:35:31.000000 falconlib-0.0.7/src/falconlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-03 18:35:31.000000 falconlib-0.0.7/src/falconlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-09-03 18:35:31.000000 falconlib-0.0.7/src/falconlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-03 18:35:31.000000 falconlib-0.0.7/src/falconlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.698062 falconlib-0.0.8/
+-rw-rw-rw-   0        0        0     1344 2022-10-29 19:56:38.000000 falconlib-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       36 2022-10-29 19:56:38.000000 falconlib-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     9223 2023-07-04 15:32:05.697062 falconlib-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6866 2022-10-29 19:56:38.000000 falconlib-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1067 2023-07-04 15:24:59.000000 falconlib-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 15:32:05.699062 falconlib-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.571890 falconlib-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.616210 falconlib-0.0.8/src/falconlib/
+-rw-rw-rw-   0        0        0       42 2022-10-29 19:56:38.000000 falconlib-0.0.8/src/falconlib/conftest.py
+-rw-rw-rw-   0        0        0    17166 2023-07-04 15:23:56.000000 falconlib-0.0.8/src/falconlib/falconlib.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.694065 falconlib-0.0.8/src/falconlib/tests/
+-rw-rw-rw-   0        0        0     6644 2022-10-29 19:56:38.000000 falconlib-0.0.8/src/falconlib/tests/gendoc.py
+-rw-rw-rw-   0        0        0     7831 2022-10-29 20:18:46.000000 falconlib-0.0.8/src/falconlib/tests/test_010_lib.py
+-rw-rw-rw-   0        0        0        0 2022-10-29 19:56:38.000000 falconlib-0.0.8/src/falconlib/x__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.660168 falconlib-0.0.8/src/falconlib.egg-info/
+-rw-rw-rw-   0        0        0     9223 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/top_level.txt
```

### Comparing `falconlib-0.0.7/LICENSE` & `falconlib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.7/PKG-INFO` & `falconlib-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falconlib
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client-side library for accessing the falconapi restful service.
 Author-email: "Thomas J. Daley, Esq." <tjd@powerdaley.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, Tom Daley
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: falconlib Version: 0.0.7 Summary: Client-side
+Metadata-Version: 2.1 Name: falconlib Version: 0.0.8 Summary: Client-side
 library for accessing the falconapi restful service. Author-email: "Thomas J.
 Daley, Esq."
 powerdaley.com> License: BSD 2-Clause License Copyright (c) 2022, Tom Daley All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

### Comparing `falconlib-0.0.7/README.md` & `falconlib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.7/pyproject.toml` & `falconlib-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "falconlib"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name="Thomas J. Daley, Esq.", email="tjd@powerdaley.com"},
 ]
 description = "Client-side library for accessing the falconapi restful service."
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">3.9"
```

### Comparing `falconlib-0.0.7/src/falconlib/falconlib.py` & `falconlib-0.0.8/src/falconlib/falconlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,46 @@
         """
         r = self.__get('/documents/props/?doc_id=' + document_id)
         self.last_response = r
         if r.status_code == 200:
             return _success(r.status_code, 'Extended document properties retrieved', r.json())
         return _error(r.status_code, 'Extended document properties retrieval failed', r.json())
     
+    def get_tracker_categories(self, tracker_id: str) -> FalconStatus:
+        """
+        GetTrackerCategories - Get categories for a tracker
+
+        Args:
+            tracker_id (str): Tracker to get categories for
+        
+        Returns:
+            (list): List of categories
+        """
+        r = self.__get(f'/trackers/{tracker_id}/categories')
+        self.last_response = r
+        if r.status_code == 200:
+            return _success(r.status_code, 'Categories retrieved', {'categories': r.json()})
+        return _error(r.status_code, 'Categories retrieval failed', r.json())
+    
+    def get_tracker_category_subcategory_pairs(self, tracker_id: str) -> FalconStatus:
+        """
+        GetTrackerCategorySubcategoryPairs - Get category/subcategory pairs for a tracker
+
+        Args:
+            tracker_id (str): Tracker to get category/subcategory pairs for
+        
+        Returns:
+            (list): List of category/subcategory pairs
+        """
+        r = self.__get(f'/trackers/{tracker_id}/category_subcategory_pairs')
+        self.last_response = r
+        if r.status_code == 200:
+            return _success(r.status_code, 'Category/subcategory pairs retrieved', {'category_subcategory_pairs': r.json()})
+        return _error(r.status_code, 'Category/subcategory pairs retrieval failed', r.json())
+    
     def get_documents(self, tracker_id: str) -> FalconStatus:
         """
         GetDocuments - Get all documents for a tracker.
 
         Args:
             tracker_id (str): Tracker to get documents for
```

### Comparing `falconlib-0.0.7/src/falconlib/tests/gendoc.py` & `falconlib-0.0.8/src/falconlib/tests/gendoc.py`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.7/src/falconlib/tests/test_010_lib.py` & `falconlib-0.0.8/src/falconlib/tests/test_010_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 import pytest
 import json
 import falconlib
 
 API_VERSION = '1_0'
 SERVER = 'http://localhost:8000'
-xSERVER = 'https://api.jdbot.us'
+SERVER = 'https://api.jdbot.us'
 PREFIX = f'/api/v{API_VERSION}'
 
 test_user = {
     'email': 'test_user@test.com',
     'username': 'test_user@test.com',
     'password': 'test_password',
     'full_name': 'Test User'
```

### Comparing `falconlib-0.0.7/src/falconlib.egg-info/PKG-INFO` & `falconlib-0.0.8/src/falconlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falconlib
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client-side library for accessing the falconapi restful service.
 Author-email: "Thomas J. Daley, Esq." <tjd@powerdaley.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, Tom Daley
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: falconlib Version: 0.0.7 Summary: Client-side
+Metadata-Version: 2.1 Name: falconlib Version: 0.0.8 Summary: Client-side
 library for accessing the falconapi restful service. Author-email: "Thomas J.
 Daley, Esq."
 powerdaley.com> License: BSD 2-Clause License Copyright (c) 2022, Tom Daley All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

