# Comparing `tmp/swarms-0.0.8.tar.gz` & `tmp/swarms-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.8.tar", last modified: Mon Jul  3 22:16:19 2023, max compression
+gzip compressed data, was "swarms-0.0.9.tar", last modified: Mon Jul  3 22:28:50 2023, max compression
```

## Comparing `swarms-0.0.8.tar` & `swarms-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:16:09.000000 swarms-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:16:19.368694 swarms-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:16:09.000000 swarms-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:16:19.368694 swarms-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:16:09.000000 swarms-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:16:09.000000 swarms-0.0.8/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:09.000000 swarms-0.0.8/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-03 22:16:09.000000 swarms-0.0.8/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:28:41.000000 swarms-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:28:50.781130 swarms-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:28:41.000000 swarms-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:28:50.785130 swarms-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:28:41.000000 swarms-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:28:41.000000 swarms-0.0.9/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:41.000000 swarms-0.0.9/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-03 22:28:41.000000 swarms-0.0.9/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.8/LICENSE` & `swarms-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.8/PKG-INFO` & `swarms-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.8
+Version: 0.0.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.8/README.md` & `swarms-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.0.8/setup.py` & `swarms-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.0.8/swarms/agents/swarms.py` & `swarms-0.0.9/swarms/agents/swarms.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from langchain.vectorstores import FAISS
 from langchain.docstore import InMemoryDocstore
 
 from langchain.agents import ZeroShotAgent, Tool, AgentExecutor
 from langchain import OpenAI, SerpAPIWrapper, LLMChain
 
 
-from swarms.agents.workers.auto_agent import agent
-worker_agent  = agent
+from swarms.agents.workers.auto_agent import agent_worker
+worker_agent  = agent_worker
 
 # Define your embedding model
 embeddings_model = OpenAIEmbeddings()
 # Initialize the vectorstore as empty
 import faiss
 
 embedding_size = 1536
```

### Comparing `swarms-0.0.8/swarms.egg-info/PKG-INFO` & `swarms-0.0.9/swarms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.8
+Version: 0.0.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.8/swarms.egg-info/requires.txt` & `swarms-0.0.9/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

