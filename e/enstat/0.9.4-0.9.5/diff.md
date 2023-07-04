# Comparing `tmp/enstat-0.9.4.tar.gz` & `tmp/enstat-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.9.4.tar", last modified: Thu Jun 29 18:11:57 2023, max compression
+gzip compressed data, was "enstat-0.9.5.tar", last modified: Tue Jul  4 13:38:25 2023, max compression
```

## Comparing `enstat-0.9.4.tar` & `enstat-0.9.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.558464 enstat-0.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 18:11:48.000000 enstat-0.9.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 18:11:48.000000 enstat-0.9.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 18:11:48.000000 enstat-0.9.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-29 18:11:48.000000 enstat-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-29 18:11:48.000000 enstat-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 18:11:48.000000 enstat-0.9.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 18:11:48.000000 enstat-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 18:11:57.562464 enstat-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-29 18:11:48.000000 enstat-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-29 18:11:48.000000 enstat-0.9.4/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    30649 2023-06-29 18:11:48.000000 enstat-0.9.4/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-29 18:11:48.000000 enstat-0.9.4/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-29 18:11:48.000000 enstat-0.9.4/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 18:11:57.000000 enstat-0.9.4/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 18:11:48.000000 enstat-0.9.4/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 18:11:48.000000 enstat-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:11:57.562464 enstat-0.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:57.562464 enstat-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-06-29 18:11:48.000000 enstat-0.9.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-04 13:38:15.000000 enstat-0.9.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 13:38:15.000000 enstat-0.9.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-04 13:38:15.000000 enstat-0.9.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-04 13:38:15.000000 enstat-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-04 13:38:15.000000 enstat-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-04 13:38:15.000000 enstat-0.9.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 13:38:15.000000 enstat-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 13:38:25.924010 enstat-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-04 13:38:15.000000 enstat-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-04 13:38:15.000000 enstat-0.9.5/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    30684 2023-07-04 13:38:15.000000 enstat-0.9.5/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-04 13:38:15.000000 enstat-0.9.5/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-04 13:38:15.000000 enstat-0.9.5/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 13:38:25.000000 enstat-0.9.5/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 13:38:15.000000 enstat-0.9.5/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 13:38:15.000000 enstat-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:38:25.924010 enstat-0.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:25.924010 enstat-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14660 2023-07-04 13:38:15.000000 enstat-0.9.5/tests/test_main.py
```

### Comparing `enstat-0.9.4/.github/workflows/ci.yml` & `enstat-0.9.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/.github/workflows/python-publish.yml` & `enstat-0.9.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/.gitignore` & `enstat-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/.pre-commit-config.yaml` & `enstat-0.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/LICENSE` & `enstat-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/PKG-INFO` & `enstat-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.4
+Version: 0.9.5
 Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enstat-0.9.4/README.md` & `enstat-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/docs/Makefile` & `enstat-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/docs/make.bat` & `enstat-0.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/docs/module.rst` & `enstat-0.9.5/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/enstat/__init__.py` & `enstat-0.9.5/enstat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         if norm is not None:
             assert first is not None
             assert first.shape == norm.shape
 
             if second is not None:
                 assert second.shape == norm.shape
 
-        ret = cls()
+        ret = cls(compute_variance=second is not None)
         ret.first = first
         ret.second = second
         ret.norm = norm
         return ret
 
     def _allocate(self, shape, dtype):
         self.norm = np.zeros(shape, np.int64)
```

### Comparing `enstat-0.9.4/enstat/detail.py` & `enstat-0.9.5/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/enstat/mean.py` & `enstat-0.9.5/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/enstat.egg-info/PKG-INFO` & `enstat-0.9.5/enstat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.4
+Version: 0.9.5
 Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enstat-0.9.4/enstat.egg-info/SOURCES.txt` & `enstat-0.9.5/enstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/tests/test_binned.py` & `enstat-0.9.5/tests/test_binned.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/tests/test_histogram.py` & `enstat-0.9.5/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.4/tests/test_main.py` & `enstat-0.9.5/tests/test_main.py`

 * *Files identical despite different names*

