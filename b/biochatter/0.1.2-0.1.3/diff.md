# Comparing `tmp/biochatter-0.1.2.tar.gz` & `tmp/biochatter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biochatter-0.1.2.tar", max compression
+gzip compressed data, was "biochatter-0.1.3.tar", max compression
```

## Comparing `biochatter-0.1.2.tar` & `biochatter-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.2/LICENSE
--rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.2/biochatter/__init__.py
--rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.2/biochatter/_stats.py
--rw-r--r--   0        0        0    12888 2023-06-28 13:06:39.433702 biochatter-0.1.2/biochatter/llm_connect.py
--rw-r--r--   0        0        0     5226 2023-06-16 12:53:15.891015 biochatter-0.1.2/biochatter/vectorstore.py
--rw-r--r--   0        0        0      667 2023-06-28 13:22:03.813541 biochatter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 biochatter-0.1.2/setup.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 biochatter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 11:08:28.958016 biochatter-0.1.3/LICENSE
+-rw-r--r--   0        0        0      453 2023-06-28 13:22:29.968048 biochatter-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 11:09:32.282374 biochatter-0.1.3/biochatter/__init__.py
+-rw-r--r--   0        0        0     2672 2023-06-16 16:39:33.107276 biochatter-0.1.3/biochatter/_stats.py
+-rw-r--r--   0        0        0    17960 2023-07-03 22:09:12.868928 biochatter-0.1.3/biochatter/llm_connect.py
+-rw-r--r--   0        0        0     5226 2023-06-16 12:53:15.891015 biochatter-0.1.3/biochatter/vectorstore.py
+-rw-r--r--   0        0        0      667 2023-07-03 15:05:25.410204 biochatter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 biochatter-0.1.3/setup.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 biochatter-0.1.3/PKG-INFO
```

### Comparing `biochatter-0.1.2/LICENSE` & `biochatter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.2/biochatter/_stats.py` & `biochatter-0.1.3/biochatter/_stats.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.2/biochatter/llm_connect.py` & `biochatter-0.1.3/biochatter/llm_connect.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 try:
     import streamlit as st
 except ImportError:
     st = None
 
 from abc import ABC, abstractmethod
+from typing import Optional
 import openai
 
-from langchain.chat_models import ChatOpenAI
+from langchain.chat_models import ChatOpenAI, AzureChatOpenAI
 from langchain.schema import AIMessage, HumanMessage, SystemMessage
 from langchain.llms import HuggingFaceHub
 
 import nltk
 import json
 
 from .vectorstore import DocumentEmbedder
@@ -204,14 +205,25 @@
         pass
 
     @abstractmethod
     def _correct_response(self, msg: str):
         pass
 
     def _inject_context(self, text: str):
+        """
+        Inject the context into the prompt from vector database similarity
+        search. Finds the most similar n text fragments and adds them to the
+        message history object for usage in the next prompt. Uses the document
+        summarisation prompt set to inject the context. The ultimate prompt
+        should include the placeholder for the statements, `{statements}` (used
+        for formatting the string).
+
+        Args:
+            text (str): The user query to be used for similarity search.
+        """
         if not self.docsum.used:
             st.info(
                 "No document has been analysed yet. To use document "
                 "summarisation, please analyse at least one document first."
             )
             return
 
@@ -238,26 +250,30 @@
                 )
             ]
 
         prompts = self.prompts["docsum_prompts"]
         if statements:
             self.current_statements = statements
             for i, prompt in enumerate(prompts):
+                # if last prompt, format the statements into the prompt
                 if i == len(prompts) - 1:
                     self.append_system_message(
                         prompt.format(statements=statements)
                     )
                 else:
                     self.append_system_message(prompt)
 
     def get_msg_json(self):
         """
         Return a JSON representation (of a list of dicts) of the messages in
         the conversation. The keys of the dicts are the roles, the values are
         the messages.
+
+        Returns:
+            str: A JSON representation of the messages in the conversation.
         """
         d = []
         for msg in self.messages:
             if isinstance(msg, SystemMessage):
                 role = "system"
             elif isinstance(msg, HumanMessage):
                 role = "user"
@@ -279,14 +295,26 @@
         split_correction: bool,
         docsum: DocumentEmbedder = None,
     ):
         """
         Connect to OpenAI's GPT API and set up a conversation with the user.
         Also initialise a second conversational agent to provide corrections to
         the model output, if necessary.
+
+        Args:
+            model_name (str): The name of the model to use.
+
+            prompts (dict): A dictionary of prompts to use for the conversation.
+
+            split_correction (bool): Whether to correct the model output by
+                splitting the output into sentences and correcting each
+                sentence individually.
+
+            docsum (DocumentEmbedder): A document summariser to use for
+                document summarisation.
         """
         super().__init__(
             model_name=model_name,
             prompts=prompts,
             split_correction=split_correction,
             docsum=docsum,
         )
@@ -294,14 +322,22 @@
         self.ca_model_name = "gpt-3.5-turbo"
         # TODO make accessible by drop-down
 
     def set_api_key(self, api_key: str, user: str):
         """
         Set the API key for the OpenAI API. If the key is valid, initialise the
         conversational agent. Set the user for usage statistics.
+
+        Args:
+            api_key (str): The API key for the OpenAI API.
+
+            user (str): The user for usage statistics.
+
+        Returns:
+            bool: True if the API key is valid, False otherwise.
         """
         openai.api_key = api_key
         self.user = user
 
         try:
             openai.Model.list()
             self.chat = ChatOpenAI(
@@ -319,14 +355,23 @@
 
             return True
 
         except openai.error.AuthenticationError as e:
             return False
 
     def _primary_query(self):
+        """
+        Query the OpenAI API with the user's message and return the response
+        using the message history (flattery system messages, prior conversation)
+        as context. Correct the response if necessary.
+
+        Returns:
+            tuple: A tuple containing the response from the OpenAI API and the
+                token usage.
+        """
         try:
             response = self.chat.generate([self.messages])
         except (
             openai.error.InvalidRequestError,
             openai.error.APIConnectionError,
             openai.error.RateLimitError,
             openai.error.APIError,
@@ -339,14 +384,25 @@
         self._update_usage_stats(self.model_name, token_usage)
 
         self.append_ai_message(msg)
 
         return msg, token_usage
 
     def _correct_response(self, msg: str):
+        """
+        Correct the response from the OpenAI API by sending it to a secondary
+        language model. Optionally split the response into single sentences and
+        correct each sentence individually. Update usage stats.
+
+        Args:
+            msg (str): The response from the OpenAI API.
+
+        Returns:
+            str: The corrected response (or OK if no correction necessary).
+        """
         ca_messages = self.ca_messages.copy()
         ca_messages.append(
             HumanMessage(
                 content=msg,
             ),
         )
         ca_messages.append(
@@ -365,22 +421,112 @@
 
         return correction
 
     def _update_usage_stats(self, model: str, token_usage: dict):
         """
         Update redis database with token usage statistics using the usage_stats
         object with the increment method.
+
+        Args:
+            model (str): The model name.
+
+            token_usage (dict): The token usage statistics.
         """
         if self.user == "community":
             self.usage_stats.increment(
                 f"usage:[date]:[user]",
                 {f"{k}:{model}": v for k, v in token_usage.items()},
             )
 
 
+class AzureGptConversation(GptConversation):
+    def __init__(
+        self,
+        deployment_name: str,
+        model_name: str,
+        prompts: dict,
+        split_correction: bool,
+        docsum: DocumentEmbedder = None,
+        version: Optional[str] = None,
+        base: Optional[str] = None,
+    ):
+        """
+        Connect to Azure's GPT API and set up a conversation with the user.
+        Extends GptConversation.
+
+        Args:
+            deployment_name (str): The name of the Azure deployment to use.
+
+            model_name (str): The name of the model to use. This is distinct
+                from the deployment name.
+
+            prompts (dict): A dictionary of prompts to use for the conversation.
+
+            split_correction (bool): Whether to correct the model output by
+                splitting the output into sentences and correcting each
+                sentence individually.
+
+            docsum (DocumentEmbedder): A vector database connection to use for
+                document summarisation.
+
+            version (str): The version of the Azure API to use.
+
+            base (str): The base URL of the Azure API to use.
+        """
+        super().__init__(
+            model_name=model_name,
+            prompts=prompts,
+            split_correction=split_correction,
+            docsum=docsum,
+        )
+
+        self.version = version
+        self.base = base
+        self.deployment_name = deployment_name
+
+    def set_api_key(self, api_key: str):
+        """
+        Set the API key for the Azure API. If the key is valid, initialise the
+        conversational agent. No user stats on Azure.
+
+        Args:
+            api_key (str): The API key for the Azure API.
+
+        Returns:
+            bool: True if the API key is valid, False otherwise.
+        """
+
+        try:
+            self.chat = AzureChatOpenAI(
+                deployment_name=self.deployment_name,
+                model_name=self.model_name,
+                openai_api_version=self.version,
+                openai_api_base=self.base,
+                openai_api_key=api_key,
+                temperature=0,
+            )
+            # TODO this is the same model as the primary one; refactor to be
+            # able to use any model for correction
+            self.ca_chat = AzureChatOpenAI(
+                deployment_name=self.deployment_name,
+                model_name=self.model_name,
+                openai_api_version=self.version,
+                openai_api_base=self.base,
+                openai_api_key=api_key,
+                temperature=0,
+            )
+
+            test = self.chat.generate([[HumanMessage(content="Hello")]])
+
+            return True
+
+        except openai.error.AuthenticationError as e:
+            return False
+
+
 class BloomConversation(Conversation):
     def __init__(
         self,
         model_name: str,
         prompts: dict,
         split_correction: bool,
         docsum: DocumentEmbedder = None,
```

### Comparing `biochatter-0.1.2/biochatter/vectorstore.py` & `biochatter-0.1.3/biochatter/vectorstore.py`

 * *Files identical despite different names*

### Comparing `biochatter-0.1.2/pyproject.toml` & `biochatter-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biochatter"
-version = "0.1.2"
+version = "0.1.3"
 description = "Backend library for conversational AI in biomedicine"
 authors = ["Sebastian Lobentanzer <sebastian.lobentanzer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `biochatter-0.1.2/setup.py` & `biochatter-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tiktoken>=0.4.0,<0.5.0']
 
 extras_require = \
 {'streamlit': ['streamlit>=1.23.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'biochatter',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Backend library for conversational AI in biomedicine',
     'long_description': '# biochatter\nThis repository contains the `biochatter` Python package, a generic backend library for the connection of biomedical applications to conversational AI. Used in [ChatGSE](https://chat.biocypher.org), which is being developed at https://github.com/biocypher/ChatGSE. More to come, so stay tuned!\n\n## Installation\nTo use the package, install it from PyPI, for instance using pip (`pip install biochatter`) or Poetry (`poetry add biochatter`).\n',
     'author': 'Sebastian Lobentanzer',
     'author_email': 'sebastian.lobentanzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `biochatter-0.1.2/PKG-INFO` & `biochatter-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biochatter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Backend library for conversational AI in biomedicine
 License: MIT
 Author: Sebastian Lobentanzer
 Author-email: sebastian.lobentanzer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

