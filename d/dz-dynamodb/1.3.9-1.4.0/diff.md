# Comparing `tmp/dz-dynamodb-1.3.9.tar.gz` & `tmp/dz-dynamodb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dz-dynamodb-1.3.9.tar", last modified: Wed Dec  7 07:57:30 2022, max compression
+gzip compressed data, was "dz-dynamodb-1.4.0.tar", last modified: Tue Jul  4 10:53:26 2023, max compression
```

## Comparing `dz-dynamodb-1.3.9.tar` & `dz-dynamodb-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2022-12-07 07:57:30.158611 dz-dynamodb-1.3.9/
--rw-r--r--   0 piyushsingariya   (501) staff       (20)    32387 2022-11-24 07:04:06.000000 dz-dynamodb-1.3.9/LICENSE
--rw-r--r--   0 piyushsingariya   (501) staff       (20)      284 2022-12-07 07:57:30.158337 dz-dynamodb-1.3.9/PKG-INFO
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     1372 2022-12-01 07:27:43.000000 dz-dynamodb-1.3.9/README.md
-drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2022-12-07 07:57:30.156286 dz-dynamodb-1.3.9/dz_dynamodb/
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     3245 2022-12-01 07:28:00.000000 dz-dynamodb-1.3.9/dz_dynamodb/__init__.py
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     4336 2022-12-01 06:48:45.000000 dz-dynamodb-1.3.9/dz_dynamodb/deserialize.py
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     2139 2022-12-01 07:28:00.000000 dz-dynamodb-1.3.9/dz_dynamodb/discover.py
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     4792 2022-12-01 06:48:45.000000 dz-dynamodb-1.3.9/dz_dynamodb/dynamodb.py
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     3620 2022-12-07 07:54:04.000000 dz-dynamodb-1.3.9/dz_dynamodb/sync.py
-drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2022-12-07 07:57:30.157949 dz-dynamodb-1.3.9/dz_dynamodb/sync_strategies/
--rw-r--r--   0 piyushsingariya   (501) staff       (20)        0 2022-12-01 06:48:45.000000 dz-dynamodb-1.3.9/dz_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 piyushsingariya   (501) staff       (20)     4837 2022-12-01 07:28:00.000000 dz-dynamodb-1.3.9/dz_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 piyushsingariya   (501) staff       (20)    11640 2022-12-01 07:28:00.000000 dz-dynamodb-1.3.9/dz_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2022-12-07 07:57:30.157251 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/
--rw-r--r--   0 piyushsingariya   (501) staff       (20)      284 2022-12-07 07:57:30.000000 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 piyushsingariya   (501) staff       (20)      480 2022-12-07 07:57:30.000000 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 piyushsingariya   (501) staff       (20)        1 2022-12-07 07:57:30.000000 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 piyushsingariya   (501) staff       (20)       60 2022-12-07 07:57:30.000000 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 piyushsingariya   (501) staff       (20)       96 2022-12-07 07:57:30.000000 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/requires.txt
--rw-r--r--   0 piyushsingariya   (501) staff       (20)       12 2022-12-07 07:57:30.000000 dz-dynamodb-1.3.9/dz_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 piyushsingariya   (501) staff       (20)       38 2022-12-07 07:57:30.158658 dz-dynamodb-1.3.9/setup.cfg
--rwxr-xr-x   0 piyushsingariya   (501) staff       (20)      767 2022-12-07 07:54:13.000000 dz-dynamodb-1.3.9/setup.py
+drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2023-07-04 10:53:26.455343 dz-dynamodb-1.4.0/
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)    32387 2022-11-24 07:04:06.000000 dz-dynamodb-1.4.0/LICENSE
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)      284 2023-07-04 10:53:26.455195 dz-dynamodb-1.4.0/PKG-INFO
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     1372 2022-12-01 07:27:43.000000 dz-dynamodb-1.4.0/README.md
+drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2023-07-04 10:53:26.453226 dz-dynamodb-1.4.0/dz_dynamodb/
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     3245 2022-12-01 07:28:00.000000 dz-dynamodb-1.4.0/dz_dynamodb/__init__.py
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     4336 2022-12-01 06:48:45.000000 dz-dynamodb-1.4.0/dz_dynamodb/deserialize.py
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     4057 2023-07-04 10:52:27.000000 dz-dynamodb-1.4.0/dz_dynamodb/discover.py
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     4792 2022-12-01 06:48:45.000000 dz-dynamodb-1.4.0/dz_dynamodb/dynamodb.py
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     3620 2022-12-07 07:54:04.000000 dz-dynamodb-1.4.0/dz_dynamodb/sync.py
+drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2023-07-04 10:53:26.454825 dz-dynamodb-1.4.0/dz_dynamodb/sync_strategies/
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)        0 2022-12-01 06:48:45.000000 dz-dynamodb-1.4.0/dz_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)     4837 2022-12-01 07:28:00.000000 dz-dynamodb-1.4.0/dz_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)    11640 2022-12-01 07:28:00.000000 dz-dynamodb-1.4.0/dz_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 piyushsingariya   (501) staff       (20)        0 2023-07-04 10:53:26.454287 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)      284 2023-07-04 10:53:26.000000 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)      480 2023-07-04 10:53:26.000000 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)        1 2023-07-04 10:53:26.000000 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)       60 2023-07-04 10:53:26.000000 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)       96 2023-07-04 10:53:26.000000 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)       12 2023-07-04 10:53:26.000000 dz-dynamodb-1.4.0/dz_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 piyushsingariya   (501) staff       (20)       38 2023-07-04 10:53:26.455398 dz-dynamodb-1.4.0/setup.cfg
+-rwxr-xr-x   0 piyushsingariya   (501) staff       (20)      767 2023-07-04 10:53:02.000000 dz-dynamodb-1.4.0/setup.py
```

### Comparing `dz-dynamodb-1.3.9/LICENSE` & `dz-dynamodb-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/README.md` & `dz-dynamodb-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/dz_dynamodb/__init__.py` & `dz-dynamodb-1.4.0/dz_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/dz_dynamodb/deserialize.py` & `dz-dynamodb-1.4.0/dz_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/dz_dynamodb/dynamodb.py` & `dz-dynamodb-1.4.0/dz_dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/dz_dynamodb/sync.py` & `dz-dynamodb-1.4.0/dz_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/dz_dynamodb/sync_strategies/full_table.py` & `dz-dynamodb-1.4.0/dz_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/dz_dynamodb/sync_strategies/log_based.py` & `dz-dynamodb-1.4.0/dz_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `dz-dynamodb-1.3.9/setup.py` & `dz-dynamodb-1.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="dz-dynamodb",
-    version="1.3.9",
+    version="1.4.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["dz_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

