# Comparing `tmp/swarms-0.1.7.tar.gz` & `tmp/swarms-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.1.7.tar", last modified: Tue Jul  4 00:25:31 2023, max compression
+gzip compressed data, was "swarms-0.1.9.tar", last modified: Tue Jul  4 00:43:00 2023, max compression
```

## Comparing `swarms-0.1.7.tar` & `swarms-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.188606 swarms-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 00:25:19.000000 swarms-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:25:31.188606 swarms-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 00:25:19.000000 swarms-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:25:31.188606 swarms-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 00:25:19.000000 swarms-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.184606 swarms-0.1.7/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.184606 swarms-0.1.7/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.188606 swarms-0.1.7/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/multi-modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 00:25:19.000000 swarms-0.1.7/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:25:31.184606 swarms-0.1.7/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 00:25:31.000000 swarms-0.1.7/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:43:00.878757 swarms-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 00:42:51.000000 swarms-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:43:00.878757 swarms-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 00:42:51.000000 swarms-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:43:00.878757 swarms-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 00:42:51.000000 swarms-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:43:00.874757 swarms-0.1.9/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:43:00.878757 swarms-0.1.9/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:43:00.878757 swarms-0.1.9/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/workers/multi-modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 00:42:51.000000 swarms-0.1.9/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:43:00.878757 swarms-0.1.9/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:43:00.000000 swarms-0.1.9/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 00:43:00.000000 swarms-0.1.9/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:43:00.000000 swarms-0.1.9/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 00:43:00.000000 swarms-0.1.9/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 00:43:00.000000 swarms-0.1.9/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.1.7/LICENSE` & `swarms-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/PKG-INFO` & `swarms-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.7
+Version: 0.1.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.7/README.md` & `swarms-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/setup.py` & `swarms-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.1.7',
+  version = '0.1.9',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.1.7/swarms/agents/swarms.py` & `swarms-0.1.9/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/swarms/agents/workers/agents.py` & `swarms-0.1.9/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/swarms/agents/workers/auto_agent.py` & `swarms-0.1.9/swarms/agents/workers/auto_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 # General 
 import os
 import pandas as pd
 from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
-from langchain.chat_models import ChatOpenAI
 
+from langchain.chat_models import ChatOpenAI
 from langchain.agents.agent_toolkits.pandas.base import create_pandas_dataframe_agent
 from langchain.docstore.document import Document
+
 import asyncio
 import nest_asyncio
 
-
-llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key="")
-
 # Tools
 import os
 from contextlib import contextmanager
 from typing import Optional
 from langchain.agents import tool
+
 from langchain.tools.file_management.read import ReadFileTool
 from langchain.tools.file_management.write import WriteFileTool
-
-ROOT_DIR = "./data/"
-
 from langchain.tools import BaseTool, DuckDuckGoSearchRun
-from langchain.text_splitter import RecursiveCharacterTextSplitter
 
+from langchain.text_splitter import RecursiveCharacterTextSplitter
 from pydantic import Field
 from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
 
 # Memory
 import faiss
 from langchain.vectorstores import FAISS
 from langchain.docstore import InMemoryDocstore
 from langchain.embeddings import OpenAIEmbeddings
-from langchain.tools.human.tool import HumanInputRun
-
-
 
+from langchain.tools.human.tool import HumanInputRun
 from swarms.agents.workers.auto_agent import MultiModalVisualAgent
 from swarms.tools.main import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
 
 class MultiModalVisualAgentTool(BaseTool):
     name = "multi_visual_agent"
     description = "Multi-Modal Visual agent tool"
 
@@ -49,63 +43,73 @@
     
     def _run(self, text: str) -> str:
         #run the multi-modal visual agent with the give task
         return self.agent.run_text(text)
 
 
 
-embeddings_model = OpenAIEmbeddings(openai_api_key="")
-embedding_size = 1536
-index = faiss.IndexFlatL2(embedding_size)
-vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
-
 
+class WorkerAgent:
+    def __init__(self, objective: str, api_key: str):
+        self.objective = objective
+        self.api_key = api_key
+        self.worker = self.create_agent_worker()
+
+    def create_agent_worker(self):
+        os.environ['OPENAI_API_KEY'] = self.api_key
+
+        llm = ChatOpenAI(model_name="gpt-4", temperature=1.0)
+        embeddings_model = OpenAIEmbeddings()
+        embedding_size = 1536
+        index = faiss.IndexFlatL2(embedding_size)
+        vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+
+        query_website_tool = WebpageQATool(qa_chain=load_qa_with_sources_chain(llm))
+        web_search = DuckDuckGoSearchRun()
+
+        multimodal_agent = MultiModalVisualAgent()
+        multimodal_agent_tool = MultiModalVisualAgentTool(multimodal_agent)
+
+        tools = [
+            web_search,
+            WriteFileTool(root_dir="./data"),
+            ReadFileTool(root_dir="./data"),
+
+            multimodal_agent_tool,
+            process_csv,
+            query_website_tool,
+            Terminal,
+
+
+            CodeWriter,
+            CodeEditor
+        ]
+
+        agent_worker = AutoGPT.from_llm_and_tools(
+            ai_name="WorkerX",
+            ai_role="Assistant",
+            tools=tools,
+            llm=llm,
+            memory=vectorstore.as_retriever(search_kwargs={"k": 8}),
+            human_in_the_loop=True,
+        )
 
+        agent_worker.chain.verbose = True
 
-query_website_tool = WebpageQATool(qa_chain=load_qa_with_sources_chain(llm))
+        return agent_worker
 
-# !pip install duckduckgo_search
-web_search = DuckDuckGoSearchRun()
-
-
-#MM CHILD AGENT
-multimodal_agent = MultiModalVisualAgent()
-
-#
-multimodal_agent_tool = MultiModalVisualAgentTool(MultiModalVisualAgent)
-
-tools = [
-    
-    web_search,
-    WriteFileTool(root_dir="./data"),
-    ReadFileTool(root_dir="./data"),
-    process_csv,
-
-    # multimodal_agent_tool,
+        # objective = "Your objective here"
+        # api_key = "Your OpenAI API key here"
 
+        # worker_agent = WorkerAgent(objective, api_key)
 
-    query_website_tool,
-    Terminal,
-    CodeWriter,
-    CodeEditor
     
 
-    # HumanInputRun(), # Activate if you want the permit asking for help from the human
-]
 
-agent_worker = AutoGPT.from_llm_and_tools(
-    ai_name="WorkerX",
-    ai_role="Assistant",
-    tools=tools,
-    llm=llm,
-    memory=vectorstore.as_retriever(search_kwargs={"k": 8}),
-    human_in_the_loop=True, # Set to True if you want to add feedback at each step.
-)
 
-agent_worker.chain.verbose = True
 
 # worker_agent = agent_worker
 # tree_of_thoughts_prompt = """
 
 # Imagine three different experts are answering this question. All experts will write down each chain of thought of each step of their thinking, then share it with the group. Then all experts will go on to the next step, etc. If any expert realises they're wrong at any point then they leave. The question is...
```

### Comparing `swarms-0.1.7/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.1.9/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/swarms/agents/workers/multi-modal.py` & `swarms-0.1.9/swarms/agents/workers/multi-modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/swarms/agents/workers/omni_agent.py` & `swarms-0.1.9/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.7/swarms.egg-info/PKG-INFO` & `swarms-0.1.9/swarms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.7
+Version: 0.1.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.7/swarms.egg-info/requires.txt` & `swarms-0.1.9/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

