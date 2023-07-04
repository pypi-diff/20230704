# Comparing `tmp/oidc_drf-1.2.7.tar.gz` & `tmp/oidc_drf-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.2.7.tar", last modified: Tue Jul  4 10:22:55 2023, max compression
+gzip compressed data, was "oidc_drf-1.2.8.tar", last modified: Tue Jul  4 11:05:30 2023, max compression
```

## Comparing `oidc_drf-1.2.7.tar` & `oidc_drf-1.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 10:22:55.310870 oidc_drf-1.2.7/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 10:22:55.310742 oidc_drf-1.2.7/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.7/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 10:22:55.309822 oidc_drf-1.2.7/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.7/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.7/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15758 2023-07-03 09:52:34.000000 oidc_drf-1.2.7/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.7/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 10:22:55.310590 oidc_drf-1.2.7/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.7/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.7/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.7/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.7/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     8622 2023-07-04 10:22:39.000000 oidc_drf-1.2.7/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 10:22:55.310468 oidc_drf-1.2.7/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 10:22:55.000000 oidc_drf-1.2.7/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 10:22:55.000000 oidc_drf-1.2.7/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 10:22:55.000000 oidc_drf-1.2.7/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 10:22:55.000000 oidc_drf-1.2.7/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 10:22:55.000000 oidc_drf-1.2.7/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 10:22:55.310904 oidc_drf-1.2.7/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 10:22:51.000000 oidc_drf-1.2.7/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.642728 oidc_drf-1.2.8/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:05:30.642597 oidc_drf-1.2.8/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5239 2023-07-04 08:38:47.000000 oidc_drf-1.2.8/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.641536 oidc_drf-1.2.8/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.2.8/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.2.8/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    16020 2023-07-04 11:05:08.000000 oidc_drf-1.2.8/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.2.8/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.642456 oidc_drf-1.2.8/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.2.8/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.2.8/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.2.8/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.2.8/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     8684 2023-07-04 11:01:44.000000 oidc_drf-1.2.8/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-04 11:05:30.642310 oidc_drf-1.2.8/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5978 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-04 11:05:30.000000 oidc_drf-1.2.8/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-04 11:05:30.642763 oidc_drf-1.2.8/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-04 11:05:27.000000 oidc_drf-1.2.8/setup.py
```

### Comparing `oidc_drf-1.2.7/PKG-INFO` & `oidc_drf-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.2.7
+Version: 1.2.8
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.2.7/README.md` & `oidc_drf-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.7/oidc_drf/admin.py` & `oidc_drf-1.2.8/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.7/oidc_drf/backends.py` & `oidc_drf-1.2.8/oidc_drf/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,34 @@
             msg = "{} alg requires OIDC_RP_IDP_SIGN_KEY or OIDC_OP_JWKS_ENDPOINT to be configured."
             raise ImproperlyConfigured(msg.format(self.OIDC_RP_SIGN_ALGO))
 
         self.UserModel = get_user_model()
 
     def authenticate(self,request, **kwargs):          
         
+        print("authenticate")
         self.request = request
         if not self.request:
+            print("1")
             return None
 
 
         state = self.request.GET.get("state")
         code = self.request.GET.get("code")
         nonce = kwargs.pop("nonce", None)
         code_verifier = kwargs.pop("code_verifier", None)
         
 
+        print("nonce")
+        print(nonce)
+        print("code_verifier")
+        print(code_verifier)
 
         if not code or not state:
+            print("2")
             return None
 
         redirect_uri = import_from_settings(
             "OIDC_AUTHENTICATION_SSO_CALLBACK_URL", "http://localhost:3000/callback"
         )
 
 
@@ -110,15 +117,17 @@
                 
         if payload:
             self.store_tokens(access_token, id_token, refresh_token)
             try:
                 return self.get_or_create_user(access_token, id_token, payload)
             except SuspiciousOperation as exc:
                 LOGGER.warning("failed to get or create user: %s", exc)
+                print("3")
                 return None
+        print("4")
         return None
         
         
     def get_userinfo(self, access_token, id_token, payload):
         """Return user details dictionary. The id_token and payload are not used in
         the default implementation, but may be used when overriding this method"""
 
@@ -278,14 +287,16 @@
                 self.save_user_data(user, user_json)
             return user
         else:
             LOGGER.debug(
                 "Login failed: No user with %s found, and " "OIDC_CREATE_USER is False",
                 self.describe_user_by_claims(user_info),
             )
+            
+            print("5")
             return None
 
     def retrieve_matching_jwk(self, token):
         """Get the signing key by exploring the JWKS endpoint of the OP."""
         response_jwks = requests.get(
             self.OIDC_OP_JWKS_ENDPOINT,
             verify=import_from_settings("OIDC_VERIFY_SSL", True),
```

### Comparing `oidc_drf-1.2.7/oidc_drf/drf.py` & `oidc_drf-1.2.8/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.7/oidc_drf/utils.py` & `oidc_drf-1.2.8/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.2.7/oidc_drf/views.py` & `oidc_drf-1.2.8/oidc_drf/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "state":  state,
         }
         
 
         
         if import_from_settings("OIDC_USE_NONCE", True):
             # nonce = get_random_string(import_from_settings("OIDC_NONCE_SIZE", 32))
-            nonce = request.GET.get('nonce')
+            nonce = request.GET.get('nonce',None)
             params.update({"nonce": nonce})
             # oidc_states.update({"nonce":nonce})
 
 
 
         if import_from_settings("OIDC_USE_PKCE", True):
             # code_verifier_length = import_from_settings("OIDC_PKCE_CODE_VERIFIER_SIZE", 64)
@@ -55,16 +55,16 @@
             # )
             # code_challenge = generate_code_challenge(
             #     code_verifier, code_challenge_method
             # )
 
             # Append code_challenge to authentication request parameters
             
-            code_challenge = request.GET.get('code_challenge')
-            code_challenge_method = request.GET.get('code_challenge_method')
+            code_challenge = request.GET.get('code_challenge',None)
+            code_challenge_method = request.GET.get('code_challenge_method',None)
             params.update(
                 {
                     "code_challenge": code_challenge,
                     "code_challenge_method": code_challenge_method,
                 })
             
 
@@ -81,14 +81,15 @@
     """OIDC client authentication callback HTTP endpoint"""
     permission_classes = [AllowAny]    
 
     def login_failure(self,error_message):
         return Response({"detail":error_message}, status=status.HTTP_401_UNAUTHORIZED)
 
     def login_success(self):   
+        print("login_success")
         try:     
             oidc_access_token = self.request.session["oidc_access_token"]
             oidc_id_token = self.request.session["oidc_id_token"]
             oidc_refresh_token = self.request.session["oidc_refresh_token"]
             
             data = {
                 'access': str(oidc_access_token),
@@ -132,15 +133,15 @@
             kwargs = {
                 "request": request,
                 "nonce": data.get("nonce",None),
                 "code_verifier": data.get("code_verifier",None),
             }
 
             self.user = auth.authenticate(**kwargs)
-            
+            print(self.user)
             if self.user and self.user.is_active:
                 return self.login_success()
         
         return self.login_failure("Login failed")
 
 class OIDCLogoutView(APIView):
     permission_classes = [AllowAny]
```

### Comparing `oidc_drf-1.2.7/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.2.8/oidc_drf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.2.7
+Version: 1.2.8
 Summary: Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.2.7/setup.py` & `oidc_drf-1.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.2.7',
+    version='1.2.8',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

