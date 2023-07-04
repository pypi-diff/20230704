# Comparing `tmp/queenbee-local-0.6.0.tar.gz` & `tmp/queenbee-local-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/queenbee-local-0.6.0.tar", last modified: Sun Jul  2 20:22:47 2023, max compression
+gzip compressed data, was "dist/queenbee-local-0.6.1.tar", last modified: Tue Jul  4 15:53:23 2023, max compression
```

## Comparing `queenbee-local-0.6.0.tar` & `queenbee-local-0.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/_build/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local/
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/queenbee_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/queenbee_local/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/queenbee_local/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/queenbee_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 20:22:47.000000 queenbee-local-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 20:21:38.000000 queenbee-local-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/_build/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local/
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/queenbee_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/queenbee_local/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/queenbee_local/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/queenbee_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-04 15:53:23.000000 queenbee-local-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-04 15:52:18.000000 queenbee-local-0.6.1/setup.py
```

### Comparing `queenbee-local-0.6.0/.github/workflows/ci.yaml` & `queenbee-local-0.6.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.6.0/LICENSE` & `queenbee-local-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.6.0/PKG-INFO` & `queenbee-local-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.6.0
+Version: 0.6.1
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.6.0/docs/conf.py` & `queenbee-local-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.6.0/queenbee_local/__init__.py` & `queenbee-local-0.6.1/queenbee_local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             command = command.replace('"', '\'')
 
         cur_dir = os.getcwd()
         dst_dir, dst = self._get_dst_folder(command)
         os.chdir(dst)
 
         self._copy_input_artifacts(dst)
-        if self.is_script:
+        if hasattr(self, 'is_script') and self.is_script:
             self._copy_script(dst)
 
         logger.info(f'Started running {self.__class__.__name__}...')
         qb_logger.info(f'Started running {self.__class__.__name__}...')
         self._update_status(logger=qb_logger, started=True)
 
         # TODO: offer an option for podman
```

### Comparing `queenbee-local-0.6.0/queenbee_local/cli.py` & `queenbee-local-0.6.1/queenbee_local/cli.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.6.0/queenbee_local/helper.py` & `queenbee-local-0.6.1/queenbee_local/helper.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.6.0/queenbee_local.egg-info/PKG-INFO` & `queenbee-local-0.6.1/queenbee_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.6.0
+Version: 0.6.1
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.6.0/queenbee_local.egg-info/SOURCES.txt` & `queenbee-local-0.6.1/queenbee_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.6.0/setup.py` & `queenbee-local-0.6.1/setup.py`

 * *Files identical despite different names*

