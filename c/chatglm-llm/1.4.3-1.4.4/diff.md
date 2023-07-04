# Comparing `tmp/chatglm-llm-1.4.3.tar.gz` & `tmp/chatglm-llm-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.4.3.tar", last modified: Wed Jun 28 09:08:57 2023, max compression
+gzip compressed data, was "chatglm-llm-1.4.4.tar", last modified: Tue Jul  4 07:13:05 2023, max compression
```

## Comparing `chatglm-llm-1.4.3.tar` & `chatglm-llm-1.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:08:57.807364 chatglm-llm-1.4.3/
--rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.3/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-28 09:08:57.807227 chatglm-llm-1.4.3/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.3/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:08:57.805982 chatglm-llm-1.4.3/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-28 09:08:57.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      540 2023-06-28 09:08:57.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-28 09:08:57.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-06-28 09:08:57.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      266 2023-06-28 09:08:57.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-06-28 09:08:57.000000 chatglm-llm-1.4.3/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:08:57.806709 chatglm-llm-1.4.3/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.3/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.3/chatglm_src/callbacks.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:08:57.806949 chatglm-llm-1.4.3/chatglm_src/chains/
--rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.3/chatglm_src/chains/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.3/chatglm_src/chains/local_qa.py
--rw-r--r--   0 mroy       (501) staff       (20)     2272 2023-06-28 08:26:21.000000 chatglm-llm-1.4.3/chatglm_src/chatglm_utils.py
--rw-r--r--   0 mroy       (501) staff       (20)     2777 2023-06-16 06:08:22.000000 chatglm-llm-1.4.3/chatglm_src/cluster_and_smi.py
--rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.3/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-06-15 08:48:00.000000 chatglm-llm-1.4.3/chatglm_src/embeding.py
--rw-r--r--   0 mroy       (501) staff       (20)    40968 2023-06-28 09:06:45.000000 chatglm-llm-1.4.3/chatglm_src/llm.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-28 09:08:57.807054 chatglm-llm-1.4.3/chatglm_src/loader/
--rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.3/chatglm_src/loader/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-28 09:08:57.807418 chatglm-llm-1.4.3/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1078 2023-06-28 08:53:27.000000 chatglm-llm-1.4.3/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.594086 chatglm-llm-1.4.4/
+-rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.4/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-04 07:13:05.593963 chatglm-llm-1.4.4/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.4/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.592478 chatglm-llm-1.4.4/chatglm_llm.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      540 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       53 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)      266 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       12 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.593361 chatglm-llm-1.4.4/chatglm_src/
+-rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.4/chatglm_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.4/chatglm_src/callbacks.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.593650 chatglm-llm-1.4.4/chatglm_src/chains/
+-rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.4/chatglm_src/chains/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.4/chatglm_src/chains/local_qa.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2272 2023-06-28 08:26:21.000000 chatglm-llm-1.4.4/chatglm_src/chatglm_utils.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2785 2023-07-04 07:10:48.000000 chatglm-llm-1.4.4/chatglm_src/cluster_and_smi.py
+-rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.4/chatglm_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3235 2023-07-04 07:11:23.000000 chatglm-llm-1.4.4/chatglm_src/embeding.py
+-rw-r--r--   0 mroy       (501) staff       (20)    41882 2023-07-04 07:12:19.000000 chatglm-llm-1.4.4/chatglm_src/llm.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.593795 chatglm-llm-1.4.4/chatglm_src/loader/
+-rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.4/chatglm_src/loader/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-07-04 07:13:05.594127 chatglm-llm-1.4.4/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1078 2023-07-04 07:12:38.000000 chatglm-llm-1.4.4/setup.py
```

### Comparing `chatglm-llm-1.4.3/README.md` & `chatglm-llm-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_llm.egg-info/SOURCES.txt` & `chatglm-llm-1.4.4/chatglm_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_src/__init__.py` & `chatglm-llm-1.4.4/chatglm_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_src/callbacks.py` & `chatglm-llm-1.4.4/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.4.4/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_src/chatglm_utils.py` & `chatglm-llm-1.4.4/chatglm_src/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_src/cluster_and_smi.py` & `chatglm-llm-1.4.4/chatglm_src/cluster_and_smi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import datetime
 import time
 from hashlib import md5
 import json
 from termcolor import colored
 import tqdm
 
-TODAY = datetime.datetime.now()
-PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
 
 def cluster(data, n_clusters=2,eps=0.5,min_samples=3, method='kmeans'):
     
     if method == 'kmeans':
         kmeans = KMeans(n_clusters=n_clusters, random_state=0, n_init='auto').fit(data)
         return kmeans.labels_
     elif method == 'dbscan':
@@ -41,14 +39,16 @@
         @eps : float, default=0.3, used in dbscan
         @min_samples : int, default=3, used in dbscan
         @n_clusters : int, default=2, used in kmeans
     
     """
     ws = create_connection(f"ws://{remote_host}:15000")
     user_id = md5(time.asctime().encode()).hexdigest()
+    TODAY = datetime.datetime.now()
+    PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
     ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}))
     # time.sleep(0.5)
     res = ws.recv()
     if res != "ok":
         print(colored("[info]:","yellow") ,res)
         raise Exception("password error")
```

### Comparing `chatglm-llm-1.4.3/chatglm_src/cmd.py` & `chatglm-llm-1.4.4/chatglm_src/cmd.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/chatglm_src/embeding.py` & `chatglm-llm-1.4.4/chatglm_src/embeding.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import time
 import json
 import tqdm
 import datetime
 from typing import List, Dict, Any, Optional, Union
 from termcolor import colored
 
-TODAY = datetime.datetime.now()
-PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
 
 class ChatGLMEmbeding(Embeddings):
 
     remote_host :str = None
 
     def __init__(self, model_path: str=None, remote_host:str=None):
         if remote_host is None:
@@ -42,14 +40,16 @@
             return msg
         except Exception as e:
             raise e
 
     def embed_documents_remote(self, texts):
         ws = create_connection(f"ws://{self.remote_host}:15000")
         user_id = md5(time.asctime().encode()).hexdigest()
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}))
         # time.sleep(0.5)
         res = ws.recv()
         if res != "ok":
             print(colored("[info]:","yellow") ,res)
             raise Exception("password error")
         
@@ -60,14 +60,16 @@
         except Exception as e:
             print(e)
             import ipdb;ipdb.set_trace()
     
     def embed_query_remote(self, text):
         ws = create_connection(f"ws://{self.remote_host}:15000")
         user_id = md5(time.asctime().encode()).hexdigest()
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}))
         # time.sleep(0.5)
         res = ws.recv()
         if res != "ok":
             print(colored("[info]:","yellow") ,res)
             raise Exception("password error")
```

### Comparing `chatglm-llm-1.4.3/chatglm_src/llm.py` & `chatglm-llm-1.4.4/chatglm_src/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,16 +65,15 @@
 ## LLM for chatglm
 # only load from local's path
 # default path is in ~/.cache/chatglm, if not exists, will download from huggingface'url :https://huggingface.co/THUDM/chatglm-6b
 # 
 """Common utility functions for working with LLM APIs."""
 import re
 from typing import List, Dict, Any, Optional, Union
-TODAY = datetime.datetime.now()
-PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
+
 # from transformers import AutoModel, AutoTokenizer
 
 os.environ["CUDA_VISIBLE_DEVICES"] = "0,1"
 def load_model_on_gpus(checkpoint_path, num_gpus=2):
     # 总共占用13GB显存,28层transformer每层0.39GB左右
     # 第一层 word_embeddings和最后一层 lm_head 层各占用1.2GB左右
     num_trans_layers = 28
@@ -237,15 +236,16 @@
         return pure_output
     
 
 
     async def _acall(self, prompt: str, stop: List[str] = None):
         assert self.remote_host is not None
         uri = f"ws://{self.remote_host}:15000"
-
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         async with AioWebSocket(uri) as aws:
             converse = aws.manipulator
             
             user_id = md5(time.asctime().encode()).hexdigest()
             await converse.send(json.dumps({"user_id":user_id, "password":PASSWORD}).encode())
             res = await converse.receive()
             res = res.decode()
@@ -286,14 +286,16 @@
             for callback in self.callbacks:
                 if is_async_method(callback.on_llm_new_token):
                         await callback.on_llm_end(result, verbose=self.verbose)
             self.history = self.history+[[prompt, result]]
             return result
 
     def _call(self, prompt: str, stop: List[str]  = None, run_manager:Any = None) -> str:
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         if self.remote_host is not None:
             ws = create_connection(f"ws://{self.remote_host}:15000")
             user_id = md5(time.asctime().encode()).hexdigest()
             # self.callback_manager =  langchain.callbacks.base.BaseCallbackManager(self.callbacks)
             
             # self.callback_manager =  BaseCallbackManager(self.callbacks)
             # self.callback_manager.set_handlers(self.callbacks)
@@ -573,14 +575,16 @@
                 },
                 verbose=self.verbose
             )
             return current_completion
         elif self.remote_host is not None :
             uri = f"ws://{self.remote_host}:15000"
             result = ''
+            TODAY = datetime.datetime.now()
+            PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
             # self.callback_manager =  BaseCallbackManager(self.callbacks)
             # self.callback_manager.set_handlers(self.callbacks)
             async with AioWebSocket(uri) as aws:
                 converse = aws.manipulator
                 
                 user_id = md5(time.asctime().encode()).hexdigest()
                 await converse.send(json.dumps({"user_id":user_id, "password":PASSWORD}).encode())
@@ -625,14 +629,16 @@
                 temperature=self.temperature,
             )
             response = enforce_stop_tokens(response, stop or [])
             self.history = self.history+[[prompt, response]]
             return response
     
     def stream(self,prompt: str, stop: List[str] = None):
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         assert self.remote_host is not None
         uri = f"ws://{self.remote_host}:15000"
         result = ''
         # self.callback_manager =  BaseCallbackManager(self.callbacks)
         # self.callback_manager.set_handlers(self.callbacks)
         
         ws = create_connection(f"ws://{self.remote_host}:15000")
@@ -684,14 +690,16 @@
         every chunk of data is 2M
         """
         for i in range(0, len(data), 1024*1024*2):
             await ws.send(data[i:i+1024*1024*2])
         await ws.send("[STOP]")
     
     def _call(self, prompt: str, stop: List[str]  = None,run_manager: Any = None) -> str:
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         if self.streaming:
             current_completion = ""
             if self.verbose:
                 print("streaming")
             
             for response, history in self.model.stream_chat(self.tokenizer, prompt, self.history, max_length=self.max_token, top_p=self.top_p,
                                                temperature=self.temperature):
@@ -956,19 +964,22 @@
     @classmethod
     async def main(cls, port):
         async with serve(cls.echo, "0.0.0.0", port):
             await asyncio.Future()  # run forever
     
     @classmethod
     async def user(cls, first_msg, websocket) -> bool:
+        TODAY = datetime.datetime.now()
+        PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
         try:
             d = json.loads(first_msg)
             user_id = d["user_id"]
             password = d["password"]
             if password != PASSWORD:
+                print("RIGHT: password is ", PASSWORD)
                 return False
             print(colored("[user-login]","green"),":",user_id)
             cls.__users[websocket] =  user_id
             await websocket.send("ok")
             return True
         except Exception as e:
             print(colored("[error]","red"),":",websocket, e)
```

### Comparing `chatglm-llm-1.4.3/chatglm_src/loader/__init__.py` & `chatglm-llm-1.4.4/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.3/setup.py` & `chatglm-llm-1.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.4.3',
+    version='1.4.4',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
```

