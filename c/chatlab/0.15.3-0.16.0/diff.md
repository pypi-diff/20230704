# Comparing `tmp/chatlab-0.15.3.tar.gz` & `tmp/chatlab-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-0.15.3.tar", max compression
+gzip compressed data, was "chatlab-0.16.0.tar", max compression
```

## Comparing `chatlab-0.15.3.tar` & `chatlab-0.16.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1504 2023-06-29 00:35:59.757480 chatlab-0.15.3/LICENSE
--rw-r--r--   0        0        0     7121 2023-06-29 00:35:59.757480 chatlab-0.15.3/README.md
--rw-r--r--   0        0        0     1863 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/__init__.py
--rw-r--r--   0        0        0       23 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/_version.py
--rw-r--r--   0        0        0      588 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/builtins.py
--rw-r--r--   0        0        0     9684 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/conversation.py
--rw-r--r--   0        0        0     2382 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/decorators.py
--rw-r--r--   0        0        0     7995 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/models.py
--rw-r--r--   0        0        0     7343 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/registry.py
--rw-r--r--   0        0        0     5783 2023-06-29 00:35:59.761481 chatlab-0.15.3/chatlab/shells/python.py
--rw-r--r--   0        0        0     2646 2023-06-29 00:35:59.765481 chatlab-0.15.3/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-29 00:35:59.765481 chatlab-0.15.3/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-06-29 00:35:59.765481 chatlab-0.15.3/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-06-29 00:35:59.765481 chatlab-0.15.3/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-06-29 00:35:59.765481 chatlab-0.15.3/tests/test_messaging.py
--rw-r--r--   0        0        0     5977 2023-06-29 00:35:59.765481 chatlab-0.15.3/tests/test_registry.py
--rw-r--r--   0        0        0     8657 1970-01-01 00:00:00.000000 chatlab-0.15.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-04 16:06:04.085049 chatlab-0.16.0/LICENSE
+-rw-r--r--   0        0        0     7121 2023-07-04 16:06:04.085049 chatlab-0.16.0/README.md
+-rw-r--r--   0        0        0     1863 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/_version.py
+-rw-r--r--   0        0        0      588 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/builtins.py
+-rw-r--r--   0        0        0     9684 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/conversation.py
+-rw-r--r--   0        0        0     2382 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/decorators.py
+-rw-r--r--   0        0        0     7995 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/models.py
+-rw-r--r--   0        0        0     7343 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/registry.py
+-rw-r--r--   0        0        0     6633 2023-07-04 16:06:04.085049 chatlab-0.16.0/chatlab/shells/python.py
+-rw-r--r--   0        0        0     2646 2023-07-04 16:06:04.089049 chatlab-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-04 16:06:04.089049 chatlab-0.16.0/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-07-04 16:06:04.089049 chatlab-0.16.0/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-07-04 16:06:04.089049 chatlab-0.16.0/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-07-04 16:06:04.089049 chatlab-0.16.0/tests/test_messaging.py
+-rw-r--r--   0        0        0     5977 2023-07-04 16:06:04.089049 chatlab-0.16.0/tests/test_registry.py
+-rw-r--r--   0        0        0     8657 1970-01-01 00:00:00.000000 chatlab-0.16.0/PKG-INFO
```

### Comparing `chatlab-0.15.3/LICENSE` & `chatlab-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/README.md` & `chatlab-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/__init__.py` & `chatlab-0.16.0/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/builtins.py` & `chatlab-0.16.0/chatlab/builtins.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/conversation.py` & `chatlab-0.16.0/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/decorators.py` & `chatlab-0.16.0/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/display.py` & `chatlab-0.16.0/chatlab/display.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/markdown.py` & `chatlab-0.16.0/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/messaging.py` & `chatlab-0.16.0/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/models.py` & `chatlab-0.16.0/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/registry.py` & `chatlab-0.16.0/chatlab/registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/chatlab/shells/python.py` & `chatlab-0.16.0/chatlab/shells/python.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Builtins for ChatLab."""
 import json
+from traceback import TracebackException
 from typing import Optional
 
 from IPython.core.formatters import DisplayFormatter
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.display import display
 from IPython.utils.capture import RichOutput, capture_output
 from repr_llm import register_llm_formatter
@@ -132,18 +133,34 @@
 
     def run_cell(self, code: str):
         """Execute code in python and return the result."""
         try:
             with capture_output() as captured:
                 result = self.shell.run_cell(code)
         except Exception as e:
-            return e
+            formatted = TracebackException.from_exception(e, limit=3).format(chain=True)
+            plaintext_traceback = '\n'.join(formatted)
+
+            return plaintext_traceback
 
         if not result.success:
-            return result
+            # Grab which exception was raised
+            exception = result.error_before_exec or result.error_in_exec
+
+            # If success was False and yet neither of these are set, then
+            # something went wrong in the IPython internals
+            if exception is None:
+                raise Exception("Unknown IPython error for result", result)
+
+            # Create a formatted traceback that includes the last 3 frames
+            # and the exception message
+            formatted = TracebackException.from_exception(exception, limit=3).format(chain=True)
+            plaintext_traceback = '\n'.join(formatted)
+
+            return plaintext_traceback
 
         outputs = ""
 
         if captured.stdout is not None and captured.stdout.strip() != '':
             stdout = captured.stdout
             # Truncate stdout if it's too long
             if len(stdout) > 1000:
```

### Comparing `chatlab-0.15.3/pyproject.toml` & `chatlab-0.16.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "0.15.3"
+version = "0.16.0"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `chatlab-0.15.3/tests/test_decorators.py` & `chatlab-0.16.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/tests/test_messaging.py` & `chatlab-0.16.0/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/tests/test_registry.py` & `chatlab-0.16.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.15.3/PKG-INFO` & `chatlab-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 0.15.3
+Version: 0.16.0
 Summary: Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 3 - Alpha
```

