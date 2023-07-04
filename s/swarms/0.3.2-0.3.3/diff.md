# Comparing `tmp/swarms-0.3.2.tar.gz` & `tmp/swarms-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.3.2.tar", last modified: Tue Jul  4 04:29:19 2023, max compression
+gzip compressed data, was "swarms-0.3.3.tar", last modified: Tue Jul  4 04:39:03 2023, max compression
```

## Comparing `swarms-0.3.2.tar` & `swarms-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:19.676018 swarms-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 04:29:10.000000 swarms-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 04:29:19.676018 swarms-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 04:29:10.000000 swarms-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:29:19.676018 swarms-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-04 04:29:10.000000 swarms-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:19.672018 swarms-0.3.2/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:19.672018 swarms-0.3.2/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:19.676018 swarms-0.3.2/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:19.676018 swarms-0.3.2/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79474 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 04:29:10.000000 swarms-0.3.2/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:19.672018 swarms-0.3.2/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 04:29:19.000000 swarms-0.3.2/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 04:29:19.000000 swarms-0.3.2/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:29:19.000000 swarms-0.3.2/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 04:29:19.000000 swarms-0.3.2/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 04:29:19.000000 swarms-0.3.2/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:39:03.313215 swarms-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 04:38:51.000000 swarms-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 04:39:03.313215 swarms-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 04:38:51.000000 swarms-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:39:03.313215 swarms-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-04 04:38:51.000000 swarms-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:39:03.309215 swarms-0.3.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:39:03.313215 swarms-0.3.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:39:03.313215 swarms-0.3.3/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:39:03.313215 swarms-0.3.3/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79474 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 04:38:51.000000 swarms-0.3.3/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:39:03.313215 swarms-0.3.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 04:39:03.000000 swarms-0.3.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 04:39:03.000000 swarms-0.3.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:39:03.000000 swarms-0.3.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 04:39:03.000000 swarms-0.3.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 04:39:03.000000 swarms-0.3.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.3.2/LICENSE` & `swarms-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/PKG-INFO` & `swarms-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.2
+Version: 0.3.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.2/README.md` & `swarms-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/setup.py` & `swarms-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.3.2',
+  version = '0.3.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.3.2/swarms/agents/swarms.py` & `swarms-0.3.3/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/swarms/agents/workers/agents.py` & `swarms-0.3.3/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/swarms/agents/workers/auto_agent.py` & `swarms-0.3.3/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.3.3/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/swarms/agents/workers/multi_modal.py` & `swarms-0.3.3/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/swarms/agents/workers/omni_agent.py` & `swarms-0.3.3/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.2/swarms.egg-info/PKG-INFO` & `swarms-0.3.3/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.2
+Version: 0.3.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.2/swarms.egg-info/requires.txt` & `swarms-0.3.3/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

