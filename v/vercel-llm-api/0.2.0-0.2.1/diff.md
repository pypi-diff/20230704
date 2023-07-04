# Comparing `tmp/vercel_llm_api-0.2.0-py3-none-any.whl.zip` & `tmp/vercel_llm_api-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 18446 bytes, number of entries: 6
--rw-r--r--  2.0 unx     5781 b- defN 23-Jun-16 22:02 vercel_ai.py
--rw-r--r--  2.0 unx    35148 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7598 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      491 b- defN 23-Jun-16 22:10 vercel_llm_api-0.2.0.dist-info/RECORD
-6 files, 49120 bytes uncompressed, 17556 bytes compressed:  64.3%
+Zip file size: 18447 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     5777 b- defN 23-Jul-04 02:33 vercel_ai.py
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7598 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      491 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/RECORD
+6 files, 49116 bytes uncompressed, 17557 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vercel_ai.py
 Comment: 
 
-Filename: vercel_llm_api-0.2.0.dist-info/LICENSE
+Filename: vercel_llm_api-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: vercel_llm_api-0.2.0.dist-info/METADATA
+Filename: vercel_llm_api-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: vercel_llm_api-0.2.0.dist-info/WHEEL
+Filename: vercel_llm_api-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: vercel_llm_api-0.2.0.dist-info/top_level.txt
+Filename: vercel_llm_api-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vercel_llm_api-0.2.0.dist-info/RECORD
+Filename: vercel_llm_api-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vercel_ai.py

```diff
@@ -10,15 +10,15 @@
 import random
 from curl_cffi import requests
 
 logging.basicConfig()
 logger = logging.getLogger()
 
 class Client:
-  base_url = "https://play.vercel.ai"
+  base_url = "https://sdk.vercel.ai"
   token_url = base_url + "/openai.jpeg" #nice try vercel
   generate_url = base_url + "/api/prompt"
   chat_url = base_url + "/api/generate"
 
   def __init__(self):
     self.session = requests.Session(impersonate="chrome107")
     self.headers = {
@@ -140,17 +140,17 @@
   
   def get_headers(self):
     token = self.get_token()
 
     headers = {**self.headers, **{
       "Accept-Encoding": "gzip, deflate, br",
       "Custom-Encoding": token,
-      "Host": "play.vercel.ai",
-      "Origin": "https://play.vercel.ai",
-      "Referrer": "https://play.vercel.ai",
+      "Host": "sdk.vercel.ai",
+      "Origin": "https://sdk.vercel.ai",
+      "Referrer": "https://sdk.vercel.ai",
       "Sec-Fetch-Dest": "empty",
       "Sec-Fetch-Mode": "cors",
       "Sec-Fetch-Site": "same-origin",
     }}
 
     return headers
```

## Comparing `vercel_llm_api-0.2.0.dist-info/LICENSE` & `vercel_llm_api-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vercel_llm_api-0.2.0.dist-info/METADATA` & `vercel_llm_api-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vercel-llm-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: A reverse engineered API for the Vercel AI playground.
 Home-page: https://github.com/ading2210/vercel-llm-api
 Author: ading2210
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

