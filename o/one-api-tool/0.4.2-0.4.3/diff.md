# Comparing `tmp/one-api-tool-0.4.2.tar.gz` & `tmp/one-api-tool-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.4.2.tar", last modified: Mon Jul  3 11:12:54 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.3.tar", last modified: Tue Jul  4 04:47:18 2023, max compression
```

## Comparing `one-api-tool-0.4.2.tar` & `one-api-tool-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.436479 one-api-tool-0.4.2/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.2/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 11:12:54.436247 one-api-tool-0.4.2/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.4.2/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.435044 one-api-tool-0.4.2/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.435652 one-api-tool-0.4.2/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.4.2/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.436016 one-api-tool-0.4.2/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.2/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.2/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    13366 2023-07-03 11:07:07.000000 one-api-tool-0.4.2/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.2/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 11:12:54.436555 one-api-tool-0.4.2/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-03 11:12:40.000000 one-api-tool-0.4.2/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.989775 one-api-tool-0.4.3/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.3/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 04:47:18.989529 one-api-tool-0.4.3/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6902 2023-07-04 04:45:40.000000 one-api-tool-0.4.3/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.987859 one-api-tool-0.4.3/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.988384 one-api-tool-0.4.3/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.3/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.989010 one-api-tool-0.4.3/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.3/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.3/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    18945 2023-07-04 04:45:54.000000 one-api-tool-0.4.3/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.3/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:47:18.989827 one-api-tool-0.4.3/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-04 04:42:33.000000 one-api-tool-0.4.3/setup.py
```

### Comparing `one-api-tool-0.4.2/LICENSE` & `one-api-tool-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.2/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.3/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.2/oneapi/one_api.py` & `one-api-tool-0.4.3/oneapi/one_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 import anthropic
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 import sys
 import os
 from typing import Callable, Optional, Sequence, List
 import tiktoken
+import logging
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
 from oneapi.utils import generate_function_description
-
+logger = logging.getLogger(__name__)
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(asctime)s %(filename)s:%(lineno)d %(levelname)s] %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S",
+    filemode="a"
+)
 CLAUDE_TEMPLATE = "\n\nHuman: {prompt}\n\nAssistant:"
-
-class ChatGPTMessage(BaseModel):
-    role: str
-    content: str
     
 class AbstrctMethod(BaseModel):
     api_key: str
     api_base: str
     api_type: str
     method_list_models :str 
     method_model_info :str
@@ -53,15 +56,15 @@
     api_type: str = "open_ai"
     method_list_models = "models"
     method_model_info = "models"
     method_chat = "/chat/completions"
     method_commpletions = "completions"
 
 class OpenAIDecodingArguments(BaseModel):
-    messages: List[ChatGPTMessage] 
+    messages: List[dict] 
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 2048
     temperature: float = 1
     functions: Optional[list] = None
     # Controls how the model responds to function calls. 
     # "none" means the model does not call a function, and responds to the end-user. 
     # "auto" means the model can pick between an end-user or calling a function. Specifying a particular function via {"name":\ "my_function"} forces the model to call that function. 
@@ -72,15 +75,15 @@
     stream: bool = False
     stop: Optional[Sequence[str]] = None
     presence_penalty: float = 0
     frequency_penalty: float = 0
     user: Optional[str] = ""
 
 class AzureDecodingArguments(BaseModel):
-    messages: List[ChatGPTMessage] 
+    messages: List[dict] 
     engine: str = "gpt-35-turbo" # The deployment name you chose when you deployed the ChatGPT or GPT-4 model
     max_tokens: int = 2048
     temperature: float = 1
     top_p: float = 1
     n: int = 1
     stream: bool = False
     stop: Optional[Sequence[str]] = None
@@ -144,19 +147,22 @@
                 chunk_choice = chunk["choices"][0]
                 chunk_message = chunk_choice["delta"]  # extract the message
                 finish_reason = chunk_choice["finish_reason"]
                 collected_messages.append(chunk_message)  # save the message
             full_reply_content = "".join([m.get("content", "") for m in collected_messages])
             return full_reply_content
         else:
+            response_message = completion.choices[0].message
             if is_function_call:
-                function_args = completion.choices[0].message.get("function_call")
-                if function_args is not None:
-                    return function_args
-            return completion.choices[0].message.get("content", "")
+                if response_message["function_call"] is not None:
+                    return response_message
+            return response_message.get("content", "")
+
+
+         
 
 
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
         assert len(texts) <= 2048, "The batch size should not be larger than 2048."
         # replace newlines, which can negatively affect performance.
         texts = [text.replace("\n", " ") for text in texts]
 
@@ -253,22 +259,22 @@
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
-    def simple_chat(self, prompt: str|list|dict|ChatGPTMessage, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
+    def simple_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
-            msgs = [] if not system else [ChatGPTMessage(role="system", content=system)]
+            msgs = [] if not system else [dict(role="system", content=system)]
             if isinstance(prompt, str):
-                msgs.append(ChatGPTMessage(role="user", content=prompt))
+                msgs.append(dict(role="user", content=prompt))
             elif isinstance(prompt, list):
                 msgs.extend(prompt)
-            elif isinstance(prompt, (dict, ChatGPTMessage)):
+            elif isinstance(prompt, dict):
                 msgs.append(prompt)
             else:
                 raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
                 if functions is not None and isinstance(functions, list):
@@ -282,14 +288,72 @@
             args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
 
+    def function_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
+        """A full chain of function calling.
+        Step1: Call the model with functions and user prompt.
+        Step2: Use the model response to call your API.
+        Step3: Send the API response back to the model to summarize.
+
+        Args:
+            prompt (str | list | dict): User input.
+            system (str, optional): System message for ChatGPT. Defaults to "".
+            functions (List[Callable], optional): A list of functions for model to decide with function to use. Defaults to None.
+            function_call (Optional[str | dict], optional): Controls how the model responds to function calls. "none" means the model does not call a function, and responds to the end-user. "auto" means the model can pick between an end-user or calling a function. Specifying a particular function via {"name":\ "my_function"} forces the model to call that function. "none" is the default when no functions are present. "auto" is the default if functions are present.. Defaults to None.
+            model (str, optional): Model name. Defaults to GPT-3.5-turbo/Claude-v1.3-100k. 
+            temperature (int, optional): What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. Defaults to 1.
+            max_new_tokens (int, optional): Defaults to 2048.
+            stream (bool, optional): Defaults to True.
+
+        Raises:
+            AssertionError: When no function response found. Usually because of prompt injection.
+        """
+        assert len(functions) > 0, "No functions found."
+        if isinstance(self.tool, OpenAITool) and isinstance(self.tool.method, OpenAIMethod):
+            msgs = [] if not system else [dict(role="system", content=system)]
+            if isinstance(prompt, str):
+                msgs.append(dict(role="user", content=prompt))
+            elif isinstance(prompt, list):
+                msgs.extend(prompt)
+            elif isinstance(prompt, dict):
+                msgs.append(prompt)
+            else:
+                raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
+            function_response = self.simple_chat(prompt, system, functions, function_call, model, temperature, max_new_tokens, stream, **kwargs)
+            function_response_detail = function_response.get("function_call")
+            logger.debug(f"Function calling step1, function_response_detail: {function_response_detail}")
+            if not function_response_detail:
+                raise AssertionError(f"Function call not found in response: {function_response}")
+            arguments = json.loads(function_response_detail["arguments"])
+            function_name = function_response_detail["name"]
+            # force to use the function name in function_call
+            if isinstance(function_call, dict) and "name" in function_call:
+                function_name = function_call["name"] 
+            func_name_vs_func = {func.__name__: func for func in functions}
+            func = func_name_vs_func.get(function_name)
+            if not func:
+                raise AssertionError(f"Chosen function {function_name} not found in functions: {functions}")
+            api_response = func(**arguments)
+            logger.debug(f"Function calling step2, calling fun: {function_name}, api_response: {api_response}")
+            msgs.append(function_response)
+            msgs.append({"role": "function", "name": function_name, "content": json.dumps(api_response)})
+            final_response = self.simple_chat(msgs, model=model, temperature=temperature, max_new_tokens=max_new_tokens, stream=stream, **kwargs)
+            logger.debug(f"Function calling step3, Model summarize, final_response: {final_response}")
+            return final_response
+        else:
+            raise AssertionError(f"Function chat currently only support api type: {type(self.tool)}")
+
+        
+
+
+
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
         if isinstance(self.tool, OpenAITool):
             return self.tool.get_embeddings(texts, engine)  
         else:
             raise AssertionError(f"Not supported api type for embeddings: {type(self.tool)}")
 
     def get_embedding(self, text: str, engine="text-embedding-ada-002") -> List[float]:
@@ -304,7 +368,32 @@
         elif isinstance(self.tool, ClaudeAITool):
             return sum([anthropic.count_tokens(text) for text in texts])
         else:
             raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
 
 
 
+# if __name__ == "__main__":
+#     api = OneAPITool.from_config_file("../ant/config/openapi_official_chenghao.json")
+#     def get_whether_of_city(city: str, date: str) -> dict:
+#         """Get the weather of a city at a date
+
+#         Args:
+#             city (str): City name
+#             date (str): Date of the weather
+
+#         Returns:
+#             Dict: Weather information
+#         """
+#         return {"city": city, "date": date, "weather": "sunny", "temperature": 30, "air_condition": "good"}
+#     res = api.function_chat("What's the weather like in New York on July 10th?", functions=[get_whether_of_city])
+#     print(res)
+    # function_response = api.simple_chat(msgs, model='gpt-3.5-turbo-0613', functions=[get_whether_of_city])
+    # print(f'Function response:\n{function_response}')
+    # function_call = function_response['function_call']
+    # arguments = json.loads(function_call['arguments'])
+    # wether_info = get_whether_of_city(**arguments)
+    # print(f'Wether_info:\n{wether_info}')
+    # msgs.append(function_response)
+    # msgs.append({"role": "function", "name": function_call["name"], "content": json.dumps(wether_info)})
+    # second_res = api.simple_chat(msgs, model='gpt-3.5-turbo-0613')
+    # print(f'Second response:\n{second_res}')
```

### Comparing `one-api-tool-0.4.2/oneapi/utils.py` & `one-api-tool-0.4.3/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.2/setup.py` & `one-api-tool-0.4.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.4.2",
+    version="0.4.3",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

