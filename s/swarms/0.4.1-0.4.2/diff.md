# Comparing `tmp/swarms-0.4.1.tar.gz` & `tmp/swarms-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.1.tar", last modified: Tue Jul  4 17:17:00 2023, max compression
+gzip compressed data, was "swarms-0.4.2.tar", last modified: Tue Jul  4 17:40:40 2023, max compression
```

## Comparing `swarms-0.4.1.tar` & `swarms-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.207509 swarms-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:16:49.000000 swarms-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:17:00.207509 swarms-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-04 17:16:49.000000 swarms-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:17:00.207509 swarms-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-04 17:16:49.000000 swarms-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.203509 swarms-0.4.1/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.203509 swarms-0.4.1/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.203509 swarms-0.4.1/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.203509 swarms-0.4.1/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.207509 swarms-0.4.1/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70806 2023-07-04 17:16:49.000000 swarms-0.4.1/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:17:00.203509 swarms-0.4.1/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:17:00.000000 swarms-0.4.1/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 17:17:00.000000 swarms-0.4.1/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:17:00.000000 swarms-0.4.1/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-04 17:17:00.000000 swarms-0.4.1/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 17:17:00.000000 swarms-0.4.1/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:40:30.000000 swarms-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:40:40.023820 swarms-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16455 2023-07-04 17:40:30.000000 swarms-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:30.000000 swarms-0.4.2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 17:40:30.000000 swarms-0.4.2/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 17:40:30.000000 swarms-0.4.2/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 17:40:30.000000 swarms-0.4.2/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:40:40.023820 swarms-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-04 17:40:30.000000 swarms-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70990 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.1/LICENSE` & `swarms-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/PKG-INFO` & `swarms-0.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.1
+Version: 0.4.2
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.1/README.md` & `swarms-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,27 @@
 # Method1
 * Pip install `python3 -m pip install swarms`
 
 * Create new python file and unleash superintelligence
 
 ```python
 
-from swarms import boss_node
+from swarms import Swarms
 
-#create a task
-task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
+# Retrieve your API key from the environment or replace with your actual key
+api_key = "api key"
 
-#or 
-# task = boss_node.create_task('Find a video of Elon Musk and make him look like a cat')
+# Initialize Swarms with your API key
+swarm = Swarms(openai_api_key=api_key)
 
-boss_node.execute(task)
+# Define an objective
+objective = "Find 20 potential customers for a Swarms based AI Agent automation infrastructure"
+
+# Run Swarms
+swarm.run_swarms(objective)
 ```
 
 # Method2
 Download via Github, and install requirements
 ```bash
 git clone https://github.com/kyegomez/swarms.git
 cd swarms
@@ -81,19 +85,27 @@
     def execute_task(self, task):
         # task execution code goes here
 ```
 
 With the `BossNode` class, you can create tasks for your tools to perform. For example, you can create a task to write a summary of a specific topic:
 
 ```python
-from swarms import boss_node
-#create a task
-task = boss_node.create_task(objective="Write a research paper on the impact of climate change on global agriculture")
-#execute the teask
-boss_node.execute_task(task)
+from swarms import Swarms
+
+# Retrieve your API key from the environment or replace with your actual key
+api_key = "api key"
+
+# Initialize Swarms with your API key
+swarm = Swarms(openai_api_key=api_key)
+
+# Define an objective
+objective = "Find 20 potential customers for a Swarms based AI Agent automation infrastructure"
+
+# Run Swarms
+swarm.run_swarms(objective)
 
 ```
 
 This will create and execute a task to write a summary about the latest news on quantum computing. The result will be the summary of the news.
 
 
 ## Share with your Friends
@@ -124,14 +136,22 @@
 
 ## TODO
 
 * Develop Conversational UI with Gradio
 
 * Integrate omni agent as a worker tool
 
+* Create a tool that creates other tools with access to write code, debug, and an architectural argent that creates the architecture and then another agent that creates the code
+
+* Create a screenshot tool that takes a screen shot and then passes it to a worker multi-modal agent for visual context.
+
+* Provide FASTAPI access in a file
+
+
+
 
 1. **Multi-Agent Debate Integration**: Integrate multi-agent debate frameworks ([Multi Agent debate](https://github.com/Skytliang/Multi-Agents-Debate) and [Multi agent2 debate](https://github.com/composable-models/llm_multiagent_debate)) to improve decision-making.
 
 2. **Meta Prompting Integration**: Include meta prompting across all worker agents to guide their actions.
 
 3. **Swarms Class**: Create a main swarms class `swarms('Increase sales by 40$', workers=4)` for managing and coordinating multiple worker nodes.
```

### Comparing `swarms-0.4.1/setup.py` & `swarms-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.4.1',
+  version = '0.4.2',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -27,14 +27,15 @@
         "torchvision==0.14.1",
         "asyncio",
         "nest_asyncio",
         "bs4",
         "playwright",
         "duckduckgo_search",
         "faiss-cpu",
+        "python-ptrace==0.9.8",
         "wget==3.2",
         "accelerate",
         "addict",
         "albumentations",
         "basicsr",
         "controlnet-aux",
         "diffusers",
```

### Comparing `swarms-0.4.1/swarms/agents/swarms.py` & `swarms-0.4.2/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/swarms/agents/workers/agents.py` & `swarms-0.4.2/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/swarms/agents/workers/auto_agent.py` & `swarms-0.4.2/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.2/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/swarms/agents/workers/multi_modal.py` & `swarms-0.4.2/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/swarms/agents/workers/omni_agent.py` & `swarms-0.4.2/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.1/swarms/tools/main.py` & `swarms-0.4.2/swarms/tools/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2149,132 +2149,132 @@
 #
 
 
 
 
 
 ############################################### ===========================> Whisperx speech to text
-import os
-from pydantic import BaseModel, Field
-from pydub import AudioSegment
-from pytube import YouTube
-import whisperx
-from langchain.tools import tool
-
-
-hf_api_key = os.environ["HF_API_KEY"]
-# define a custom input schema for the youtube url
-class YouTubeVideoInput(BaseModel):
-    video_url: str = Field(description="YouTube Video URL to transcribe")
+# import os
+# from pydantic import BaseModel, Field
+# from pydub import AudioSegment
+# from pytube import YouTube
+# import whisperx
+# from langchain.tools import tool
+
+
+# hf_api_key = os.environ["HF_API_KEY"]
+# # define a custom input schema for the youtube url
+# class YouTubeVideoInput(BaseModel):
+#     video_url: str = Field(description="YouTube Video URL to transcribe")
 
 
-def download_youtube_video(video_url, audio_format='mp3'):
-    audio_file = f'video.{audio_format}'
+# def download_youtube_video(video_url, audio_format='mp3'):
+#     audio_file = f'video.{audio_format}'
     
-    # Download video
-    yt = YouTube(video_url)
-    yt_stream = yt.streams.filter(only_audio=True).first()
-    yt_stream.download(filename='video.mp4')
-
-    # Convert video to audio
-    video = AudioSegment.from_file("video.mp4", format="mp4")
-    video.export(audio_file, format=audio_format)
-    os.remove("video.mp4")
+#     # Download video
+#     yt = YouTube(video_url)
+#     yt_stream = yt.streams.filter(only_audio=True).first()
+#     yt_stream.download(filename='video.mp4')
+
+#     # Convert video to audio
+#     video = AudioSegment.from_file("video.mp4", format="mp4")
+#     video.export(audio_file, format=audio_format)
+#     os.remove("video.mp4")
     
-    return audio_file
+#     return audio_file
 
 
-@tool("transcribe_youtube_video", args_schema=YouTubeVideoInput, return_direct=True)
-def transcribe_youtube_video(video_url: str) -> str:
-    """Transcribes a YouTube video."""
-    audio_file = download_youtube_video(video_url)
+# @tool("transcribe_youtube_video", args_schema=YouTubeVideoInput, return_direct=True)
+# def transcribe_youtube_video(video_url: str) -> str:
+#     """Transcribes a YouTube video."""
+#     audio_file = download_youtube_video(video_url)
     
-    device = "cuda"
-    batch_size = 16
-    compute_type = "float16"
-
-    # 1. Transcribe with original Whisper (batched)
-    model = whisperx.load_model("large-v2", device, compute_type=compute_type)
-    audio = whisperx.load_audio(audio_file)
-    result = model.transcribe(audio, batch_size=batch_size)
-
-    # 2. Align Whisper output
-    model_a, metadata = whisperx.load_align_model(language_code=result["language"], device=device)
-    result = whisperx.align(result["segments"], model_a, metadata, audio, device, return_char_alignments=False)
+#     device = "cuda"
+#     batch_size = 16
+#     compute_type = "float16"
+
+#     # 1. Transcribe with original Whisper (batched)
+#     model = whisperx.load_model("large-v2", device, compute_type=compute_type)
+#     audio = whisperx.load_audio(audio_file)
+#     result = model.transcribe(audio, batch_size=batch_size)
+
+#     # 2. Align Whisper output
+#     model_a, metadata = whisperx.load_align_model(language_code=result["language"], device=device)
+#     result = whisperx.align(result["segments"], model_a, metadata, audio, device, return_char_alignments=False)
 
-    # 3. Assign speaker labels
+#     # 3. Assign speaker labels
 
-    diarize_model = whisperx.DiarizationPipeline(use_auth_token=hf_api_key, device=device)
-    diarize_segments = diarize_model(audio_file)
+#     diarize_model = whisperx.DiarizationPipeline(use_auth_token=hf_api_key, device=device)
+#     diarize_segments = diarize_model(audio_file)
     
-    try:
-      segments = result["segments"]
-      transcription = " ".join(segment['text'] for segment in segments)
-      return transcription
-    except KeyError:
-      print("The key 'segments' is not found in the result.")
+#     try:
+#       segments = result["segments"]
+#       transcription = " ".join(segment['text'] for segment in segments)
+#       return transcription
+#     except KeyError:
+#       print("The key 'segments' is not found in the result.")
 
 
 
-################################################### BASE WHISPER TOOL
-from typing import Optional, Type
-from pydantic import BaseModel, Field
-from langchain.tools import BaseTool
-from langchain.callbacks.manager import (
-    AsyncCallbackManagerForToolRun,
-    CallbackManagerForToolRun,
-)
-import requests
-import whisperx
-
-class AudioInput(BaseModel):
-    audio_file: str = Field(description="Path to audio file")
-
-
-class TranscribeAudioTool(BaseTool):
-    name = "transcribe_audio"
-    description = "Transcribes an audio file using WhisperX"
-    args_schema: Type[AudioInput] = AudioInput
-
-    def _run(
-        self,
-        audio_file: str,
-        device: str = "cuda",
-        batch_size: int = 16,
-        compute_type: str = "float16",
-        run_manager: Optional[CallbackManagerForToolRun] = None,
-    ) -> str:
-        """Use the tool."""
-        model = whisperx.load_model("large-v2", device, compute_type=compute_type)
-        audio = whisperx.load_audio(audio_file)
-        result = model.transcribe(audio, batch_size=batch_size)
+# ################################################### BASE WHISPER TOOL
+# from typing import Optional, Type
+# from pydantic import BaseModel, Field
+# from langchain.tools import BaseTool
+# from langchain.callbacks.manager import (
+#     AsyncCallbackManagerForToolRun,
+#     CallbackManagerForToolRun,
+# )
+# import requests
+# import whisperx
+
+# class AudioInput(BaseModel):
+#     audio_file: str = Field(description="Path to audio file")
+
+
+# class TranscribeAudioTool(BaseTool):
+#     name = "transcribe_audio"
+#     description = "Transcribes an audio file using WhisperX"
+#     args_schema: Type[AudioInput] = AudioInput
+
+#     def _run(
+#         self,
+#         audio_file: str,
+#         device: str = "cuda",
+#         batch_size: int = 16,
+#         compute_type: str = "float16",
+#         run_manager: Optional[CallbackManagerForToolRun] = None,
+#     ) -> str:
+#         """Use the tool."""
+#         model = whisperx.load_model("large-v2", device, compute_type=compute_type)
+#         audio = whisperx.load_audio(audio_file)
+#         result = model.transcribe(audio, batch_size=batch_size)
         
-        model_a, metadata = whisperx.load_align_model(language_code=result["language"], device=device)
-        result = whisperx.align(result["segments"], model_a, metadata, audio, device, return_char_alignments=False)
+#         model_a, metadata = whisperx.load_align_model(language_code=result["language"], device=device)
+#         result = whisperx.align(result["segments"], model_a, metadata, audio, device, return_char_alignments=False)
 
-        diarize_model = whisperx.DiarizationPipeline(use_auth_token=hf_api_key, device=device)
-        diarize_segments = diarize_model(audio_file)
+#         diarize_model = whisperx.DiarizationPipeline(use_auth_token=hf_api_key, device=device)
+#         diarize_segments = diarize_model(audio_file)
         
-        try:
-            segments = result["segments"]
-            transcription = " ".join(segment['text'] for segment in segments)
-            return transcription
-        except KeyError:
-            print("The key 'segments' is not found in the result.")
-
-    async def _arun(
-        self,
-        audio_file: str,
-        device: str = "cuda",
-        batch_size: int = 16,
-        compute_type: str = "float16",
-        run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
-    ) -> str:
-        """Use the tool asynchronously."""
-        raise NotImplementedError("transcribe_audio does not support async")
+#         try:
+#             segments = result["segments"]
+#             transcription = " ".join(segment['text'] for segment in segments)
+#             return transcription
+#         except KeyError:
+#             print("The key 'segments' is not found in the result.")
+
+#     async def _arun(
+#         self,
+#         audio_file: str,
+#         device: str = "cuda",
+#         batch_size: int = 16,
+#         compute_type: str = "float16",
+#         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
+#     ) -> str:
+#         """Use the tool asynchronously."""
+#         raise NotImplementedError("transcribe_audio does not support async")
 
 
 
 ###########=========================>
 
 #======> Calculator
 from langchain import LLMMathChain
```

### Comparing `swarms-0.4.1/swarms.egg-info/PKG-INFO` & `swarms-0.4.2/swarms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.1
+Version: 0.4.2
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.1/swarms.egg-info/requires.txt` & `swarms-0.4.2/swarms.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 torchvision==0.14.1
 asyncio
 nest_asyncio
 bs4
 playwright
 duckduckgo_search
 faiss-cpu
+python-ptrace==0.9.8
 wget==3.2
 accelerate
 addict
 albumentations
 basicsr
 controlnet-aux
 diffusers
```

