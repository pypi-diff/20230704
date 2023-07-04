# Comparing `tmp/gpt_fn-0.0.6.tar.gz` & `tmp/gpt_fn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.6.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.7.tar", max compression
```

## Comparing `gpt_fn-0.0.6.tar` & `gpt_fn-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-06-16 03:39:37.942535 gpt_fn-0.0.6/LICENSE
--rw-r--r--   0        0        0     4119 2023-06-16 03:39:37.942535 gpt_fn-0.0.6/README.md
--rw-r--r--   0        0        0      810 2023-06-16 03:40:00.870205 gpt_fn-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0      767 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0     4135 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/completion.py
--rw-r--r--   0        0        0      537 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      342 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/exceptions.py
--rw-r--r--   0        0        0      878 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0     4623 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__snapshots__/test_completion.ambr
--rw-r--r--   0        0        0      330 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0    13049 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0    15305 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0    13478 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0    12997 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
--rw-r--r--   0        0        0     5955 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion.yaml
--rw-r--r--   0        0        0     3239 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
--rw-r--r--   0        0        0     3892 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
--rw-r--r--   0        0        0      872 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0     2927 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/test_completion.py
--rw-r--r--   0        0        0      522 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     3560 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0      960 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0    14006 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0      892 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     2647 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 gpt_fn-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4119 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/README.md
+-rw-r--r--   0        0        0      810 2023-07-04 06:43:22.850904 gpt_fn-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0     4278 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      342 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      878 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0     9184 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      330 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0    13049 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0    15305 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0    13478 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0    12997 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
+-rw-r--r--   0        0        0     5955 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion.yaml
+-rw-r--r--   0        0        0     3138 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_enough_tokens.yaml
+-rw-r--r--   0        0        0     3239 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
+-rw-r--r--   0        0        0     3892 2023-07-04 06:42:58.989965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
+-rw-r--r--   0        0        0     3311 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_structural_completion_without_enough_tokens.yaml
+-rw-r--r--   0        0        0      872 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0     4151 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0      522 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     3560 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0      960 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0    14006 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0      892 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     2647 2023-07-04 06:42:58.993965 gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 gpt_fn-0.0.7/PKG-INFO
```

### Comparing `gpt_fn-0.0.6/LICENSE` & `gpt_fn-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/README.md` & `gpt_fn-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/pyproject.toml` & `gpt_fn-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `gpt_fn-0.0.6/src/gpt_fn/ai_function.py` & `gpt_fn-0.0.7/src/gpt_fn/ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/completion.py` & `gpt_fn-0.0.7/src/gpt_fn/completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,20 +47,21 @@
     )
     if max_tokens is not None:
         kwargs.update(max_tokens=max_tokens)
 
     response = openai.ChatCompletion.create(**kwargs)
     output = response.choices[0]
     message = output["message"]
+    finish_reason = output.finish_reason
 
-    if "function_call" in message:
+    if "function_call" in message and finish_reason in ["stop", "function_call"]:
         return message["function_call"]
 
     raise CompletionIncompleteError(
-        f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {output.finish_reason} Message:{message.content}",
+        f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {finish_reason} Message:{message.content}",
         response=response,
         request=kwargs,
     )
 
 
 def structural_completion(
     structure: Type[T],
@@ -94,21 +95,22 @@
     if max_tokens is not None:
         kwargs.update(max_tokens=max_tokens)
 
     response = openai.ChatCompletion.create(**kwargs)
 
     output = response.choices[0]
     message = output.message
+    finish_reason = output.finish_reason
 
-    if "function_call" in message:
+    if "function_call" in message and finish_reason == "stop":
         args = message.function_call.arguments
         return pydantic.parse_raw_as(structure, args)
 
     raise CompletionIncompleteError(
-        f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {output.finish_reason} Message:{message.content}",
+        f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {finish_reason} Message:{message.content}",
         response=response,
         request=kwargs,
     )
 
 
 def chat_completion(
     messages: list[Message],
```

### Comparing `gpt_fn-0.0.6/src/gpt_fn/conftest.py` & `gpt_fn-0.0.7/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/prompt.py` & `gpt_fn-0.0.7/src/gpt_fn/prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_chat_completion.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_structural_completion.yaml` & `gpt_fn-0.0.7/src/gpt_fn/tests/cassettes/test_structural_completion.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.0.7/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/test_completion.py` & `gpt_fn-0.0.7/src/gpt_fn/tests/test_completion.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,29 @@
         ],
         functions=[book_a_flight],
     )
     assert snapshot == msg
 
 
 @pytest.mark.vcr(match_on=["method", "scheme", "host", "port", "path", "query", "body"])
+def test_function_completion_without_enough_tokens(snapshot: SnapshotAssertion) -> None:
+    with pytest.raises(CompletionIncompleteError) as excinfo:
+        msg = function_completion(
+            [
+                {"role": "system", "content": "You are a helpful assistant."},
+                {"role": "user", "content": "I want to book a restaurant in London."},
+            ],
+            max_tokens=10,
+            functions=[book_a_flight],
+        )
+    assert snapshot == excinfo.exconly()
+    assert snapshot == vars(excinfo.value)
+
+
+@pytest.mark.vcr(match_on=["method", "scheme", "host", "port", "path", "query", "body"])
 def test_function_completion_without_neccess_function(
     snapshot: SnapshotAssertion,
 ) -> None:
     with pytest.raises(CompletionIncompleteError) as excinfo:
         msg = function_completion(
             [
                 {"role": "system", "content": "You are a helpful assistant."},
@@ -34,32 +49,48 @@
             ],
             functions=[book_a_flight],
         )
     assert snapshot == excinfo.exconly()
     assert snapshot == vars(excinfo.value)
 
 
+class Email(pydantic.BaseModel):
+    subject: str = pydantic.Field(description="the subject of email")
+    body: str = pydantic.Field(description="the body of email")
+
+
 @pytest.mark.vcr(match_on=["method", "scheme", "host", "port", "path", "query", "body"])
 def test_structural_completion(snapshot: SnapshotAssertion) -> None:
-    class Email(pydantic.BaseModel):
-        subject: str = pydantic.Field(description="the subject of email")
-        body: str = pydantic.Field(description="the body of email")
-
     email = structural_completion(
         Email,
         [
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": "Give me a sample email."},
         ],
     )
 
     assert snapshot == email
 
 
 @pytest.mark.vcr(match_on=["method", "scheme", "host", "port", "path", "query", "body"])
+def test_structural_completion_without_enough_tokens(snapshot: SnapshotAssertion) -> None:
+    with pytest.raises(CompletionIncompleteError) as excinfo:
+        email = structural_completion(
+            Email,
+            [
+                {"role": "system", "content": "You are a helpful assistant."},
+                {"role": "user", "content": "Give me a sample email."},
+            ],
+            max_tokens=10,
+        )
+    assert snapshot == excinfo.exconly()
+    assert snapshot == vars(excinfo.value)
+
+
+@pytest.mark.vcr(match_on=["method", "scheme", "host", "port", "path", "query", "body"])
 def test_chat_completion(snapshot: SnapshotAssertion) -> None:
     msg = chat_completion(
         [
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": "Hello, who are you?"},
         ],
     )
```

### Comparing `gpt_fn-0.0.6/src/gpt_fn/tests/test_prompt.py` & `gpt_fn-0.0.7/src/gpt_fn/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.0.7/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/utils/signature.py` & `gpt_fn-0.0.7/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.0.7/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_signature.py` & `gpt_fn-0.0.7/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.6/PKG-INFO` & `gpt_fn-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

