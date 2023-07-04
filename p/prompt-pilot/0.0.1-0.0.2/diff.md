# Comparing `tmp/prompt_pilot-0.0.1.tar.gz` & `tmp/prompt_pilot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_pilot-0.0.1.tar", max compression
+gzip compressed data, was "prompt_pilot-0.0.2.tar", max compression
```

## Comparing `prompt_pilot-0.0.1.tar` & `prompt_pilot-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rwxr-xr-x   0        0        0      711 2023-07-04 00:31:51.304591 prompt_pilot-0.0.1/README.md
--rwxr-xr-x   0        0        0      178 2023-06-10 13:32:54.211564 prompt_pilot-0.0.1/prompt-pilot/__init__.py
--rwxr-xr-x   0        0        0       46 2023-06-10 13:30:06.476133 prompt_pilot-0.0.1/prompt-pilot/api/__init__.py
--rwxr-xr-x   0        0        0        0 2023-06-10 13:29:37.491549 prompt_pilot-0.0.1/prompt-pilot/api/openai.py
--rwxr-xr-x   0        0        0        0 2023-06-10 13:29:45.080510 prompt_pilot-0.0.1/prompt-pilot/api/replicate.py
--rwxr-xr-x   0        0        0       77 2023-06-23 03:48:57.037511 prompt_pilot-0.0.1/prompt-pilot/database/__init__.py
--rwxr-xr-x   0        0        0        0 2023-06-23 03:47:20.502300 prompt_pilot-0.0.1/prompt-pilot/database/pinecone.py
--rwxr-xr-x   0        0        0        0 2023-06-23 03:47:25.180198 prompt_pilot-0.0.1/prompt-pilot/database/vectorvault.py
--rwxr-xr-x   0        0        0        0 2023-06-23 03:49:43.426746 prompt_pilot-0.0.1/prompt-pilot/database/weaviate.py
--rwxr-xr-x   0        0        0       77 2023-06-22 08:39:57.594475 prompt_pilot-0.0.1/prompt-pilot/hello.py
--rwxr-xr-x   0        0        0       52 2023-06-30 06:20:29.554760 prompt_pilot-0.0.1/prompt-pilot/language/__init__.py
--rwxr-xr-x   0        0        0    17131 2023-07-04 00:33:36.504234 prompt_pilot-0.0.1/prompt-pilot/language/assistants.py
--rwxr-xr-x   0        0        0     4030 2023-07-03 23:22:47.647291 prompt_pilot-0.0.1/prompt-pilot/language/characters.py
--rwxr-xr-x   0        0        0      552 2023-07-03 22:33:27.616353 prompt_pilot-0.0.1/prompt-pilot/language/others.py
--rwxr-xr-x   0        0        0     3228 2023-07-03 22:03:48.206564 prompt_pilot-0.0.1/prompt-pilot/language/psychology.py
--rwxr-xr-x   0        0        0      103 2023-06-30 06:20:22.612831 prompt_pilot-0.0.1/prompt-pilot/language/techniques/__init__.py
--rwxr-xr-x   0        0        0     1904 2023-06-30 06:15:19.304174 prompt_pilot-0.0.1/prompt-pilot/language/techniques/few_shot.py
--rwxr-xr-x   0        0        0      724 2023-05-30 08:28:53.337680 prompt_pilot-0.0.1/prompt-pilot/language/techniques/nlp_tasks.py
--rwxr-xr-x   0        0        0     1192 2023-06-23 03:37:17.453328 prompt_pilot-0.0.1/prompt-pilot/language/techniques/promptingtypes.py
--rwxr-xr-x   0        0        0     1238 2023-06-23 03:49:06.026906 prompt_pilot-0.0.1/prompt-pilot/language/techniques/zero_shot.py
--rwxr-xr-x   0        0        0       80 2023-06-10 13:25:50.199950 prompt_pilot-0.0.1/prompt-pilot/vision/__init__.py
--rwxr-xr-x   0        0        0    13904 2023-06-10 13:25:42.393016 prompt_pilot-0.0.1/prompt-pilot/vision/image_generation.py
--rwxr-xr-x   0        0        0      336 2023-05-30 12:25:46.080948 prompt_pilot-0.0.1/prompt-pilot/vision/img2img.py
--rwxr-xr-x   0        0        0      355 2023-06-30 06:15:16.320627 prompt_pilot-0.0.1/prompt-pilot/vision/inpainting.py
--rwxr-xr-x   0        0        0      501 2023-06-30 06:15:56.934396 prompt_pilot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 prompt_pilot-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      711 2023-07-04 00:31:51.304591 prompt_pilot-0.0.2/README.md
+-rwxr-xr-x   0        0        0      178 2023-06-10 13:32:54.211564 prompt_pilot-0.0.2/prompt-pilot/__init__.py
+-rwxr-xr-x   0        0        0       46 2023-06-10 13:30:06.476133 prompt_pilot-0.0.2/prompt-pilot/api/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-10 13:29:37.491549 prompt_pilot-0.0.2/prompt-pilot/api/openai.py
+-rwxr-xr-x   0        0        0        0 2023-06-10 13:29:45.080510 prompt_pilot-0.0.2/prompt-pilot/api/replicate.py
+-rwxr-xr-x   0        0        0       77 2023-06-23 03:48:57.037511 prompt_pilot-0.0.2/prompt-pilot/database/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-23 03:47:20.502300 prompt_pilot-0.0.2/prompt-pilot/database/pinecone.py
+-rwxr-xr-x   0        0        0        0 2023-06-23 03:47:25.180198 prompt_pilot-0.0.2/prompt-pilot/database/vectorvault.py
+-rwxr-xr-x   0        0        0        0 2023-06-23 03:49:43.426746 prompt_pilot-0.0.2/prompt-pilot/database/weaviate.py
+-rwxr-xr-x   0        0        0       77 2023-06-22 08:39:57.594475 prompt_pilot-0.0.2/prompt-pilot/hello.py
+-rwxr-xr-x   0        0        0       52 2023-06-30 06:20:29.554760 prompt_pilot-0.0.2/prompt-pilot/language/__init__.py
+-rwxr-xr-x   0        0        0    17131 2023-07-04 05:57:12.624391 prompt_pilot-0.0.2/prompt-pilot/language/assistants.py
+-rwxr-xr-x   0        0        0     4030 2023-07-03 23:22:47.647291 prompt_pilot-0.0.2/prompt-pilot/language/characters.py
+-rwxr-xr-x   0        0        0      552 2023-07-03 22:33:27.616353 prompt_pilot-0.0.2/prompt-pilot/language/others.py
+-rwxr-xr-x   0        0        0     3228 2023-07-03 22:03:48.206564 prompt_pilot-0.0.2/prompt-pilot/language/psychology.py
+-rwxr-xr-x   0        0        0      103 2023-06-30 06:20:22.612831 prompt_pilot-0.0.2/prompt-pilot/language/techniques/__init__.py
+-rwxr-xr-x   0        0        0     1904 2023-06-30 06:15:19.304174 prompt_pilot-0.0.2/prompt-pilot/language/techniques/few_shot.py
+-rwxr-xr-x   0        0        0      724 2023-05-30 08:28:53.337680 prompt_pilot-0.0.2/prompt-pilot/language/techniques/nlp_tasks.py
+-rwxr-xr-x   0        0        0     1192 2023-06-23 03:37:17.453328 prompt_pilot-0.0.2/prompt-pilot/language/techniques/promptingtypes.py
+-rwxr-xr-x   0        0        0     1238 2023-06-23 03:49:06.026906 prompt_pilot-0.0.2/prompt-pilot/language/techniques/zero_shot.py
+-rwxr-xr-x   0        0        0       80 2023-06-10 13:25:50.199950 prompt_pilot-0.0.2/prompt-pilot/vision/__init__.py
+-rwxr-xr-x   0        0        0    13904 2023-06-10 13:25:42.393016 prompt_pilot-0.0.2/prompt-pilot/vision/image_generation.py
+-rwxr-xr-x   0        0        0      336 2023-05-30 12:25:46.080948 prompt_pilot-0.0.2/prompt-pilot/vision/img2img.py
+-rwxr-xr-x   0        0        0      355 2023-06-30 06:15:16.320627 prompt_pilot-0.0.2/prompt-pilot/vision/inpainting.py
+-rwxr-xr-x   0        0        0      500 2023-07-04 06:03:32.579833 prompt_pilot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 prompt_pilot-0.0.2/PKG-INFO
```

### Comparing `prompt_pilot-0.0.1/README.md` & `prompt_pilot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/assistants.py` & `prompt_pilot-0.0.2/prompt-pilot/language/assistants.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/characters.py` & `prompt_pilot-0.0.2/prompt-pilot/language/characters.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/others.py` & `prompt_pilot-0.0.2/prompt-pilot/language/others.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/psychology.py` & `prompt_pilot-0.0.2/prompt-pilot/language/psychology.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/techniques/few_shot.py` & `prompt_pilot-0.0.2/prompt-pilot/language/techniques/few_shot.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/techniques/nlp_tasks.py` & `prompt_pilot-0.0.2/prompt-pilot/language/techniques/nlp_tasks.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/techniques/promptingtypes.py` & `prompt_pilot-0.0.2/prompt-pilot/language/techniques/promptingtypes.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/language/techniques/zero_shot.py` & `prompt_pilot-0.0.2/prompt-pilot/language/techniques/zero_shot.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/prompt-pilot/vision/image_generation.py` & `prompt_pilot-0.0.2/prompt-pilot/vision/image_generation.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.0.1/PKG-INFO` & `prompt_pilot-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: prompt-pilot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for Prompt Engineering
 Home-page: https://github.com/Amar-89
 License: MIT
 Author: Amar
 Author-email: amar439412@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/Amar-89/prompt-pilot
 Description-Content-Type: text/markdown
 
 # Prompt Pilot
 
 *DISCLAIMER: It's currently in development and I am uploading this primarily as a placeholder with some functions that you guys can play around with.*
```

