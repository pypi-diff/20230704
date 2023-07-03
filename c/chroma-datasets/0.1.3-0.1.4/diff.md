# Comparing `tmp/chroma_datasets-0.1.3.tar.gz` & `tmp/chroma_datasets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroma_datasets-0.1.3.tar", last modified: Mon Jul  3 23:32:03 2023, max compression
+gzip compressed data, was "chroma_datasets-0.1.4.tar", last modified: Mon Jul  3 23:32:46 2023, max compression
```

## Comparing `chroma_datasets-0.1.3.tar` & `chroma_datasets-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.723549 chroma_datasets-0.1.3/
--rw-r--r--   0 jeff       (501) staff       (20)      130 2023-07-01 20:58:36.000000 chroma_datasets-0.1.3/.gitignore
--rw-r--r--   0 jeff       (501) staff       (20)      166 2023-07-01 21:08:45.000000 chroma_datasets-0.1.3/DEVELOP.md
--rw-r--r--   0 jeff       (501) staff       (20)    11357 2023-06-28 23:45:35.000000 chroma_datasets-0.1.3/LICENSE.md
--rw-r--r--   0 jeff       (501) staff       (20)     5918 2023-07-03 23:32:03.723407 chroma_datasets-0.1.3/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     5301 2023-07-03 23:30:44.000000 chroma_datasets-0.1.3/README.md
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.720582 chroma_datasets-0.1.3/bin/
--rw-r--r--   0 jeff       (501) staff       (20)      151 2023-06-28 23:46:19.000000 chroma_datasets-0.1.3/bin/version
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.720949 chroma_datasets-0.1.3/chroma_datasets/
--rw-r--r--   0 jeff       (501) staff       (20)      200 2023-07-03 23:31:57.000000 chroma_datasets-0.1.3/chroma_datasets/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.721778 chroma_datasets-0.1.3/chroma_datasets/__pycache__/
--rw-r--r--   0 jeff       (501) staff       (20)      395 2023-07-01 21:34:37.000000 chroma_datasets-0.1.3/chroma_datasets/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.722285 chroma_datasets-0.1.3/chroma_datasets/datasets/
--rw-r--r--   0 jeff       (501) staff       (20)     1432 2023-07-03 22:27:26.000000 chroma_datasets-0.1.3/chroma_datasets/datasets/glue.py
--rw-r--r--   0 jeff       (501) staff       (20)     1555 2023-07-03 22:26:03.000000 chroma_datasets-0.1.3/chroma_datasets/datasets/paul_graham_essay.py
--rw-r--r--   0 jeff       (501) staff       (20)     1812 2023-07-03 22:24:59.000000 chroma_datasets-0.1.3/chroma_datasets/datasets/sciq.py
--rw-r--r--   0 jeff       (501) staff       (20)     1484 2023-07-03 22:23:45.000000 chroma_datasets-0.1.3/chroma_datasets/datasets/state_of_the_union.py
--rw-r--r--   0 jeff       (501) staff       (20)     1681 2023-07-03 23:30:30.000000 chroma_datasets-0.1.3/chroma_datasets/types.py
--rw-r--r--   0 jeff       (501) staff       (20)     8127 2023-07-03 23:03:59.000000 chroma_datasets-0.1.3/chroma_datasets/utils.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.721656 chroma_datasets-0.1.3/chroma_datasets.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)     5918 2023-07-03 23:32:03.000000 chroma_datasets-0.1.3/chroma_datasets.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      741 2023-07-03 23:32:03.000000 chroma_datasets-0.1.3/chroma_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-03 23:32:03.000000 chroma_datasets-0.1.3/chroma_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       19 2023-07-03 23:32:03.000000 chroma_datasets-0.1.3/chroma_datasets.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)       16 2023-07-03 23:32:03.000000 chroma_datasets-0.1.3/chroma_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.722859 chroma_datasets-0.1.3/examples/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:03.723168 chroma_datasets-0.1.3/examples/data/
--rw-r--r--   0 jeff       (501) staff       (20)    78216 2023-07-01 14:06:09.000000 chroma_datasets-0.1.3/examples/data/paul_graham_essay.txt
--rw-r--r--   0 jeff       (501) staff       (20)    39027 2023-06-29 16:17:28.000000 chroma_datasets-0.1.3/examples/data/state_of_the_union.txt
--rw-r--r--   0 jeff       (501) staff       (20)   386826 2023-07-03 23:07:25.000000 chroma_datasets-0.1.3/examples/example_export.ipynb
--rw-r--r--   0 jeff       (501) staff       (20)     3242 2023-07-03 22:40:34.000000 chroma_datasets-0.1.3/examples/example_import.ipynb
--rw-r--r--   0 jeff       (501) staff       (20)     2944 2023-07-01 20:53:57.000000 chroma_datasets-0.1.3/examples/example_misc_hf_import.ipynb
--rw-r--r--   0 jeff       (501) staff       (20)      879 2023-07-03 23:31:53.000000 chroma_datasets-0.1.3/pyproject.toml
--rw-r--r--   0 jeff       (501) staff       (20)       18 2023-07-03 22:39:18.000000 chroma_datasets-0.1.3/requirements.txt
--rw-r--r--   0 jeff       (501) staff       (20)       38 2023-07-03 23:32:03.723586 chroma_datasets-0.1.3/setup.cfg
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.896324 chroma_datasets-0.1.4/
+-rw-r--r--   0 jeff       (501) staff       (20)      130 2023-07-01 20:58:36.000000 chroma_datasets-0.1.4/.gitignore
+-rw-r--r--   0 jeff       (501) staff       (20)      166 2023-07-01 21:08:45.000000 chroma_datasets-0.1.4/DEVELOP.md
+-rw-r--r--   0 jeff       (501) staff       (20)    11357 2023-06-28 23:45:35.000000 chroma_datasets-0.1.4/LICENSE.md
+-rw-r--r--   0 jeff       (501) staff       (20)     5918 2023-07-03 23:32:46.896180 chroma_datasets-0.1.4/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     5301 2023-07-03 23:30:44.000000 chroma_datasets-0.1.4/README.md
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.892958 chroma_datasets-0.1.4/bin/
+-rw-r--r--   0 jeff       (501) staff       (20)      151 2023-06-28 23:46:19.000000 chroma_datasets-0.1.4/bin/version
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.893502 chroma_datasets-0.1.4/chroma_datasets/
+-rw-r--r--   0 jeff       (501) staff       (20)      200 2023-07-03 23:32:31.000000 chroma_datasets-0.1.4/chroma_datasets/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.894316 chroma_datasets-0.1.4/chroma_datasets/__pycache__/
+-rw-r--r--   0 jeff       (501) staff       (20)      395 2023-07-01 21:34:37.000000 chroma_datasets-0.1.4/chroma_datasets/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.894932 chroma_datasets-0.1.4/chroma_datasets/datasets/
+-rw-r--r--   0 jeff       (501) staff       (20)     1432 2023-07-03 22:27:26.000000 chroma_datasets-0.1.4/chroma_datasets/datasets/glue.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1555 2023-07-03 22:26:03.000000 chroma_datasets-0.1.4/chroma_datasets/datasets/paul_graham_essay.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1812 2023-07-03 22:24:59.000000 chroma_datasets-0.1.4/chroma_datasets/datasets/sciq.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1484 2023-07-03 22:23:45.000000 chroma_datasets-0.1.4/chroma_datasets/datasets/state_of_the_union.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1681 2023-07-03 23:30:30.000000 chroma_datasets-0.1.4/chroma_datasets/types.py
+-rw-r--r--   0 jeff       (501) staff       (20)     8127 2023-07-03 23:03:59.000000 chroma_datasets-0.1.4/chroma_datasets/utils.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.894168 chroma_datasets-0.1.4/chroma_datasets.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     5918 2023-07-03 23:32:46.000000 chroma_datasets-0.1.4/chroma_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      741 2023-07-03 23:32:46.000000 chroma_datasets-0.1.4/chroma_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-03 23:32:46.000000 chroma_datasets-0.1.4/chroma_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       19 2023-07-03 23:32:46.000000 chroma_datasets-0.1.4/chroma_datasets.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       16 2023-07-03 23:32:46.000000 chroma_datasets-0.1.4/chroma_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.895612 chroma_datasets-0.1.4/examples/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-03 23:32:46.895939 chroma_datasets-0.1.4/examples/data/
+-rw-r--r--   0 jeff       (501) staff       (20)    78216 2023-07-01 14:06:09.000000 chroma_datasets-0.1.4/examples/data/paul_graham_essay.txt
+-rw-r--r--   0 jeff       (501) staff       (20)    39027 2023-06-29 16:17:28.000000 chroma_datasets-0.1.4/examples/data/state_of_the_union.txt
+-rw-r--r--   0 jeff       (501) staff       (20)   386826 2023-07-03 23:07:25.000000 chroma_datasets-0.1.4/examples/example_export.ipynb
+-rw-r--r--   0 jeff       (501) staff       (20)     3242 2023-07-03 22:40:34.000000 chroma_datasets-0.1.4/examples/example_import.ipynb
+-rw-r--r--   0 jeff       (501) staff       (20)     2944 2023-07-01 20:53:57.000000 chroma_datasets-0.1.4/examples/example_misc_hf_import.ipynb
+-rw-r--r--   0 jeff       (501) staff       (20)      879 2023-07-03 23:32:33.000000 chroma_datasets-0.1.4/pyproject.toml
+-rw-r--r--   0 jeff       (501) staff       (20)       18 2023-07-03 22:39:18.000000 chroma_datasets-0.1.4/requirements.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       38 2023-07-03 23:32:46.896366 chroma_datasets-0.1.4/setup.cfg
```

### Comparing `chroma_datasets-0.1.3/LICENSE.md` & `chroma_datasets-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/PKG-INFO` & `chroma_datasets-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chroma_datasets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Chroma Datasets - easy to use datasets for vector retrieval
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma-datasets
 Project-URL: Bug Tracker, https://github.com/chroma-core/chromachroma-datasets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `chroma_datasets-0.1.3/README.md` & `chroma_datasets-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets/datasets/glue.py` & `chroma_datasets-0.1.4/chroma_datasets/datasets/glue.py`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets/datasets/paul_graham_essay.py` & `chroma_datasets-0.1.4/chroma_datasets/datasets/paul_graham_essay.py`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets/datasets/sciq.py` & `chroma_datasets-0.1.4/chroma_datasets/datasets/sciq.py`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets/datasets/state_of_the_union.py` & `chroma_datasets-0.1.4/chroma_datasets/datasets/state_of_the_union.py`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets/types.py` & `chroma_datasets-0.1.4/chroma_datasets/types.py`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets/utils.py` & `chroma_datasets-0.1.4/chroma_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/chroma_datasets.egg-info/PKG-INFO` & `chroma_datasets-0.1.4/chroma_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chroma-datasets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Chroma Datasets - easy to use datasets for vector retrieval
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma-datasets
 Project-URL: Bug Tracker, https://github.com/chroma-core/chromachroma-datasets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `chroma_datasets-0.1.3/chroma_datasets.egg-info/SOURCES.txt` & `chroma_datasets-0.1.4/chroma_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/examples/data/paul_graham_essay.txt` & `chroma_datasets-0.1.4/examples/data/paul_graham_essay.txt`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/examples/data/state_of_the_union.txt` & `chroma_datasets-0.1.4/examples/data/state_of_the_union.txt`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/examples/example_export.ipynb` & `chroma_datasets-0.1.4/examples/example_export.ipynb`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/examples/example_import.ipynb` & `chroma_datasets-0.1.4/examples/example_import.ipynb`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/examples/example_misc_hf_import.ipynb` & `chroma_datasets-0.1.4/examples/example_misc_hf_import.ipynb`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.3/pyproject.toml` & `chroma_datasets-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chroma_datasets"
-version = "0.1.3"
+version = "0.1.4"
 
 authors = [
   { name="Jeff Huber", email="jeff@trychroma.com" },
   { name="Anton Troynikov", email="anton@trychroma.com" }
 ]
 description = "Chroma Datasets - easy to use datasets for vector retrieval"
 readme = "README.md"
```

