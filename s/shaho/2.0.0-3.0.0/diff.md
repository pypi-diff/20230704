# Comparing `tmp/shaho-2.0.0.tar.gz` & `tmp/shaho-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaho-2.0.0.tar", last modified: Sat Jul  1 21:33:17 2023, max compression
+gzip compressed data, was "shaho-3.0.0.tar", last modified: Tue Jul  4 18:57:42 2023, max compression
```

## Comparing `shaho-2.0.0.tar` & `shaho-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 21:33:17.149191 shaho-2.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-2.0.0/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-01 21:33:17.119191 shaho-2.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-2.0.0/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-01 21:33:17.149191 shaho-2.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-01 21:06:13.000000 shaho-2.0.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 21:33:16.939190 shaho-2.0.0/shaho/
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-2.0.0/shaho/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    18290 2023-07-01 21:30:03.000000 shaho-2.0.0/shaho/mb.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 21:33:17.099191 shaho-2.0.0/shaho.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      172 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-04 18:57:42.433614 shaho-3.0.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-3.0.0/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-04 18:57:42.413614 shaho-3.0.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-3.0.0/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-04 18:57:42.433614 shaho-3.0.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-04 18:45:18.000000 shaho-3.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-04 18:57:42.253614 shaho-3.0.0/shaho/
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-3.0.0/shaho/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    22222 2023-07-04 18:44:18.000000 shaho-3.0.0/shaho/mb.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-04 18:57:42.393614 shaho-3.0.0/shaho.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-04 18:57:41.000000 shaho-3.0.0/shaho.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      172 2023-07-04 18:57:42.000000 shaho-3.0.0/shaho.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-04 18:57:41.000000 shaho-3.0.0/shaho.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-04 18:57:42.000000 shaho-3.0.0/shaho.egg-info/top_level.txt
```

### Comparing `shaho-2.0.0/LICENCE` & `shaho-3.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `shaho-2.0.0/PKG-INFO` & `shaho-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 2.0.0
+Version: 3.0.0
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
 Platform: UNKNOWN
```

### Comparing `shaho-2.0.0/setup.py` & `shaho-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from setuptools import setup
 
 _long_description = open('README.md').read()
 
 setup(
     name = "shaho",
-    version = "2.0.0",
+    version = "3.0.0",
     author = "shaho",
     author_email = "mbshahoorg@gmail.com",
     description = (" library Robot"),
     license = "MIT",
     keywords = ["shaho","Shaho"],
     url = "https://github.com",
     packages=['shaho'],
```

### Comparing `shaho-2.0.0/shaho/mb.py` & `shaho-3.0.0/shaho/mb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import base64
 from json import dumps, loads
 from random import randint,choice
 import datetime
+import math
 import urllib3
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 from Crypto.Signature import pkcs1_15
 from Crypto.Cipher import PKCS1_OAEP
 from Crypto.Hash import SHA256
 from Crypto.PublicKey import RSA
 from requests import post
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 import json
 from json import dumps, loads
 import random
 from requests import post, get
 import urllib
+import io
 from urllib import request
 from pathlib import Path
 from re import findall
+from PIL import Image , ImageFont, ImageDraw
 from tinytag import TinyTag
 class encryption:
 	def __init__(self, auth:str, private_key:str=None):
 
 		self.key = bytearray(self.secret(auth), "UTF-8")
 		self.iv = bytearray.fromhex('00000000000000000000000000000000')
 		if private_key:
@@ -574,7 +577,149 @@
 		return self.send_data(input,method)
 	
 	def getGroupLink(self, chat_id):
 		input = {
 		"group_guid":chat_id}
 		method = "getGroupLink"
 		return self.send_data(input,method)
+		
+	def requestFile(self, name, size , mime):
+		input = {
+		"file_name":name,
+		"size":size,
+		"mime":mime}
+		method = "requestSendFile"
+		return self.send_data(input,method)
+		
+		
+	def fileUpload(self, bytef ,hash_send ,file_id ,url):
+		if len(bytef) <= 131072:
+			h = {
+				'auth':self.auth,
+				'chunk-size':str(len(bytef)),
+				'file-id':str(file_id),
+				'access-hash-send':hash_send,
+				'total-part':str(1),
+				'part-number':str(1)
+			}
+			t = False
+			while t == False:
+				try:
+					j = post(data=bytef,url=url,headers=h).text
+					j = loads(j)['data']['access_hash_rec']
+					t = True
+				except:
+					t = False
+			
+			return j
+		else:
+			t = len(bytef) / 131072
+			t += 1
+			t = math.floor(t)
+			for i in range(1,t+1):
+				if i != t:
+					k = i - 1
+					k = k * 131072
+					t2 = False
+					while t2 == False:
+						try:
+							o = post(data=bytef[k:k + 131072],url=url,headers={
+								'auth':self.auth,
+								'chunk-size':str(131072),
+								'file-id':file_id,
+								'access-hash-send':hash_send,
+								'total-part':str(t),
+								'part-number':str(i)
+							}).text
+							o = loads(o)['data']
+							t2 = True
+						except:
+							t2 = False
+					j = k + 131072
+					j = round(j / 1024)
+					j2 = round(len(bytef) / 1024)
+					print(str(j) + 'kb / ' + str(j2) + ' kb')                
+				else:
+					k = i - 1
+					k = k * 131072
+					t2 = False
+					while t2 == False:
+						try:
+							p = post(data=bytef[k:],url=url,headers={
+								'auth':self.auth,
+								'chunk-size':str(len(bytef[k:])),
+								'file-id':file_id,
+								'access-hash-send':hash_send,
+								'total-part':str(t),
+								'part-number':str(i)
+							}).text
+							p = loads(p)['data']['access_hash_rec']
+							t2 = True
+						except:
+							t2 = False
+					j2 = round(len(bytef) / 1024)
+					print(str(j2) + 'kb / ' + str(j2) + ' kb') 
+					return p
+					
+	
+	def sendImage(self, chat_id, file_id , mime , dc_id, access_hash_rec, file_name,  size, thumb_inline , width , height, text=None, message_id=None):
+		input = {
+		"object_guid":chat_id,
+		"rnd":f"{randint(100000,900000)}",
+		"file_inline":{
+		"dc_id":str(dc_id),
+		"file_id":str(file_id),
+		"type":"Image",
+		"file_name":file_name,
+		"size":size,
+		"mime":mime,
+		"access_hash_rec":access_hash_rec,
+		'thumb_inline':thumb_inline,
+		'width':width,
+		'height':height}}
+		method = "sendMessage"
+		if text != None: input["text"] = text
+		if message_id != None: input["reply_to_message_id"] = message_id
+		return self.send_data(input,method)
+		
+	
+	def getImageSize(self,image_bytes:bytes):
+		im = Image.open(io.BytesIO(image_bytes))
+		width, height = im.size
+		return width , height
+		
+		
+	
+	def getThumbInline(self,image_bytes:bytes):
+		im = Image.open(io.BytesIO(image_bytes))
+		width, height = im.size
+		if height > width:
+			new_height = 40
+			new_width  = round(new_height * width / height)
+		else:
+			new_width  = 40
+			new_height = round(new_width * height / width)
+		im = im.resize((new_width, new_height), Image.ANTIALIAS)
+		changed_image = io.BytesIO()
+		im.save(changed_image, format='PNG')
+		changed_image = changed_image.getvalue()
+		return base64.b64encode(changed_image)
+		
+		
+		
+	def sendVoice1(self, chat_id, file_id , mime , dc_id, access_hash_rec, file_name,  size, duration, text=None, message_id=None):
+		input = {
+		"object_guid":chat_id,
+		"rnd":f"{randint(100000,900000)}",
+		"file_inline":{
+		"dc_id":str(dc_id),
+		"file_id":str(file_id),
+		"type":"Voice",
+		"file_name":file_name,
+		"size":size,
+		"mime":mime,
+		"access_hash_rec":access_hash_rec,
+		'time':duration,}}
+		method = "sendMessage"
+		if text != None: input["text"] = text
+		if message_id != None: input["reply_to_message_id"] = message_id
+		return self.send_data(input,method)
```

### Comparing `shaho-2.0.0/shaho.egg-info/PKG-INFO` & `shaho-3.0.0/shaho.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 2.0.0
+Version: 3.0.0
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
 Platform: UNKNOWN
```

