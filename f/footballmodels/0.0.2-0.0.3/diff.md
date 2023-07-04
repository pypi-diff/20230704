# Comparing `tmp/footballmodels-0.0.2.tar.gz` & `tmp/footballmodels-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footballmodels-0.0.2.tar", last modified: Sun Jul  2 10:36:37 2023, max compression
+gzip compressed data, was "footballmodels-0.0.3.tar", last modified: Tue Jul  4 20:48:29 2023, max compression
```

## Comparing `footballmodels-0.0.2.tar` & `footballmodels-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.659916 footballmodels-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.663916 footballmodels-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.663916 footballmodels-0.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 10:36:26.000000 footballmodels-0.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-02 10:36:26.000000 footballmodels-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 10:36:37.667916 footballmodels-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-02 10:36:26.000000 footballmodels-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-02 10:36:26.000000 footballmodels-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 10:36:26.000000 footballmodels-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-02 10:36:37.667916 footballmodels-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-02 10:36:26.000000 footballmodels-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.659916 footballmodels-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.663916 footballmodels-0.0.2/src/footballmodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/definitions/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels/player_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/player_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/player_similarity/column_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/player_similarity/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-02 10:36:26.000000 footballmodels-0.0.2/src/footballmodels/utils/possession_adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:36:37.667916 footballmodels-0.0.2/src/footballmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 10:36:37.000000 footballmodels-0.0.2/src/footballmodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.528609 footballmodels-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 20:48:21.000000 footballmodels-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 20:48:29.528609 footballmodels-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 20:48:21.000000 footballmodels-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 20:48:21.000000 footballmodels-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 20:48:21.000000 footballmodels-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-04 20:48:29.528609 footballmodels-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-04 20:48:21.000000 footballmodels-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/footballmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/footballmodels/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/definitions/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.528609 footballmodels-0.0.3/src/footballmodels/player_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/player_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/player_similarity/column_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/player_similarity/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.528609 footballmodels-0.0.3/src/footballmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/utils/possession_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/footballmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/top_level.txt
```

### Comparing `footballmodels-0.0.2/.gitignore` & `footballmodels-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/.vscode/settings.json` & `footballmodels-0.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/LICENSE` & `footballmodels-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/PKG-INFO` & `footballmodels-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.2
+Version: 0.0.3
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.2/setup.cfg` & `footballmodels-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/setup.py` & `footballmodels-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/src/footballmodels/definitions/templates.py` & `footballmodels-0.0.3/src/footballmodels/definitions/templates.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/src/footballmodels/player_similarity/column_defs.py` & `footballmodels-0.0.3/src/footballmodels/player_similarity/column_defs.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/src/footballmodels/utils/distance.py` & `footballmodels-0.0.3/src/footballmodels/utils/distance.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/src/footballmodels/utils/possession_adjustment.py` & `footballmodels-0.0.3/src/footballmodels/utils/possession_adjustment.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.2/src/footballmodels.egg-info/PKG-INFO` & `footballmodels-0.0.3/src/footballmodels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.2
+Version: 0.0.3
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.2/src/footballmodels.egg-info/SOURCES.txt` & `footballmodels-0.0.3/src/footballmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

