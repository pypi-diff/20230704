# Comparing `tmp/swarms-0.4.7.tar.gz` & `tmp/swarms-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.7.tar", last modified: Tue Jul  4 18:31:50 2023, max compression
+gzip compressed data, was "swarms-0.4.8.tar", last modified: Tue Jul  4 18:46:09 2023, max compression
```

## Comparing `swarms-0.4.7.tar` & `swarms-0.4.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:31:41.000000 swarms-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:31:50.724549 swarms-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-04 18:31:41.000000 swarms-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.720548 swarms-0.4.7/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:41.000000 swarms-0.4.7/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 18:31:41.000000 swarms-0.4.7/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:31:41.000000 swarms-0.4.7/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:31:41.000000 swarms-0.4.7/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:31:50.724549 swarms-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:31:41.000000 swarms-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.720548 swarms-0.4.7/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70828 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.011498 swarms-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:45:59.000000 swarms-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:46:09.011498 swarms-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 18:45:59.000000 swarms-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:59.000000 swarms-0.4.8/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 18:45:59.000000 swarms-0.4.8/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:45:59.000000 swarms-0.4.8/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:45:59.000000 swarms-0.4.8/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:46:09.011498 swarms-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:45:59.000000 swarms-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70834 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.011498 swarms-0.4.8/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 18:46:09.000000 swarms-0.4.8/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.7/LICENSE` & `swarms-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/PKG-INFO` & `swarms-0.4.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.7
+Version: 0.4.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.7/README.md` & `swarms-0.4.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,21 +40,27 @@
 * Create new python file and unleash superintelligence
 
 ```python
 
 from swarms import Swarms
 
 # Retrieve your API key from the environment or replace with your actual key
-api_key = "api key"
+api_key = "sksdsds"
 
 # Initialize Swarms with your API key
 swarm = Swarms(openai_api_key=api_key)
 
 # Define an objective
-objective = "Find 20 potential customers for a Swarms based AI Agent automation infrastructure"
+objective = """
+Please develop and serve a simple community web service. 
+People can signup, login, post, comment. 
+Post and comment should be visible at once. 
+I want it to have neumorphism-style. 
+The ports you can use are 4500 and 6500.
+"""
 
 # Run Swarms
 swarm.run_swarms(objective)
 ```
 
 # Method2
 Download via Github, and install requirements
@@ -88,25 +94,30 @@
 
 With the `BossNode` class, you can create tasks for your tools to perform. For example, you can create a task to write a summary of a specific topic:
 
 ```python
 from swarms import Swarms
 
 # Retrieve your API key from the environment or replace with your actual key
-api_key = "api key"
+api_key = "sksdsds"
 
 # Initialize Swarms with your API key
 swarm = Swarms(openai_api_key=api_key)
 
 # Define an objective
-objective = "Find 20 potential customers for a Swarms based AI Agent automation infrastructure"
+objective = """
+Please develop and serve a simple community web service. 
+People can signup, login, post, comment. 
+Post and comment should be visible at once. 
+I want it to have neumorphism-style. 
+The ports you can use are 4500 and 6500.
+"""
 
 # Run Swarms
 swarm.run_swarms(objective)
-
 ```
 
 This will create and execute a task to write a summary about the latest news on quantum computing. The result will be the summary of the news.
 
 
 ## Share with your Friends
```

### Comparing `swarms-0.4.7/api/container.py` & `swarms-0.4.8/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/api/main.py` & `swarms-0.4.8/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/api/worker.py` & `swarms-0.4.8/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/setup.py` & `swarms-0.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.4.7',
+  version = '0.4.8',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.4.7/swarms/agents/swarms.py` & `swarms-0.4.8/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/agents/workers/agents.py` & `swarms-0.4.8/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/agents/workers/auto_agent.py` & `swarms-0.4.8/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.8/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/agents/workers/multi_modal.py` & `swarms-0.4.8/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/agents/workers/omni_agent.py` & `swarms-0.4.8/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/tools/main.py` & `swarms-0.4.8/swarms/tools/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,16 +431,15 @@
 
 import os
 import subprocess
 import time
 from datetime import datetime
 from typing import Dict, List
 
-from swarms.utils import ANSI, Color, Style
-
+from swarms.utils import ANSI, Color, Style # test
 
 
 class Terminal(BaseToolSet):
     def __init__(self):
         self.sessions: Dict[str, List[SyscallTracer]] = {}
 
     @tool(
```

### Comparing `swarms-0.4.7/swarms/utils/ansi.py` & `swarms-0.4.8/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms/utils/utils.py` & `swarms-0.4.8/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms.egg-info/PKG-INFO` & `swarms-0.4.8/swarms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.7
+Version: 0.4.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.7/swarms.egg-info/SOURCES.txt` & `swarms-0.4.8/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.4.7/swarms.egg-info/requires.txt` & `swarms-0.4.8/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

