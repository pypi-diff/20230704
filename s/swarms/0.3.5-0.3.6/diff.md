# Comparing `tmp/swarms-0.3.5.tar.gz` & `tmp/swarms-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.3.5.tar", last modified: Tue Jul  4 13:22:37 2023, max compression
+gzip compressed data, was "swarms-0.3.6.tar", last modified: Tue Jul  4 13:38:17 2023, max compression
```

## Comparing `swarms-0.3.5.tar` & `swarms-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:37.253424 swarms-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 13:22:26.000000 swarms-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:22:37.253424 swarms-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 13:22:26.000000 swarms-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:22:37.253424 swarms-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-04 13:22:26.000000 swarms-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:37.249424 swarms-0.3.5/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:37.253424 swarms-0.3.5/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:37.253424 swarms-0.3.5/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:37.253424 swarms-0.3.5/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 13:22:26.000000 swarms-0.3.5/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:22:37.253424 swarms-0.3.5/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:22:37.000000 swarms-0.3.5/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 13:22:37.000000 swarms-0.3.5/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:22:37.000000 swarms-0.3.5/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 13:22:37.000000 swarms-0.3.5/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 13:22:37.000000 swarms-0.3.5/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:17.346747 swarms-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 13:38:03.000000 swarms-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:38:17.346747 swarms-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 13:38:03.000000 swarms-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:38:17.350747 swarms-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-04 13:38:03.000000 swarms-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:17.342747 swarms-0.3.6/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:17.346747 swarms-0.3.6/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:17.346747 swarms-0.3.6/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:17.346747 swarms-0.3.6/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 13:38:03.000000 swarms-0.3.6/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:38:17.342747 swarms-0.3.6/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 13:38:17.000000 swarms-0.3.6/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 13:38:17.000000 swarms-0.3.6/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:38:17.000000 swarms-0.3.6/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 13:38:17.000000 swarms-0.3.6/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 13:38:17.000000 swarms-0.3.6/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.3.5/LICENSE` & `swarms-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/PKG-INFO` & `swarms-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.5
+Version: 0.3.6
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.5/README.md` & `swarms-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/setup.py` & `swarms-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.3.5',
+  version = '0.3.6',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.3.5/swarms/agents/swarms.py` & `swarms-0.3.6/swarms/agents/swarms.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from langchain.tools import BaseTool, DuckDuckGoSearchRun
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
 
 from langchain.tools.human.tool import HumanInputRun
 
 # from swarms.agents.workers.auto_agent import MultiModalVisualAgent
-from swarms.agents.workers import multimodal_agent_tool
+# from swarms.agents.workers import multimodal_agent_tool
 from swarms.tools.main import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
 from swarms.tools.main import math_tool
 
 
 openai_api_key = os.environ["OPENAI_API_KEY"]
 
 llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
@@ -229,15 +229,16 @@
 
     def initialize_llm(self):
         return ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=self.openai_api_key)
 
     def initialize_tools(self, llm):
         web_search = DuckDuckGoSearchRun()
         tools = [web_search, WriteFileTool(root_dir="./data"), ReadFileTool(root_dir="./data"), process_csv,
-                 multimodal_agent_tool, WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
+                #  multimodal_agent_tool, 
+                WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
                  Terminal, CodeWriter, CodeEditor, math_tool]
         return tools
 
     def initialize_vectorstore(self):
         embeddings_model = OpenAIEmbeddings()
         embedding_size = 1536
         index = faiss.IndexFlatL2(embedding_size)
```

### Comparing `swarms-0.3.5/swarms/agents/workers/agents.py` & `swarms-0.3.6/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/swarms/agents/workers/auto_agent.py` & `swarms-0.3.6/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.3.6/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/swarms/agents/workers/multi_modal.py` & `swarms-0.3.6/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/swarms/agents/workers/omni_agent.py` & `swarms-0.3.6/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.5/swarms.egg-info/PKG-INFO` & `swarms-0.3.6/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.5
+Version: 0.3.6
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.5/swarms.egg-info/requires.txt` & `swarms-0.3.6/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

