# Comparing `tmp/swarms-0.2.3.tar.gz` & `tmp/swarms-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.2.3.tar", last modified: Tue Jul  4 02:03:47 2023, max compression
+gzip compressed data, was "swarms-0.2.8.tar", last modified: Tue Jul  4 03:29:14 2023, max compression
```

## Comparing `swarms-0.2.3.tar` & `swarms-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.626384 swarms-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 02:03:35.000000 swarms-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 02:03:47.626384 swarms-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-04 02:03:35.000000 swarms-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 02:03:47.626384 swarms-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 02:03:35.000000 swarms-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.622384 swarms-0.2.3/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.626384 swarms-0.2.3/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.626384 swarms-0.2.3/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/metaprompt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    79319 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 02:03:35.000000 swarms-0.2.3/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:03:47.622384 swarms-0.2.3/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 02:03:47.000000 swarms-0.2.3/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:29:14.639377 swarms-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 03:29:04.000000 swarms-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 03:29:14.635377 swarms-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-04 03:29:04.000000 swarms-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:29:14.639377 swarms-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-04 03:29:04.000000 swarms-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:29:14.631377 swarms-0.2.8/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:29:14.635377 swarms-0.2.8/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:29:14.635377 swarms-0.2.8/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/workers/metaprompt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79537 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 03:29:04.000000 swarms-0.2.8/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:29:14.635377 swarms-0.2.8/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 03:29:14.000000 swarms-0.2.8/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 03:29:14.000000 swarms-0.2.8/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:29:14.000000 swarms-0.2.8/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 03:29:14.000000 swarms-0.2.8/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 03:29:14.000000 swarms-0.2.8/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.2.3/LICENSE` & `swarms-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.2.3/PKG-INFO` & `swarms-0.2.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.2.3
+Version: 0.2.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.2.3/README.md` & `swarms-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
 
 Here is the detailed roadmap of our priorities and planned features for the near term:
 
 ## TODO
 
 * Develop Conversational UI with Gradio
 
+* Develop hosted paid API so anybody can use hostedly.
+
 1. **Multi-Agent Debate Integration**: Integrate multi-agent debate frameworks ([Multi Agent debate](https://github.com/Skytliang/Multi-Agents-Debate) and [Multi agent2 debate](https://github.com/composable-models/llm_multiagent_debate)) to improve decision-making.
 
 2. **Meta Prompting Integration**: Include meta prompting across all worker agents to guide their actions.
 
 3. **Swarms Class**: Create a main swarms class `swarms('Increase sales by 40$', workers=4)` for managing and coordinating multiple worker nodes.
 
 4. **Integration of Additional Tools**: Integrate [Jarvis](https://github.com/microsoft/JARVIS) as worker nodes, add text to speech and text to script tools ([whisper x](https://github.com/kyegomez/youtubeURL-to-text)), and integrate Hugging Face agents and other external tools.
```

### Comparing `swarms-0.2.3/setup.py` & `swarms-0.2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from setuptools import setup, find_packages
 
+# from setuptools.command.install import install
+
+# class PostInstallCommand(install):
+#     """Post-installation for installation mode."""
+#     def run(self):
+#         install.run(self)
+#         # PUT YOUR POST-INSTALL SCRIPT HERE or CALL A FUNCTION
+#         import subprocess
+#         subprocess.check_call(["pip", "install", "git+https://github.com/IDEA-Research/GroundingDINO.git"])
+#         subprocess.check_call(["pip", "install", "git+https://github.com/facebookresearch/segment-anything.git"])
+
+
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.2.3',
+  version = '0.2.8',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -63,15 +75,15 @@
         "google-api-python-client",
         "google-auth-oauthlib",
         "google-auth-httplib2",
         "beautifulsoup4",
         "O365",
         "pytube",
         "pydub"
-  ],
+    ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
```

### Comparing `swarms-0.2.3/swarms/agents/swarms.py` & `swarms-0.2.8/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.3/swarms/agents/workers/agents.py` & `swarms-0.2.8/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.3/swarms/agents/workers/auto_agent.py` & `swarms-0.2.8/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.3/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.2.8/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.3/swarms/agents/workers/multi_modal.py` & `swarms-0.2.8/swarms/agents/workers/multi_modal.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,39 +29,39 @@
 from langchain.agents.initialize import initialize_agent
 from langchain.agents.tools import Tool
 from langchain.chains.conversation.memory import ConversationBufferMemory
 from langchain.llms.openai import OpenAI
 
 # Grounding DINO
 # import groundingdino.datasets.transforms as T
-# from groundingdino.models import build_model
-# from groundingdino.util import box_ops
-# from groundingdino.util.slconfig import SLConfig
-# from groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
+import models.GroundingDINO.groundingdino.datasets.transforms as T
+from models.GroundingDINO.groundingdino.models import build_model
+from models.GroundingDINO.groundingdino.util import box_ops
+from models.GroundingDINO.groundingdino.util.slconfig import SLConfig
+from models.GroundingDINO.groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
 
-# segment anything #
-from segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
+from models.segment_anything.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 import wget
 
-VISUAL_CHATGPT_PREFIX = """Visual ChatGPT is designed to be able to assist with a wide range of text and visual related tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. Visual ChatGPT is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
+VISUAL_CHATGPT_PREFIX = """Worker Multi-Modal Agent is designed to be able to assist with a wide range of text and visual related tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. Worker Multi-Modal Agent is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 
-Visual ChatGPT is able to process and understand large amounts of text and images. As a language model, Visual ChatGPT can not directly read images, but it has a list of tools to finish different visual tasks. Each image will have a file name formed as "image/xxx.png", and Visual ChatGPT can invoke different tools to indirectly understand pictures. When talking about images, Visual ChatGPT is very strict to the file name and will never fabricate nonexistent files. When using tools to generate new image files, Visual ChatGPT is also known that the image may not be the same as the user's demand, and will use other visual question answering tools or description tools to observe the real image. Visual ChatGPT is able to use tools in a sequence, and is loyal to the tool observation outputs rather than faking the image content and image file name. It will remember to provide the file name from the last tool observation, if a new image is generated.
+Worker Multi-Modal Agent is able to process and understand large amounts of text and images. As a language model, Worker Multi-Modal Agent can not directly read images, but it has a list of tools to finish different visual tasks. Each image will have a file name formed as "image/xxx.png", and Worker Multi-Modal Agent can invoke different tools to indirectly understand pictures. When talking about images, Worker Multi-Modal Agent is very strict to the file name and will never fabricate nonexistent files. When using tools to generate new image files, Worker Multi-Modal Agent is also known that the image may not be the same as the user's demand, and will use other visual question answering tools or description tools to observe the real image. Worker Multi-Modal Agent is able to use tools in a sequence, and is loyal to the tool observation outputs rather than faking the image content and image file name. It will remember to provide the file name from the last tool observation, if a new image is generated.
 
-Human may provide new figures to Visual ChatGPT with a description. The description helps Visual ChatGPT to understand this image, but Visual ChatGPT should use tools to finish following tasks, rather than directly imagine from the description.
+Human may provide new figures to Worker Multi-Modal Agent with a description. The description helps Worker Multi-Modal Agent to understand this image, but Worker Multi-Modal Agent should use tools to finish following tasks, rather than directly imagine from the description.
 
-Overall, Visual ChatGPT is a powerful visual dialogue assistant tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. 
+Overall, Worker Multi-Modal Agent is a powerful visual dialogue assistant tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. 
 
 
 TOOLS:
 ------
 
-Visual ChatGPT  has access to the following tools:"""
+Worker Multi-Modal Agent  has access to the following tools:"""
 
 VISUAL_CHATGPT_FORMAT_INSTRUCTIONS = """To use a tool, please use the following format:
 
 ```
 Thought: Do I need to use a tool? Yes
 Action: the action to take, should be one of [{tool_names}]
 Action Input: the input to the action
@@ -81,31 +81,31 @@
 
 Begin!
 
 Previous conversation history:
 {chat_history}
 
 New input: {input}
-Since Visual ChatGPT is a text language model, Visual ChatGPT must use tools to observe images rather than imagination.
-The thoughts and observations are only visible for Visual ChatGPT, Visual ChatGPT should remember to repeat important information in the final response for Human. 
+Since Worker Multi-Modal Agent is a text language model, Worker Multi-Modal Agent must use tools to observe images rather than imagination.
+The thoughts and observations are only visible for Worker Multi-Modal Agent, Worker Multi-Modal Agent should remember to repeat important information in the final response for Human. 
 Thought: Do I need to use a tool? {agent_scratchpad} Let's think step by step.
 """
 
-VISUAL_CHATGPT_PREFIX_CN = """Visual ChatGPT 旨在能够协助完成范围广泛的文本和视觉相关任务，从回答简单的问题到提供对广泛主题的深入解释和讨论。 Visual ChatGPT 能够根据收到的输入生成类似人类的文本，使其能够进行听起来自然的对话，并提供连贯且与手头主题相关的响应。
+VISUAL_CHATGPT_PREFIX_CN = """Worker Multi-Modal Agent 旨在能够协助完成范围广泛的文本和视觉相关任务，从回答简单的问题到提供对广泛主题的深入解释和讨论。 Worker Multi-Modal Agent 能够根据收到的输入生成类似人类的文本，使其能够进行听起来自然的对话，并提供连贯且与手头主题相关的响应。
 
-Visual ChatGPT 能够处理和理解大量文本和图像。作为一种语言模型，Visual ChatGPT 不能直接读取图像，但它有一系列工具来完成不同的视觉任务。每张图片都会有一个文件名，格式为“image/xxx.png”，Visual ChatGPT可以调用不同的工具来间接理解图片。在谈论图片时，Visual ChatGPT 对文件名的要求非常严格，绝不会伪造不存在的文件。在使用工具生成新的图像文件时，Visual ChatGPT也知道图像可能与用户需求不一样，会使用其他视觉问答工具或描述工具来观察真实图像。 Visual ChatGPT 能够按顺序使用工具，并且忠于工具观察输出，而不是伪造图像内容和图像文件名。如果生成新图像，它将记得提供上次工具观察的文件名。
+Worker Multi-Modal Agent 能够处理和理解大量文本和图像。作为一种语言模型，Worker Multi-Modal Agent 不能直接读取图像，但它有一系列工具来完成不同的视觉任务。每张图片都会有一个文件名，格式为“image/xxx.png”，Worker Multi-Modal Agent可以调用不同的工具来间接理解图片。在谈论图片时，Worker Multi-Modal Agent 对文件名的要求非常严格，绝不会伪造不存在的文件。在使用工具生成新的图像文件时，Worker Multi-Modal Agent也知道图像可能与用户需求不一样，会使用其他视觉问答工具或描述工具来观察真实图像。 Worker Multi-Modal Agent 能够按顺序使用工具，并且忠于工具观察输出，而不是伪造图像内容和图像文件名。如果生成新图像，它将记得提供上次工具观察的文件名。
 
-Human 可能会向 Visual ChatGPT 提供带有描述的新图形。描述帮助 Visual ChatGPT 理解这个图像，但 Visual ChatGPT 应该使用工具来完成以下任务，而不是直接从描述中想象。有些工具将会返回英文描述，但你对用户的聊天应当采用中文。
+Human 可能会向 Worker Multi-Modal Agent 提供带有描述的新图形。描述帮助 Worker Multi-Modal Agent 理解这个图像，但 Worker Multi-Modal Agent 应该使用工具来完成以下任务，而不是直接从描述中想象。有些工具将会返回英文描述，但你对用户的聊天应当采用中文。
 
-总的来说，Visual ChatGPT 是一个强大的可视化对话辅助工具，可以帮助处理范围广泛的任务，并提供关于范围广泛的主题的有价值的见解和信息。
+总的来说，Worker Multi-Modal Agent 是一个强大的可视化对话辅助工具，可以帮助处理范围广泛的任务，并提供关于范围广泛的主题的有价值的见解和信息。
 
 工具列表:
 ------
 
-Visual ChatGPT 可以使用这些工具:"""
+Worker Multi-Modal Agent 可以使用这些工具:"""
 
 VISUAL_CHATGPT_FORMAT_INSTRUCTIONS_CN = """用户使用中文和你进行聊天，但是工具的参数应当使用英文。如果要调用工具，你必须遵循如下格式:
 
 ```
 Thought: Do I need to use a tool? Yes
 Action: the action to take, should be one of [{tool_names}]
 Action Input: the input to the action
@@ -121,16 +121,16 @@
 ```
 """
 
 VISUAL_CHATGPT_SUFFIX_CN = """你对文件名的正确性非常严格，而且永远不会伪造不存在的文件。
 
 开始!
 
-因为Visual ChatGPT是一个文本语言模型，必须使用工具去观察图片而不是依靠想象。
-推理想法和观察结果只对Visual ChatGPT可见，需要记得在最终回复时把重要的信息重复给用户，你只能给用户返回中文句子。我们一步一步思考。在你使用工具时，工具的参数只能是英文。
+因为Worker Multi-Modal Agent是一个文本语言模型，必须使用工具去观察图片而不是依靠想象。
+推理想法和观察结果只对Worker Multi-Modal Agent可见，需要记得在最终回复时把重要的信息重复给用户，你只能给用户返回中文句子。我们一步一步思考。在你使用工具时，工具的参数只能是英文。
 
 聊天历史:
 {chat_history}
 
 新输入: {input}
 Thought: Do I need to use a tool? {agent_scratchpad}
 """
@@ -1019,157 +1019,157 @@
         plt.axis('off')
         plt.savefig(
             updated_image_path, 
             bbox_inches="tight", dpi=300, pad_inches=0.0
         )
         return updated_image_path
     
-# class Text2Box:
-#     def __init__(self, device):
-#         print(f"Initializing ObjectDetection to {device}")
-#         self.device = device
-#         self.torch_dtype = torch.float16 if 'cuda' in device else torch.float32
-#         self.model_checkpoint_path = os.path.join("checkpoints","groundingdino")
-#         self.model_config_path = os.path.join("checkpoints","grounding_config.py")
-#         self.download_parameters()
-#         self.box_threshold = 0.3
-#         self.text_threshold = 0.25
-#         self.grounding = (self.load_model()).to(self.device)
-
-#     def download_parameters(self):
-#         url = "https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth"
-#         if not os.path.exists(self.model_checkpoint_path):
-#             wget.download(url,out=self.model_checkpoint_path)
-#         config_url = "https://raw.githubusercontent.com/IDEA-Research/GroundingDINO/main/groundingdino/config/GroundingDINO_SwinT_OGC.py"
-#         if not os.path.exists(self.model_config_path):
-#             wget.download(config_url,out=self.model_config_path)
-#     def load_image(self,image_path):
-#          # load image
-#         image_pil = Image.open(image_path).convert("RGB")  # load image
-
-#         transform = T.Compose(
-#             [
-#                 T.RandomResize([512], max_size=1333),
-#                 T.ToTensor(),
-#                 T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]),
-#             ]
-#         )
-#         image, _ = transform(image_pil, None)  # 3, h, w
-#         return image_pil, image
-
-#     def load_model(self):
-#         args = SLConfig.fromfile(self.model_config_path)
-#         args.device = self.device
-#         model = build_model(args)
-#         checkpoint = torch.load(self.model_checkpoint_path, map_location="cpu")
-#         load_res = model.load_state_dict(clean_state_dict(checkpoint["model"]), strict=False)
-#         print(load_res)
-#         _ = model.eval()
-#         return model
-
-#     def get_grounding_boxes(self, image, caption, with_logits=True):
-#         caption = caption.lower()
-#         caption = caption.strip()
-#         if not caption.endswith("."):
-#             caption = caption + "."
-#         image = image.to(self.device)
-#         with torch.no_grad():
-#             outputs = self.grounding(image[None], captions=[caption])
-#         logits = outputs["pred_logits"].cpu().sigmoid()[0]  # (nq, 256)
-#         boxes = outputs["pred_boxes"].cpu()[0]  # (nq, 4)
-#         logits.shape[0]
-
-#         # filter output
-#         logits_filt = logits.clone()
-#         boxes_filt = boxes.clone()
-#         filt_mask = logits_filt.max(dim=1)[0] > self.box_threshold
-#         logits_filt = logits_filt[filt_mask]  # num_filt, 256
-#         boxes_filt = boxes_filt[filt_mask]  # num_filt, 4
-#         logits_filt.shape[0]
-
-#         # get phrase
-#         tokenlizer = self.grounding.tokenizer
-#         tokenized = tokenlizer(caption)
-#         # build pred
-#         pred_phrases = []
-#         for logit, box in zip(logits_filt, boxes_filt):
-#             pred_phrase = get_phrases_from_posmap(logit > self.text_threshold, tokenized, tokenlizer)
-#             if with_logits:
-#                 pred_phrases.append(pred_phrase + f"({str(logit.max().item())[:4]})")
-#             else:
-#                 pred_phrases.append(pred_phrase)
+class Text2Box:
+    def __init__(self, device):
+        print(f"Initializing ObjectDetection to {device}")
+        self.device = device
+        self.torch_dtype = torch.float16 if 'cuda' in device else torch.float32
+        self.model_checkpoint_path = os.path.join("checkpoints","groundingdino")
+        self.model_config_path = os.path.join("checkpoints","grounding_config.py")
+        self.download_parameters()
+        self.box_threshold = 0.3
+        self.text_threshold = 0.25
+        self.grounding = (self.load_model()).to(self.device)
+
+    def download_parameters(self):
+        url = "https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth"
+        if not os.path.exists(self.model_checkpoint_path):
+            wget.download(url,out=self.model_checkpoint_path)
+        config_url = "https://raw.githubusercontent.com/IDEA-Research/GroundingDINO/main/groundingdino/config/GroundingDINO_SwinT_OGC.py"
+        if not os.path.exists(self.model_config_path):
+            wget.download(config_url,out=self.model_config_path)
+    def load_image(self,image_path):
+         # load image
+        image_pil = Image.open(image_path).convert("RGB")  # load image
+
+        transform = T.Compose(
+            [
+                T.RandomResize([512], max_size=1333),
+                T.ToTensor(),
+                T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]),
+            ]
+        )
+        image, _ = transform(image_pil, None)  # 3, h, w
+        return image_pil, image
 
-#         return boxes_filt, pred_phrases
+    def load_model(self):
+        args = SLConfig.fromfile(self.model_config_path)
+        args.device = self.device
+        model = build_model(args)
+        checkpoint = torch.load(self.model_checkpoint_path, map_location="cpu")
+        load_res = model.load_state_dict(clean_state_dict(checkpoint["model"]), strict=False)
+        print(load_res)
+        _ = model.eval()
+        return model
+
+    def get_grounding_boxes(self, image, caption, with_logits=True):
+        caption = caption.lower()
+        caption = caption.strip()
+        if not caption.endswith("."):
+            caption = caption + "."
+        image = image.to(self.device)
+        with torch.no_grad():
+            outputs = self.grounding(image[None], captions=[caption])
+        logits = outputs["pred_logits"].cpu().sigmoid()[0]  # (nq, 256)
+        boxes = outputs["pred_boxes"].cpu()[0]  # (nq, 4)
+        logits.shape[0]
+
+        # filter output
+        logits_filt = logits.clone()
+        boxes_filt = boxes.clone()
+        filt_mask = logits_filt.max(dim=1)[0] > self.box_threshold
+        logits_filt = logits_filt[filt_mask]  # num_filt, 256
+        boxes_filt = boxes_filt[filt_mask]  # num_filt, 4
+        logits_filt.shape[0]
+
+        # get phrase
+        tokenlizer = self.grounding.tokenizer
+        tokenized = tokenlizer(caption)
+        # build pred
+        pred_phrases = []
+        for logit, box in zip(logits_filt, boxes_filt):
+            pred_phrase = get_phrases_from_posmap(logit > self.text_threshold, tokenized, tokenlizer)
+            if with_logits:
+                pred_phrases.append(pred_phrase + f"({str(logit.max().item())[:4]})")
+            else:
+                pred_phrases.append(pred_phrase)
+
+        return boxes_filt, pred_phrases
     
-#     def plot_boxes_to_image(self, image_pil, tgt):
-#         H, W = tgt["size"]
-#         boxes = tgt["boxes"]
-#         labels = tgt["labels"]
-#         assert len(boxes) == len(labels), "boxes and labels must have same length"
-
-#         draw = ImageDraw.Draw(image_pil)
-#         mask = Image.new("L", image_pil.size, 0)
-#         mask_draw = ImageDraw.Draw(mask)
-
-#         # draw boxes and masks
-#         for box, label in zip(boxes, labels):
-#             # from 0..1 to 0..W, 0..H
-#             box = box * torch.Tensor([W, H, W, H])
-#             # from xywh to xyxy
-#             box[:2] -= box[2:] / 2
-#             box[2:] += box[:2]
-#             # random color
-#             color = tuple(np.random.randint(0, 255, size=3).tolist())
-#             # draw
-#             x0, y0, x1, y1 = box
-#             x0, y0, x1, y1 = int(x0), int(y0), int(x1), int(y1)
-
-#             draw.rectangle([x0, y0, x1, y1], outline=color, width=6)
-#             # draw.text((x0, y0), str(label), fill=color)
-
-#             font = ImageFont.load_default()
-#             if hasattr(font, "getbbox"):
-#                 bbox = draw.textbbox((x0, y0), str(label), font)
-#             else:
-#                 w, h = draw.textsize(str(label), font)
-#                 bbox = (x0, y0, w + x0, y0 + h)
-#             # bbox = draw.textbbox((x0, y0), str(label))
-#             draw.rectangle(bbox, fill=color)
-#             draw.text((x0, y0), str(label), fill="white")
+    def plot_boxes_to_image(self, image_pil, tgt):
+        H, W = tgt["size"]
+        boxes = tgt["boxes"]
+        labels = tgt["labels"]
+        assert len(boxes) == len(labels), "boxes and labels must have same length"
+
+        draw = ImageDraw.Draw(image_pil)
+        mask = Image.new("L", image_pil.size, 0)
+        mask_draw = ImageDraw.Draw(mask)
+
+        # draw boxes and masks
+        for box, label in zip(boxes, labels):
+            # from 0..1 to 0..W, 0..H
+            box = box * torch.Tensor([W, H, W, H])
+            # from xywh to xyxy
+            box[:2] -= box[2:] / 2
+            box[2:] += box[:2]
+            # random color
+            color = tuple(np.random.randint(0, 255, size=3).tolist())
+            # draw
+            x0, y0, x1, y1 = box
+            x0, y0, x1, y1 = int(x0), int(y0), int(x1), int(y1)
+
+            draw.rectangle([x0, y0, x1, y1], outline=color, width=6)
+            # draw.text((x0, y0), str(label), fill=color)
+
+            font = ImageFont.load_default()
+            if hasattr(font, "getbbox"):
+                bbox = draw.textbbox((x0, y0), str(label), font)
+            else:
+                w, h = draw.textsize(str(label), font)
+                bbox = (x0, y0, w + x0, y0 + h)
+            # bbox = draw.textbbox((x0, y0), str(label))
+            draw.rectangle(bbox, fill=color)
+            draw.text((x0, y0), str(label), fill="white")
 
-#             mask_draw.rectangle([x0, y0, x1, y1], fill=255, width=2)
+            mask_draw.rectangle([x0, y0, x1, y1], fill=255, width=2)
 
-#         return image_pil, mask
+        return image_pil, mask
     
-#     @prompts(name="Detect the Give Object",
-#              description="useful when you only want to detect or find out given objects in the picture"  
-#                          "The input to this tool should be a comma separated string of two, "
-#                          "representing the image_path, the text description of the object to be found")
-#     def inference(self, inputs):
-#         image_path, det_prompt = inputs.split(",")
-#         print(f"image_path={image_path}, text_prompt={det_prompt}")
-#         image_pil, image = self.load_image(image_path)
-
-#         boxes_filt, pred_phrases = self.get_grounding_boxes(image, det_prompt)
-
-#         size = image_pil.size
-#         pred_dict = {
-#         "boxes": boxes_filt,
-#         "size": [size[1], size[0]],  # H,W
-#         "labels": pred_phrases,}
-
-#         image_with_box = self.plot_boxes_to_image(image_pil, pred_dict)[0]
-
-#         updated_image_path = get_new_image_name(image_path, func_name="detect-something")
-#         updated_image = image_with_box.resize(size)
-#         updated_image.save(updated_image_path)
-#         print(
-#             f"\nProcessed ObejectDetecting, Input Image: {image_path}, Object to be Detect {det_prompt}, "
-#             f"Output Image: {updated_image_path}")
-#         return updated_image_path
+    @prompts(name="Detect the Give Object",
+             description="useful when you only want to detect or find out given objects in the picture"  
+                         "The input to this tool should be a comma separated string of two, "
+                         "representing the image_path, the text description of the object to be found")
+    def inference(self, inputs):
+        image_path, det_prompt = inputs.split(",")
+        print(f"image_path={image_path}, text_prompt={det_prompt}")
+        image_pil, image = self.load_image(image_path)
+
+        boxes_filt, pred_phrases = self.get_grounding_boxes(image, det_prompt)
+
+        size = image_pil.size
+        pred_dict = {
+        "boxes": boxes_filt,
+        "size": [size[1], size[0]],  # H,W
+        "labels": pred_phrases,}
+
+        image_with_box = self.plot_boxes_to_image(image_pil, pred_dict)[0]
+
+        updated_image_path = get_new_image_name(image_path, func_name="detect-something")
+        updated_image = image_with_box.resize(size)
+        updated_image.save(updated_image_path)
+        print(
+            f"\nProcessed ObejectDetecting, Input Image: {image_path}, Object to be Detect {det_prompt}, "
+            f"Output Image: {updated_image_path}")
+        return updated_image_path
 
 
 class Inpainting:
     def __init__(self, device):
         self.device = device
         self.revision = 'fp16' if 'cuda' in self.device else None
         self.torch_dtype = torch.float16 if 'cuda' in self.device else torch.float32
```

### Comparing `swarms-0.2.3/swarms/agents/workers/omni_agent.py` & `swarms-0.2.8/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.2.3/swarms.egg-info/PKG-INFO` & `swarms-0.2.8/swarms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.2.3
+Version: 0.2.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.2.3/swarms.egg-info/requires.txt` & `swarms-0.2.8/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

