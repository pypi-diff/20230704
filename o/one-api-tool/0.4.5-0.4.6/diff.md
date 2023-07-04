# Comparing `tmp/one-api-tool-0.4.5.tar.gz` & `tmp/one-api-tool-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.4.5.tar", last modified: Tue Jul  4 05:10:09 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.6.tar", last modified: Tue Jul  4 05:17:10 2023, max compression
```

## Comparing `one-api-tool-0.4.5.tar` & `one-api-tool-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:10:09.145154 one-api-tool-0.4.5/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.5/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 05:10:09.144935 one-api-tool-0.4.5/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     6902 2023-07-04 04:45:40.000000 one-api-tool-0.4.5/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:10:09.143659 one-api-tool-0.4.5/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 05:10:09.000000 one-api-tool-0.4.5/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-04 05:10:09.000000 one-api-tool-0.4.5/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-04 05:10:09.000000 one-api-tool-0.4.5/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-04 05:10:09.000000 one-api-tool-0.4.5/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-04 05:10:09.000000 one-api-tool-0.4.5/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-04 05:10:09.000000 one-api-tool-0.4.5/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:10:09.144233 one-api-tool-0.4.5/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.5/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:10:09.144717 one-api-tool-0.4.5/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.5/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.5/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    17782 2023-07-04 05:08:54.000000 one-api-tool-0.4.5/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.5/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 05:10:09.145204 one-api-tool-0.4.5/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-04 05:10:04.000000 one-api-tool-0.4.5/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:17:10.259046 one-api-tool-0.4.6/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.6/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 05:17:10.258815 one-api-tool-0.4.6/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6902 2023-07-04 04:45:40.000000 one-api-tool-0.4.6/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:17:10.257334 one-api-tool-0.4.6/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7458 2023-07-04 05:17:10.000000 one-api-tool-0.4.6/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-04 05:17:10.000000 one-api-tool-0.4.6/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-04 05:17:10.000000 one-api-tool-0.4.6/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-04 05:17:10.000000 one-api-tool-0.4.6/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-04 05:17:10.000000 one-api-tool-0.4.6/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-04 05:17:10.000000 one-api-tool-0.4.6/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:17:10.257917 one-api-tool-0.4.6/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.6/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-04 05:17:10.258400 one-api-tool-0.4.6/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.6/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.6/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    17775 2023-07-04 05:16:00.000000 one-api-tool-0.4.6/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.6/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 05:17:10.259154 one-api-tool-0.4.6/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-04 05:17:06.000000 one-api-tool-0.4.6/setup.py
```

### Comparing `one-api-tool-0.4.5/LICENSE` & `one-api-tool-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.5/PKG-INFO` & `one-api-tool-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.5
+Version: 0.4.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.5/README.md` & `one-api-tool-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.5/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.4.6/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.5
+Version: 0.4.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.5/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.6/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.5/oneapi/one_api.py` & `one-api-tool-0.4.6/oneapi/one_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             elif isinstance(prompt, list):
                 msgs.extend(prompt)
             elif isinstance(prompt, dict):
                 msgs.append(prompt)
             else:
                 raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
             function_response = self.simple_chat(prompt, system, functions, function_call, model, temperature, max_new_tokens, stream, **kwargs)
-            if not isinstance(function_response, dict) or not function_response_detail.get("function_call"):
+            if not isinstance(function_response, dict) or not function_response.get("function_call"):
                 raise AssertionError(f"Function call not found in response: {function_response}")
             function_response_detail = function_response.get("function_call")
             logger.debug(f"Function calling step1, function_response_detail: {function_response_detail}")
             arguments = json.loads(function_response_detail["arguments"])
             function_name = function_response_detail["name"]
             # force to use the function name in function_call
             if isinstance(function_call, dict) and "name" in function_call:
```

### Comparing `one-api-tool-0.4.5/oneapi/utils.py` & `one-api-tool-0.4.6/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.5/setup.py` & `one-api-tool-0.4.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.4.5",
+    version="0.4.6",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

