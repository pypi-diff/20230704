# Comparing `tmp/dsw-models-3.24.0rc1.tar.gz` & `tmp/dsw-models-3.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-models-3.24.0rc1.tar", last modified: Tue May 30 11:45:59 2023, max compression
+gzip compressed data, was "dsw-models-3.25.0.tar", last modified: Tue Jul  4 07:29:32 2023, max compression
```

## Comparing `dsw-models-3.24.0rc1.tar` & `dsw-models-3.25.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:59.602633 dsw-models-3.24.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 11:45:59.602633 dsw-models-3.24.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:59.598633 dsw-models-3.24.0rc1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:59.598633 dsw-models-3.24.0rc1/dsw/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/dsw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-30 11:45:59.000000 dsw-models-3.24.0rc1/dsw/models/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/dsw/models/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:59.598633 dsw-models-3.24.0rc1/dsw/models/km/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/dsw/models/km/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90332 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/dsw/models/km/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/dsw/models/km/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:59.602633 dsw-models-3.24.0rc1/dsw_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 11:45:59.000000 dsw-models-3.24.0rc1/dsw_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-30 11:45:59.000000 dsw-models-3.24.0rc1/dsw_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:59.000000 dsw-models-3.24.0rc1/dsw_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:59.000000 dsw-models-3.24.0rc1/dsw_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 11:45:59.000000 dsw-models-3.24.0rc1/dsw_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:59.602633 dsw-models-3.24.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:49.000000 dsw-models-3.24.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:32.886868 dsw-models-3.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-04 07:29:25.000000 dsw-models-3.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-04 07:29:32.886868 dsw-models-3.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-04 07:29:25.000000 dsw-models-3.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:32.882868 dsw-models-3.25.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:32.886868 dsw-models-3.25.0/dsw/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:25.000000 dsw-models-3.25.0/dsw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 07:29:32.000000 dsw-models-3.25.0/dsw/models/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 07:29:25.000000 dsw-models-3.25.0/dsw/models/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:32.886868 dsw-models-3.25.0/dsw/models/km/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:25.000000 dsw-models-3.25.0/dsw/models/km/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90332 2023-07-04 07:29:25.000000 dsw-models-3.25.0/dsw/models/km/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-04 07:29:25.000000 dsw-models-3.25.0/dsw/models/km/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:32.886868 dsw-models-3.25.0/dsw_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-04 07:29:32.000000 dsw-models-3.25.0/dsw_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 07:29:32.000000 dsw-models-3.25.0/dsw_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:32.000000 dsw-models-3.25.0/dsw_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:32.000000 dsw-models-3.25.0/dsw_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 07:29:32.000000 dsw-models-3.25.0/dsw_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 07:29:25.000000 dsw-models-3.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:32.886868 dsw-models-3.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:25.000000 dsw-models-3.25.0/setup.py
```

### Comparing `dsw-models-3.24.0rc1/LICENSE` & `dsw-models-3.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-models-3.24.0rc1/PKG-INFO` & `dsw-models-3.25.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-models
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library with DSW models and basic IO operations
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-models-3.24.0rc1/README.md` & `dsw-models-3.25.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-models-3.24.0rc1/dsw/models/km/events.py` & `dsw-models-3.25.0/dsw/models/km/events.py`

 * *Files identical despite different names*

### Comparing `dsw-models-3.24.0rc1/dsw/models/km/package.py` & `dsw-models-3.25.0/dsw/models/km/package.py`

 * *Files identical despite different names*

### Comparing `dsw-models-3.24.0rc1/dsw_models.egg-info/PKG-INFO` & `dsw-models-3.25.0/dsw_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-models
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library with DSW models and basic IO operations
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-models-3.24.0rc1/pyproject.toml` & `dsw-models-3.25.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-models'
-version = "3.24.0rc.1"
+version = "3.25.0"
 description = 'Library with DSW models and basic IO operations'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

