# Comparing `tmp/swarms-0.2.9.tar.gz` & `tmp/swarms-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.2.9.tar", last modified: Tue Jul  4 03:44:09 2023, max compression
+gzip compressed data, was "swarms-0.3.0.tar", last modified: Tue Jul  4 03:55:04 2023, max compression
```

## Comparing `swarms-0.2.9.tar` & `swarms-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:44:09.910397 swarms-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 03:43:57.000000 swarms-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 03:44:09.910397 swarms-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 03:43:57.000000 swarms-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:44:09.910397 swarms-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-04 03:43:57.000000 swarms-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:44:09.910397 swarms-0.2.9/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:44:09.910397 swarms-0.2.9/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:44:09.910397 swarms-0.2.9/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 03:43:57.000000 swarms-0.2.9/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:44:09.910397 swarms-0.2.9/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 03:44:09.000000 swarms-0.2.9/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 03:44:09.000000 swarms-0.2.9/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:44:09.000000 swarms-0.2.9/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 03:44:09.000000 swarms-0.2.9/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 03:44:09.000000 swarms-0.2.9/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:55:04.677638 swarms-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 03:54:55.000000 swarms-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 03:55:04.677638 swarms-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 03:54:55.000000 swarms-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:55:04.677638 swarms-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-04 03:54:55.000000 swarms-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:55:04.673638 swarms-0.3.0/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:55:04.673638 swarms-0.3.0/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:55:04.673638 swarms-0.3.0/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:55:04.673638 swarms-0.3.0/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79474 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 03:54:55.000000 swarms-0.3.0/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:55:04.673638 swarms-0.3.0/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 03:55:04.000000 swarms-0.3.0/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 03:55:04.000000 swarms-0.3.0/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:55:04.000000 swarms-0.3.0/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 03:55:04.000000 swarms-0.3.0/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 03:55:04.000000 swarms-0.3.0/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.2.9/LICENSE` & `swarms-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/PKG-INFO` & `swarms-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.2.9
+Version: 0.3.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.2.9/README.md` & `swarms-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/setup.py` & `swarms-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #         subprocess.check_call(["pip", "install", "git+https://github.com/IDEA-Research/GroundingDINO.git"])
 #         subprocess.check_call(["pip", "install", "git+https://github.com/facebookresearch/segment-anything.git"])
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.2.9',
+  version = '0.3.0',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.2.9/swarms/agents/swarms.py` & `swarms-0.3.0/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/swarms/agents/workers/agents.py` & `swarms-0.3.0/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/swarms/agents/workers/auto_agent.py` & `swarms-0.3.0/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.3.0/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/swarms/agents/workers/multi_modal.py` & `swarms-0.3.0/swarms/agents/workers/multi_modal.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from langchain.agents.initialize import initialize_agent
 from langchain.agents.tools import Tool
 from langchain.chains.conversation.memory import ConversationBufferMemory
 from langchain.llms.openai import OpenAI
 
 # Grounding DINO
 # import groundingdino.datasets.transforms as T
-import swarms.agents.workers.models.GroundingDINO.groundingdino.datasets.transforms as T
-from swarms.agents.workers.models.GroundingDINO.groundingdino.models import build_model
-from swarms.agents.workers.models.GroundingDINO.groundingdino.util import box_ops
-from swarms.agents.workers.models.GroundingDINO.groundingdino.util.slconfig import SLConfig
-from swarms.agents.workers.models.GroundingDINO.groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
+from swarms.agents.workers.models import T
+from swarms.agents.workers.models import build_model
+from swarms.agents.workers.models import box_ops
+from swarms.agents.workers.models import SLConfig
+from swarms.agents.workers.models import clean_state_dict, get_phrases_from_posmap
 
 from swarms.agents.workers.models.segment_anything.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 import wget
```

### Comparing `swarms-0.2.9/swarms/agents/workers/omni_agent.py` & `swarms-0.3.0/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.9/swarms.egg-info/PKG-INFO` & `swarms-0.3.0/swarms.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.2.9
+Version: 0.3.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.2.9/swarms.egg-info/requires.txt` & `swarms-0.3.0/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

