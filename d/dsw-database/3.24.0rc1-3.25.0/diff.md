# Comparing `tmp/dsw-database-3.24.0rc1.tar.gz` & `tmp/dsw-database-3.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-database-3.24.0rc1.tar", last modified: Tue May 30 11:45:54 2023, max compression
+gzip compressed data, was "dsw-database-3.25.0.tar", last modified: Tue Jul  4 07:29:26 2023, max compression
```

## Comparing `dsw-database-3.24.0rc1.tar` & `dsw-database-3.25.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:54.653102 dsw-database-3.24.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 11:45:54.653102 dsw-database-3.24.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:54.649102 dsw-database-3.24.0rc1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:54.649102 dsw-database-3.24.0rc1/dsw/database/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/dsw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw/database/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/dsw/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/dsw/database/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:54.653102 dsw-database-3.24.0rc1/dsw_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw_database.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 11:45:54.000000 dsw-database-3.24.0rc1/dsw_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:54.653102 dsw-database-3.24.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:46.000000 dsw-database-3.24.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.203403 dsw-database-3.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-04 07:29:20.000000 dsw-database-3.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 07:29:26.203403 dsw-database-3.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-04 07:29:20.000000 dsw-database-3.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.199403 dsw-database-3.25.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.203403 dsw-database-3.25.0/dsw/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 07:29:20.000000 dsw-database-3.25.0/dsw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 07:29:25.000000 dsw-database-3.25.0/dsw/database/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-07-04 07:29:20.000000 dsw-database-3.25.0/dsw/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-04 07:29:20.000000 dsw-database-3.25.0/dsw/database/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:26.203403 dsw-database-3.25.0/dsw_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 07:29:26.000000 dsw-database-3.25.0/dsw_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-04 07:29:20.000000 dsw-database-3.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:26.203403 dsw-database-3.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:20.000000 dsw-database-3.25.0/setup.py
```

### Comparing `dsw-database-3.24.0rc1/LICENSE` & `dsw-database-3.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-database-3.24.0rc1/PKG-INFO` & `dsw-database-3.25.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
```

### Comparing `dsw-database-3.24.0rc1/README.md` & `dsw-database-3.25.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-database-3.24.0rc1/dsw/database/database.py` & `dsw-database-3.25.0/dsw/database/database.py`

 * *Files identical despite different names*

### Comparing `dsw-database-3.24.0rc1/dsw/database/model.py` & `dsw-database-3.25.0/dsw/database/model.py`

 * *Files identical despite different names*

### Comparing `dsw-database-3.24.0rc1/dsw_database.egg-info/PKG-INFO` & `dsw-database-3.25.0/dsw_database.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
```

### Comparing `dsw-database-3.24.0rc1/pyproject.toml` & `dsw-database-3.25.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-database'
-version = "3.24.0rc.1"
+version = "3.25.0"
 description = 'Library for managing DSW database'
 readme = 'README.md'
 keywords = ['dsw', 'database']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -22,15 +22,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     'psycopg[binary]',
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

