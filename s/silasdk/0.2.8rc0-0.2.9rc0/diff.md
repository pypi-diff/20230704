# Comparing `tmp/silasdk-0.2.8rc0.tar.gz` & `tmp/silasdk-0.2.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/silasdk-0.2.8rc0.tar", last modified: Mon Jun  8 23:16:27 2020, max compression
+gzip compressed data, was "dist/silasdk-0.2.9rc0.tar", last modified: Wed Jul 22 21:56:08 2020, max compression
```

## Comparing `silasdk-0.2.8rc0.tar` & `silasdk-0.2.9rc0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 sila      (1001) sila      (1001)        0 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/
--rw-rw-r--   0 sila      (1001) sila      (1001)       38 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/setup.cfg
--rw-rw-r--   0 sila      (1001) sila      (1001)     1005 2020-06-08 22:34:08.000000 silasdk-0.2.8rc0/setup.py
-drwxrwxr-x   0 sila      (1001) sila      (1001)        0 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/
--rw-rw-r--   0 sila      (1001) sila      (1001)      396 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 sila      (1001) sila      (1001)        1 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/not-zip-safe
--rw-rw-r--   0 sila      (1001) sila      (1001)        1 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 sila      (1001) sila      (1001)        8 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/top_level.txt
--rw-rw-r--   0 sila      (1001) sila      (1001)       75 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/requires.txt
--rw-rw-r--   0 sila      (1001) sila      (1001)      500 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk.egg-info/PKG-INFO
--rw-rw-r--   0 sila      (1001) sila      (1001)       67 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/README.md
-drwxrwxr-x   0 sila      (1001) sila      (1001)        0 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/silasdk/
--rw-rw-r--   0 sila      (1001) sila      (1001)     2585 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/transactions.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     2055 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/message.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     3756 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/client.py
--rw-rw-r--   0 sila      (1001) sila      (1001)      470 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/errors.py
--rw-rw-r--   0 sila      (1001) sila      (1001)      146 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/__init__.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     2349 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/ethwallet.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     1160 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/endpoints.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     2280 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/wallet.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     5947 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/users.py
--rw-rw-r--   0 sila      (1001) sila      (1001)     4295 2020-06-08 19:10:36.000000 silasdk-0.2.8rc0/silasdk/schema.py
--rw-rw-r--   0 sila      (1001) sila      (1001)      500 2020-06-08 23:16:27.000000 silasdk-0.2.8rc0/PKG-INFO
+drwxrwxr-x   0 sila      (1001) sila      (1001)        0 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/
+-rw-rw-r--   0 sila      (1001) sila      (1001)       38 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/setup.cfg
+-rw-rw-r--   0 sila      (1001) sila      (1001)     1005 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/setup.py
+drwxrwxr-x   0 sila      (1001) sila      (1001)        0 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk.egg-info/
+-rw-rw-r--   0 sila      (1001) sila      (1001)      457 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 sila      (1001) sila      (1001)        1 2020-06-08 23:16:27.000000 silasdk-0.2.9rc0/silasdk.egg-info/not-zip-safe
+-rw-rw-r--   0 sila      (1001) sila      (1001)        1 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 sila      (1001) sila      (1001)        8 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk.egg-info/top_level.txt
+-rw-rw-r--   0 sila      (1001) sila      (1001)       75 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk.egg-info/requires.txt
+-rw-rw-r--   0 sila      (1001) sila      (1001)      500 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 sila      (1001) sila      (1001)    22312 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/README.md
+drwxrwxr-x   0 sila      (1001) sila      (1001)        0 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/silasdk/
+-rw-rw-r--   0 sila      (1001) sila      (1001)     2265 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/businessOperations.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     2585 2020-06-08 19:10:36.000000 silasdk-0.2.9rc0/silasdk/transactions.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     2012 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/message.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     3669 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/client.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)      470 2020-06-08 19:10:36.000000 silasdk-0.2.9rc0/silasdk/errors.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)      250 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/__init__.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     1241 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/businessInformation.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     2364 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/ethwallet.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     1585 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/endpoints.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     2280 2020-06-08 19:10:36.000000 silasdk-0.2.9rc0/silasdk/wallet.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     7207 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/users.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)     6971 2020-07-22 21:50:58.000000 silasdk-0.2.9rc0/silasdk/schema.py
+-rw-rw-r--   0 sila      (1001) sila      (1001)      500 2020-07-22 21:56:08.000000 silasdk-0.2.9rc0/PKG-INFO
```

### Comparing `silasdk-0.2.8rc0/setup.py` & `silasdk-0.2.9rc0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from codecs import open
 from os import path
 
 setup(
     name='silasdk',
 
 
-    version='0.2.8.rc.0',
+    version='0.2.9.rc.0',
 
     description='Sila Python library for message signing and api wrapper',
 
     url="https://github.com/Sila-Money/Sila-Python",
 
     author='Sila',
     author_email='support@silamoney.com',
@@ -29,15 +29,15 @@
 
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3.6'
 
     ],
 
-    keywords='Sila v0.2.8.rc.0 Rest API',
+    keywords='Sila v0.2.9.rc.0 Rest API',
 
     packages=["silasdk"],
 
     install_requires=["requests>=2.20.0","pyaml>=15.8.2","eth-account==0.3.0","uuid==1.30","pysha3==1.0.2"],
 
     zip_safe=False,
```

### Comparing `silasdk-0.2.8rc0/silasdk/transactions.py` & `silasdk-0.2.9rc0/silasdk/transactions.py`

 * *Files identical despite different names*

### Comparing `silasdk-0.2.8rc0/silasdk/message.py` & `silasdk-0.2.9rc0/silasdk/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,21 +60,18 @@
                     inpt[i][key] = data[key]
     inpt["header"]["created"] = int(time.time())
 
     inpt = cull_null_values(inpt)
 
     return inpt
 
-def postRequest(self, path, msg_type, payload, key=None):
+def postRequest(self, path, msg_type, payload, key=None, business_key=None):
     """post the message and return resposne
     Args:
         payload:customer message
         path : endpoint
         key :user_private_key
     """
     data = createMessage(self, payload, msg_type)
-    if key is not None:
-        header = self.setHeader(data, key)
-    else:
-        header = self.setHeader(data)
+    header = self.setHeader(data, key, business_key)
     response = self.post(path, data, header)
     return response
```

### Comparing `silasdk-0.2.8rc0/silasdk/client.py` & `silasdk-0.2.9rc0/silasdk/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import requests
 from .ethwallet import EthWallet
 from .endpoints import endPoints
 from .errors import Errors
 from .schema import Schema
 
+
 class App():
 
     def __init__(self, tier, app_private_key, app_handle):
         """Initalize the application 
             This lets users initialize the application by providing the tier, application privatekey and application handle
         Args:
             tier  : SANDBOX,PROD etc
@@ -16,15 +17,15 @@
             app_handle  : application sila handle (app.silamoney.eth)
         """
         self.session = requests.Session()
         self.tier = tier.lower()
         self.app_private_key = app_private_key
         self.app_handle = app_handle
         self.updateSchema()
-        
+
     def updateSchema(self):
         """updates schema.py on initialization of app
             This lets users initialize the schema into schema.py for ease of use
         Args:
             None
         """
         endpoint = endPoints["schemaUrl"]
@@ -87,28 +88,24 @@
             path : path to the endpoint
         """
         endpoint = path
         response = self.session.get(endpoint)
         output = response.json()
         return output
 
-    def setHeader(self, msg, key=None):
+    def setHeader(self, msg, key=None, business_key=None):
         """set the application header with usersignature and authsignature
         Args:
             key : ethereum private key for the user
             msg : message being sent should be signed by user
         """
         appsignature = EthWallet.signMessage(msg, self.app_private_key)
-        if key != None:
-            usersignature = EthWallet.signMessage(msg, key.lower())
-            header = {
-                'Content-Type': 'application/json',
-                "usersignature": usersignature,
-                "authsignature": appsignature
-            }
-            return header
-        else:
-            header = {
-                'Content-Type': 'application/json',
-                "authsignature": appsignature
-            }
-            return header
+        header = {
+            'Content-Type': 'application/json',
+            "authsignature": appsignature
+        }
+        if key is not None:
+            header["usersignature"] = EthWallet.signMessage(msg, key.lower())
+        if business_key is not None:
+            header["businesssignature"] = EthWallet.signMessage(msg, business_key.lower())
+
+        return header
```

### Comparing `silasdk-0.2.8rc0/silasdk/ethwallet.py` & `silasdk-0.2.9rc0/silasdk/ethwallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from eth_account import Account
-import sha3
+import sha3, _pysha3
 import json
 
 from typing import Dict, Union
 
 
 class EthWallet:
 
@@ -28,15 +28,15 @@
         This method signs the message for the user authentication mechanism
         Args:
         msg: message to be signed
         private_key: the key can be an app key or a user key used to sign the message
         Returns:
         string: a signed message
         """
-        k = sha3.keccak_256()
+        k = _pysha3.keccak_256()
         if isinstance(msg, str):
             encoded_message = msg.encode('utf-8')
         else:
             encoded_message = (json.dumps(msg)).encode("utf-8")
         k.update(encoded_message)
         message_hash = k.hexdigest()
         if key is not None:
@@ -54,15 +54,15 @@
         This method signs the message for the user authentication mechanism
         Args:
         msg: original message
         sign : the signed hash obtained after signing the message with private key
         Returns:
         string: returns the Ethereum address corresponding to the private key the message was signed with
         """
-        k = sha3.keccak_256()
+        k = _pysha3.keccak_256()
         if isinstance(msg, str):
             encoded_message = msg.encode('utf-8')
         else:
             encoded_message = (json.dumps(msg)).encode("utf-8")
         k.update(encoded_message)
         message_hash = k.hexdigest()
         return Account.recoverHash(message_hash, signature=sign)
```

### Comparing `silasdk-0.2.8rc0/silasdk/endpoints.py` & `silasdk-0.2.9rc0/silasdk/endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,9 +21,18 @@
     "getWallet": "/get_wallet",
     "updateWallet": "/update_wallet",
     "deleteWallet": "/delete_wallet",
     "getSilaBalance": "get_sila_balance",
     "schemaUrl": "https://api.silamoney.com/0.2/getmessage?emptymessage=%sTestMessage",
     "apiUrl": "https://%s.silamoney.com/0.2",
     "silaBalanceProd": "https://silatokenapi.silamoney.com/silaBalance",
-    "silaBalanceSandbox": "https://sandbox.silatokenapi.silamoney.com/silaBalance"
-}
+    "silaBalanceSandbox": "https://sandbox.silatokenapi.silamoney.com/silaBalance",
+    "getBusinessTypes": "/get_business_types",
+    "getBusinessRoles": "/get_business_roles",
+    "getNaicsCategories": "/get_naics_categories",
+    "linkBusinessMember": "/link_business_member",
+    "unlinkBusinessMember": "/unlink_business_member",
+    "getEntities": "/get_entities?",
+    "getEntity": "/get_entity",
+    "certifyBeneficialOwner": "/certify_beneficial_owner",
+    "certifyBusiness": "/certify_business",
+}
```

### Comparing `silasdk-0.2.8rc0/silasdk/wallet.py` & `silasdk-0.2.9rc0/silasdk/wallet.py`

 * *Files identical despite different names*

### Comparing `silasdk-0.2.8rc0/silasdk/users.py` & `silasdk-0.2.9rc0/silasdk/users.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .endpoints import endPoints
 from silasdk import message
 import json
 import requests
 
+
 class User():
     def checkHandle(self, payload):
         """Check if the user handle is available.
         These endpoint returns the validity of a user handle
         Args:
         payload : Required user_handle to check if its available
         Returns:
@@ -35,98 +36,106 @@
            This user will be kyced and ethereum address will be registered with sila 
         Args:
             payload : info about user like name,ssn, dob,ethereum address, ethereum handle etc
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["requestKyc"]
-        msg_type = ("header_msg" if (use_kyc_level is False) else "header_msg_kyc_level")
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        msg_type = "header_msg"
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def linkAccount(self, payload, user_private_key, plaid=False):
         """link the bank account of user using plad
            This users bank account will be linked  
         Args:
             payload : need user handle and plad token
             user_private_key: users ethereum private key 
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["linkAccount"]
-        msg_type = ("link_account_msg" if (plaid is False) else "link_account_msg_plaid")
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        msg_type = ("link_account_msg" if (plaid is False)
+                    else "link_account_msg_plaid")
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def checkKyc(self, payload, user_private_key):
         """check if the user has been kyced.
             The user will be checked if the they have been kyced
         Args:
             payload : includes 
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["checkKyc"]
         msg_type = "header_msg"
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def addIdentity(self, payload, user_private_key):
         """change the info about user like change ssn, email ,etc.
             The used will be checked if the they have been kyced
         Args:
             payload : includes information to be edited and usee handle
             user_private_key: users ethereum private key 
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["addIdentity"]
         msg_type = "identity_msg"
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def getAccounts(self, payload, user_private_key):
         """get the accounts of users registered with sila
             The user will be checked if they have been kyced, along with app
         Args:
             user_hanlde: users handle registered with app
             user_private_key: user private key asscoicated with crypto address
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["getAccounts"]
         msg_type = "get_accounts_msg"
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def getAccountBalance(self, payload, user_private_key):
         """get the account balance of a user registered with sila
         Args:
             user_hanlde: users handle registered with app
             user_private_key: user private key asscoicated with crypto address
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["getAccountBalance"]
         msg_type = "account_name_msg"
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def getTransactions(self, payload, user_private_key):
         """get the users transactions registered with ur app
            The user will be checked if they have been kyced, along with app
         Args:
             user_hanlde: users handle registered with app
             user_private_key: user private key asscoicated with crypto address
         Returns:
             dict: response body (a confirmation message)
         """
         path = endPoints["getTransactions"]
         msg_type = "header_msg"
-        response = message.postRequest(self, path, msg_type, payload, user_private_key)
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
         return response
 
     def silaBalance(self, address):
         """get sila balance of the addresses registered with sila
            The user will be checked if they have been kyced, along with app
         Args:
             address: requires valid ethereum address
@@ -137,7 +146,37 @@
         header = {'content-type': 'application/json'}
         if self.tier == "prod":
             endpoint = endPoints["silaBalanceProd"]
         elif self.tier == "sandbox":
             endpoint = endPoints["silaBalanceSandbox"]
         response = requests.post(endpoint, data=data, headers=header)
         return response.json()
+
+    def getEntities(self, payload, per_page=None, page=None):
+        """Return all end-user and legal entities (businesses) associated with a customer application.
+            This endpoint allows the listing of all entities registered to an application.
+        Args:
+            payload: filters information
+            per_page: pagination information
+            page: pagination information
+        Returns:
+            dict: response body (entities list)
+        """
+        path = endPoints["getEntities"] + (('&per_page=' + str(per_page)) if per_page is not None else '') + (('&page=' + str(page)) if page is not None else '') 
+        msg_type = "header_msg"
+        response = message.postRequest(
+            self, path, msg_type, payload)
+        return response
+
+    def getEntity(self, payload, user_private_key):
+        """
+        Args:
+            payload: filters information
+            user_private_key
+        Returns:
+            dict: response body (entity information)
+        """
+        path = endPoints["getEntity"]
+        msg_type = "get_entity_msg"
+        response = message.postRequest(
+            self, path, msg_type, payload, user_private_key)
+        return response
```

### Comparing `silasdk-0.2.8rc0/silasdk/schema.py` & `silasdk-0.2.9rc0/silasdk/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Schema = [
-    {"header_msg_kyc_level": {
+    {"header_msg": {
         "header": {
             "reference": "",
             "created": "",
             "user_handle": "",
             "auth_handle": "",
             "version": "0.2",
             "crypto": "ETH"
         },
         "message": "header_msg",
-        "kyc_level": ""
+        "kyc_level": "",
+        "entity_type": ""
     }},
     {"link_account_msg_plaid": {
         "header": {
             "created": "",
             "auth_handle": "",
             "user_handle": "",
             "version": "0.2",
@@ -162,9 +163,117 @@
             "crypto": "ETH",
             "reference": ""
         },
         "message": "get_accounts_msg"
     }},
     {"sila_balance_msg": {
         "address": ""
+    }},
+    {"business_types_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": ""
+        }
+    }},
+    {"business_roles_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": ""
+        }
+    }},
+    {"naics_categories_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": ""
+        }
+    }},
+    {"entity_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": "",
+            "user_handle": "",
+            "version": "0.2",
+            "crypto": "ETH",
+            "reference": ""
+        },
+        "message": "entity_msg",
+        "address": {
+            "address_alias": "default",
+            "street_address_1": "",
+            "city": "",
+            "state": "",
+            "country": "",
+            "postal_code": ""
+        },
+        "identity": {
+            "identity_alias": "SSN",
+            "identity_value": ""
+        },
+        "contact": {
+            "contact_alias": "default",
+            "phone": "",
+            "email": ""
+        },
+        "crypto_entry": {
+            "crypto_alias": "default",
+            "crypto_code": "ETH",
+            "crypto_address": ""
+        },
+        "entity": {
+            "first_name": "",
+            "last_name": "",
+            "entity_name": "",
+            "birthdate": "",
+            "relationship": "",
+            "type": "",
+            "business_type": "",
+            "business_website": "",
+            "doing_business_as": "",
+            "naics_code": ""
+        }
+    }},
+    {"link_business_member_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": "",
+            "user_handle": "",
+            "business_handle": ""
+        },
+        "role": "",
+        "details": "",
+        "ownership_stake": ""
+    }},
+    {"unlink_business_member_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": "",
+            "user_handle": "",
+            "business_handle": ""
+        },
+        "role": ""
+    }},
+    {"get_entity_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": "",
+            "user_handle": ""
+        }
+    }},
+    {"certify_beneficial_owner_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": "",
+            "user_handle": "",
+            "business_handle": ""
+        },
+        "member_handle": "",
+        "certification_token": ""
+    }},
+    {"certify_business_msg": {
+        "header": {
+            "created": "",
+            "auth_handle": "",
+            "user_handle": "",
+            "business_handle": ""
+        }
     }}
 ]
```

