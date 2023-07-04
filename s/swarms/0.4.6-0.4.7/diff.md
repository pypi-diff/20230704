# Comparing `tmp/swarms-0.4.6.tar.gz` & `tmp/swarms-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.6.tar", last modified: Tue Jul  4 18:16:08 2023, max compression
+gzip compressed data, was "swarms-0.4.7.tar", last modified: Tue Jul  4 18:31:50 2023, max compression
```

## Comparing `swarms-0.4.6.tar` & `swarms-0.4.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.096828 swarms-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:15:58.000000 swarms-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:16:08.096828 swarms-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-04 18:15:58.000000 swarms-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:15:58.000000 swarms-0.4.6/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 18:15:58.000000 swarms-0.4.6/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:15:58.000000 swarms-0.4.6/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:15:58.000000 swarms-0.4.6/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:16:08.096828 swarms-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:15:58.000000 swarms-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.096828 swarms-0.4.6/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70820 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.096828 swarms-0.4.6/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:31:41.000000 swarms-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:31:50.724549 swarms-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-04 18:31:41.000000 swarms-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.720548 swarms-0.4.7/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:41.000000 swarms-0.4.7/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 18:31:41.000000 swarms-0.4.7/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:31:41.000000 swarms-0.4.7/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:31:41.000000 swarms-0.4.7/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:31:50.724549 swarms-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:31:41.000000 swarms-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.720548 swarms-0.4.7/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70828 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 18:31:41.000000 swarms-0.4.7/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:31:50.724549 swarms-0.4.7/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:31:50.000000 swarms-0.4.7/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.6/LICENSE` & `swarms-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/PKG-INFO` & `swarms-0.4.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.6
+Version: 0.4.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.6/README.md` & `swarms-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/api/container.py` & `swarms-0.4.7/api/container.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 import re
 from pathlib import Path
 from typing import Dict, List
 
 from fastapi.templating import Jinja2Templates
 
 from swarms.agents.workers.agents import AgentManager
-from swarms.tools.main import BaseHandler, FileHandler, FileType
-from swarms.tools.main import CsvToDataframe
+from swarms.utils import BaseHandler, FileHandler, FileType, StaticUploader, CsvToDataframe
 
-from swarms.tools.main import BaseToolSet
-from swarms.tools.main import ExitConversation, RequestsGet
-from swarms.tools.main import CodeEditor
+from swarms.tools.main import BaseToolSet, ExitConversation, RequestsGet, CodeEditor, Terminal
 
-from swarms.tools.main import Terminal
-from swarms.tools.main import StaticUploader
+from env import settings
 
 
 BASE_DIR = Path(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 os.chdir(BASE_DIR / os.getenv["PLAYGROUND_DIR"])
 
 
 toolsets: List[BaseToolSet] = [
```

### Comparing `swarms-0.4.6/api/main.py` & `swarms-0.4.7/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/api/worker.py` & `swarms-0.4.7/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/setup.py` & `swarms-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.4.6',
+  version = '0.4.7',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.4.6/swarms/agents/swarms.py` & `swarms-0.4.7/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/agents/workers/agents.py` & `swarms-0.4.7/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/agents/workers/auto_agent.py` & `swarms-0.4.7/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.7/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/agents/workers/multi_modal.py` & `swarms-0.4.7/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/agents/workers/omni_agent.py` & `swarms-0.4.7/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/tools/main.py` & `swarms-0.4.7/swarms/tools/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
 
 import os
 import subprocess
 import time
 from datetime import datetime
 from typing import Dict, List
 
-from ansi import ANSI, Color, Style
+from swarms.utils import ANSI, Color, Style
 
 
 
 class Terminal(BaseToolSet):
     def __init__(self):
         self.sessions: Dict[str, List[SyscallTracer]] = {}
```

### Comparing `swarms-0.4.6/swarms/utils/ansi.py` & `swarms-0.4.7/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms/utils/utils.py` & `swarms-0.4.7/swarms/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
 
 
 
 #############===========================>
 import pandas as pd
 
-from core.prompts.file import DATAFRAME_PROMPT
+from swarms.prompts.prompts import DATAFRAME_PROMPT
 
 
 class CsvToDataframe(BaseHandler):
     def handle(self, filename: str):
         df = pd.read_csv(filename)
         description = (
             f"Dataframe with {len(df)} rows and {len(df.columns)} columns. "
@@ -431,15 +431,16 @@
 
 
 #========================> handlers/image
 import torch
 from PIL import Image
 from transformers import BlipForConditionalGeneration, BlipProcessor
 
-from core.prompts.file import IMAGE_PROMPT
+# from core.prompts.file import IMAGE_PROMPT
+from swarms.prompts.prompts import IMAGE_PROMPT
 
 
 
 class ImageCaptioning(BaseHandler):
     def __init__(self, device):
         print("Initializing ImageCaptioning to %s" % device)
         self.device = device
@@ -531,36 +532,36 @@
     return res
 ################# END
 
 
 
 
 
-################# MultiAgent
+# ################# MultiAgent
 
-from autogpt.agent import Agent
-from swarms.agents.swarms import worker_node
+# from autogpt.agent import Agent
+# from swarms.agents.swarms import worker_node
 
-class MultiAgent(worker_node):
+# class MultiAgent(worker_node):
 
-    def __init__(
-            self,
-            ai_name,
-            memory,
-            full_message_history,
-            prompt,
-            user_input,
-            agent_id
-    ):
-        super().__init__(
-            ai_name=ai_name,
-            memory=memory,
-            full_message_history=full_message_history,
-            next_action_count=0,
-            prompt=prompt,
-            user_input=user_input,
-        )
-        self.agent_id = agent_id
-        self.auditory_buffer = []  # contains the non processed parts of the conversation
+#     def __init__(
+#             self,
+#             ai_name,
+#             memory,
+#             full_message_history,
+#             prompt,
+#             user_input,
+#             agent_id
+#     ):
+#         super().__init__(
+#             ai_name=ai_name,
+#             memory=memory,
+#             full_message_history=full_message_history,
+#             next_action_count=0,
+#             prompt=prompt,
+#             user_input=user_input,
+#         )
+#         self.agent_id = agent_id
+#         self.auditory_buffer = []  # contains the non processed parts of the conversation
 
-    def receive_message(self, speaker, message):
-        self.auditory_buffer.append((speaker.ai_name, message))
+#     def receive_message(self, speaker, message):
+#         self.auditory_buffer.append((speaker.ai_name, message))
```

### Comparing `swarms-0.4.6/swarms.egg-info/PKG-INFO` & `swarms-0.4.7/swarms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.6
+Version: 0.4.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.6/swarms.egg-info/SOURCES.txt` & `swarms-0.4.7/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.4.6/swarms.egg-info/requires.txt` & `swarms-0.4.7/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

