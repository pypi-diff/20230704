# Comparing `tmp/swarms-0.4.3.tar.gz` & `tmp/swarms-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.3.tar", last modified: Tue Jul  4 17:44:28 2023, max compression
+gzip compressed data, was "swarms-0.4.4.tar", last modified: Tue Jul  4 17:57:49 2023, max compression
```

## Comparing `swarms-0.4.3.tar` & `swarms-0.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.381006 swarms-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:44:19.000000 swarms-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:44:28.381006 swarms-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16455 2023-07-04 17:44:19.000000 swarms-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:19.000000 swarms-0.4.3/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 17:44:19.000000 swarms-0.4.3/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 17:44:19.000000 swarms-0.4.3/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 17:44:19.000000 swarms-0.4.3/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:44:28.381006 swarms-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 17:44:19.000000 swarms-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.381006 swarms-0.4.3/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70990 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.758441 swarms-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:57:39.000000 swarms-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:57:49.758441 swarms-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-04 17:57:39.000000 swarms-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.754441 swarms-0.4.4/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:39.000000 swarms-0.4.4/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 17:57:39.000000 swarms-0.4.4/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 17:57:39.000000 swarms-0.4.4/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 17:57:39.000000 swarms-0.4.4/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:57:49.758441 swarms-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 17:57:39.000000 swarms-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.754441 swarms-0.4.4/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.754441 swarms-0.4.4/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.754441 swarms-0.4.4/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.754441 swarms-0.4.4/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.758441 swarms-0.4.4/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70990 2023-07-04 17:57:39.000000 swarms-0.4.4/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:57:49.754441 swarms-0.4.4/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:57:49.000000 swarms-0.4.4/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 17:57:49.000000 swarms-0.4.4/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:57:49.000000 swarms-0.4.4/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 17:57:49.000000 swarms-0.4.4/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 17:57:49.000000 swarms-0.4.4/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.3/LICENSE` & `swarms-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/PKG-INFO` & `swarms-0.4.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.3
+Version: 0.4.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.3/README.md` & `swarms-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Agora
 
-![Agora banner](Agora-Banner-blend.png)
+![Agora banner](images/Agora-Banner-blend.png)
 
 [Swarms is brought to you by Agora, the open source AI research organization. Join Agora and Help create swarms and or recieve support to advance Humanity. ](https://discord.gg/qUtxnK2NMf)
 
 # Swarming Language Models (Swarms)
 
-![Swarming banner](swarms.png)
+![Swarming banner](images/swarms.png)
 
 [![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
```

### Comparing `swarms-0.4.3/api/container.py` & `swarms-0.4.4/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/api/main.py` & `swarms-0.4.4/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/api/worker.py` & `swarms-0.4.4/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/setup.py` & `swarms-0.4.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.4.3',
+  version = '0.4.4',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -17,15 +17,16 @@
     'optimizers',
     "Prompt Engineering"
   ],
     install_requires=[
         'transformers',
         'openai',
         'langchain',
-        'torch==2.0.0',
+        'torch',
+        'ansi',
         'torchvision',
         'asyncio',
         'nest_asyncio',
         'bs4',
         'playwright',
         'duckduckgo_search',
         'faiss-cpu',
```

### Comparing `swarms-0.4.3/swarms/agents/swarms.py` & `swarms-0.4.4/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms/agents/workers/agents.py` & `swarms-0.4.4/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms/agents/workers/auto_agent.py` & `swarms-0.4.4/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.4/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms/agents/workers/multi_modal.py` & `swarms-0.4.4/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms/agents/workers/omni_agent.py` & `swarms-0.4.4/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms/tools/main.py` & `swarms-0.4.4/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms.egg-info/PKG-INFO` & `swarms-0.4.4/swarms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.3
+Version: 0.4.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.3/swarms.egg-info/SOURCES.txt` & `swarms-0.4.4/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.4.3/swarms.egg-info/requires.txt` & `swarms-0.4.4/swarms.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 transformers
 openai
 langchain
-torch==2.0.0
+torch
+ansi
 torchvision
 asyncio
 nest_asyncio
 bs4
 playwright
 duckduckgo_search
 faiss-cpu
```

