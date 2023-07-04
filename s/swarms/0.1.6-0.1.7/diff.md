# Comparing `tmp/swarms-0.1.6.tar.gz` & `tmp/swarms-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.1.6.tar", last modified: Tue Jul  4 00:22:19 2023, max compression
+gzip compressed data, was "swarms-0.1.7.tar", last modified: Tue Jul  4 00:25:31 2023, max compression
```

## Comparing `swarms-0.1.6.tar` & `swarms-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:22:19.077995 swarms-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 00:22:07.000000 swarms-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:22:19.077995 swarms-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 00:22:07.000000 swarms-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:22:19.077995 swarms-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 00:22:07.000000 swarms-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:22:19.073994 swarms-0.1.6/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:22:19.073994 swarms-0.1.6/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:22:19.077995 swarms-0.1.6/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/workers/multi-modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 00:22:07.000000 swarms-0.1.6/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:22:19.073994 swarms-0.1.6/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:22:19.000000 swarms-0.1.6/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 00:22:19.000000 swarms-0.1.6/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:22:19.000000 swarms-0.1.6/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 00:22:19.000000 swarms-0.1.6/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 00:22:19.000000 swarms-0.1.6/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.188606 swarms-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 00:25:19.000000 swarms-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:25:31.188606 swarms-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 00:25:19.000000 swarms-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:25:31.188606 swarms-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 00:25:19.000000 swarms-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.184606 swarms-0.1.7/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.184606 swarms-0.1.7/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.188606 swarms-0.1.7/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/multi-modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.184606 swarms-0.1.7/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.1.6/LICENSE` & `swarms-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/PKG-INFO` & `swarms-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.6
+Version: 0.1.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.6/README.md` & `swarms-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/setup.py` & `swarms-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.1.6/swarms/agents/swarms.py` & `swarms-0.1.7/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/swarms/agents/workers/agents.py` & `swarms-0.1.7/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/swarms/agents/workers/auto_agent.py` & `swarms-0.1.7/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.1.7/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/swarms/agents/workers/multi-modal.py` & `swarms-0.1.7/swarms/agents/workers/multi-modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/swarms/agents/workers/omni_agent.py` & `swarms-0.1.7/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.6/swarms.egg-info/PKG-INFO` & `swarms-0.1.7/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.6
+Version: 0.1.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.6/swarms.egg-info/requires.txt` & `swarms-0.1.7/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

