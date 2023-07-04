# Comparing `tmp/swarms-0.5.0.tar.gz` & `tmp/swarms-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.5.0.tar", last modified: Tue Jul  4 19:31:11 2023, max compression
+gzip compressed data, was "swarms-0.5.1.tar", last modified: Tue Jul  4 19:39:02 2023, max compression
```

## Comparing `swarms-0.5.0.tar` & `swarms-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.694220 swarms-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 19:31:02.000000 swarms-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 19:31:11.694220 swarms-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 19:31:02.000000 swarms-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:02.000000 swarms-0.5.0/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 19:31:02.000000 swarms-0.5.0/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 19:31:02.000000 swarms-0.5.0/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 19:31:02.000000 swarms-0.5.0/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:31:11.694220 swarms-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 19:31:02.000000 swarms-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70839 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.694220 swarms-0.5.0/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 19:31:02.000000 swarms-0.5.0/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:31:11.690220 swarms-0.5.0/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 19:31:11.000000 swarms-0.5.0/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 19:31:11.000000 swarms-0.5.0/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:31:11.000000 swarms-0.5.0/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 19:31:11.000000 swarms-0.5.0/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 19:31:11.000000 swarms-0.5.0/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.923791 swarms-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 19:38:53.000000 swarms-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 19:39:02.923791 swarms-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 19:38:53.000000 swarms-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:38:53.000000 swarms-0.5.1/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 19:38:53.000000 swarms-0.5.1/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 19:38:53.000000 swarms-0.5.1/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 19:38:53.000000 swarms-0.5.1/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:39:02.923791 swarms-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-04 19:38:53.000000 swarms-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70839 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.923791 swarms-0.5.1/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 19:38:53.000000 swarms-0.5.1/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:02.919791 swarms-0.5.1/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 19:39:02.000000 swarms-0.5.1/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 19:39:02.000000 swarms-0.5.1/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:39:02.000000 swarms-0.5.1/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-04 19:39:02.000000 swarms-0.5.1/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 19:39:02.000000 swarms-0.5.1/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.5.0/LICENSE` & `swarms-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/PKG-INFO` & `swarms-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.0
+Version: 0.5.1
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.0/README.md` & `swarms-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/api/container.py` & `swarms-0.5.1/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/api/main.py` & `swarms-0.5.1/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/api/worker.py` & `swarms-0.5.1/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/setup.py` & `swarms-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.5.0',
+  version = '0.5.1',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -18,15 +18,14 @@
     "Prompt Engineering"
   ],
     install_requires=[
         'transformers',
         'openai',
         'langchain',
         'torch',
-        'ansi',
         'torchvision',
         'asyncio',
         'nest_asyncio',
         'bs4',
         'playwright',
         'duckduckgo_search',
         'faiss-cpu',
```

### Comparing `swarms-0.5.0/swarms/agents/swarms.py` & `swarms-0.5.1/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/agents/workers/agents.py` & `swarms-0.5.1/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/agents/workers/auto_agent.py` & `swarms-0.5.1/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.5.1/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/agents/workers/multi_modal.py` & `swarms-0.5.1/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/agents/workers/omni_agent.py` & `swarms-0.5.1/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/tools/main.py` & `swarms-0.5.1/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/utils/ansi.py` & `swarms-0.5.1/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms/utils/utils.py` & `swarms-0.5.1/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms.egg-info/PKG-INFO` & `swarms-0.5.1/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.5.0
+Version: 0.5.1
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.5.0/swarms.egg-info/SOURCES.txt` & `swarms-0.5.1/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.5.0/swarms.egg-info/requires.txt` & `swarms-0.5.1/swarms.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 transformers
 openai
 langchain
 torch
-ansi
 torchvision
 asyncio
 nest_asyncio
 bs4
 playwright
 duckduckgo_search
 faiss-cpu
```

