# Comparing `tmp/swarms-0.0.5.tar.gz` & `tmp/swarms-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.5.tar", last modified: Fri Jun 30 19:30:07 2023, max compression
+gzip compressed data, was "swarms-0.0.7.tar", last modified: Mon Jul  3 22:09:07 2023, max compression
```

## Comparing `swarms-0.0.5.tar` & `swarms-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 19:29:56.000000 swarms-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 19:30:07.878474 swarms-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-30 19:29:56.000000 swarms-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:30:07.878474 swarms-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-30 19:29:56.000000 swarms-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/agents/swarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-06-30 19:29:56.000000 swarms-0.0.5/swarms/agents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:30:07.878474 swarms-0.0.5/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 19:30:07.000000 swarms-0.0.5/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:08:54.000000 swarms-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:09:07.389770 swarms-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:08:54.000000 swarms-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:09:07.389770 swarms-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-03 22:08:54.000000 swarms-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:08:54.000000 swarms-0.0.7/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:08:54.000000 swarms-0.0.7/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-03 22:08:54.000000 swarms-0.0.7/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.5/LICENSE` & `swarms-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.5/PKG-INFO` & `swarms-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.5
+Version: 0.0.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.5/README.md` & `swarms-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -14,81 +14,59 @@
 
 [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 
 Welcome to Swarms - the future of AI, where we leverage the power of autonomous agents to create 'swarms' of Language Models (LLM) that work together, creating a dynamic and interactive AI system.
 
 ## Vision
-In the world of AI and machine learning, individual models have made significant strides in understanding and generating human-like text. But imagine the possibilities when these models are no longer solitary units, but part of a cooperative and communicative swarm. This is the future we envision.
+In the world of AI and machine learning, individual models have made significant strides in understanding and generating human-like text.
 
-Just as a swarm of bees works together, communicating and coordinating their actions for the betterment of the hive, swarming LLM agents can work together to create richer, more nuanced outputs. By harnessing the strengths of individual agents and combining them through a swarming architecture, we can unlock a new level of performance and responsiveness in AI systems. We envision swarms of LLM agents revolutionizing fields like customer support, content creation, research, and much more.
+But imagine the possibilities when these models are no longer solitary units, but part of a cooperative and communicative swarm. This is the future we envision.
+
+Just as a swarm of bees works together, communicating and coordinating their actions for the betterment of the hive, swarming LLM agents can work together to create richer, more nuanced outputs. 
+
+By harnessing the strengths of individual agents and combining them through a swarming architecture, we can unlock a new level of performance and responsiveness in AI systems. We envision swarms of LLM agents revolutionizing fields like customer support, content creation, research, and much more.
 
 
 ## Table of Contents
 1. [Installation](#installation)
-2. [Usage](#usage)
-3. [Sharing](#sharing)
+2. [Sharing](#sharing)
 
 ## Installation
-There are 2 methods, one is through `git clone` and the other is by `pip install swarms`
+There are 2 methods, one is through `git clone` and the other is by `pip install swarms`. Check out the [document](/DOCUMENTATION.md) for more information on the classes.
 
 # Method1
 * Pip install `python3 -m pip install swarms`
 
 * Create new python file and unleash superintelligence
 
 ```python
 
-from swarms import BossNode
-
-boss_node = BossNode()
+from swarms import boss_node
 
-#create and execute a task
-task = boss_node.create_task("Write a weather report for SF today")
+#create a task
+task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
 
 #or 
 # task = boss_node.create_task('Find a video of Elon Musk and make him look like a cat')
 
 boss_node.execute(task)
 ```
 
+# Method2
+Download via Github, and install requirements
 ```bash
 git clone https://github.com/kyegomez/swarms.git
 cd swarms
 pip install -r requirements.txt
 ```
 
-## Usage
-There are 2 methods, one is very simple to test it out and then there is another to explore the agents and so on! Check out the [Documetation file ](/DOCUMENTATION.md) to understand the classes
-
-### Method 1
-Simple example `python3 example.py`
-
-
-### Method2
-
-I see, my apologies for the confusion. Here is an updated usage example that just utilizes the `BossNode` class:
-
-One of the main components of swarms is the `BossNode` class. This class acts as a "boss" that assigns tasks to other components.
-
-Below is an example of how to use the `BossNode` class in Langchain:
-
-```python
-from swarms import BossNode
-#or swarms.agents.swarms import BossNode
+# Method 3
+Simple example by `git cloning https://github.com/kyegomez/swarms.git` `python3 example.py`
 
-# Initialize BossNode
-boss_node = BossNode()
-
-# Create and execute a task
-task = boss_node.create_task("Write a summary of the latest news about artificial intelligence.")
-boss_node.execute_task(task)
-```
-
-This will create a task for the BossNode, which is to write a summary of the latest news about artificial intelligence. 
 
 ## BossNode
 
 The `BossNode` class is a key component of Swarms. It represents a "boss" in the system that assigns tasks to other components.
 
 Here is an example of how you can use it:
 
@@ -103,28 +81,24 @@
     def execute_task(self, task):
         # task execution code goes here
 ```
 
 With the `BossNode` class, you can create tasks for your tools to perform. For example, you can create a task to write a summary of a specific topic:
 
 ```python
-boss_node = BossNode()
-task = boss_node.create_task("Write a summary of the latest news about quantum computing.")
+from swarms import boss_node
+#create a task
+task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
+#execute the teask
 boss_node.execute_task(task)
+
 ```
 
 This will create and execute a task to write a summary about the latest news on quantum computing. The result will be the summary of the news.
 
-## Note
-- The `AutoAgent` makes use of several helper tools and context managers for tasks such as processing CSV files, browsing web pages, and querying web pages. For the best use of this agent, understanding these tools is crucial.
-
-- Additionally, the agent uses the ChatOpenAI, a language learning model (LLM), to perform its tasks. You need to provide an OpenAI API key to make use of it. 
-
-- Detailed knowledge of FAISS, a library for efficient similarity search and clustering of dense vectors, is also essential as it's used for memory storage and retrieval. 
-
 
 ## Share with your Friends
 
 Share on Twitter: [![Share on Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)](https://twitter.com/intent/tweet?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 Share on Facebook: [![Share on Facebook](https://img.shields.io/badge/-Share%20on%20Facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
@@ -140,63 +114,115 @@
 
 ## Contribute
 We're always looking for contributors to help us improve and expand this project. If you're interested, please check out our [Contributing Guidelines](./CONTRIBUTING.md).
 
 Thank you for being a part of our project!
 
 
-# To do:
+# Open Source Roadmap
+
+Here is the detailed roadmap of our priorities and planned features for the near term:
+
+## TODO
+
+1. **Multi-Agent Debate Integration**: Integrate multi-agent debate frameworks ([Multi Agent debate](https://github.com/Skytliang/Multi-Agents-Debate) and [Multi agent2 debate](https://github.com/composable-models/llm_multiagent_debate)) to improve decision-making.
+
+2. **Meta Prompting Integration**: Include meta prompting across all worker agents to guide their actions.
+
+3. **Swarms Class**: Create a main swarms class `swarms('Increase sales by 40$', workers=4)` for managing and coordinating multiple worker nodes.
+
+4. **Integration of Additional Tools**: Integrate [Jarvis](https://github.com/microsoft/JARVIS) as worker nodes, add text to speech and text to script tools ([whisper x](https://github.com/kyegomez/youtubeURL-to-text)), and integrate Hugging Face agents and other external tools.
+
+5. **Task Completion and Evaluation Logic**: Include task completion logic with meta prompting, and evaluate task completion on a scale from 0.0 to 1.0.
+
+7. **Ocean Integration**: Use the [Ocean](https://github.com/kyegomez/Ocean) vector database as the main embedding database for all the agents, both boss and worker.
+
+8. **Improved Communication**: Develop a universal vector database that is only used when a task is completed in this format `[TASK][COMPLETED]`.
+
+9. **Testing and Evaluation**: Create unit tests, benchmarks, and evaluations for performance monitoring and continuous improvement.
+
+10. **Worker Swarm Class**: Create a class for self-scaling worker swarms. If they need help, they can spawn an entirely new worker and more workers if needed.
+
+## Documentation
+
+1. **Examples**: Create extensive and useful examples for a variety of use cases.
+
+2. **README**: Update the README to include the examples and usage instructions.
+
+
+# Mid-Long term
+Here are some potential middle-to-long-term improvements to consider for this project:
+
+1. **Modular Design**: Aim to design a more modular and scalable framework, making it easy for developers to plug-and-play various components.
+
+2. **Interactive User Interface**: Develop a more interactive, user-friendly GUI that allows users to interact with the system without needing to understand the underlying code.
+
+3. **Advanced Error Handling**: Implement advanced error handling and debugging capabilities to make it easier for developers to diagnose and fix issues.
+
+4. **Optimized Resource Utilization**: Improve the efficiency of resource use, aiming to reduce memory consumption and improve speed without sacrificing accuracy.
+
+5. **Collaborative Learning**: Integrate more sophisticated techniques for collaborative learning among the swarm, allowing them to share knowledge and learn from each other's successes and failures.
+
+6. **Autonomous Self-Improvement**: Implement mechanisms that allow the swarm to autonomously learn from its past experiences and improve its performance over time.
 
-* Integrate [Multi Agent debate](https://github.com/Skytliang/Multi-Agents-Debate)
+7. **Security Enhancements**: Include robust security measures to protect sensitive data and prevent unauthorized access.
 
-* Integrate [Multi agent2 debate](https://github.com/composable-models/llm_multiagent_debate)
+8. **Privacy-Preserving Techniques**: Consider incorporating privacy-preserving techniques such as differential privacy to ensure the confidentiality of user data.
 
-* Integrate meta prompting into all worker agents
+9. **Support for More Languages**: Expand language support to allow the system to cater to a more global audience.
 
-* Create 1 main swarms class `swarms('Increase sales by 40$', workers=4)`
+10. **Robustness and Resilience**: Improve the system's robustness and resilience, ensuring that it can operate effectively even in the face of hardware or software failures.
 
-* Integrate [Jarvis](https://github.com/microsoft/JARVIS) as worker nodes
+11. **Continual Learning**: Implement continual learning techniques to allow the system to adapt and evolve as new data comes in.
 
-* Integrate guidance and token healing
+12. **More Contextual Understanding**: Enhance the system's capability to understand context better, making it more effective in handling real-world, complex tasks.
 
-* Add text to speech [whisper x, youtube script](https://github.com/kyegomez/youtubeURL-to-text) and text to speech code models as tools 
+13. **Dynamic Task Prioritization**: Develop advanced algorithms for dynamic task prioritization, ensuring that the most important tasks are addressed first.
 
-* Add task completion logic with meta prompting, task evaluation as a state from 0.0 to 1.0, and critiquing for meta prompting.
+14. **Expanding the Swarm's Skills**: Train the swarm on a wider range of tasks, gradually expanding their skill set and problem-solving capabilities.
 
-* Integrate meta prompting for every agent boss and worker
+15. **Real-World Deployment**: Test and refine the system in real-world settings, learning from these experiences to further improve and adapt the system. 
 
-* Get baby agi set up with the autogpt instance as a tool
+Remember, these are potential improvements. It's important to revisit your priorities regularly and adjust them based on project needs, feedback, and learning from both successes and failures.
 
-* Integrate [Ocean](https://github.com/kyegomez/Ocean) vector db as the main embedding database for all the agents boss and or worker
+## Optimization Priorities
 
-* Communication, a universal vector database that is only used when a task is completed in this format `[TASK][COMPLETED]`
+1. **Reliability**: Increase the reliability of the swarm - obtaining the desired output with a basic and un-detailed input.
 
-* Create unit tests
+2. **Speed**: Reduce the time it takes for the swarm to accomplish tasks by improving the communication layer, critiquing, and self-alignment with meta prompting.
 
-* Create benchmrks
+3. **Scalability**: Ensure that the system is asynchronous, concurrent, and self-healing to support scalability.
 
-* Create evaluations
+Our goal is to continuously improve Swarms by following this roadmap, while also being adaptable to new needs and opportunities as they arise.
 
-* Add new tool that uses WhiseperX to transcribe a youtube video
 
-* Integrate hf agents as tools
 
-* [Integrate tools from here](https://integrations.langchain.com/)
+# Inspiration
 
 
-* Create extensive and useful examples 
+* [🐪CAMEL🐪](https://twitter.com/hwchase17/status/1645834030519296000)
+* [MultiAgent](https://github.com/rumpfmax/Multi-GPT/blob/master/multigpt/multi_agent_manager.py)
+* [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
-* And, recreate exampels and usage in readme.
+* [SuperAGI]()
+* [AgentForge](https://github.com/DataBassGit/AgentForge)
+* [Voyager](https://github.com/MineDojo/Voyager)
 
-* Create a worker Swarm class, where it's just workers who are equal and that can self scale. If they need help they'll just spawn an entirely new worker and they can spawn more workers
 
+* [Gorilla: Large Language Model Connected with Massive APIs](https://arxiv.org/abs/2305.15334)
+* [LLM powered agents](https://lilianweng.github.io/posts/2023-06-23-agent/)
 
 
+## Agent System Overview
+In a LLM-powered autonomous agent system, LLM functions as the agent’s brain, complemented by several key components:
 
+* Planning Subgoal and decomposition: The agent breaks down large tasks into smaller, manageable subgoals, enabling efficient handling of complex tasks.
+Reflection and refinement: The agent can do self-criticism and self-reflection over past actions, learn from mistakes and refine them for future steps, thereby improving the quality of final results.
 
-# Optimization
+* Memory Short-term memory: I would consider all the in-context learning (See Prompt Engineering) as utilizing short-term memory of the model to learn.
+Long-term memory: This provides the agent with the capability to retain and recall (infinite) information over extended periods, often by leveraging an external vector store and fast retrieval.
 
-* Reliability => The swarm needs to be reliable. How do we quantify reliability -> Reliability is obtaining an desired output with a basic and un-detailed input. 
+* Tool use
+The agent learns to call external APIs for extra information that is missing from the model weights (often hard to change after pre-training), including current information, code execution capability, access to proprietary information sources and more.
 
-* Speed => How long does it take the swarm to accomplish a task, such as `let's respond to all the emails`, we need to minimize this => we can do this by cultivating an efficient communication layer, critiquing, and self-alignment with meta prompting.
+* Communication -> How reliable and fast is the communication between each indivual agent.
 
-* Scalability => Asynchrony, Concurrent, and self-healing.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `swarms-0.0.5/setup.py` & `swarms-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.7',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.0.5/swarms/agents/swarms.py` & `swarms-0.0.7/swarms/agents/swarms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-from swarms.agents.workers.auto_agent import AutoGPT
 from collections import deque
 from typing import Dict, Any
 
 
 import os
 from collections import deque
 from typing import Dict, List, Optional, Any
@@ -31,15 +29,15 @@
 # Initialize the vectorstore as empty
 import faiss
 
 embedding_size = 1536
 index = faiss.IndexFlatL2(embedding_size)
 vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
 
-
+# from swarms.agents.workers.auto_agent import AutoGPT
 
 
 
 
 #-------------------------------------------------------------------------- WORKER NODE
 import pandas as pd
 from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
```

### Comparing `swarms-0.0.5/swarms.egg-info/PKG-INFO` & `swarms-0.0.7/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.5
+Version: 0.0.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.5/swarms.egg-info/requires.txt` & `swarms-0.0.7/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

