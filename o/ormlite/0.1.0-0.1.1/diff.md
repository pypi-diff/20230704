# Comparing `tmp/ormlite-0.1.0.tar.gz` & `tmp/ormlite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormlite-0.1.0.tar", last modified: Tue Jul  4 18:47:34 2023, max compression
+gzip compressed data, was "ormlite-0.1.1.tar", last modified: Tue Jul  4 21:11:05 2023, max compression
```

## Comparing `ormlite-0.1.0.tar` & `ormlite-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 18:47:23.000000 ormlite-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 18:47:34.328352 ormlite-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-04 18:47:23.000000 ormlite-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-04 18:47:23.000000 ormlite-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:47:34.328352 ormlite-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.324352 ormlite-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/src/ormlite/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 18:47:23.000000 ormlite-0.1.0/src/ormlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/src/ormlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 18:47:34.000000 ormlite-0.1.0/src/ormlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:47:34.328352 ormlite-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-04 18:47:23.000000 ormlite-0.1.0/tests/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-04 18:47:23.000000 ormlite-0.1.0/tests/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-04 18:47:23.000000 ormlite-0.1.0/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:11:05.904979 ormlite-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 21:10:50.000000 ormlite-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-04 21:11:05.904979 ormlite-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-04 21:10:50.000000 ormlite-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-04 21:10:50.000000 ormlite-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:11:05.904979 ormlite-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:11:05.900979 ormlite-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:11:05.900979 ormlite-0.1.1/src/ormlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 21:10:50.000000 ormlite-0.1.1/src/ormlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:11:05.904979 ormlite-0.1.1/src/ormlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-04 21:11:05.000000 ormlite-0.1.1/src/ormlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 21:11:05.000000 ormlite-0.1.1/src/ormlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:11:05.000000 ormlite-0.1.1/src/ormlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 21:11:05.000000 ormlite-0.1.1/src/ormlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 21:11:05.000000 ormlite-0.1.1/src/ormlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:11:05.904979 ormlite-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-04 21:10:50.000000 ormlite-0.1.1/tests/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-04 21:10:50.000000 ormlite-0.1.1/tests/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-04 21:10:50.000000 ormlite-0.1.1/tests/test_query.py
```

### Comparing `ormlite-0.1.0/LICENSE` & `ormlite-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/PKG-INFO` & `ormlite-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: ormlite
-Version: 0.1.0
+Version: 0.1.1
+Summary: Two way binding from Python Dataclasses to Sqlite tables
 Author-email: Charles Taylor <charlestaylor95@gmail.com>
 License: Copyright 2023 Charles Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `ormlite-0.1.0/README.md` & `ormlite-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/pyproject.toml` & `ormlite-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "ormlite"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.11"
 keywords = ["sqlite", "orm", "dataclass", "data", "query", "migration"]
 authors = [
   {name = "Charles Taylor", email = "charlestaylor95@gmail.com" }
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.11",
 ]
+description = "Two way binding from Python Dataclasses to Sqlite tables"
 
 [project.urls]
 "Github Repo" = "https://github.com/CharlesTaylor7/ormlite"
 "Issue Tracker" = "https://github.com/CharlesTaylor7/ormlite/issues"
 
 [project.optional-dependencies] 
 dev = [ "black", "pytest", "pytest-cov", "sphinx", "myst_parser" ]
```

### Comparing `ormlite-0.1.0/src/ormlite/adapters.py` & `ormlite-0.1.1/src/ormlite/adapters.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/src/ormlite/migrate.py` & `ormlite-0.1.1/src/ormlite/migrate.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # - Done: add columns
 # - Done: drop columns
 # - Done: create tables
 # - Done: drop tables
 # - Renaming columns or tables can be done with manual sql at the cli
 # changing constraints, is a tricky multi step process:
 # https://sqlite.org/lang_altertable.html#making_other_kinds_of_table_schema_changes
-def run(db: DatabaseConnection):
+def migrate(db: DatabaseConnection):
     db.execute("""BEGIN EXCLUSIVE TRANSACTION""")
     cursor = db.execute(
         """
         SELECT tbl_name, sql
         FROM sqlite_schema
         WHERE type = 'table'
     """
```

### Comparing `ormlite-0.1.0/src/ormlite/orm.py` & `ormlite-0.1.1/src/ormlite/orm.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/src/ormlite/query.py` & `ormlite-0.1.1/src/ormlite/query.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/src/ormlite/utils.py` & `ormlite-0.1.1/src/ormlite/utils.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/src/ormlite.egg-info/PKG-INFO` & `ormlite-0.1.1/src/ormlite.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: ormlite
-Version: 0.1.0
+Version: 0.1.1
+Summary: Two way binding from Python Dataclasses to Sqlite tables
 Author-email: Charles Taylor <charlestaylor95@gmail.com>
 License: Copyright 2023 Charles Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `ormlite-0.1.0/tests/test_migrate.py` & `ormlite-0.1.1/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/tests/test_orm.py` & `ormlite-0.1.1/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `ormlite-0.1.0/tests/test_query.py` & `ormlite-0.1.1/tests/test_query.py`

 * *Files identical despite different names*

