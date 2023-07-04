# Comparing `tmp/one-api-tool-0.4.3.tar.gz` & `tmp/one-api-tool-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.4.3.tar", last modified: Tue Jul  4 04:47:18 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.4.tar", last modified: Tue Jul  4 05:02:15 2023, max compression
```

## Comparing `one-api-tool-0.4.3.tar` & `one-api-tool-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.989775 one-api-tool-0.4.3/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.3/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 04:47:18.989529 one-api-tool-0.4.3/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     6902 2023-07-04 04:45:40.000000 one-api-tool-0.4.3/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.987859 one-api-tool-0.4.3/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-04 04:47:18.000000 one-api-tool-0.4.3/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.988384 one-api-tool-0.4.3/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.3/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 04:47:18.989010 one-api-tool-0.4.3/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.3/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.3/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    18945 2023-07-04 04:45:54.000000 one-api-tool-0.4.3/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.3/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:47:18.989827 one-api-tool-0.4.3/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-04 04:42:33.000000 one-api-tool-0.4.3/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:02:15.041786 one-api-tool-0.4.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 05:02:15.041558 one-api-tool-0.4.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6902 2023-07-04 04:45:40.000000 one-api-tool-0.4.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:02:15.039827 one-api-tool-0.4.4/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 05:02:15.000000 one-api-tool-0.4.4/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-04 05:02:15.000000 one-api-tool-0.4.4/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-04 05:02:15.000000 one-api-tool-0.4.4/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-04 05:02:15.000000 one-api-tool-0.4.4/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-04 05:02:15.000000 one-api-tool-0.4.4/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-04 05:02:15.000000 one-api-tool-0.4.4/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:02:15.040563 one-api-tool-0.4.4/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.4/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:02:15.041164 one-api-tool-0.4.4/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.4/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.4/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    17763 2023-07-04 05:00:50.000000 one-api-tool-0.4.4/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.4/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 05:02:15.041839 one-api-tool-0.4.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-04 05:02:11.000000 one-api-tool-0.4.4/setup.py
```

### Comparing `one-api-tool-0.4.3/LICENSE` & `one-api-tool-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.3/PKG-INFO` & `one-api-tool-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.3
+Version: 0.4.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.3/README.md` & `one-api-tool-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.3/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.4.4/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.3
+Version: 0.4.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.3/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.4/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.3/oneapi/one_api.py` & `one-api-tool-0.4.4/oneapi/one_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 import sys
 import os
 from typing import Callable, Optional, Sequence, List
 import tiktoken
 import logging
+from openai.openai_object import OpenAIObject
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
 from oneapi.utils import generate_function_description
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(filename)s:%(lineno)d %(levelname)s] %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
@@ -149,15 +150,15 @@
                 finish_reason = chunk_choice["finish_reason"]
                 collected_messages.append(chunk_message)  # save the message
             full_reply_content = "".join([m.get("content", "") for m in collected_messages])
             return full_reply_content
         else:
             response_message = completion.choices[0].message
             if is_function_call:
-                if response_message["function_call"] is not None:
+                if response_message.get("function_call") is not None:
                     return response_message
             return response_message.get("content", "")
 
 
          
 
 
@@ -321,15 +322,15 @@
             elif isinstance(prompt, dict):
                 msgs.append(prompt)
             else:
                 raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
             function_response = self.simple_chat(prompt, system, functions, function_call, model, temperature, max_new_tokens, stream, **kwargs)
             function_response_detail = function_response.get("function_call")
             logger.debug(f"Function calling step1, function_response_detail: {function_response_detail}")
-            if not function_response_detail:
+            if not function_response_detail or not isinstance(function_response_detail, dict):
                 raise AssertionError(f"Function call not found in response: {function_response}")
             arguments = json.loads(function_response_detail["arguments"])
             function_name = function_response_detail["name"]
             # force to use the function name in function_call
             if isinstance(function_call, dict) and "name" in function_call:
                 function_name = function_call["name"] 
             func_name_vs_func = {func.__name__: func for func in functions}
@@ -364,36 +365,8 @@
     
     def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
         if isinstance(self.tool, OpenAITool):
             return self.tool.count_tokens(texts, encoding_name)
         elif isinstance(self.tool, ClaudeAITool):
             return sum([anthropic.count_tokens(text) for text in texts])
         else:
-            raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
-
-
-
-# if __name__ == "__main__":
-#     api = OneAPITool.from_config_file("../ant/config/openapi_official_chenghao.json")
-#     def get_whether_of_city(city: str, date: str) -> dict:
-#         """Get the weather of a city at a date
-
-#         Args:
-#             city (str): City name
-#             date (str): Date of the weather
-
-#         Returns:
-#             Dict: Weather information
-#         """
-#         return {"city": city, "date": date, "weather": "sunny", "temperature": 30, "air_condition": "good"}
-#     res = api.function_chat("What's the weather like in New York on July 10th?", functions=[get_whether_of_city])
-#     print(res)
-    # function_response = api.simple_chat(msgs, model='gpt-3.5-turbo-0613', functions=[get_whether_of_city])
-    # print(f'Function response:\n{function_response}')
-    # function_call = function_response['function_call']
-    # arguments = json.loads(function_call['arguments'])
-    # wether_info = get_whether_of_city(**arguments)
-    # print(f'Wether_info:\n{wether_info}')
-    # msgs.append(function_response)
-    # msgs.append({"role": "function", "name": function_call["name"], "content": json.dumps(wether_info)})
-    # second_res = api.simple_chat(msgs, model='gpt-3.5-turbo-0613')
-    # print(f'Second response:\n{second_res}')
+            raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
```

### Comparing `one-api-tool-0.4.3/oneapi/utils.py` & `one-api-tool-0.4.4/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.3/setup.py` & `one-api-tool-0.4.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.4.3",
+    version="0.4.4",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

