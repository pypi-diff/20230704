# Comparing `tmp/langchain_interpreter-0.0.2.tar.gz` & `tmp/langchain_interpreter-0.0.3.tar.gz`

## Comparing `langchain_interpreter-0.0.2.tar` & `langchain_interpreter-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/examples/chains_from_json.ipynb
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/examples/json_from_chains.ipynb
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/llmchain.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/seq_chain.json
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/seq_chain_memory.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/simple_seq_chain.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/langchain_interpreter/__init__.py
--rwxr-xr-x   0        0        0     2393 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/langchain_interpreter/main.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/LICENSE
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    12943 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/examples/chains_from_json.ipynb
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/examples/json_from_chains.ipynb
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/json/conv_buffer_memory.json
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/json/llmchain.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/json/seq_chain.json
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/json/seq_chain_memory.json
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/json/simple_seq_chain.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/langchain_interpreter/__init__.py
+-rwxr-xr-x   0        0        0     4092 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/src/langchain_interpreter/main.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/LICENSE
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.3/PKG-INFO
```

### Comparing `langchain_interpreter-0.0.2/src/examples/chains_from_json.ipynb` & `langchain_interpreter-0.0.3/src/examples/chains_from_json.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9430555555555555%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1}, insert: [(5, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 10), ('metadata', OrderedDict()), ('outputs', "*

 * *            '[OrderedDict([(\'data\', OrderedDict([(\'text/plain\', ["{\'input\': \'Tell me '*

 * *            'more!\',\\n", \' \\\'history\\\': "Human: hi\\\\nAI: whats up\\\\nHuman: ot much. '*

 * *            "what about you?\\\\nAI: \\'ve been learning about linear algebra recently. It\\'s "*

 * *            'really interesting!",\\n\', \' \\\'res […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from dotenv import load_dotenv\n",
                 "load_dotenv()\n",
                 "\n",
                 "import sys\n",
@@ -156,14 +156,106 @@
             ],
             "source": [
                 "from main import chain_from_file\n",
                 "\n",
                 "seq_chain = chain_from_file(\"json/seq_chain_memory.json\")\n",
                 "seq_chain({\"title\": \"Tragedy at sunset on the beach\", \"era\": \"Victorian England\"})"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'input': 'Tell me more!',\n",
+                            " 'history': \"Human: hi\\nAI: whats up\\nHuman: ot much. what about you?\\nAI: 've been learning about linear algebra recently. It's really interesting!\",\n",
+                            " 'response': \" Sure! Linear algebra is a branch of mathematics that deals with linear equations and vectors. It's used in a lot of different fields, like machine learning, engineering, and economics. It's also the foundation of a lot of higher-level mathematics courses.\"}"
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "\n",
+                "conv_chain = chain_from_file(\"../json/conv_buffer_memory.json\", history=\"Human: hi\\nAI: whats up\\nHuman: not much. what about you?\\nAI: I've been learning about linear algebra recently. It's really interesting!\")\n",
+                "conv_chain(\"Tell me more!\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from langchain.llms import OpenAI\n",
+                "from langchain.chains import ConversationChain\n",
+                "from langchain.memory import ConversationBufferMemory\n",
+                "\n",
+                "llm = OpenAI(temperature=0)\n",
+                "mem = ConversationBufferMemory()\n",
+                "mem.save_context({\"input\": \"hi\"}, {\"output\": \"whats up\"})\n",
+                "conversation = ConversationChain(\n",
+                "    llm = llm,\n",
+                "    verbose=True,\n",
+                "    memory=mem\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "\n",
+                        "\u001b[1m> Entering new  chain...\u001b[0m\n",
+                        "Prompt after formatting:\n",
+                        "\u001b[32;1m\u001b[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.\n",
+                        "\n",
+                        "Current conversation:\n",
+                        "Human: hi\n",
+                        "AI: whats up\n",
+                        "Human: not much. what about you?\n",
+                        "AI:\u001b[0m\n",
+                        "\n",
+                        "\u001b[1m> Finished chain.\u001b[0m\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "\" I'm doing great! I'm currently learning about the latest advancements in artificial intelligence. It's really fascinating to see how far we've come in such a short amount of time. What about you? What have you been up to lately?\""
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "conversation.predict(input=\"not much. what about you?\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from main import chain_from_file\n"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "langchain",
             "language": "python",
             "name": "python3"
```

### Comparing `langchain_interpreter-0.0.2/src/examples/json_from_chains.ipynb` & `langchain_interpreter-0.0.3/src/examples/json_from_chains.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'cells'": "{2: {'source': ['# mychain']}}"}*

```diff
@@ -47,15 +47,15 @@
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "mychain"
+                "# mychain"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "langchain",
             "language": "python",
```

### Comparing `langchain_interpreter-0.0.2/src/json/seq_chain.json` & `langchain_interpreter-0.0.3/src/json/seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.2/src/json/seq_chain_memory.json` & `langchain_interpreter-0.0.3/src/json/seq_chain_memory.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.2/src/json/simple_seq_chain.json` & `langchain_interpreter-0.0.3/src/json/simple_seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.2/.gitignore` & `langchain_interpreter-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.2/LICENSE` & `langchain_interpreter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.2/pyproject.toml` & `langchain_interpreter-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "langchain_interpreter"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Elijah Tarr", email="elijahotarr@gmail.com" },
 ]
 description = "A way to turn json into langchain pipelines."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `langchain_interpreter-0.0.2/PKG-INFO` & `langchain_interpreter-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_interpreter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A way to turn json into langchain pipelines.
 Project-URL: Homepage, https://github.com/eoriont/langchain_interpreter
 Project-URL: Bug Tracker, https://github.com/eoriont/langchain_interpreter/issues
 Author-email: Elijah Tarr <elijahotarr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

