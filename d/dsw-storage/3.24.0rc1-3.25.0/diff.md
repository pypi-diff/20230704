# Comparing `tmp/dsw-storage-3.24.0rc1.tar.gz` & `tmp/dsw-storage-3.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-storage-3.24.0rc1.tar", last modified: Tue May 30 11:46:10 2023, max compression
+gzip compressed data, was "dsw-storage-3.25.0.tar", last modified: Tue Jul  4 07:29:50 2023, max compression
```

## Comparing `dsw-storage-3.24.0rc1.tar` & `dsw-storage-3.25.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:46:10.403402 dsw-storage-3.24.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-30 11:46:05.000000 dsw-storage-3.24.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 11:46:10.403402 dsw-storage-3.24.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-30 11:46:05.000000 dsw-storage-3.24.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:46:10.399402 dsw-storage-3.24.0rc1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:46:10.399402 dsw-storage-3.24.0rc1/dsw/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 11:46:05.000000 dsw-storage-3.24.0rc1/dsw/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw/storage/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-30 11:46:05.000000 dsw-storage-3.24.0rc1/dsw/storage/s3storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:46:10.403402 dsw-storage-3.24.0rc1/dsw_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 11:46:10.000000 dsw-storage-3.24.0rc1/dsw_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-30 11:46:05.000000 dsw-storage-3.24.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:46:10.403402 dsw-storage-3.24.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:46:05.000000 dsw-storage-3.24.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:50.567580 dsw-storage-3.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-04 07:29:43.000000 dsw-storage-3.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-04 07:29:50.567580 dsw-storage-3.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-04 07:29:43.000000 dsw-storage-3.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:50.563580 dsw-storage-3.25.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:50.567580 dsw-storage-3.25.0/dsw/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-04 07:29:43.000000 dsw-storage-3.25.0/dsw/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw/storage/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-04 07:29:43.000000 dsw-storage-3.25.0/dsw/storage/s3storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:50.567580 dsw-storage-3.25.0/dsw_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 07:29:50.000000 dsw-storage-3.25.0/dsw_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-04 07:29:43.000000 dsw-storage-3.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:50.567580 dsw-storage-3.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:43.000000 dsw-storage-3.25.0/setup.py
```

### Comparing `dsw-storage-3.24.0rc1/LICENSE` & `dsw-storage-3.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-storage-3.24.0rc1/PKG-INFO` & `dsw-storage-3.25.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-storage
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for managing DSW S3 storage
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,s3,bucket,storage
```

### Comparing `dsw-storage-3.24.0rc1/README.md` & `dsw-storage-3.25.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-storage-3.24.0rc1/dsw/storage/s3storage.py` & `dsw-storage-3.25.0/dsw/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `dsw-storage-3.24.0rc1/dsw_storage.egg-info/PKG-INFO` & `dsw-storage-3.25.0/dsw_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-storage
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for managing DSW S3 storage
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,s3,bucket,storage
```

### Comparing `dsw-storage-3.24.0rc1/pyproject.toml` & `dsw-storage-3.25.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-storage'
-version = "3.24.0rc.1"
+version = "3.25.0"
 description = 'Library for managing DSW S3 storage'
 readme = 'README.md'
 keywords = ['dsw', 's3', 'bucket', 'storage']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -22,15 +22,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     'minio',
     'tenacity',
     # DSW
-    "dsw-config==3.24.0rc.1",
+    "dsw-config==3.25.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

