# Comparing `tmp/swarms-0.0.9.tar.gz` & `tmp/swarms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.9.tar", last modified: Mon Jul  3 22:28:50 2023, max compression
+gzip compressed data, was "swarms-0.1.1.tar", last modified: Mon Jul  3 22:43:26 2023, max compression
```

## Comparing `swarms-0.0.9.tar` & `swarms-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:28:41.000000 swarms-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:28:50.781130 swarms-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:28:41.000000 swarms-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:28:50.785130 swarms-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:28:41.000000 swarms-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:28:41.000000 swarms-0.0.9/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:41.000000 swarms-0.0.9/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-03 22:28:41.000000 swarms-0.0.9/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:28:50.781130 swarms-0.0.9/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:28:50.000000 swarms-0.0.9/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.853130 swarms-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:43:17.000000 swarms-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:43:26.853130 swarms-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:43:17.000000 swarms-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:43:26.853130 swarms-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:43:17.000000 swarms-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.849130 swarms-0.1.1/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:43:17.000000 swarms-0.1.1/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.853130 swarms-0.1.1/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:17.000000 swarms-0.1.1/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-03 22:43:17.000000 swarms-0.1.1/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:26.849130 swarms-0.1.1/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:43:26.000000 swarms-0.1.1/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.9/LICENSE` & `swarms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.9/PKG-INFO` & `swarms-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.9
+Version: 0.1.1
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.9/README.md` & `swarms-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.0.9/setup.py` & `swarms-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.0.9',
+  version = '0.1.1',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.0.9/swarms/agents/swarms.py` & `swarms-0.1.1/swarms/agents/swarms.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,26 +17,18 @@
 from langchain.vectorstores import FAISS
 from langchain.docstore import InMemoryDocstore
 
 from langchain.agents import ZeroShotAgent, Tool, AgentExecutor
 from langchain import OpenAI, SerpAPIWrapper, LLMChain
 
 
-from swarms.agents.workers.auto_agent import agent_worker
-worker_agent  = agent_worker
-
 # Define your embedding model
-embeddings_model = OpenAIEmbeddings()
+# embeddings_model = OpenAIEmbeddings()
 # Initialize the vectorstore as empty
 import faiss
-
-embedding_size = 1536
-index = faiss.IndexFlatL2(embedding_size)
-vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
-
 # from swarms.agents.workers.auto_agent import AutoGPT
 
 
 
 
 #-------------------------------------------------------------------------- WORKER NODE
 import pandas as pd
@@ -119,19 +111,31 @@
 
 
 ############## Vectorstore
 embeddings_model = OpenAIEmbeddings(openai_api_key="")
 embedding_size = 1536
 index = faiss.IndexFlatL2(embedding_size)
 vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+####################################################################### => Worker Node
+
+
+worker_agent = AutoGPT.from_llm_and_tools(
+    ai_name="WorkerX",
+    ai_role="Assistant",
+    tools=tools,
+    llm=llm,
+    memory=vectorstore.as_retriever(search_kwargs={"k": 8}),
+    human_in_the_loop=True, # Set to True if you want to add feedback at each step.
+)
+
+worker_agent.chain.verbose = True
 
 
 
 
-####################################################################### => Worker Node
 
 class WorkerNode:
     def __init__(self, llm, tools, vectorstore):
         self.llm = llm
         self.tools = tools
         self.vectorstore = vectorstore
 
@@ -166,109 +170,109 @@
 #use the agent to perform a task
 worker_node.run_agent("Find 20 potential customers for a Swarms based AI Agent automation infrastructure")
 
 
 #======================================> WorkerNode
 
 
-class MetaWorkerNode:
-    def __init__(self, llm, tools, vectorstore):
-        self.llm = llm
-        self.tools = tools
-        self.vectorstore = vectorstore
+# class MetaWorkerNode:
+#     def __init__(self, llm, tools, vectorstore):
+#         self.llm = llm
+#         self.tools = tools
+#         self.vectorstore = vectorstore
         
-        self.agent = None
-        self.meta_chain = None
-
-    def init_chain(self, instructions):
-        self.agent = WorkerNode(self.llm, self.tools, self.vectorstore)
-        self.agent.create_agent("Assistant", "Assistant Role", False, {})
-
-    def initialize_meta_chain():
-        meta_template = """
-        Assistant has just had the below interactions with a User. Assistant followed their "Instructions" closely. Your job is to critique the Assistant's performance and then revise the Instructions so that Assistant would quickly and correctly respond in the future.
-
-        ####
-
-        {chat_history}
-
-        ####
-
-        Please reflect on these interactions.
-
-        You should first critique Assistant's performance. What could Assistant have done better? What should the Assistant remember about this user? Are there things this user always wants? Indicate this with "Critique: ...".
-
-        You should next revise the Instructions so that Assistant would quickly and correctly respond in the future. Assistant's goal is to satisfy the user in as few interactions as possible. Assistant will only see the new Instructions, not the interaction history, so anything important must be summarized in the Instructions. Don't forget any important details in the current Instructions! Indicate the new Instructions by "Instructions: ...".
-        """
-
-        meta_prompt = PromptTemplate(
-            input_variables=["chat_history"], template=meta_template
-        )
-
-        meta_chain = LLMChain(
-            llm=OpenAI(temperature=0),
-            prompt=meta_prompt,
-            verbose=True,
-        )
-        return meta_chain
+#         self.agent = None
+#         self.meta_chain = None
 
-    def meta_chain(self):
-        #define meta template and meta prompting as per your needs
-        self.meta_chain = initialize_meta_chain()
-
-
-    def get_chat_history(chain_memory):
-        memory_key = chain_memory.memory_key
-        chat_history = chain_memory.load_memory_variables(memory_key)[memory_key]
-        return chat_history
-
-
-    def get_new_instructions(meta_output):
-        delimiter = "Instructions: "
-        new_instructions = meta_output[meta_output.find(delimiter) + len(delimiter) :]
-        return new_instructions
-
-
-    def main(self, task, max_iters=3, max_meta_iters=5):
-        failed_phrase = "task failed"
-        success_phrase = "task succeeded"
-        key_phrases = [success_phrase, failed_phrase]
-
-        instructions = "None"
-        for i in range(max_meta_iters):
-            print(f"[Episode {i+1}/{max_meta_iters}]")
-            self.initialize_chain(instructions)
-            output = self.agent.perform('Assistant', {'request': task})
-            for j in range(max_iters):
-                print(f"(Step {j+1}/{max_iters})")
-                print(f"Assistant: {output}")
-                print(f"Human: ")
-                human_input = input()
-                if any(phrase in human_input.lower() for phrase in key_phrases):
-                    break
-                output = self.agent.perform('Assistant', {'request': human_input})
-            if success_phrase in human_input.lower():
-                print(f"You succeeded! Thanks for playing!")
-                return
-            self.initialize_meta_chain()
-            meta_output = self.meta_chain.predict(chat_history=self.get_chat_history())
-            print(f"Feedback: {meta_output}")
-            instructions = self.get_new_instructions(meta_output)
-            print(f"New Instructions: {instructions}")
-            print("\n" + "#" * 80 + "\n")
-        print(f"You failed! Thanks for playing!")
-
-
-#init instance of MetaWorkerNode
-meta_worker_node = MetaWorkerNode(llm=OpenAI, tools=tools, vectorstore=vectorstore)
-
-
-#specify a task and interact with the agent
-task = "Provide a sysmatic argument for why we should always eat past with olives"
-meta_worker_node.main(task)
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
 
 
 ####################################################################### => Boss Node
 ####################################################################### => Boss Node
 ####################################################################### => Boss Node
 
 class BossNode:
@@ -352,19 +356,19 @@
 agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=tool_names)
 agent_executor = AgentExecutor.from_agent_and_tools(
     agent=agent, tools=tools, verbose=True
 )
 
 boss_node = BossNode(llm=llm, vectorstore=vectorstore, task_execution_chain=agent_executor, verbose=True, max_iterations=5)
 
-#create  a task 
-task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
+# #create  a task 
+# task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
 
-#execute the task
-boss_node.execute_task(task)
+# #execute the task
+# boss_node.execute_task(task)
 
 
 class Swarms:
     def __init__(self, num_nodes: int, llm: BaseLLM, self_scaling: bool): 
         self.nodes = [WorkerNode(llm) for _ in range(num_nodes)]
         self.self_scaling = self_scaling
```

### Comparing `swarms-0.0.9/swarms.egg-info/PKG-INFO` & `swarms-0.1.1/swarms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.9
+Version: 0.1.1
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.9/swarms.egg-info/requires.txt` & `swarms-0.1.1/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

