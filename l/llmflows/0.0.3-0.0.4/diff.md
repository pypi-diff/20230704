# Comparing `tmp/llmflows-0.0.3.tar.gz` & `tmp/llmflows-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.3.tar", last modified: Mon Jun 26 01:39:29 2023, max compression
+gzip compressed data, was "llmflows-0.0.4.tar", last modified: Tue Jul  4 05:41:52 2023, max compression
```

## Comparing `llmflows-0.0.3.tar` & `llmflows-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.484185 llmflows-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 01:39:13.000000 llmflows-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-26 01:39:29.484185 llmflows-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-06-26 01:39:13.000000 llmflows-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.476185 llmflows-0.0.3/llmflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/callbacks/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/async_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/async_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/flowstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/openai_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/prompts/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/vectorstores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/vectorstores/vector_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.476185 llmflows-0.0.3/llmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-26 01:39:13.000000 llmflows-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:39:29.484185 llmflows-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-04 05:41:41.000000 llmflows-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-04 05:41:52.589293 llmflows-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-04 05:41:41.000000 llmflows-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/async_base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/async_functional_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/callbacks/functional_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/functional_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/flows/vectorstore_flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.589293 llmflows-0.0.4/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/vector_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 05:41:41.000000 llmflows-0.0.4/llmflows/vectorstores/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:41:52.585293 llmflows-0.0.4/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 05:41:52.000000 llmflows-0.0.4/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-04 05:41:41.000000 llmflows-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:41:52.589293 llmflows-0.0.4/setup.cfg
```

### Comparing `llmflows-0.0.3/LICENSE` & `llmflows-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.3/PKG-INFO` & `llmflows-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.3
+Version: 0.0.4
 Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
 Author: Stoyan Stoyanov
 Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
 Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LLMFlows - Simple, Explicit and Transparent LLM Apps
+# LLMFlows - Simple, Explicit, and Transparent LLM Apps
 
 <p align="center">
   <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 ![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
@@ -30,27 +30,28 @@
 
 ## Installation
 You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
+## Documentation
+The full documentation including user guides and api reference can be found at readthedocs.
+
 ## Philosophy
 
 ### Simple
-We want to build a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.
+Our goal is to build a simple, well documented framework with a minimal set of classes and abstractions that allow users to build flexible LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.
+We want to create an explicit API enabling users to write clean, and readable code while being able to easily create complex flows of LLMs interacting with each other.
 
 ### Transparent
-Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts. Default prompts introduce unexpected behavior and behavior drift when models are updated. 
+We aim helping users have full transparency on their LLM-powered apps by providing traceable flows, and complete information for each component of the app making it easy to monitor, maintain, and debug.
 
-## Documentation
-The full documentation for LLMFlows can be found here.
 
 ## Usage
 Here is a minimal example of an LLM with a PromptTemplate:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
@@ -67,21 +68,17 @@
 ```
 
 While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
 With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
-from llmflows.flows.flow import Flow
-from llmflows.flows.flowstep import FlowStep
-from llmflows.llms.openai import OpenAI
-from llmflows.prompts.prompt_template import PromptTemplate
-
-# Create LLM
-open_ai_llm = OpenAI()
+from llmflows.flows import Flow, Flowstep
+from llmflows.llms import OpenAI
+from llmflows.prompts import PromptTemplate
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
     "What is a good song title of a soundtrack for a movie called {movie_title}?"
 )
 characters_template = PromptTemplate(
@@ -91,36 +88,36 @@
     "Write lyrics of a movie song called {song_title}. The main characters are"
     " {main_characters}"
 )
 
 # Create flowsteps
 flowstep1 = FlowStep(
     name="Flowstep 1",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=title_template,
     output_key="movie_title",
 )
 
 flowstep2 = FlowStep(
     name="Flowstep 2",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=song_template,
     output_key="song_title",
 )
 
 flowstep3 = FlowStep(
     name="Flowstep 3",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=characters_template,
     output_key="main_characters",
 )
 
 flowstep4 = FlowStep(
     name="Flowstep 4",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=lyrics_template,
     output_key="song_lyrics",
 )
 
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
```

### Comparing `llmflows-0.0.3/README.md` & `llmflows-0.0.4/llmflows.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# LLMFlows - Simple, Explicit and Transparent LLM Apps
+Metadata-Version: 2.1
+Name: llmflows
+Version: 0.0.4
+Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
+Author: Stoyan Stoyanov
+Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
+Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LLMFlows - Simple, Explicit, and Transparent LLM Apps
 
 <p align="center">
   <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 ![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
@@ -16,27 +30,28 @@
 
 ## Installation
 You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
+## Documentation
+The full documentation including user guides and api reference can be found at readthedocs.
+
 ## Philosophy
 
 ### Simple
-We want to build a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.
+Our goal is to build a simple, well documented framework with a minimal set of classes and abstractions that allow users to build flexible LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.
+We want to create an explicit API enabling users to write clean, and readable code while being able to easily create complex flows of LLMs interacting with each other.
 
 ### Transparent
-Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts. Default prompts introduce unexpected behavior and behavior drift when models are updated. 
+We aim helping users have full transparency on their LLM-powered apps by providing traceable flows, and complete information for each component of the app making it easy to monitor, maintain, and debug.
 
-## Documentation
-The full documentation for LLMFlows can be found here.
 
 ## Usage
 Here is a minimal example of an LLM with a PromptTemplate:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
@@ -53,21 +68,17 @@
 ```
 
 While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
 With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
-from llmflows.flows.flow import Flow
-from llmflows.flows.flowstep import FlowStep
-from llmflows.llms.openai import OpenAI
-from llmflows.prompts.prompt_template import PromptTemplate
-
-# Create LLM
-open_ai_llm = OpenAI()
+from llmflows.flows import Flow, Flowstep
+from llmflows.llms import OpenAI
+from llmflows.prompts import PromptTemplate
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
     "What is a good song title of a soundtrack for a movie called {movie_title}?"
 )
 characters_template = PromptTemplate(
@@ -77,36 +88,36 @@
     "Write lyrics of a movie song called {song_title}. The main characters are"
     " {main_characters}"
 )
 
 # Create flowsteps
 flowstep1 = FlowStep(
     name="Flowstep 1",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=title_template,
     output_key="movie_title",
 )
 
 flowstep2 = FlowStep(
     name="Flowstep 2",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=song_template,
     output_key="song_title",
 )
 
 flowstep3 = FlowStep(
     name="Flowstep 3",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=characters_template,
     output_key="main_characters",
 )
 
 flowstep4 = FlowStep(
     name="Flowstep 4",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=lyrics_template,
     output_key="song_lyrics",
 )
 
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
```

### Comparing `llmflows-0.0.3/llmflows/callbacks/callback.py` & `llmflows-0.0.4/llmflows/callbacks/functional_callback.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,18 @@
 """
-This module provides the Callback and FunctionalCallback classes.
-
-The Callback class is designed to be subclassed by users who want to create their
-own custom callbacks for different stages of a FlowStep execution.
+This module provides FunctionalCallback class.
 
 The FunctionalCallback class allows users to provide specific functions to be
 executed at each stage of a FlowStep execution, without the need for subclassing.
 """
 
 from typing import Callable, Optional, Any
+from llmflows.callbacks.base_callback import BaseCallback
 
-
-class Callback:
-    """
-    Represents a callback to be invoked at different stages of a FlowStep execution.
-
-    The user can subclass this and override the methods corresponding to
-    the stages where they want their callback logic to be executed.
-    """
-    def on_start(self, inputs: dict[str, Any]):
-        """
-        Method invoked at the start of the FlowStep's execution. Can be overridden
-        for custom logic.
-
-        Args:
-            inputs (dict[str, Any]): Inputs provided to the FlowStep at the start.
-        """
-
-    def on_results(self, results: dict[str, Any]):
-        """
-        Method invoked when the FlowStep produces results. Can be overridden for
-        custom logic.
-
-        Args:
-            results (dict[str, Any]): Results produced by the FlowStep's execution.
-        """
-
-    def on_end(self, execution_info: dict[str, Any]):
-        """
-        Method invoked at the end of the FlowStep's execution. Can be overridden for
-        custom logic.
-
-        Args:
-            execution_info (dict[str, Any]): Information about the FlowStep's execution.
-        """
-
-    def on_error(self, error: Exception):
-        """
-        Method invoked when an error occurs during the FlowStep's execution. Can be 
-        overridden for custom error handling.
-
-        Args:
-            error (Exception): The error that occurred during execution.
-        """
-
-
-class FunctionalCallback(Callback):
+class FunctionalCallback(BaseCallback):
     """
     Represents a callback to be invoked at different stages of a FlowStep execution,
     with a specific function provided for each stage.
 
     Args:
         on_start_fn (Optional[Callable[[dict[str, Any]], None]]): The function to be
             invoked at the start stage.
```

### Comparing `llmflows-0.0.3/llmflows/llms/llm.py` & `llmflows-0.0.4/llmflows/llms/llm.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,17 +8,32 @@
 from abc import ABC
 
 
 class BaseLLM(ABC):
     """
     Base class for all Large Language Models (LLMs). Each specific LLM should extend 
     this class.
+
+    Args:
+        model (str): The model name used in the LLM class.
     """
 
     def __init__(self, model: str):
+        self.model = model
+
+    def generate(self):
         """
-        Initializes the BaseLLM with a model.
+        Generates text from the LLM.
 
-        Args:
-            model (str): The model name used in the LLM class.
+        Raises:
+            NotImplementedError: If the LLM does not implement the generate method.
         """
-        self.model = model
+        raise NotImplementedError
+
+    async def generate_async(self):
+        """
+        Generates text from the LLM asynchronously.
+
+        Raises:
+            NotImplementedError: If the LLM does not implement the generate_async method.
+        """
+        raise NotImplementedError
```

### Comparing `llmflows-0.0.3/llmflows/llms/llm_utils.py` & `llmflows-0.0.4/llmflows/llms/llm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
             APIError,
             Timeout,
             RateLimitError,
             APIConnectionError,
             ServiceUnavailableError,
         ) as error:
             num_retries += 1
-            print("Retrying: Attempt %s. Error: %s", num_retries, str(error))
             logging.warning("Retrying: Attempt %s. Error: %s", num_retries, str(error))
             time.sleep(min(delay, max_delay))
             delay *= delay_multiplier
 
         except (InvalidRequestError, AuthenticationError) as error:
             logging.error(
                 "An error occurred that cannot be resolved by retrying. Error: %s",
@@ -109,15 +108,14 @@
             APIError,
             Timeout,
             RateLimitError,
             APIConnectionError,
             ServiceUnavailableError,
         ) as error:
             num_retries += 1
-
             logging.warning("Retrying: Attempt %s. Error: %s", num_retries, str(error))
             await asyncio.sleep(min(delay, max_delay))
             delay *= delay_multiplier
 
         except (InvalidRequestError, AuthenticationError) as error:
             logging.error(
                 "An error occurred that cannot be resolved by retrying. Error: %s",
```

### Comparing `llmflows-0.0.3/llmflows/llms/openai.py` & `llmflows-0.0.4/llmflows/llms/openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,21 @@
     """
     A class for interacting with the OpenAI completion API.
 
     Inherits from BaseLLM.
 
     Uses the specified OpenAI model and parameters for interacting with the OpenAI API.
 
+    Args:
+        model (str): The name of the OpenAI model to use.
+        temperature (float): The temperature to use for text generation.
+        max_tokens (int): The maximum number of tokens to generate.
+        max_retries (int): The maximum number of retries for generating tokens.
+
     Attributes:
-        api_key (str): OpenAI API key, retrieved from environment variables.
-        model (str): Identifier of the OpenAI model to use.
         temperature (float): The temperature to use for text generation.
         max_tokens (int): The maximum number of tokens to generate.
         max_retries (int): The maximum number of retries for generating tokens.
     """
 
     def __init__(
         self,
@@ -34,15 +38,15 @@
         max_tokens: int = 500,
         max_retries: int = 3,
     ):
         super().__init__(model)
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.max_retries = max_retries
-        self.api_key = os.environ["OPENAI_API_KEY"]
+        self._api_key = os.environ["OPENAI_API_KEY"]
 
     def perepare_results(self, model_outputs, retries) -> tuple[str, dict, dict]:
         """
         Formats results after generation.
 
         Args:
             model_outputs: Raw output after model generation.
```

### Comparing `llmflows-0.0.3/llmflows/llms/openai_chat.py` & `llmflows-0.0.4/llmflows/llms/openai_chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,44 @@
 
     Inherits from BaseLLM.
 
     Uses the specified OpenAI model and parameters for interacting with the OpenAI chat
     API, and provides methods to add, remove, replace messages, update system prompts,
     and generate responses.
 
-    Attributes:
-        api_key (str): The API key to use for authentication.
+    Args:
+        system_prompt (str): The system prompt to use for the chat model.
         model (str): The name of the OpenAI model to use.
         temperature (float): The temperature to use for text generation.
         max_messages (int): The maximum number of messages to send to the chat API.
         max_tokens (int): The maximum number of tokens to generate.
         max_retries (int): The maximum number of retries for generating tokens.
         verbose (bool): Whether to print debug information.
+
+    Attributes:
+        temperature (float): The temperature to use for text generation.
+        max_messages (int): The maximum number of messages to send to the chat API.
+        max_tokens (int): The maximum number of tokens to generate.
+        max_retries (int): The maximum number of retries for generating tokens.
         messages (list[dict[str, str]]): A list of messages sent to the chat API.
+        verbose (bool): Whether to print debug information.
     """
 
     def __init__(
         self,
         system_prompt: str = "",
         model: str = "gpt-3.5-turbo",
         temperature: float = 0.7,
         max_messages: int = 0,
         max_tokens: int = 250,
         max_retries: int = 3,
         verbose: bool = False,
     ):
         super().__init__(model)
-        self.api_key = os.environ["OPENAI_API_KEY"]
+        self._api_key = os.environ["OPENAI_API_KEY"]
         self.temperature = temperature
         self.max_messages = max_messages
         self.max_tokens = max_tokens
         self.max_retries = max_retries
         self.messages = [{"role": "system", "content": system_prompt}]
         self.verbose = verbose
 
@@ -55,14 +62,27 @@
         """
         Returns the conversation history.
         """
         return self._messages
 
     @messages.setter
     def messages(self, value):
+        """
+        Sets the conversation history.
+
+        Each message in the list should be a dictionary containing 
+        "role" and "content" keys.
+
+        Args:
+            value (list): A list of message dictionaries.
+
+        Raises:
+            ValueError: If the provided value is not a list or if any 
+            dictionary in the list is not a valid message.
+        """
         if not isinstance(value, list):
             raise ValueError("messages must be a list of dicts")
         for item in value:
             self.validate_message(item)
         self._messages = value
 
     def add_message(self, message_str: str, role: str = "user") -> list[dict[str, str]]:
@@ -195,19 +215,14 @@
         """
         Sends the messages to the OpenAI chat API and returns a chat message response.
 
         Returns:
             A tuple containing the generated chat message, raw output data, and model
                 configuration.
         """
-        if self.verbose:
-            print("[SYSTEM] Messages sent to OpenAI chat API:")
-            for msg in self.messages:
-                print(msg)
-            print("---------")
 
         completion, retries = call_with_retry(
             api_obj=openai.ChatCompletion,
             max_retries=self.max_retries,
             model=self.model,
             messages=self.messages,
             max_tokens=self.max_tokens,
@@ -227,19 +242,14 @@
         Async function that sends the messages to the OpenAI chat API and returns
         a chat message response.
 
         Returns:
             A tuple containing the generated chat message, raw output data, and model
                 configuration.
         """
-        if self.verbose:
-            print("[SYSTEM] Messages sent to OpenAI chat API:")
-            for msg in self.messages:
-                print(msg)
-            print("---------")
 
         completion, retries = await async_call_with_retry(
             api_obj=openai.ChatCompletion,
             max_retries=self.max_retries,
             model=self.model,
             messages=self.messages,
             max_tokens=self.max_tokens,
```

### Comparing `llmflows-0.0.3/llmflows/llms/openai_embeddings.py` & `llmflows-0.0.4/llmflows/llms/openai_embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,21 @@
     embeddings API. Adds embeddings to a single VectorDoc or a list of VectorDoc 
     classes, based on the text in the VectorDoc.
 
     Args:
         model (str): The name of the OpenAI model to use.
 
     Attributes:
-        api_key (str): The API key to use for authentication.
-        model (str): The name of the OpenAI model to use.
+        _api_key (str): The API key to use for authentication.
         max_retries (int): The maximum number of retries for generating embeddings.
     """
 
     def __init__(self, model: str = "text-embedding-ada-002", max_retries: int = 3):
         super().__init__(model)
-        self.api_key = os.getenv("OPENAI_API_KEY")
-        self.model = model
+        self._api_key = os.getenv("OPENAI_API_KEY")
         self.max_retries = max_retries
 
     def generate(
         self, docs: Union[VectorDoc, list[VectorDoc]]
     ) -> Union[VectorDoc, list[VectorDoc]]:
         """
         Adds embeddings to a single or list of VectorDocs using OpenAI's service.
```

### Comparing `llmflows-0.0.3/llmflows/prompts/prompt_template.py` & `llmflows-0.0.4/llmflows/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.3/llmflows/vectorstores/pinecone.py` & `llmflows-0.0.4/llmflows/vectorstores/pinecone.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,91 @@
 """
 Module to interact with Pinecone, a vector database service.
 
 This module contains a class `Pinecone` which provides several methods to
 interact with the Pinecone vector database service.
 """
 
-import pinecone # pylint: disable=import-error
+import pinecone  # pylint: disable=import-error
 from llmflows.vectorstores.vector_doc import VectorDoc
+from llmflows.vectorstores.vector_store import VectorStore
 
 
-class Pinecone:
+class Pinecone(VectorStore):
     """
     Interact with Pinecone, a vector database service.
 
     This class has methods to initialize the Pinecone client, describe the index,
     search the index for similar vectors, and insert or update vectors in the index.
 
     Args:
         index_name (str): The name of the index to use.
-        api_key (str): The API key to use for authentication.
+        api_key (str): The Pinecone API key to use for authentication.
         environment (str): The environment to use, e.g. "production" or "development".
+    
+    Attributes:
+        index_name (str): The name of the index to use.
+        environment (str): The pinecone environment to use.
     """
 
     def __init__(self, index_name: str, api_key: str, environment: str):
         self.index_name = index_name
-        self.api_key = api_key
+        self._api_key = api_key
         self.environment = environment
         self._init_client()
 
+    def _prepare_results(self, search_result) -> tuple[list, dict, dict]:
+        """
+        Format the search results for the Pinecone vector store client.
+
+        Args:
+            search_result (dict): The search result returned by the Pinecone search.
+
+        Returns:
+            A tuple containing list of matches, the call parameters, and the pinecone 
+                config.
+        """
+        search_results = search_result["matches"]
+
+        call_data = {
+            "raw_outputs": search_result,
+        }
+
+        config = {
+            "environment": self.environment,
+            "index_name": self.index_name
+        }
+
+        return search_results, call_data, config
+
     def _init_client(self):
-        pinecone.init(api_key=self.api_key, environment=self.environment)
+        pinecone.init(api_key=self._api_key, environment=self.environment)
         self.index = pinecone.Index(self.index_name)
         self.describe()
 
     def describe(self):
         """Describe the index."""
         print(self.index.describe_index_stats())
 
-    def search(self, query: VectorDoc, top_k: int) -> list[dict]:
+    def search(self, query: VectorDoc, top_k: int) -> tuple[list, dict, dict]:
         """
         Search the index for similar vectors.
 
         Args:
             query (VectorDoc): The query vector to search for.
             top_k (int): The number of results to return.
 
         Returns:
             list[dict]: A list of dictionaries representing the search results.
         """
         query_embedding = query.embedding
         search_result = self.index.query(
             query_embedding, top_k=top_k, include_metadata=True
         )
-        return search_result["matches"]
+        return self._prepare_results(search_result)
 
     def upsert(self, docs: list[VectorDoc]):
         """Insert or update vectors in the index.
 
         Args:
             docs (list[VectorDoc]): VectorDoc objects to insert or update.
         """
```

### Comparing `llmflows-0.0.3/llmflows/vectorstores/vector_doc.py` & `llmflows-0.0.4/llmflows/vectorstores/vector_doc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module defines the VectorDoc class which is used to represent a document 
 with an optional embedding and metadata.
 """
 
-from typing import Optional
+from typing import Union
 from uuid import uuid4
 
 
 class VectorDoc:
     """
     Class representing a document with an optional embedding and metadata.
 
@@ -23,17 +23,17 @@
         doc (str): The document text.
         metadata (dict): Optional metadata for the document.
     """
 
     def __init__(
         self,
         doc: str,
-        doc_id: str = None,
-        metadata: Optional[dict] = None,
-        embedding: Optional[list] = None,
+        doc_id: Union[str, None] = None,
+        metadata: Union[dict, None] = None,
+        embedding: Union[list, None] = None,
     ):
         self.doc_id = doc_id if doc_id is not None else str(uuid4())
         self.doc = doc
         self.metadata = metadata if metadata is not None else {}
         self._embedding = embedding
 
     @property
@@ -41,15 +41,15 @@
         """
         The embedding for the document.
 
         Raises:
             ValueError: If the embedding for the document has not been set.
 
         Returns:
-            list: The embedding of the document.
+            The embedding of the document.
         """
         if self._embedding is not None:
             return self._embedding
         raise ValueError(
             "The embedding for this VectorDoc has not been set.\nDoc Id:"
             f" {self.doc_id}\nDoc:{self.doc}"
         )
```

### Comparing `llmflows-0.0.3/llmflows.egg-info/PKG-INFO` & `llmflows-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: llmflows
-Version: 0.0.3
-Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
-Author: Stoyan Stoyanov
-Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
-Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# LLMFlows - Simple, Explicit and Transparent LLM Apps
+# LLMFlows - Simple, Explicit, and Transparent LLM Apps
 
 <p align="center">
   <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 ![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
@@ -30,27 +16,28 @@
 
 ## Installation
 You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
+## Documentation
+The full documentation including user guides and api reference can be found at readthedocs.
+
 ## Philosophy
 
 ### Simple
-We want to build a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.
+Our goal is to build a simple, well documented framework with a minimal set of classes and abstractions that allow users to build flexible LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.
+We want to create an explicit API enabling users to write clean, and readable code while being able to easily create complex flows of LLMs interacting with each other.
 
 ### Transparent
-Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts. Default prompts introduce unexpected behavior and behavior drift when models are updated. 
+We aim helping users have full transparency on their LLM-powered apps by providing traceable flows, and complete information for each component of the app making it easy to monitor, maintain, and debug.
 
-## Documentation
-The full documentation for LLMFlows can be found here.
 
 ## Usage
 Here is a minimal example of an LLM with a PromptTemplate:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
@@ -67,21 +54,17 @@
 ```
 
 While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
 With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
-from llmflows.flows.flow import Flow
-from llmflows.flows.flowstep import FlowStep
-from llmflows.llms.openai import OpenAI
-from llmflows.prompts.prompt_template import PromptTemplate
-
-# Create LLM
-open_ai_llm = OpenAI()
+from llmflows.flows import Flow, Flowstep
+from llmflows.llms import OpenAI
+from llmflows.prompts import PromptTemplate
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
     "What is a good song title of a soundtrack for a movie called {movie_title}?"
 )
 characters_template = PromptTemplate(
@@ -91,36 +74,36 @@
     "Write lyrics of a movie song called {song_title}. The main characters are"
     " {main_characters}"
 )
 
 # Create flowsteps
 flowstep1 = FlowStep(
     name="Flowstep 1",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=title_template,
     output_key="movie_title",
 )
 
 flowstep2 = FlowStep(
     name="Flowstep 2",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=song_template,
     output_key="song_title",
 )
 
 flowstep3 = FlowStep(
     name="Flowstep 3",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=characters_template,
     output_key="main_characters",
 )
 
 flowstep4 = FlowStep(
     name="Flowstep 4",
-    llm=open_ai_llm,
+    llm=OpenAI(),
     prompt_template=lyrics_template,
     output_key="song_lyrics",
 )
 
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
```

### Comparing `llmflows-0.0.3/pyproject.toml` & `llmflows-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
 description = "LLMFlows - Simple, Explicit and Transparent LLM Apps"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

