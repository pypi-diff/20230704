# Comparing `tmp/oidc_drf-1.2.0.tar.gz` & `tmp/oidc_drf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.2.0.tar", last modified: Mon Jul  3 11:40:35 2023, max compression
+gzip compressed data, was "oidc_drf-1.2.1.tar", last modified: Tue Jul  4 08:41:21 2023, max compression
```

## Comparing `oidc_drf-1.2.0.tar` & `oidc_drf-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-03 11:40:35.625851 oidc_drf-1.2.0/
--rw-r--r--   0 hmogbl     (501) staff       (20)     6041 2023-07-03 11:40:35.625728 oidc_drf-1.2.0/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     5302 2023-07-03 11:37:51.000000 oidc_drf-1.2.0/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-03 11:40:35.624608 oidc_drf-1.2.0/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.0/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.0/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15758 2023-07-03 09:52:34.000000 oidc_drf-1.2.0/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.0/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-03 11:40:35.625570 oidc_drf-1.2.0/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.0/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.0/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.0/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.0/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     7824 2023-07-03 09:53:29.000000 oidc_drf-1.2.0/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-03 11:40:35.625445 oidc_drf-1.2.0/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     6041 2023-07-03 11:40:35.000000 oidc_drf-1.2.0/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-03 11:40:35.000000 oidc_drf-1.2.0/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-03 11:40:35.000000 oidc_drf-1.2.0/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-03 11:40:35.000000 oidc_drf-1.2.0/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-03 11:40:35.000000 oidc_drf-1.2.0/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-03 11:40:35.625887 oidc_drf-1.2.0/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-03 11:40:11.000000 oidc_drf-1.2.0/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 08:41:21.068105 oidc_drf-1.2.1/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 08:41:21.067974 oidc_drf-1.2.1/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.1/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 08:41:21.066877 oidc_drf-1.2.1/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.1/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.1/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    15758 2023-07-03 09:52:34.000000 oidc_drf-1.2.1/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.1/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 08:41:21.067815 oidc_drf-1.2.1/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.1/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.1/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.1/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.1/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8012 2023-07-04 08:33:56.000000 oidc_drf-1.2.1/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 08:41:21.067683 oidc_drf-1.2.1/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 08:41:21.000000 oidc_drf-1.2.1/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 08:41:21.000000 oidc_drf-1.2.1/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 08:41:21.000000 oidc_drf-1.2.1/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 08:41:21.000000 oidc_drf-1.2.1/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 08:41:21.000000 oidc_drf-1.2.1/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 08:41:21.068169 oidc_drf-1.2.1/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 08:41:05.000000 oidc_drf-1.2.1/setup.py
```

### Comparing `oidc_drf-1.2.0/PKG-INFO` & `oidc_drf-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -142,36 +142,32 @@
 
 ## AUTH ENDPOINT
 
 ### Request
 
 `GET /oidc/auth/`
 
-    curl --location 'http://localhost:8000/oidc/auth'
+    curl --location 'http://localhost:8000/oidc/auth?code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss&code_challenge_method=S256&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc'
 ### Response
 
     Status: 200 OK
     {
-        "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA&code_challenge=OcDWjPAEzNI-mzrjSa2lKATcIH4oaXp7rpasc5CkRj0&code_challenge_method=S256",
-        "oidc_states": {
-            "nonce": "Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA",
-            "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
-        }
+        "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc&code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss0&code_challenge_method=S256"
     }
     
 ## CALLBACK ENDPOINT
 
 ### Request
 
 `POST /oidc/callback/`
 
     curl --location 'http://localhost:8000/oidc/callback/?state=alksdfjlka&session_state=alsdjflajsdk&code=alsdjflaksdflkjls' \
     --header 'Content-Type: application/json' \
     --data '{
-            "nonce": "Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA",
+            "nonce": "cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc",
             "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
     }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
```

### Comparing `oidc_drf-1.2.0/README.md` & `oidc_drf-1.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -126,36 +126,32 @@
 
 ## AUTH ENDPOINT
 
 ### Request
 
 `GET /oidc/auth/`
 
-    curl --location 'http://localhost:8000/oidc/auth'
+    curl --location 'http://localhost:8000/oidc/auth?code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss&code_challenge_method=S256&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc'
 ### Response
 
     Status: 200 OK
     {
-        "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA&code_challenge=OcDWjPAEzNI-mzrjSa2lKATcIH4oaXp7rpasc5CkRj0&code_challenge_method=S256",
-        "oidc_states": {
-            "nonce": "Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA",
-            "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
-        }
+        "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc&code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss0&code_challenge_method=S256"
     }
     
 ## CALLBACK ENDPOINT
 
 ### Request
 
 `POST /oidc/callback/`
 
     curl --location 'http://localhost:8000/oidc/callback/?state=alksdfjlka&session_state=alsdjflajsdk&code=alsdjflaksdflkjls' \
     --header 'Content-Type: application/json' \
     --data '{
-            "nonce": "Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA",
+            "nonce": "cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc",
             "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
     }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
```

### Comparing `oidc_drf-1.2.0/oidc_drf/admin.py` & `oidc_drf-1.2.1/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.0/oidc_drf/backends.py` & `oidc_drf-1.2.1/oidc_drf/backends.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.0/oidc_drf/drf.py` & `oidc_drf-1.2.1/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.0/oidc_drf/utils.py` & `oidc_drf-1.2.1/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.0/oidc_drf/views.py` & `oidc_drf-1.2.1/oidc_drf/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,66 +14,71 @@
 
 class OIDCGenerateAuthenticationUrlView(APIView):
     permission_classes = [AllowAny]    
     def get(self, request):
 
         state = get_random_string(import_from_settings("OIDC_STATE_SIZE", 32))
         auth_url = import_from_settings("OIDC_OP_AUTHORIZATION_ENDPOINT")
-        oidc_states = {}
+        # oidc_states = {}
 
         params ={
             "response_type":  'code',
             "client_id":  import_from_settings("OIDC_RP_CLIENT_ID"),
             "redirect_uri":  import_from_settings("OIDC_AUTHENTICATION_SSO_CALLBACK_URL"),
             "scope":  import_from_settings("OIDC_RP_SCOPES"),
             "state":  state,
         }
         
 
         
         if import_from_settings("OIDC_USE_NONCE", True):
-            nonce = get_random_string(import_from_settings("OIDC_NONCE_SIZE", 32))
+            # nonce = get_random_string(import_from_settings("OIDC_NONCE_SIZE", 32))
+            nonce = request.GET.get('nonce')
             params.update({"nonce": nonce})
-            oidc_states.update({"nonce":nonce})
+            # oidc_states.update({"nonce":nonce})
 
 
 
         if import_from_settings("OIDC_USE_PKCE", True):
-            code_verifier_length = import_from_settings("OIDC_PKCE_CODE_VERIFIER_SIZE", 64)
+            # code_verifier_length = import_from_settings("OIDC_PKCE_CODE_VERIFIER_SIZE", 64)
             # Check that code_verifier_length is between the min and max length
             # defined in https://datatracker.ietf.org/doc/html/rfc7636#section-4.1
-            if not (43 <= code_verifier_length <= 128):
-                raise ValueError("code_verifier_length must be between 43 and 128")
+            # if not (43 <= code_verifier_length <= 128):
+            #     raise ValueError("code_verifier_length must be between 43 and 128")
 
             # Generate code_verifier and code_challenge pair
-            code_verifier = get_random_string(code_verifier_length)
-            oidc_states.update({"code_verifier":code_verifier})
-            code_challenge_method = import_from_settings(
-                "OIDC_PKCE_CODE_CHALLENGE_METHOD", "S256"
-            )
-            code_challenge = generate_code_challenge(
-                code_verifier, code_challenge_method
-            )
+            # code_verifier = get_random_string(code_verifier_length)
+
+
+            # oidc_states.update({"code_verifier":code_verifier})
+            # code_challenge_method = import_from_settings(
+            #     "OIDC_PKCE_CODE_CHALLENGE_METHOD", "S256"
+            # )
+            # code_challenge = generate_code_challenge(
+            #     code_verifier, code_challenge_method
+            # )
 
             # Append code_challenge to authentication request parameters
+            
+            code_challenge = request.GET.get('code_challenge')
+            code_challenge_method = request.GET.get('code_challenge_method')
             params.update(
                 {
                     "code_challenge": code_challenge,
                     "code_challenge_method": code_challenge_method,
                 })
             
 
 
         query = urlencode(params)
         redirect_url = "{url}?{query}".format(url=auth_url, query=query)
 
 
         return Response({
-            "redirect_url":redirect_url,
-            "oidc_states":oidc_states,
+            "redirect_url":redirect_url
             } )
 
 class OIDCAuthenticationCallbackView(APIView):
     """OIDC client authentication callback HTTP endpoint"""
     permission_classes = [AllowAny]    
 
     def login_failure(self):
```

### Comparing `oidc_drf-1.2.0/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.2.1/oidc_drf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.2.0
+Version: 1.2.1
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -142,36 +142,32 @@
 
 ## AUTH ENDPOINT
 
 ### Request
 
 `GET /oidc/auth/`
 
-    curl --location 'http://localhost:8000/oidc/auth'
+    curl --location 'http://localhost:8000/oidc/auth?code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss&code_challenge_method=S256&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc'
 ### Response
 
     Status: 200 OK
     {
-        "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA&code_challenge=OcDWjPAEzNI-mzrjSa2lKATcIH4oaXp7rpasc5CkRj0&code_challenge_method=S256",
-        "oidc_states": {
-            "nonce": "Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA",
-            "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
-        }
+        "redirect_url": "http://127.0.0.1:8080/realms/mol/protocol/openid-connect/auth?response_type=code&client_id=mowaamah&redirect_uri=http%3A%2F%2Flocalhost%3A3000%2Fcallback&scope=openid+email&state=rhG5l83rwd81SytApbl7MzrTDBFRXqbo&nonce=cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc&code_challenge=4qZTfBVpD5xkxUIw0srf5rVV5H418hr-xQJLAd4c2Ss0&code_challenge_method=S256"
     }
     
 ## CALLBACK ENDPOINT
 
 ### Request
 
 `POST /oidc/callback/`
 
     curl --location 'http://localhost:8000/oidc/callback/?state=alksdfjlka&session_state=alsdjflajsdk&code=alsdjflaksdflkjls' \
     --header 'Content-Type: application/json' \
     --data '{
-            "nonce": "Pgsq3IlSLumPca81YjXc8ut03Oz7bPHA",
+            "nonce": "cFYLOJXZ8CANDC1SdQbvfUobixJdgUIc",
             "code_verifier": "cNa9FYCujvVibPnosk1Fk3wvPPisaTjE8Ns83X0UcGsNlEfIUc3j49hFftYPEGAb"
     }'
 ### Response
 
     Status: 200 OK
     {
        "access":"jwt access token",
```

### Comparing `oidc_drf-1.2.0/setup.py` & `oidc_drf-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.2.0',
+    version='1.2.1',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

