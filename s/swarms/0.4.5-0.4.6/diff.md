# Comparing `tmp/swarms-0.4.5.tar.gz` & `tmp/swarms-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.5.tar", last modified: Tue Jul  4 18:13:37 2023, max compression
+gzip compressed data, was "swarms-0.4.6.tar", last modified: Tue Jul  4 18:16:08 2023, max compression
```

## Comparing `swarms-0.4.5.tar` & `swarms-0.4.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.781633 swarms-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:13:25.000000 swarms-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:13:37.781633 swarms-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-04 18:13:25.000000 swarms-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.777633 swarms-0.4.5/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.000000 swarms-0.4.5/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 18:13:25.000000 swarms-0.4.5/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:13:25.000000 swarms-0.4.5/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:13:25.000000 swarms-0.4.5/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:13:37.781633 swarms-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:13:25.000000 swarms-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.777633 swarms-0.4.5/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.781633 swarms-0.4.5/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.781633 swarms-0.4.5/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.781633 swarms-0.4.5/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.781633 swarms-0.4.5/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70990 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.781633 swarms-0.4.5/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-07-04 18:13:25.000000 swarms-0.4.5/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:37.777633 swarms-0.4.5/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:13:37.000000 swarms-0.4.5/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-04 18:13:37.000000 swarms-0.4.5/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:13:37.000000 swarms-0.4.5/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:13:37.000000 swarms-0.4.5/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:13:37.000000 swarms-0.4.5/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.096828 swarms-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:15:58.000000 swarms-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:16:08.096828 swarms-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-04 18:15:58.000000 swarms-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:15:58.000000 swarms-0.4.6/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 18:15:58.000000 swarms-0.4.6/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:15:58.000000 swarms-0.4.6/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:15:58.000000 swarms-0.4.6/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:16:08.096828 swarms-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:15:58.000000 swarms-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.096828 swarms-0.4.6/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70820 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.096828 swarms-0.4.6/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-07-04 18:15:58.000000 swarms-0.4.6/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:16:08.092828 swarms-0.4.6/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:16:08.000000 swarms-0.4.6/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.5/LICENSE` & `swarms-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/PKG-INFO` & `swarms-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.5
+Version: 0.4.6
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.5/README.md` & `swarms-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/api/container.py` & `swarms-0.4.6/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/api/main.py` & `swarms-0.4.6/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/api/worker.py` & `swarms-0.4.6/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/setup.py` & `swarms-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.4.5',
+  version = '0.4.6',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.4.5/swarms/agents/swarms.py` & `swarms-0.4.6/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms/agents/workers/agents.py` & `swarms-0.4.6/swarms/agents/workers/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,16 +220,15 @@
 
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.schema import AgentAction, AgentFinish, LLMResult
 from celery import Task
 
-from ansi import ANSI, Color, Style, dim_multiline
-from logger import logger
+from swarms.utils import ANSI, Color, Style, dim_multiline, logger
 
 
 class EVALCallbackHandler(BaseCallbackHandler):
     @property
     def ignore_llm(self) -> bool:
         return False
```

### Comparing `swarms-0.4.5/swarms/agents/workers/auto_agent.py` & `swarms-0.4.6/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.6/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms/agents/workers/multi_modal.py` & `swarms-0.4.6/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms/agents/workers/omni_agent.py` & `swarms-0.4.6/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms/tools/main.py` & `swarms-0.4.6/swarms/tools/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,25 +19,15 @@
 
 # import llama_index
 # from llama_index import GPTVectorStoreIndex
 # from llama_index.readers.database import DatabaseReader
 
 # from logger import logger
 
-
-import logging
-
-logger = logging.getLogger()
-formatter = logging.Formatter("%(message)s")
-ch = logging.StreamHandler()
-ch.setFormatter(formatter)
-logger.addHandler(ch)
-
-logger.setLevel(logging.DEBUG)
-
+from swarms.utils import logger
 
 class ToolScope(Enum):
     GLOBAL = "global"
     SESSION = "session"
 
 
 SessionGetter = Callable[[], Tuple[str, AgentExecutor]]
```

### Comparing `swarms-0.4.5/swarms/utils/ansi.py` & `swarms-0.4.6/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms/utils/utils.py` & `swarms-0.4.6/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.5/swarms.egg-info/PKG-INFO` & `swarms-0.4.6/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.5
+Version: 0.4.6
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.5/swarms.egg-info/SOURCES.txt` & `swarms-0.4.6/swarms.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 swarms/agents/workers/multi_modal.py
 swarms/agents/workers/omni_agent.py
 swarms/agents/workers/models/__init__.py
 swarms/tools/__init__.py
 swarms/tools/main.py
 swarms/utils/__init__.py
 swarms/utils/ansi.py
+swarms/utils/logger.py
 swarms/utils/utils.py
```

### Comparing `swarms-0.4.5/swarms.egg-info/requires.txt` & `swarms-0.4.6/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

