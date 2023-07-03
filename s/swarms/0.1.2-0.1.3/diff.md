# Comparing `tmp/swarms-0.1.2.tar.gz` & `tmp/swarms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.1.2.tar", last modified: Mon Jul  3 22:53:21 2023, max compression
+gzip compressed data, was "swarms-0.1.3.tar", last modified: Mon Jul  3 23:03:58 2023, max compression
```

## Comparing `swarms-0.1.2.tar` & `swarms-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:53:11.000000 swarms-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:53:21.726582 swarms-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:53:11.000000 swarms-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:53:21.726582 swarms-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:53:11.000000 swarms-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:53:11.000000 swarms-0.1.2/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:11.000000 swarms-0.1.2/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15165 2023-07-03 22:53:11.000000 swarms-0.1.2/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.099295 swarms-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 23:03:46.000000 swarms-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:03:58.095295 swarms-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 23:03:46.000000 swarms-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:03:58.099295 swarms-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 23:03:46.000000 swarms-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.091295 swarms-0.1.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.095295 swarms-0.1.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.095295 swarms-0.1.3/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/multi-modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.091295 swarms-0.1.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.1.2/LICENSE` & `swarms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.1.2/PKG-INFO` & `swarms-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.2
+Version: 0.1.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.2/README.md` & `swarms-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.1.2/setup.py` & `swarms-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.1.2/swarms/agents/swarms.py` & `swarms-0.1.3/swarms/agents/swarms.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,16 @@
 from langchain.vectorstores import FAISS
 from langchain.docstore import InMemoryDocstore
 
 from langchain.agents import ZeroShotAgent, Tool, AgentExecutor
 from langchain import OpenAI, SerpAPIWrapper, LLMChain
 
 
-# Define your embedding model
-# embeddings_model = OpenAIEmbeddings()
-# Initialize the vectorstore as empty
-import faiss
-# from swarms.agents.workers.auto_agent import AutoGPT
 
+import faiss
 
 
 
 #-------------------------------------------------------------------------- WORKER NODE
 import pandas as pd
 from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
 from langchain.chat_models import ChatOpenAI
@@ -53,15 +49,15 @@
 from langchain.tools import BaseTool, DuckDuckGoSearchRun
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
 
 from langchain.tools.human.tool import HumanInputRun
 
 # from swarms.agents.workers.auto_agent import MultiModalVisualAgent
-from swarms.agents.workers.auto_agent import multimodal_agent_tool
+from swarms.agents.workers import multimodal_agent_tool
 from swarms.tools.main import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
 from swarms.tools.main import math_tool
 
 
 openai_api_key = os.environ["OPENAI_API_KEY"]
 
 llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
@@ -143,19 +139,19 @@
         self.agent.run([f"{tree_of_thoughts_prompt} {prompt}"])
 
 
 
 #inti worker node with llm
 worker_node = WorkerNode(llm=llm, tools=tools, vectorstore=vectorstore)
 
-#create an agent within the worker node
-worker_node.create_agent(ai_name="AI Assistant", ai_role="Assistant", human_in_the_loop=True, search_kwargs={})
+# #create an agent within the worker node
+# worker_node.create_agent(ai_name="AI Assistant", ai_role="Assistant", human_in_the_loop=True, search_kwargs={})
 
-#use the agent to perform a task
-worker_node.run_agent("Find 20 potential customers for a Swarms based AI Agent automation infrastructure")
+# #use the agent to perform a task
+# worker_node.run_agent("Find 20 potential customers for a Swarms based AI Agent automation infrastructure")
 
 
 #======================================> WorkerNode
 
 
 # class MetaWorkerNode:
 #     def __init__(self, llm, tools, vectorstore):
```

### Comparing `swarms-0.1.2/swarms.egg-info/PKG-INFO` & `swarms-0.1.3/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.2
+Version: 0.1.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.2/swarms.egg-info/requires.txt` & `swarms-0.1.3/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

