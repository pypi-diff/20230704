# Comparing `tmp/angola-0.14.4.tar.gz` & `tmp/angola-0.14.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.14.4.tar", last modified: Fri Jun 30 07:41:44 2023, max compression
+gzip compressed data, was "angola-0.14.5.tar", last modified: Tue Jul  4 07:17:32 2023, max compression
```

## Comparing `angola-0.14.4.tar` & `angola-0.14.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.228037 angola-0.14.4/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.4/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.4/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-30 07:41:44.228109 angola-0.14.4/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.4/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-30 07:41:44.228364 angola-0.14.4/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      776 2023-06-30 07:41:36.000000 angola-0.14.4/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.222094 angola-0.14.4/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.225587 angola-0.14.4/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.4/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    51001 2023-06-28 16:10:18.000000 angola-0.14.4/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.4/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.4/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    18673 2023-06-30 07:41:24.000000 angola-0.14.4/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.4/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.226748 angola-0.14.4/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       47 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.227937 angola-0.14.4/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.4/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.4/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.4/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.14.4/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.4/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.035042 angola-0.14.5/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.5/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.5/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-07-04 07:17:32.035113 angola-0.14.5/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.5/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-07-04 07:17:32.035376 angola-0.14.5/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      776 2023-07-04 07:17:19.000000 angola-0.14.5/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.027635 angola-0.14.5/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.031650 angola-0.14.5/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.5/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    51001 2023-06-28 16:10:18.000000 angola-0.14.5/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.5/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.5/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18643 2023-07-04 07:17:12.000000 angola-0.14.5/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.5/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.033099 angola-0.14.5/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       47 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-07-04 07:17:32.000000 angola-0.14.5/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-07-04 07:17:32.034900 angola-0.14.5/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.5/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.5/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.5/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.14.5/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.5/tests/test_query.py
```

### Comparing `angola-0.14.4/LICENSE` & `angola-0.14.5/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/PKG-INFO` & `angola-0.14.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.4
+Version: 0.14.5
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.4/README.md` & `angola-0.14.5/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/setup.py` & `angola-0.14.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.14.4"
+VERSION = "0.14.5"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.14.4/src/angola/database.py` & `angola-0.14.5/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/src/angola/dict_mutator.py` & `angola-0.14.5/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/src/angola/dict_query.py` & `angola-0.14.5/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/src/angola/lib.py` & `angola-0.14.5/src/angola/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import hashlib
 import datetime
 from slugify import slugify
 from jinja2 import Template
 from functools import reduce
 from operator import itemgetter
 from typing import Iterator, Any
-from uuid_extensions import uuid7
 
 # Date format
 FORMAT_ISO_DATE = "YYYY-MM-DD"
 FORMAT_ISO_TIME = "HH:mm:ss"
 FORMAT_ISO_DATETIME = "YYYY-MM-DD HH:mm:ss"
 
 DATES_FORMAT = {
@@ -65,15 +64,15 @@
 
 def keyname_valid(name:str) -> bool:
     """
     Test if a key name is valid. 
 
     For example, it can test if a key in a dict is valid
 
-    pattern: start with letters or underscrore. Contains alphanum + underscore + hyphen
+    pattern: start with letters or underscrore. Contains alphanum + underscore + hyphen + $
 
     Params:
         name:str
     Returns:
         bool
     """
     if not name or not isinstance(name, str):
```

### Comparing `angola-0.14.4/src/angola/lib_xql.py` & `angola-0.14.5/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/src/angola.egg-info/PKG-INFO` & `angola-0.14.5/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.4
+Version: 0.14.5
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.4/tests/test_database.py` & `angola-0.14.5/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/tests/test_dict_mutator.py` & `angola-0.14.5/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.4/tests/test_lib.py` & `angola-0.14.5/tests/test_lib.py`

 * *Files identical despite different names*

