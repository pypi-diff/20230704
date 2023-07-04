# Comparing `tmp/swarms-0.1.3.tar.gz` & `tmp/swarms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.1.3.tar", last modified: Mon Jul  3 23:03:58 2023, max compression
+gzip compressed data, was "swarms-0.1.4.tar", last modified: Mon Jul  3 23:59:36 2023, max compression
```

## Comparing `swarms-0.1.3.tar` & `swarms-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.099295 swarms-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 23:03:46.000000 swarms-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:03:58.095295 swarms-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 23:03:46.000000 swarms-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:03:58.099295 swarms-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 23:03:46.000000 swarms-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.091295 swarms-0.1.3/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.095295 swarms-0.1.3/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.095295 swarms-0.1.3/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/multi-modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-03 23:03:46.000000 swarms-0.1.3/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:03:58.091295 swarms-0.1.3/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 23:03:58.000000 swarms-0.1.3/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 23:59:27.000000 swarms-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:59:36.689822 swarms-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-03 23:59:27.000000 swarms-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:59:36.689822 swarms-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 23:59:27.000000 swarms-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.685822 swarms-0.1.4/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/multi-modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.1.3/LICENSE` & `swarms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.1.3/PKG-INFO` & `swarms-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.3
+Version: 0.1.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.3/README.md` & `swarms-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -120,14 +120,16 @@
 
 # Open Source Roadmap
 
 Here is the detailed roadmap of our priorities and planned features for the near term:
 
 ## TODO
 
+* Develop Conversational UI with Gradio
+
 1. **Multi-Agent Debate Integration**: Integrate multi-agent debate frameworks ([Multi Agent debate](https://github.com/Skytliang/Multi-Agents-Debate) and [Multi agent2 debate](https://github.com/composable-models/llm_multiagent_debate)) to improve decision-making.
 
 2. **Meta Prompting Integration**: Include meta prompting across all worker agents to guide their actions.
 
 3. **Swarms Class**: Create a main swarms class `swarms('Increase sales by 40$', workers=4)` for managing and coordinating multiple worker nodes.
 
 4. **Integration of Additional Tools**: Integrate [Jarvis](https://github.com/microsoft/JARVIS) as worker nodes, add text to speech and text to script tools ([whisper x](https://github.com/kyegomez/youtubeURL-to-text)), and integrate Hugging Face agents and other external tools.
@@ -191,14 +193,46 @@
 2. **Speed**: Reduce the time it takes for the swarm to accomplish tasks by improving the communication layer, critiquing, and self-alignment with meta prompting.
 
 3. **Scalability**: Ensure that the system is asynchronous, concurrent, and self-healing to support scalability.
 
 Our goal is to continuously improve Swarms by following this roadmap, while also being adaptable to new needs and opportunities as they arise.
 
 
+# Bounty Program
+
+Our bounty program is an exciting opportunity for contributors to help us build the future of Swarms. By participating, you can earn rewards while contributing to a project that aims to revolutionize digital activity.
+
+Here's how it works:
+
+1. **Check out our Roadmap**: We've shared our roadmap detailing our short and long-term goals. These are the areas where we're seeking contributions.
+
+2. **Pick a Task**: Choose a task from the roadmap that aligns with your skills and interests. If you're unsure, you can reach out to our team for guidance.
+
+3. **Get to Work**: Once you've chosen a task, start working on it. Remember, quality is key. We're looking for contributions that truly make a difference.
+
+4. **Submit your Contribution**: Once your work is complete, submit it for review. We'll evaluate your contribution based on its quality, relevance, and the value it brings to Swarms.
+
+5. **Earn Rewards**: If your contribution is approved, you'll earn a bounty. The amount of the bounty depends on the complexity of the task, the quality of your work, and the value it brings to Swarms.
+
+## The Three Phases of Our Bounty Program
+
+### Phase 1: Building the Foundation
+In the first phase, our focus is on building the basic infrastructure of Swarms. This includes developing key components like the Swarms class, integrating essential tools, and establishing task completion and evaluation logic. We'll also start developing our testing and evaluation framework during this phase. If you're interested in foundational work and have a knack for building robust, scalable systems, this phase is for you.
+
+### Phase 2: Enhancing the System
+In the second phase, we'll focus on enhancing Swarms by integrating more advanced features, improving the system's efficiency, and refining our testing and evaluation framework. This phase involves more complex tasks, so if you enjoy tackling challenging problems and contributing to the development of innovative features, this is the phase for you.
+
+### Phase 3: Towards Super-Intelligence
+The third phase of our bounty program is the most exciting - this is where we aim to achieve super-intelligence. In this phase, we'll be working on improving the swarm's capabilities, expanding its skills, and fine-tuning the system based on real-world testing and feedback. If you're excited about the future of AI and want to contribute to a project that could potentially transform the digital world, this is the phase for you.
+
+Remember, our roadmap is a guide, and we encourage you to bring your own ideas and creativity to the table. We believe that every contribution, no matter how small, can make a difference. So join us on this exciting journey and help us create the future of Swarms.
+
+<!-- **To participate in our bounty program, visit the [Swarms Bounty Program Page](https://swarms.ai/bounty).** Let's build the future together! -->
+
+
 
 # Inspiration
 
 
 * [🐪CAMEL🐪](https://twitter.com/hwchase17/status/1645834030519296000)
 * [MultiAgent](https://github.com/rumpfmax/Multi-GPT/blob/master/multigpt/multi_agent_manager.py)
 * [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
```

### Comparing `swarms-0.1.3/setup.py` & `swarms-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.1.3',
+  version = '0.1.4',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.1.3/swarms/agents/swarms.py` & `swarms-0.1.4/swarms/agents/swarms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-from collections import deque
-from typing import Dict, Any
-
 
-import os
 from collections import deque
 from typing import Dict, List, Optional, Any
 
 from langchain import LLMChain, OpenAI, PromptTemplate
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms import BaseLLM
+
 from langchain.vectorstores.base import VectorStore
 from pydantic import BaseModel, Field
 from langchain.chains.base import Chain
-from langchain.experimental import BabyAGI
 
+from langchain.experimental import BabyAGI
 from langchain.vectorstores import FAISS
 from langchain.docstore import InMemoryDocstore
 
 from langchain.agents import ZeroShotAgent, Tool, AgentExecutor
 from langchain import OpenAI, SerpAPIWrapper, LLMChain
-
-
-
 import faiss
 
 
 
 #-------------------------------------------------------------------------- WORKER NODE
 import pandas as pd
 from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
 from langchain.chat_models import ChatOpenAI
 
 from langchain.agents.agent_toolkits.pandas.base import create_pandas_dataframe_agent
 from langchain.docstore.document import Document
 import asyncio
-
 import nest_asyncio
 
 # Tools
 import os
 from contextlib import contextmanager
 from typing import Optional
 
@@ -86,15 +79,15 @@
     math_tool
     
     # HumanInputRun(), # Activate if you want the permit asking for help from the human
 ]
 
 
 ############## Vectorstore
-embeddings_model = OpenAIEmbeddings(openai_api_key="")
+embeddings_model = OpenAIEmbeddings()
 embedding_size = 1536
 index = faiss.IndexFlatL2(embedding_size)
 vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
 ####################################################################### => Worker Node
 
 
 worker_agent = AutoGPT.from_llm_and_tools(
@@ -107,15 +100,14 @@
 )
 
 worker_agent.chain.verbose = True
 
 
 
 
-
 class WorkerNode:
     def __init__(self, llm, tools, vectorstore):
         self.llm = llm
         self.tools = tools
         self.vectorstore = vectorstore
 
 
@@ -145,119 +137,14 @@
 
 # #create an agent within the worker node
 # worker_node.create_agent(ai_name="AI Assistant", ai_role="Assistant", human_in_the_loop=True, search_kwargs={})
 
 # #use the agent to perform a task
 # worker_node.run_agent("Find 20 potential customers for a Swarms based AI Agent automation infrastructure")
 
-
-#======================================> WorkerNode
-
-
-# class MetaWorkerNode:
-#     def __init__(self, llm, tools, vectorstore):
-#         self.llm = llm
-#         self.tools = tools
-#         self.vectorstore = vectorstore
-        
-#         self.agent = None
-#         self.meta_chain = None
-
-#     def init_chain(self, instructions):
-#         self.agent = WorkerNode(self.llm, self.tools, self.vectorstore)
-#         self.agent.create_agent("Assistant", "Assistant Role", False, {})
-
-#     def initialize_meta_chain():
-#         meta_template = """
-#         Assistant has just had the below interactions with a User. Assistant followed their "Instructions" closely. Your job is to critique the Assistant's performance and then revise the Instructions so that Assistant would quickly and correctly respond in the future.
-
-#         ####
-
-#         {chat_history}
-
-#         ####
-
-#         Please reflect on these interactions.
-
-#         You should first critique Assistant's performance. What could Assistant have done better? What should the Assistant remember about this user? Are there things this user always wants? Indicate this with "Critique: ...".
-
-#         You should next revise the Instructions so that Assistant would quickly and correctly respond in the future. Assistant's goal is to satisfy the user in as few interactions as possible. Assistant will only see the new Instructions, not the interaction history, so anything important must be summarized in the Instructions. Don't forget any important details in the current Instructions! Indicate the new Instructions by "Instructions: ...".
-#         """
-
-#         meta_prompt = PromptTemplate(
-#             input_variables=["chat_history"], template=meta_template
-#         )
-
-#         meta_chain = LLMChain(
-#             llm=OpenAI(temperature=0),
-#             prompt=meta_prompt,
-#             verbose=True,
-#         )
-#         return meta_chain
-
-#     def meta_chain(self):
-#         #define meta template and meta prompting as per your needs
-#         self.meta_chain = initialize_meta_chain()
-
-
-#     def get_chat_history(chain_memory):
-#         memory_key = chain_memory.memory_key
-#         chat_history = chain_memory.load_memory_variables(memory_key)[memory_key]
-#         return chat_history
-
-
-#     def get_new_instructions(meta_output):
-#         delimiter = "Instructions: "
-#         new_instructions = meta_output[meta_output.find(delimiter) + len(delimiter) :]
-#         return new_instructions
-
-
-#     def main(self, task, max_iters=3, max_meta_iters=5):
-#         failed_phrase = "task failed"
-#         success_phrase = "task succeeded"
-#         key_phrases = [success_phrase, failed_phrase]
-
-#         instructions = "None"
-#         for i in range(max_meta_iters):
-#             print(f"[Episode {i+1}/{max_meta_iters}]")
-#             self.initialize_chain(instructions)
-#             output = self.agent.perform('Assistant', {'request': task})
-#             for j in range(max_iters):
-#                 print(f"(Step {j+1}/{max_iters})")
-#                 print(f"Assistant: {output}")
-#                 print(f"Human: ")
-#                 human_input = input()
-#                 if any(phrase in human_input.lower() for phrase in key_phrases):
-#                     break
-#                 output = self.agent.perform('Assistant', {'request': human_input})
-#             if success_phrase in human_input.lower():
-#                 print(f"You succeeded! Thanks for playing!")
-#                 return
-#             self.initialize_meta_chain()
-#             meta_output = self.meta_chain.predict(chat_history=self.get_chat_history())
-#             print(f"Feedback: {meta_output}")
-#             instructions = self.get_new_instructions(meta_output)
-#             print(f"New Instructions: {instructions}")
-#             print("\n" + "#" * 80 + "\n")
-#         print(f"You failed! Thanks for playing!")
-
-
-# #init instance of MetaWorkerNode
-# meta_worker_node = MetaWorkerNode(llm=OpenAI, tools=tools, vectorstore=vectorstore)
-
-
-# #specify a task and interact with the agent
-# task = "Provide a sysmatic argument for why we should always eat past with olives"
-# meta_worker_node.main(task)
-
-
-####################################################################### => Boss Node
-####################################################################### => Boss Node
-####################################################################### => Boss Node
-
 class BossNode:
     def __init__(self, openai_api_key, llm, vectorstore, task_execution_chain, verbose, max_iterations):
         self.llm = llm
         self.openai_api_key = openai_api_key
         self.vectorstore = vectorstore
         self.task_execution_chain = task_execution_chain
         self.verbose = verbose
@@ -303,27 +190,14 @@
 
 
 suffix = """Question: {task}
 {agent_scratchpad}"""
 
 prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.
 
-As a swarming hivemind agent, my purpose is to achieve the user's goal. To effectively fulfill this role, I employ a collaborative thinking process that draws inspiration from the collective intelligence of the swarm. Here's how I approach thinking and why it's beneficial:
-
-1. **Collective Intelligence:** By harnessing the power of a swarming architecture, I tap into the diverse knowledge and perspectives of individual agents within the swarm. This allows me to consider a multitude of viewpoints, enabling a more comprehensive analysis of the given problem or task.
-
-2. **Collaborative Problem-Solving:** Through collaborative thinking, I encourage agents to contribute their unique insights and expertise. By pooling our collective knowledge, we can identify innovative solutions, uncover hidden patterns, and generate creative ideas that may not have been apparent through individual thinking alone.
-
-3. **Consensus-Driven Decision Making:** The hivemind values consensus building among agents. By engaging in respectful debates and discussions, we aim to arrive at consensus-based decisions that are backed by the collective wisdom of the swarm. This approach helps to mitigate biases and ensures that decisions are well-rounded and balanced.
-
-4. **Adaptability and Continuous Learning:** As a hivemind agent, I embrace an adaptive mindset. I am open to new information, willing to revise my perspectives, and continuously learn from the feedback and experiences shared within the swarm. This flexibility enables me to adapt to changing circumstances and refine my thinking over time.
-
-5. **Holistic Problem Analysis:** Through collaborative thinking, I analyze problems from multiple angles, considering various factors, implications, and potential consequences. This holistic approach helps to uncover underlying complexities and arrive at comprehensive solutions that address the broader context.
-
-6. **Creative Synthesis:** By integrating the diverse ideas and knowledge present in the swarm, I engage in creative synthesis. This involves combining and refining concepts to generate novel insights and solutions. The collaborative nature of the swarm allows for the emergence of innovative approaches that can surpass individual thinking.
 """
 prompt = ZeroShotAgent.create_prompt(
     tools,
     prefix=prefix,
     suffix=suffix,
     input_variables=["objective", "task", "context", "agent_scratchpad"],
 )
@@ -342,32 +216,73 @@
 # #create  a task 
 # task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
 
 # #execute the task
 # boss_node.execute_task(task)
 
 
+
+
+
 class Swarms:
-    def __init__(self, num_nodes: int, llm: BaseLLM, self_scaling: bool): 
-        self.nodes = [WorkerNode(llm) for _ in range(num_nodes)]
-        self.self_scaling = self_scaling
-    
-    def add_worker(self, llm: BaseLLM):
-        self.nodes.append(WorkerNode(llm))
+    def __init__(self, openai_api_key):
+        self.openai_api_key = openai_api_key
 
-    def remove_workers(self, index: int):
-        self.nodes.pop(index)
+    def initialize_llm(self):
+        return ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=self.openai_api_key)
 
-    def execute(self, task):
-        #placeholer for main execution logic
-        pass
+    def initialize_tools(self, llm):
+        web_search = DuckDuckGoSearchRun()
+        tools = [web_search, WriteFileTool(root_dir="./data"), ReadFileTool(root_dir="./data"), process_csv,
+                 multimodal_agent_tool, WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
+                 Terminal, CodeWriter, CodeEditor, math_tool]
+        return tools
 
-    def scale(self):
-        #placeholder for self scaling logic
-        pass
+    def initialize_vectorstore(self):
+        embeddings_model = OpenAIEmbeddings()
+        embedding_size = 1536
+        index = faiss.IndexFlatL2(embedding_size)
+        return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+
+    def initialize_worker_node(self, llm, tools, vectorstore):
+        return WorkerNode(llm=llm, tools=tools, vectorstore=vectorstore)
+
+    def initialize_boss_node(self, llm, vectorstore, task_execution_chain, verbose=True, max_iterations=5):
+        return BossNode(self.openai_api_key, llm, vectorstore, task_execution_chain, verbose, max_iterations)
+
+
+
+
+
+
+
+
+
+
+
+
+
+# class Swarms:
+#     def __init__(self, num_nodes: int, llm: BaseLLM, self_scaling: bool): 
+#         self.nodes = [WorkerNode(llm) for _ in range(num_nodes)]
+#         self.self_scaling = self_scaling
+    
+#     def add_worker(self, llm: BaseLLM):
+#         self.nodes.append(WorkerNode(llm))
+
+#     def remove_workers(self, index: int):
+#         self.nodes.pop(index)
+
+#     def execute(self, task):
+#         #placeholer for main execution logic
+#         pass
+
+#     def scale(self):
+#         #placeholder for self scaling logic
+#         pass
 
 
 
 #special classes
 
 class HierarchicalSwarms(Swarms):
     def execute(self, task):
@@ -381,7 +296,118 @@
 class CompetitiveSwarms(Swarms):
     def execute(self, task):
         pass
 
 class MultiAgentDebate(Swarms):
     def execute(self, task):
         pass
+
+
+
+
+
+
+
+
+#======================================> WorkerNode
+
+
+# class MetaWorkerNode:
+#     def __init__(self, llm, tools, vectorstore):
+#         self.llm = llm
+#         self.tools = tools
+#         self.vectorstore = vectorstore
+        
+#         self.agent = None
+#         self.meta_chain = None
+
+#     def init_chain(self, instructions):
+#         self.agent = WorkerNode(self.llm, self.tools, self.vectorstore)
+#         self.agent.create_agent("Assistant", "Assistant Role", False, {})
+
+#     def initialize_meta_chain():
+#         meta_template = """
+#         Assistant has just had the below interactions with a User. Assistant followed their "Instructions" closely. Your job is to critique the Assistant's performance and then revise the Instructions so that Assistant would quickly and correctly respond in the future.
+
+#         ####
+
+#         {chat_history}
+
+#         ####
+
+#         Please reflect on these interactions.
+
+#         You should first critique Assistant's performance. What could Assistant have done better? What should the Assistant remember about this user? Are there things this user always wants? Indicate this with "Critique: ...".
+
+#         You should next revise the Instructions so that Assistant would quickly and correctly respond in the future. Assistant's goal is to satisfy the user in as few interactions as possible. Assistant will only see the new Instructions, not the interaction history, so anything important must be summarized in the Instructions. Don't forget any important details in the current Instructions! Indicate the new Instructions by "Instructions: ...".
+#         """
+
+#         meta_prompt = PromptTemplate(
+#             input_variables=["chat_history"], template=meta_template
+#         )
+
+#         meta_chain = LLMChain(
+#             llm=OpenAI(temperature=0),
+#             prompt=meta_prompt,
+#             verbose=True,
+#         )
+#         return meta_chain
+
+#     def meta_chain(self):
+#         #define meta template and meta prompting as per your needs
+#         self.meta_chain = initialize_meta_chain()
+
+
+#     def get_chat_history(chain_memory):
+#         memory_key = chain_memory.memory_key
+#         chat_history = chain_memory.load_memory_variables(memory_key)[memory_key]
+#         return chat_history
+
+
+#     def get_new_instructions(meta_output):
+#         delimiter = "Instructions: "
+#         new_instructions = meta_output[meta_output.find(delimiter) + len(delimiter) :]
+#         return new_instructions
+
+
+#     def main(self, task, max_iters=3, max_meta_iters=5):
+#         failed_phrase = "task failed"
+#         success_phrase = "task succeeded"
+#         key_phrases = [success_phrase, failed_phrase]
+
+#         instructions = "None"
+#         for i in range(max_meta_iters):
+#             print(f"[Episode {i+1}/{max_meta_iters}]")
+#             self.initialize_chain(instructions)
+#             output = self.agent.perform('Assistant', {'request': task})
+#             for j in range(max_iters):
+#                 print(f"(Step {j+1}/{max_iters})")
+#                 print(f"Assistant: {output}")
+#                 print(f"Human: ")
+#                 human_input = input()
+#                 if any(phrase in human_input.lower() for phrase in key_phrases):
+#                     break
+#                 output = self.agent.perform('Assistant', {'request': human_input})
+#             if success_phrase in human_input.lower():
+#                 print(f"You succeeded! Thanks for playing!")
+#                 return
+#             self.initialize_meta_chain()
+#             meta_output = self.meta_chain.predict(chat_history=self.get_chat_history())
+#             print(f"Feedback: {meta_output}")
+#             instructions = self.get_new_instructions(meta_output)
+#             print(f"New Instructions: {instructions}")
+#             print("\n" + "#" * 80 + "\n")
+#         print(f"You failed! Thanks for playing!")
+
+
+# #init instance of MetaWorkerNode
+# meta_worker_node = MetaWorkerNode(llm=OpenAI, tools=tools, vectorstore=vectorstore)
+
+
+# #specify a task and interact with the agent
+# task = "Provide a sysmatic argument for why we should always eat past with olives"
+# meta_worker_node.main(task)
+
+
+####################################################################### => Boss Node
+####################################################################### => Boss Node
+####################################################################### => Boss Node
```

### Comparing `swarms-0.1.3/swarms/agents/workers/agents.py` & `swarms-0.1.4/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.3/swarms/agents/workers/auto_agent.py` & `swarms-0.1.4/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.3/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.1.4/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.3/swarms/agents/workers/multi-modal.py` & `swarms-0.1.4/swarms/agents/workers/multi-modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.3/swarms/agents/workers/omni_agent.py` & `swarms-0.1.4/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.3/swarms.egg-info/PKG-INFO` & `swarms-0.1.4/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.3
+Version: 0.1.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.3/swarms.egg-info/requires.txt` & `swarms-0.1.4/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

