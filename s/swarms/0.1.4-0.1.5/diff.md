# Comparing `tmp/swarms-0.1.4.tar.gz` & `tmp/swarms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.1.4.tar", last modified: Mon Jul  3 23:59:36 2023, max compression
+gzip compressed data, was "swarms-0.1.5.tar", last modified: Tue Jul  4 00:08:47 2023, max compression
```

## Comparing `swarms-0.1.4.tar` & `swarms-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 23:59:27.000000 swarms-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:59:36.689822 swarms-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-03 23:59:27.000000 swarms-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:59:36.689822 swarms-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 23:59:27.000000 swarms-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.685822 swarms-0.1.4/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/multi-modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-03 23:59:27.000000 swarms-0.1.4/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:59:36.689822 swarms-0.1.4/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 23:59:36.000000 swarms-0.1.4/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:47.457491 swarms-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 00:08:36.000000 swarms-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:08:47.457491 swarms-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 00:08:36.000000 swarms-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:08:47.457491 swarms-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 00:08:36.000000 swarms-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:47.453491 swarms-0.1.5/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:47.453491 swarms-0.1.5/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:47.457491 swarms-0.1.5/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79059 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/workers/multi-modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 00:08:36.000000 swarms-0.1.5/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:47.453491 swarms-0.1.5/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 00:08:47.000000 swarms-0.1.5/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 00:08:47.000000 swarms-0.1.5/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:08:47.000000 swarms-0.1.5/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 00:08:47.000000 swarms-0.1.5/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 00:08:47.000000 swarms-0.1.5/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.1.4/LICENSE` & `swarms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/PKG-INFO` & `swarms-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.4/README.md` & `swarms-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/setup.py` & `swarms-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.1.4/swarms/agents/swarms.py` & `swarms-0.1.5/swarms/agents/swarms.py`

 * *Files 10% similar despite different names*

```diff
@@ -240,22 +240,46 @@
     def initialize_vectorstore(self):
         embeddings_model = OpenAIEmbeddings()
         embedding_size = 1536
         index = faiss.IndexFlatL2(embedding_size)
         return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
 
     def initialize_worker_node(self, llm, tools, vectorstore):
-        return WorkerNode(llm=llm, tools=tools, vectorstore=vectorstore)
-
-    def initialize_boss_node(self, llm, vectorstore, task_execution_chain, verbose=True, max_iterations=5):
-        return BossNode(self.openai_api_key, llm, vectorstore, task_execution_chain, verbose, max_iterations)
-
-
-
-
+        worker_node = WorkerNode(llm=llm, tools=tools, vectorstore=vectorstore)
+        worker_node.create_agent(ai_name="AI Assistant", ai_role="Assistant", human_in_the_loop=True, search_kwargs={})
+        return worker_node
+
+    def initialize_boss_node(self, llm, vectorstore):
+        todo_prompt = PromptTemplate.from_template("You are a planner who is an expert at coming up with a todo list for a given objective. Come up with a todo list for this objective: {objective}""")
+        todo_chain = LLMChain(llm=OpenAI(temperature=0), prompt=todo_prompt)
+        search = SerpAPIWrapper()
+        tools = [
+            Tool(name="Search", func=search.run, description="useful for when you need to answer questions about current events"),
+            Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for. Output: a todo list for that objective. Please be very clear what the objective is!"),
+            Tool(name="AUTONOMOUS Worker AGENT", func=self.worker_node.agent.run, description="Useful for when you need to spawn an autonomous agent instance as a worker to accomplish complex tasks, it can search the internet or spawn child multi-modality models to process and generate images and text or audio and so on")
+        ]
+
+        suffix = """Question: {task}\n{agent_scratchpad}"""
+        prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n"""
+        prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
+
+        llm_chain = LLMChain(llm=OpenAI(temperature=0), prompt=prompt)
+        agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
+        agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=tools, verbose=True)
+        return BossNode(self.openai_api_key, llm, vectorstore, agent_executor, verbose=True, max_iterations=5)
+
+    def run_swarms(self, objective):
+        llm = self.initialize_llm()
+        tools = self.initialize_tools(llm)
+        vectorstore = self.initialize_vectorstore()
+        worker_node = self.initialize_worker_node(llm, tools, vectorstore)
+        boss_node = self.initialize_boss_node(llm, vectorstore)
+        task = boss_node.create_task(objective)
+        boss_node.execute_task(task)
+        worker_node.run_agent(objective)
 
 
 
 
 
 
 
@@ -280,36 +304,30 @@
 #         #placeholder for self scaling logic
 #         pass
 
 
 
 #special classes
 
-class HierarchicalSwarms(Swarms):
-    def execute(self, task):
-        pass
-
-
-class CollaborativeSwarms(Swarms):
-    def execute(self, task):
-        pass
-
-class CompetitiveSwarms(Swarms):
-    def execute(self, task):
-        pass
-
-class MultiAgentDebate(Swarms):
-    def execute(self, task):
-        pass
-
-
+# class HierarchicalSwarms(Swarms):
+#     def execute(self, task):
+#         pass
 
 
+# class CollaborativeSwarms(Swarms):
+#     def execute(self, task):
+#         pass
 
+# class CompetitiveSwarms(Swarms):
+#     def execute(self, task):
+#         pass
 
+# class MultiAgentDebate(Swarms):
+#     def execute(self, task):
+#         pass
 
 
 #======================================> WorkerNode
 
 
 # class MetaWorkerNode:
 #     def __init__(self, llm, tools, vectorstore):
```

### Comparing `swarms-0.1.4/swarms/agents/workers/agents.py` & `swarms-0.1.5/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/swarms/agents/workers/auto_agent.py` & `swarms-0.1.5/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.1.5/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/swarms/agents/workers/multi-modal.py` & `swarms-0.1.5/swarms/agents/workers/multi-modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/swarms/agents/workers/omni_agent.py` & `swarms-0.1.5/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.1.4/swarms.egg-info/PKG-INFO` & `swarms-0.1.5/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.1.4/swarms.egg-info/requires.txt` & `swarms-0.1.5/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

