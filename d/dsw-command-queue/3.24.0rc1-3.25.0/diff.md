# Comparing `tmp/dsw-command-queue-3.24.0rc1.tar.gz` & `tmp/dsw-command-queue-3.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-command-queue-3.24.0rc1.tar", last modified: Tue May 30 11:45:32 2023, max compression
+gzip compressed data, was "dsw-command-queue-3.25.0.tar", last modified: Tue Jul  4 07:29:29 2023, max compression
```

## Comparing `dsw-command-queue-3.24.0rc1.tar` & `dsw-command-queue-3.25.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:32.503225 dsw-command-queue-3.24.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 11:45:32.499225 dsw-command-queue-3.24.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:32.499225 dsw-command-queue-3.24.0rc1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:32.499225 dsw-command-queue-3.24.0rc1/dsw/command_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/dsw/command_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw/command_queue/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/dsw/command_queue/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/dsw/command_queue/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:32.499225 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 11:45:32.000000 dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:32.503225 dsw-command-queue-3.24.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:26.000000 dsw-command-queue-3.24.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:29.367880 dsw-command-queue-3.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-04 07:29:29.363880 dsw-command-queue-3.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:29.359880 dsw-command-queue-3.25.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:29.363880 dsw-command-queue-3.25.0/dsw/command_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/dsw/command_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 07:29:28.000000 dsw-command-queue-3.25.0/dsw/command_queue/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/dsw/command_queue/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/dsw/command_queue/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:29:29.363880 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-04 07:29:29.000000 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 07:29:29.000000 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:29.000000 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:29:29.000000 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 07:29:29.000000 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-04 07:29:29.000000 dsw-command-queue-3.25.0/dsw_command_queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:29.367880 dsw-command-queue-3.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:29:13.000000 dsw-command-queue-3.25.0/setup.py
```

### Comparing `dsw-command-queue-3.24.0rc1/LICENSE` & `dsw-command-queue-3.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.24.0rc1/PKG-INFO` & `dsw-command-queue-3.25.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
```

### Comparing `dsw-command-queue-3.24.0rc1/README.md` & `dsw-command-queue-3.25.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.24.0rc1/dsw/command_queue/command_queue.py` & `dsw-command-queue-3.25.0/dsw/command_queue/command_queue.py`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.24.0rc1/dsw/command_queue/query.py` & `dsw-command-queue-3.25.0/dsw/command_queue/query.py`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-3.24.0rc1/dsw_command_queue.egg-info/PKG-INFO` & `dsw-command-queue-3.25.0/dsw_command_queue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 3.24.0rc1
+Version: 3.25.0
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
```

### Comparing `dsw-command-queue-3.24.0rc1/pyproject.toml` & `dsw-command-queue-3.25.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-command-queue'
-version = "3.24.0rc.1"
+version = "3.25.0"
 description = 'Library for working with command queue and persistent commands'
 readme = 'README.md'
 keywords = ['dsw', 'subscriber', 'publisher', 'database', 'queue', 'processing']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -21,15 +21,15 @@
     'Topic :: Database',
     'Topic :: Text Processing',
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     # DSW
-    "dsw-database==3.24.0rc.1",
+    "dsw-database==3.25.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

