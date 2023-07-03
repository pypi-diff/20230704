# Comparing `tmp/swarms-0.1.1.tar.gz` & `tmp/swarms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.1.1.tar", last modified: Mon Jul  3 22:43:26 2023, max compression
+gzip compressed data, was "swarms-0.1.2.tar", last modified: Mon Jul  3 22:53:21 2023, max compression
```

## Comparing `swarms-0.1.1.tar` & `swarms-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.853130 swarms-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:43:17.000000 swarms-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:43:26.853130 swarms-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:43:17.000000 swarms-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:43:26.853130 swarms-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:43:17.000000 swarms-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.849130 swarms-0.1.1/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:43:17.000000 swarms-0.1.1/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.853130 swarms-0.1.1/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:17.000000 swarms-0.1.1/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-03 22:43:17.000000 swarms-0.1.1/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.849130 swarms-0.1.1/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:53:11.000000 swarms-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:53:21.726582 swarms-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:53:11.000000 swarms-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:53:21.726582 swarms-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:53:11.000000 swarms-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:53:11.000000 swarms-0.1.2/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:11.000000 swarms-0.1.2/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15165 2023-07-03 22:53:11.000000 swarms-0.1.2/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:53:21.726582 swarms-0.1.2/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:53:21.000000 swarms-0.1.2/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.1.1/LICENSE` & `swarms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.1.1/PKG-INFO` & `swarms-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.1
+Version: 0.1.2
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.1/README.md` & `swarms-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.1.1/setup.py` & `swarms-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.1.1',
+  version = '0.1.2',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.1.1/swarms/agents/swarms.py` & `swarms-0.1.2/swarms/agents/swarms.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,48 +51,31 @@
 ROOT_DIR = "./data/"
 
 from langchain.tools import BaseTool, DuckDuckGoSearchRun
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
 
 from langchain.tools.human.tool import HumanInputRun
-from swarms.agents.workers.auto_agent import MultiModalVisualAgent
-from swarms.tools.main import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
 
+# from swarms.agents.workers.auto_agent import MultiModalVisualAgent
+from swarms.agents.workers.auto_agent import multimodal_agent_tool
+from swarms.tools.main import Terminal, CodeWriter, CodeEditor, process_csv, WebpageQATool
 from swarms.tools.main import math_tool
 
 
 openai_api_key = os.environ["OPENAI_API_KEY"]
 
 llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
 
 
-####################### TOOLS
-class MultiModalVisualAgentTool(BaseTool):
-    name = "multi_visual_agent"
-    description = "Multi-Modal Visual agent tool"
-
-    def __init__(self, agent: MultiModalVisualAgent):
-        self.agent = agent
-    
-    def _run(self, text: str) -> str:
-        #run the multi-modal visual agent with the give task
-        return self.agent.run_text(text)
-
-
-
 query_website_tool = WebpageQATool(qa_chain=load_qa_with_sources_chain(llm))
 
 # !pip install duckduckgo_search
 web_search = DuckDuckGoSearchRun()
 
-#======>
-multimodal_agent_tool = MultiModalVisualAgentTool(MultiModalVisualAgent)
-
-
 
 tools = [
     
     web_search,
     WriteFileTool(root_dir="./data"),
     ReadFileTool(root_dir="./data"),
```

### Comparing `swarms-0.1.1/swarms.egg-info/PKG-INFO` & `swarms-0.1.2/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.1
+Version: 0.1.2
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.1/swarms.egg-info/requires.txt` & `swarms-0.1.2/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

