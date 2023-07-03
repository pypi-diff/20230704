# Comparing `tmp/SecureMessaging-1.0.5-py3-none-any.whl.zip` & `tmp/SecureMessaging-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5514 bytes, number of entries: 5
--rw-r--r--  2.0 unx    12558 b- defN 23-Jul-01 17:36 SecureMessaging.py
--rw-r--r--  2.0 unx     1883 b- defN 23-Jul-01 17:53 SecureMessaging-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 17:53 SecureMessaging-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 17:53 SecureMessaging-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      406 b- defN 23-Jul-01 17:53 SecureMessaging-1.0.5.dist-info/RECORD
-5 files, 14955 bytes uncompressed, 4756 bytes compressed:  68.2%
+Zip file size: 5686 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    13646 b- defN 23-Jul-03 23:51 SecureMessaging.py
+-rw-r--r--  2.0 unx     1907 b- defN 23-Jul-03 23:52 SecureMessaging-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 23:52 SecureMessaging-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-03 23:52 SecureMessaging-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      406 b- defN 23-Jul-03 23:52 SecureMessaging-1.0.6.dist-info/RECORD
+5 files, 16067 bytes uncompressed, 4928 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: SecureMessaging.py
 Comment: 
 
-Filename: SecureMessaging-1.0.5.dist-info/METADATA
+Filename: SecureMessaging-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: SecureMessaging-1.0.5.dist-info/WHEEL
+Filename: SecureMessaging-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: SecureMessaging-1.0.5.dist-info/top_level.txt
+Filename: SecureMessaging-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: SecureMessaging-1.0.5.dist-info/RECORD
+Filename: SecureMessaging-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SecureMessaging.py

```diff
@@ -1,11 +1,13 @@
 import threading
 import string
 import random
 import time
+import os
+import platform
 import sys
 import socket
 import pickle
 import hmac
 import hashlib
 from cryptography.hazmat.primitives.asymmetric import dh
 from cryptography.hazmat.backends import default_backend
@@ -16,14 +18,22 @@
 from prompt_toolkit.patch_stdout import patch_stdout
 from prompt_toolkit.shortcuts import print_formatted_text
 
 rng = "False"
 keyboard = string.printable[:-5]
 one_time_pad = list(keyboard)
 
+def selfdestruct():
+    if platform == "Linux":
+        os.system('clear')
+    elif platform == "Windows":
+        os.system('cls')
+    else:
+        os.system('clear')
+
 def get_ip_address():
     try:
         # The following line of code could fail if the computer is not connected to a network
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         # The IP address isn't important here, we just need to specify a valid address
         s.connect(("8.8.8.8", 80))
         ip_address = s.getsockname()[0]
@@ -273,28 +283,51 @@
     with patch_stdout():
         # Prompt for the IP address
         session = PromptSession(history=InMemoryHistory(), auto_suggest=AutoSuggestFromHistory())
         ip = session.prompt("Enter the IP address to send the message to (q to quit): ")
         
         if ip == "q":
             print_formatted_text("Please don't go!")
+            time.sleep(1)
+            print("\n5")
+            time.sleep(1)
+            print("\n4")
+            time.sleep(1)
+            print("\n3")
+            time.sleep(1)
+            print("\n2")
+            time.sleep(1)
+            print("\n1")
+            print("\n[-] Self destruct initiated!")
+            time.sleep(1)
+            selfdestruct()
             exit(0)
     with patch_stdout():
         # Send and receive messages
             # loop for sending messages
         while True:
             # Get the message to send
             msg = session.prompt("\nEnter the message (press 'q' to quit, 'CHANGEIP' to change the listener IP): ")
 
             # Handle the different types of input
             if msg == "q":
                 print_formatted_text("I want more lettuce though!")
+                time.sleep(1)
+                print_formatted_text("\n5")
+                time.sleep(1)
+                print_formatted_text("\n4")
+                time.sleep(1)
+                print_formatted_text("\n3")
+                time.sleep(1)
+                print_formatted_text("\n2")
+                time.sleep(1)
+                print_formatted_text("\n1")
+                print_formatted_text("\n[-] Self destruct initiated!")
+                time.sleep(1)
+                selfdestruct()
                 exit(0)
             elif msg == "CHANGEIP":
                 ip = session.prompt("Enter the new IP address to send the message to: ")
             else:
                 # Start the send thread
                 send_thread = threading.Thread(target=send_message, args=(ip, msg))
                 send_thread.start()
-
-
-
```

## Comparing `SecureMessaging-1.0.5.dist-info/METADATA` & `SecureMessaging-1.0.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: SecureMessaging
-Version: 1.0.5
+Version: 1.0.6
 Summary: Secure Messaging
 Home-page: https://github.com/ethicalhacker7192/SecureMessaging
 Author: Guinea_Pig_Lord
 Author-email: bear@lowrey.us
 License: MIT
 Keywords: Secure Messaging
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
+Requires-Dist: platform
 Requires-Dist: prompt-toolkit
 
 # SecureMessaging
 A module for messaging securely.
 
 Pretty much the same thing as GuineaSend but more lightweight.
```

