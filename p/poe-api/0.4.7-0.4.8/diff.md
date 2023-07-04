# Comparing `tmp/poe_api-0.4.7-py3-none-any.whl.zip` & `tmp/poe_api-0.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40992 bytes, number of entries: 42
--rw-r--r--  2.0 unx    21681 b- defN 23-Jun-29 06:05 poe.py
+Zip file size: 41548 bytes, number of entries: 42
+-rw-r--r--  2.0 unx    23325 b- defN 23-Jul-04 01:53 poe.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-May-27 23:16 poe_graphql/AddHumanMessageMutation.graphql
 -rw-r--r--  2.0 unx      504 b- defN 23-Jun-04 03:20 poe_graphql/AddMessageBreakMutation.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/AutoSubscriptionMutation.graphql
 -rw-r--r--  2.0 unx       97 b- defN 23-May-27 23:16 poe_graphql/BioFragment.graphql
 -rw-r--r--  2.0 unx       73 b- defN 23-May-27 23:16 poe_graphql/ChatAddedSubscription.graphql
 -rw-r--r--  2.0 unx      100 b- defN 23-May-27 23:16 poe_graphql/ChatFragment.graphql
 -rw-r--r--  2.0 unx    11486 b- defN 23-Jun-04 03:16 poe_graphql/ChatListPaginationQuery.graphql
@@ -32,13 +32,13 @@
 -rw-r--r--  2.0 unx      147 b- defN 23-May-27 23:16 poe_graphql/SummarizeQuotePostQuery.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/SummarizeSharePostQuery.graphql
 -rw-r--r--  2.0 unx      368 b- defN 23-May-27 23:16 poe_graphql/UserSnippetFragment.graphql
 -rw-r--r--  2.0 unx      400 b- defN 23-May-27 23:16 poe_graphql/ViewerInfoQuery.graphql
 -rw-r--r--  2.0 unx     1038 b- defN 23-May-27 23:16 poe_graphql/ViewerStateFragment.graphql
 -rw-r--r--  2.0 unx      657 b- defN 23-May-27 23:16 poe_graphql/ViewerStateUpdatedSubscription.graphql
 -rw-r--r--  2.0 unx        0 b- defN 23-May-27 23:16 poe_graphql/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    18103 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3969 b- defN 23-Jun-29 06:08 poe_api-0.4.7.dist-info/RECORD
-42 files, 105288 bytes uncompressed, 34450 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-04 01:56 poe_api-0.4.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18289 b- defN 23-Jul-04 01:56 poe_api-0.4.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 01:56 poe_api-0.4.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-04 01:56 poe_api-0.4.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3969 b- defN 23-Jul-04 01:56 poe_api-0.4.8.dist-info/RECORD
+42 files, 107118 bytes uncompressed, 35006 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -105,23 +105,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.4.7.dist-info/LICENSE
+Filename: poe_api-0.4.8.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.4.7.dist-info/METADATA
+Filename: poe_api-0.4.8.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.4.7.dist-info/WHEEL
+Filename: poe_api-0.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.4.7.dist-info/top_level.txt
+Filename: poe_api-0.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.4.7.dist-info/RECORD
+Filename: poe_api-0.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -1,13 +1,14 @@
 import re, json, random, logging, time, queue, threading, traceback, hashlib, string, random, os
 import requests
 import tls_client as requests_tls
 import secrets
 import websocket
 import uuid
+import random
 from pathlib import Path
 from urllib.parse import urlparse
 
 parent_path = Path(__file__).resolve().parent
 queries_path = parent_path / "poe_graphql"
 queries = {}
 
@@ -29,19 +30,45 @@
   for path in queries_path.iterdir():
     if path.suffix != ".graphql":
       continue
     with open(path) as f:
       queries[path.stem] = f.read()
 
 def generate_payload(query_name, variables):
+  if query_name == "recv":
+    return generate_recv_payload(variables)
   return {
     "query": queries[query_name],
     "variables": variables
   }
 
+def generate_recv_payload(variables):
+  payload = [
+    {
+      "category": "poe/bot_response_speed",
+      "data": variables,
+    }
+  ]
+  
+  if random.random() > 0.9:
+    payload.append({
+      "category": "poe/statsd_event",
+      "data": {
+        "key": "poe.speed.web_vitals.INP",
+        "value": random.randint(100, 125),
+        "category": "time",
+        "path": "/[handle]",
+        "extra_data": {},
+      },
+    })
+
+  print(payload)
+  return payload
+
+
 def request_with_retries(method, *args, **kwargs):
   attempts = kwargs.get("attempts") or 10
   url = args[0]
   for i in range(attempts):
     r = method(*args, **kwargs)
     if r.status_code == 200:
       return r
@@ -177,15 +204,15 @@
     cipher_regex = r'.\[(\d+)\]=.\[(\d+)\]'
     cipher_pairs = re.findall(cipher_regex, script_text)
 
     formkey_list = [""] * len(cipher_pairs)
     for pair in cipher_pairs:
       formkey_index, key_index = map(int, pair)
       formkey_list[formkey_index] = key_text[key_index]
-    formkey = "".join(formkey_list)
+    formkey = "".join(formkey_list)[:-1] # credit to @aditiaryan on realizing my mistake
     
     return formkey
 
   def get_next_data(self, overwrite_vars=False):
     logger.info("Downloading next_data...")
     
     r = request_with_retries(self.session.get, self.home_url)
@@ -205,17 +232,17 @@
     return next_data
   
   def get_bot(self, display_name):
     url = f'https://poe.com/_next/data/{self.next_data["buildId"]}/{display_name}.json'
     
     data = request_with_retries(self.session.get, url).json()
     if "payload" in data["pageProps"]:
-      chat_data = data["pageProps"]["payload"]["chatOfBotDisplayName"]
+      chat_data = data["pageProps"]["payload"]["chatOfBotHandle"]
     else:
-      chat_data = data["pageProps"]["data"]["chatOfBotDisplayName"]
+      chat_data = data["pageProps"]["data"]["chatOfBotHandle"]
     return chat_data
     
   def get_bots(self, download_next_data=True):
     logger.info("Downloading all bots...")
     if download_next_data:
       next_data = self.get_next_data(overwrite_vars=True)
     else:
@@ -317,15 +344,19 @@
       
       headers = {
         "content-type": "application/json",
         "poe-tag-id": hashlib.md5(base_string.encode()).hexdigest()
       }
       headers = {**self.gql_headers, **headers}
       
-      r = request_with_retries(self.session.post, self.gql_url, data=payload, headers=headers)
+      if query_name == "recv":
+        r = request_with_retries(self.session.post, self.gql_recv_url, data=payload, headers=headers)
+        return None
+      else:
+        r = request_with_retries(self.session.post, self.gql_url, data=payload, headers=headers)
       
       data = r.json()
       if data["data"] == None:
         logger.warn(f'{query_name} returned an error: {data["errors"][0]["message"]} | Retrying ({i+1}/20)')
         time.sleep(2)
         continue
 
@@ -457,15 +488,15 @@
             return
 
     except Exception:
       logger.error(traceback.format_exc())
       self.disconnect_ws()
       self.connect_ws()
 
-  def send_message(self, chatbot, message, with_chat_break=False, timeout=20):
+  def send_message(self, chatbot, message, with_chat_break=False, timeout=20, async_recv=True):
     # if there is another active message, wait until it has finished sending
     timer = 0
     while None in self.active_messages.values():
       time.sleep(0.01)
       timer += 0.01
       if timer > timeout:
         raise RuntimeError("Timed out waiting for other messages to send.")
@@ -524,14 +555,40 @@
 
       #update info about response
       message["text_new"] = message["text"][len(last_text):]
       last_text = message["text"]
       message_id = message["messageId"]
 
       yield message
+    
+    def recv_post_thread():
+      bot_message_id = self.active_messages[human_message_id]
+
+      # wait 2 seconds after sending the request
+      time.sleep(2.5)
+
+      # send recv_post after receiving the last message
+      self.send_query("recv", {
+        "bot": chatbot,
+        "time_to_first_typing_indicator": 300, # randomly select
+        "time_to_first_subscription_response": 600,
+        "time_to_full_bot_response": 1100,
+        "full_response_length": len(last_text) + 1,
+        "full_response_word_count": len(last_text.split(" ")) + 1,
+        "human_message_id": human_message_id,
+        "bot_message_id": bot_message_id,
+        "chat_id": chat_id,
+        "bot_response_status": "success",
+      })
+      time.sleep(0.5)
+    
+    t = threading.Thread(target=recv_post_thread, daemon=True)
+    t.start()
+    if not async_recv:
+      t.join()
 
     del self.active_messages[human_message_id]
     del self.message_queues[human_message_id]
   
   def send_chat_break(self, chatbot):
     logger.info(f"Sending chat break to {chatbot}")
     result = self.send_query("AddMessageBreakMutation", {
@@ -658,8 +715,8 @@
     self.get_bots()
     return data
   
   def purge_all_conversations(self):
     logger.info("Purging all conversations")
     self.send_query("DeleteUserMessagesMutation", {})
 
-load_queries()
+load_queries()
```

## Comparing `poe_api-0.4.7.dist-info/LICENSE` & `poe_api-0.4.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.4.7.dist-info/METADATA` & `poe_api-0.4.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.4.7
+Version: 0.4.8
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,15 @@
 
 #### Sending Messages:
 You can use the `client.send_message` function to send a message to a chatbot, which accepts the following arguments:
  - `chatbot` - The codename of the chatbot. (example: `capybara`)
  - `message` - The message to send to the chatbot.
  - `with_chat_break = False` - Whether the conversation context should be cleared.
  - `timeout = 20` - The max number of seconds in between received chunks until a `RuntimeError` is raised. 
+ - `async_recv = True` - Whether or not to make the `receive_POST` request async. If this is disabled, then there will be an extra wait of about 3 seconds after the message is complete.
 
 The function is a generator which returns the most recent version of the generated message whenever it is updated.
 
 Streamed Example:
 ```python
 message = "Summarize the GNU GPL v3"
 for chunk in client.send_message("capybara", message):
```

## Comparing `poe_api-0.4.7.dist-info/RECORD` & `poe_api-0.4.8.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-poe.py,sha256=vty7y4zUbHJ4cvVotLagR5FbVyu40KWMKp9MNEDwZeY,21681
+poe.py,sha256=Y4xlNcn44VGnV-KUcW2ObsNKeADiQHlKnaC1A79wkcM,23325
 poe_graphql/AddHumanMessageMutation.graphql,sha256=Va4SoysKE2qPlJfbwoKp6mNv0vs5hnVR20g8hPvAxdY,1093
 poe_graphql/AddMessageBreakMutation.graphql,sha256=lFDgYYX0ZTHso-ZQwm-oUk-HaSTRqOmj-zIjBQRL2sM,504
 poe_graphql/AutoSubscriptionMutation.graphql,sha256=3i8EnqwUrjOcJ2Hxly-lKhwPBJdbpO99POiM_K6jVD4,180
 poe_graphql/BioFragment.graphql,sha256=3ZdXaPtuHK38bG10WFH6bvpebcyrTLu5fs-ddtfLjf0,97
 poe_graphql/ChatAddedSubscription.graphql,sha256=NFLZJAwi0V2WQea1oelyRUrtNrwOE58NOeX8ChzVE10,73
 poe_graphql/ChatFragment.graphql,sha256=NFVSvT3NdYlEquue3yTHPu9ezCIgx6k1OXJZo2ytIzU,100
 poe_graphql/ChatListPaginationQuery.graphql,sha256=WameJV_yyS6Ey_VKn7okXAzR45AE9wOB2U6QlRgp-M4,11486
@@ -31,12 +31,12 @@
 poe_graphql/SummarizeQuotePostQuery.graphql,sha256=V4PQ1XkEDCsVR3z7h4SLsonZsWG7RptFd6JPwlGwOvE,147
 poe_graphql/SummarizeSharePostQuery.graphql,sha256=iCN8oiUUp2jfsiBxmsTA7k3_60E0MNwA5gnNrhnYpJc,180
 poe_graphql/UserSnippetFragment.graphql,sha256=Eg8rK7XM6-HqVJkpEBY0bJaYqF-FdDdWdg-Jj3VTnF0,368
 poe_graphql/ViewerInfoQuery.graphql,sha256=Xtn-VGGiknKgrW81s7YfIJwhmilobrSqiCObpoJdYfw,400
 poe_graphql/ViewerStateFragment.graphql,sha256=aicUJncsRpPBh_L2xqDv0aHcUIPIsDrDFPfDs3jcFoU,1038
 poe_graphql/ViewerStateUpdatedSubscription.graphql,sha256=1dPs0WuOLl4ybZXm4bUF60eVc94O10EkKOtqnQYODic,657
 poe_graphql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-poe_api-0.4.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-poe_api-0.4.7.dist-info/METADATA,sha256=b5Yir6Qz7hZX2UGEqerz70NeQVnQeFq4QML2n-3PA6U,18103
-poe_api-0.4.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-poe_api-0.4.7.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
-poe_api-0.4.7.dist-info/RECORD,,
+poe_api-0.4.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+poe_api-0.4.8.dist-info/METADATA,sha256=x5_lbFBGm0vCqayizVEO7CuZA7ahxi18bah_2jCZlPc,18289
+poe_api-0.4.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+poe_api-0.4.8.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
+poe_api-0.4.8.dist-info/RECORD,,
```

