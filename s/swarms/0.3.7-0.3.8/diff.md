# Comparing `tmp/swarms-0.3.7.tar.gz` & `tmp/swarms-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.3.7.tar", last modified: Tue Jul  4 13:51:24 2023, max compression
+gzip compressed data, was "swarms-0.3.8.tar", last modified: Tue Jul  4 13:54:17 2023, max compression
```

## Comparing `swarms-0.3.7.tar` & `swarms-0.3.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.154787 swarms-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 13:51:14.000000 swarms-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:51:24.154787 swarms-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-04 13:51:14.000000 swarms-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:51:24.154787 swarms-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-04 13:51:14.000000 swarms-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.150787 swarms-0.3.7/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.150787 swarms-0.3.7/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.154787 swarms-0.3.7/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.154787 swarms-0.3.7/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.154787 swarms-0.3.7/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70720 2023-07-04 13:51:14.000000 swarms-0.3.7/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:51:24.150787 swarms-0.3.7/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:51:24.000000 swarms-0.3.7/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 13:51:24.000000 swarms-0.3.7/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:51:24.000000 swarms-0.3.7/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 13:51:24.000000 swarms-0.3.7/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 13:51:24.000000 swarms-0.3.7/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 13:54:06.000000 swarms-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:54:17.458953 swarms-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-04 13:54:06.000000 swarms-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:54:17.458953 swarms-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-04 13:54:06.000000 swarms-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70720 2023-07-04 13:54:06.000000 swarms-0.3.8/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:54:17.458953 swarms-0.3.8/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:54:17.000000 swarms-0.3.8/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 13:54:17.000000 swarms-0.3.8/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:54:17.000000 swarms-0.3.8/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 13:54:17.000000 swarms-0.3.8/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 13:54:17.000000 swarms-0.3.8/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.3.7/LICENSE` & `swarms-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/PKG-INFO` & `swarms-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.7
+Version: 0.3.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.7/README.md` & `swarms-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/setup.py` & `swarms-0.3.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.3.7',
+  version = '0.3.8',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.3.7/swarms/agents/swarms.py` & `swarms-0.3.8/swarms/agents/swarms.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
 
 from langchain.tools.human.tool import HumanInputRun
 
 # from swarms.agents.workers.auto_agent import MultiModalVisualAgent
 # from swarms.agents.workers import multimodal_agent_tool
 from swarms.tools import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
-from swarms.tools.main import math_tool
+from swarms.tools import math_tool
 
 
 openai_api_key = os.environ["OPENAI_API_KEY"]
 
 llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
```

### Comparing `swarms-0.3.7/swarms/agents/workers/agents.py` & `swarms-0.3.8/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms/agents/workers/auto_agent.py` & `swarms-0.3.8/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.3.8/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms/agents/workers/multi_modal.py` & `swarms-0.3.8/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms/agents/workers/omni_agent.py` & `swarms-0.3.8/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms/tools/main.py` & `swarms-0.3.8/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms.egg-info/PKG-INFO` & `swarms-0.3.8/swarms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.7
+Version: 0.3.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.7/swarms.egg-info/SOURCES.txt` & `swarms-0.3.8/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.3.7/swarms.egg-info/requires.txt` & `swarms-0.3.8/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

