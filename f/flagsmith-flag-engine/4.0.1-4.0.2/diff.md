# Comparing `tmp/flagsmith-flag-engine-4.0.1.tar.gz` & `tmp/flagsmith-flag-engine-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-flag-engine-4.0.1.tar", last modified: Mon Jul  3 15:44:31 2023, max compression
+gzip compressed data, was "flagsmith-flag-engine-4.0.2.tar", last modified: Tue Jul  4 14:25:48 2023, max compression
```

## Comparing `flagsmith-flag-engine-4.0.1.tar` & `flagsmith-flag-engine-4.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/environments/builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/environments/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/environments/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/environments/integrations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/environments/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/features/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/features/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/identities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/identities/traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/traits/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/traits/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/identities/traits/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/organisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/organisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/organisations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/projects/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/segments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/segments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/segments/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/segments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/segments/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flag_engine/utils/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/json/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/semver.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/flag_engine/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-03 15:44:31.000000 flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-03 15:44:31.000000 flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:44:31.000000 flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 15:44:31.000000 flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 15:44:31.000000 flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 15:44:31.431469 flagsmith-flag-engine-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 15:44:30.000000 flagsmith-flag-engine-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/environments/builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/environments/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/environments/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/environments/integrations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/environments/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/features/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/features/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/identities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/identities/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/traits/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/traits/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/identities/traits/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.613705 flagsmith-flag-engine-4.0.2/flag_engine/organisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/organisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/organisations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/flag_engine/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/projects/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/flag_engine/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/segments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/segments/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/segments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/segments/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/flag_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/flag_engine/utils/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/json/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flag_engine/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:25:48.617706 flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 14:25:48.621706 flagsmith-flag-engine-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-04 14:25:48.000000 flagsmith-flag-engine-4.0.2/setup.py
```

### Comparing `flagsmith-flag-engine-4.0.1/LICENSE.txt` & `flagsmith-flag-engine-4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/PKG-INFO` & `flagsmith-flag-engine-4.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith-flag-engine
-Version: 4.0.1
+Version: 4.0.2
 Summary: Flag engine for the Flagsmith API.
 Home-page: https://github.com/Flagsmith/flagsmith-engine
 Author: Flagsmith
 Author-email: support@flagsmith.com
 License: BSD3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flagsmith-flag-engine-4.0.1/README.md` & `flagsmith-flag-engine-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/engine.py` & `flagsmith-flag-engine-4.0.2/flag_engine/engine.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/environments/models.py` & `flagsmith-flag-engine-4.0.2/flag_engine/environments/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/features/models.py` & `flagsmith-flag-engine-4.0.2/flag_engine/features/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/identities/models.py` & `flagsmith-flag-engine-4.0.2/flag_engine/identities/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/segments/constants.py` & `flagsmith-flag-engine-4.0.2/flag_engine/segments/constants.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/segments/evaluator.py` & `flagsmith-flag-engine-4.0.2/flag_engine/segments/evaluator.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/segments/models.py` & `flagsmith-flag-engine-4.0.2/flag_engine/segments/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/utils/hashing.py` & `flagsmith-flag-engine-4.0.2/flag_engine/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/utils/semver.py` & `flagsmith-flag-engine-4.0.2/flag_engine/utils/semver.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flag_engine/utils/types.py` & `flagsmith-flag-engine-4.0.2/flag_engine/utils/types.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/PKG-INFO` & `flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith-flag-engine
-Version: 4.0.1
+Version: 4.0.2
 Summary: Flag engine for the Flagsmith API.
 Home-page: https://github.com/Flagsmith/flagsmith-engine
 Author: Flagsmith
 Author-email: support@flagsmith.com
 License: BSD3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flagsmith-flag-engine-4.0.1/flagsmith_flag_engine.egg-info/SOURCES.txt` & `flagsmith-flag-engine-4.0.2/flagsmith_flag_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-4.0.1/setup.py` & `flagsmith-flag-engine-4.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="flagsmith-flag-engine",
-    version="4.0.1",
+    version="4.0.2",
     author="Flagsmith",
     author_email="support@flagsmith.com",
     packages=find_packages(include=["flag_engine", "flag_engine.*"]),
     url="https://github.com/Flagsmith/flagsmith-engine",
     license="BSD3",
     description="Flag engine for the Flagsmith API.",
     long_description=open("README.md").read(),
```

