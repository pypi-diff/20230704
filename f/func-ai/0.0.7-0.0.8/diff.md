# Comparing `tmp/func_ai-0.0.7.tar.gz` & `tmp/func_ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.7.tar", max compression
+gzip compressed data, was "func_ai-0.0.8.tar", max compression
```

## Comparing `func_ai-0.0.7.tar` & `func_ai-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.7/LICENSE
--rw-r--r--   0        0        0     4323 2023-07-03 07:47:52.395570 func_ai-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.7/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.7/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.7/func_ai/utils/__init__.py
--rw-r--r--   0        0        0     4852 2023-07-03 07:47:52.396052 func_ai-0.0.7/func_ai/utils/jinja_template_functions.py
--rw-r--r--   0        0        0    15155 2023-07-03 07:47:52.396377 func_ai-0.0.7/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0    11068 2023-07-03 07:47:52.396708 func_ai-0.0.7/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3444 2023-07-03 07:47:52.397246 func_ai-0.0.7/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-06-30 06:36:30.641834 func_ai-0.0.7/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      907 2023-07-03 07:47:52.399129 func_ai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 func_ai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-04 07:21:24.340481 func_ai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4791 2023-07-04 07:21:24.340481 func_ai-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/__init__.py
+-rw-r--r--   0        0        0     4082 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0     4852 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/jinja_template_functions.py
+-rw-r--r--   0        0        0    15515 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0    11280 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3444 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      907 2023-07-04 07:21:24.344481 func_ai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5863 1970-01-01 00:00:00.000000 func_ai-0.0.8/PKG-INFO
```

### Comparing `func_ai-0.0.7/LICENSE` & `func_ai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.7/README.md` & `func_ai-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -98,12 +98,30 @@
 # prints
 """
 Name: John 
 Age: 20
 """
 ```
 
+### Jinja2 Templating
+
+```python
+from dotenv import load_dotenv
+from func_ai.utils.jinja_template_functions import JinjaOpenAITemplateFunction
+from func_ai.utils.llm_tools import OpenAIInterface
+load_dotenv()
+ji = JinjaOpenAITemplateFunction.from_string_template("Name: {{ NAME }} \n Age: {{ AGE }}", OpenAIInterface())
+resp = ji.render_from_prompt("John is 20 years old")
+assert "Name: John" in resp
+assert "Age: 20" in resp
+# prints
+"""
+Name: John 
+Age: 20
+"""
+```
+
 ## Inspiration
 
 - https://github.com/jxnl/openai_function_call
 - https://github.com/rizerphe/openai-functions
 - https://github.com/aurelio-labs/funkagent
```

### Comparing `func_ai-0.0.7/func_ai/function_indexer.py` & `func_ai-0.0.8/func_ai/function_indexer.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.7/func_ai/utils/jinja_template_functions.py` & `func_ai-0.0.8/func_ai/utils/jinja_template_functions.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.7/func_ai/utils/llm_tools.py` & `func_ai-0.0.8/func_ai/utils/llm_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,15 @@
                 "total_tokens": 0
             }
         self.usage[model]["prompt_tokens"] += api_response['usage']['prompt_tokens']
         self.usage[model]["completion_tokens"] += api_response['usage']['completion_tokens']
         self.usage[model]["total_tokens"] += api_response['usage']['total_tokens']
 
 
+
 class OpenAISchema(BaseModel):
     @classmethod
     @property
     def openai_schema(cls):
         schema = cls.schema()
 
         return {
@@ -380,17 +381,30 @@
             "description": self.description,
             "parameters": self.parameters,
         }
 
     def __str__(self) -> str:
         return f"{self.schema}"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.schema}"
 
+    def to_dict(self) -> dict[str, any]:
+        """
+        Returns a dict representation of the function
+
+        :return: dict containing the function
+        """
+        return {
+            "name": self.name,
+            "description": self.description,
+            "parameters": self.parameters,
+            "metadata": self.metadata,
+        }
+
     @property
     def last_call(self) -> dict[str, any]:
         """
         Returns the last response from the function call
 
         :return: dict containing the last response
         """
```

### Comparing `func_ai-0.0.7/func_ai/utils/openapi_function_parser.py` & `func_ai-0.0.8/func_ai/utils/openapi_function_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,22 @@
         """
         Return the dictionary of functions that can be called
 
         :return:
         """
         return self._funcs
 
+    def to_dict(self) -> dict[str, any]:
+        """
+        Return the dictionary of functions that can be called
+
+        :return:
+        """
+        return {fn: f.to_dict() for fn, f in self._funcs.items()}
+
     def get_operation(self, name: str) -> OpenAIFunctionWrapper:
         """
         Get a function by name
 
         :param name: The name of the function
         :return:
         """
```

### Comparing `func_ai-0.0.7/func_ai/utils/py_function_parser.py` & `func_ai-0.0.8/func_ai/utils/py_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.7/func_ai/workflow_creator.py` & `func_ai-0.0.8/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.7/pyproject.toml` & `func_ai-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.7"
+version = "0.0.8"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
```

### Comparing `func_ai-0.0.7/PKG-INFO` & `func_ai-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-ai
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI Functional Catalog - OpenAI functions on steriods
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -113,14 +113,32 @@
 
 ### Jinja2 Templating
 
 ```python
 from dotenv import load_dotenv
 from func_ai.utils.jinja_template_functions import JinjaOpenAITemplateFunction
 from func_ai.utils.llm_tools import OpenAIInterface
+load_dotenv()
+ji = JinjaOpenAITemplateFunction.from_string_template("Name: {{ NAME }} \n Age: {{ AGE }}", OpenAIInterface())
+resp = ji.render_from_prompt("John is 20 years old")
+assert "Name: John" in resp
+assert "Age: 20" in resp
+# prints
+"""
+Name: John 
+Age: 20
+"""
+```
+
+### Jinja2 Templating
+
+```python
+from dotenv import load_dotenv
+from func_ai.utils.jinja_template_functions import JinjaOpenAITemplateFunction
+from func_ai.utils.llm_tools import OpenAIInterface
 load_dotenv()
 ji = JinjaOpenAITemplateFunction.from_string_template("Name: {{ NAME }} \n Age: {{ AGE }}", OpenAIInterface())
 resp = ji.render_from_prompt("John is 20 years old")
 assert "Name: John" in resp
 assert "Age: 20" in resp
 # prints
 """
```

