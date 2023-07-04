# Comparing `tmp/autopack_tools-0.2.2.tar.gz` & `tmp/autopack_tools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.2.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.3.tar", max compression
```

## Comparing `autopack_tools-0.2.2.tar` & `autopack_tools-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.2/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.2/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.2/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.2/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.2/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.2/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.2/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.2/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.2/autopack/get_pack.py
--rw-r--r--   0        0        0     3877 2023-07-04 00:57:01.539973 autopack_tools-0.2.2/autopack/installation.py
--rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.2/autopack/pack.py
--rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.2/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.2/autopack/search.py
--rw-r--r--   0        0        0     2608 2023-07-04 00:57:01.095471 autopack_tools-0.2.2/autopack/selection.py
--rw-r--r--   0        0        0     4405 2023-07-04 00:57:01.553490 autopack_tools-0.2.2/autopack/utils.py
--rw-r--r--   0        0        0      910 2023-07-04 00:56:03.603405 autopack_tools-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.3/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.3/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.3/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.3/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.3/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.3/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.3/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.3/autopack/get_pack.py
+-rw-r--r--   0        0        0     3877 2023-07-04 01:58:56.151275 autopack_tools-0.2.3/autopack/installation.py
+-rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.3/autopack/pack.py
+-rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.3/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.3/autopack/search.py
+-rw-r--r--   0        0        0     2094 2023-07-04 01:58:55.758062 autopack_tools-0.2.3/autopack/selection.py
+-rw-r--r--   0        0        0     4405 2023-07-04 01:58:56.161504 autopack_tools-0.2.3/autopack/utils.py
+-rw-r--r--   0        0        0      910 2023-07-04 01:59:16.152339 autopack_tools-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.3/PKG-INFO
```

### Comparing `autopack_tools-0.2.2/LICENSE` & `autopack_tools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/README.md` & `autopack_tools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/api.py` & `autopack_tools-0.2.3/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/cli.py` & `autopack_tools-0.2.3/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/get_pack.py` & `autopack_tools-0.2.3/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/installation.py` & `autopack_tools-0.2.3/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/pack.py` & `autopack_tools-0.2.3/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/pack_response.py` & `autopack_tools-0.2.3/autopack/pack_response.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/autopack/selection.py` & `autopack_tools-0.2.3/autopack/selection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
-from json import JSONDecodeError
 
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import HumanMessage
 
 from autopack.api import pack_search
 
 TOOL_SELECTION_PROMPT = """
-I have a list of tools to choose from and a task I need to accomplish. Give me, as a valid JSON array, a list of the
-Tool IDs that are necessary to complete this task. Return only the JSON array and no other content.
+You are an autonomous AI Agent. I have a list of tools to choose from and a task I need you to accomplish. Recommend
+tools that would be required for you to complete the task. Return only a comma-separated list of tool_ids and no
+other content.
 
 ---- TASK ----
 {user_input}
 ---- TOOLS ----
 {tools_string}
 """
 
@@ -31,50 +31,35 @@
         llm (BaseChatModel): An LLM which will be used to evaluate the selection
 
     Returns:
         list[str]: A list of selected Pack IDs
     """
 
     packs = pack_search("")
-    packs_by_pseudo_id = {}
     pack_summaries = []
     for pack in packs:
-        # The AI can get messed up with the author/repo/name Pack IDs here, so give a hashed pack ID
-        pseudo_id = pack.pack_id.__hash__()
-        packs_by_pseudo_id[pseudo_id] = pack.pack_id
-
         pack_summaries.append(
             {
-                "tool_id": pseudo_id,
+                "tool_id": pack.pack_id,
                 "name": pack.name,
                 "description": pack.description,
                 "arguments": pack.run_args,
             }
         )
 
     tools_string = json.dumps(pack_summaries)
     prompt = TOOL_SELECTION_PROMPT.format(
         user_input=task_description, tools_string=tools_string
     )
 
-    pseudo_ids = ask_llm(prompt, llm)
-
-    selected_packs = []
-    for pseudo_id in pseudo_ids:
-        # Get the proper pack_id from the pseudo_id
-        proper_id = packs_by_pseudo_id[pseudo_id]
-        selected_packs.append(proper_id)
+    selected_packs = ask_llm(prompt, llm)
 
     return selected_packs
 
 
-def ask_llm(prompt: str, llm: BaseChatModel):
+def ask_llm(prompt: str, llm: BaseChatModel) -> list[str]:
     """Encapsulate the OpenAI specific stuff to easier support other frameworks in the future"""
     message = HumanMessage(content=prompt)
 
     response = llm(messages=[message])
 
-    try:
-        return json.loads(response.content)
-    except JSONDecodeError as e:
-        # TODO: Better handle error
-        return []
+    return response.content.split(",")
```

### Comparing `autopack_tools-0.2.2/autopack/utils.py` & `autopack_tools-0.2.3/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.2/pyproject.toml` & `autopack_tools-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.2.2"
+version = "0.2.3"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.2.2/PKG-INFO` & `autopack_tools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

