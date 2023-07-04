# Comparing `tmp/seatconnect-1.1.6.tar.gz` & `tmp/seatconnect-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatconnect-1.1.6.tar", last modified: Thu Feb 17 07:58:59 2022, max compression
+gzip compressed data, was "seatconnect-1.1.7.tar", last modified: Tue Jul  4 18:32:49 2023, max compression
```

## Comparing `seatconnect-1.1.6.tar` & `seatconnect-1.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2022-02-17 07:58:59.991279 seatconnect-1.1.6/
--rw-rw-r--   0 KINIL      (502) staff       (20)       66 2021-10-12 09:09:47.000000 seatconnect-1.1.6/.gitignore
--rw-rw-r--   0 KINIL      (502) staff       (20)    11357 2021-06-03 09:37:48.000000 seatconnect-1.1.6/LICENSE
--rw-r--r--   0 KINIL      (502) staff       (20)     6547 2022-02-17 07:58:59.991348 seatconnect-1.1.6/PKG-INFO
--rw-rw-r--   0 KINIL      (502) staff       (20)     6234 2022-01-31 13:29:38.000000 seatconnect-1.1.6/README.md
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2022-02-17 07:58:59.988433 seatconnect-1.1.6/example/
--rw-r--r--   0 KINIL      (502) staff       (20)    11980 2022-01-31 13:05:23.000000 seatconnect-1.1.6/example/example.py
--rw-r--r--   0 KINIL      (502) staff       (20)       57 2022-02-03 08:08:32.000000 seatconnect-1.1.6/requirements.txt
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2022-02-17 07:58:59.990237 seatconnect-1.1.6/seatconnect/
--rw-rw-r--   0 KINIL      (502) staff       (20)      223 2021-09-23 11:26:59.000000 seatconnect-1.1.6/seatconnect/__init__.py
--rw-rw-r--   0 KINIL      (502) staff       (20)      207 2022-02-17 07:56:07.000000 seatconnect-1.1.6/seatconnect/__version__.py
--rw-rw-r--   0 KINIL      (502) staff       (20)    79296 2022-02-17 07:56:02.000000 seatconnect-1.1.6/seatconnect/connection.py
--rw-rw-r--   0 KINIL      (502) staff       (20)     7668 2022-01-31 11:40:22.000000 seatconnect-1.1.6/seatconnect/const.py
--rw-rw-r--   0 KINIL      (502) staff       (20)    32970 2022-01-31 13:05:56.000000 seatconnect-1.1.6/seatconnect/dashboard.py
--rw-rw-r--   0 KINIL      (502) staff       (20)     2917 2021-09-23 11:53:58.000000 seatconnect-1.1.6/seatconnect/exceptions.py
--rw-rw-r--   0 KINIL      (502) staff       (20)     2563 2021-06-03 09:37:48.000000 seatconnect-1.1.6/seatconnect/utilities.py
--rw-rw-r--   0 KINIL      (502) staff       (20)   106232 2022-01-31 13:03:39.000000 seatconnect-1.1.6/seatconnect/vehicle.py
-drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2022-02-17 07:58:59.991196 seatconnect-1.1.6/seatconnect.egg-info/
--rw-rw-r--   0 KINIL      (502) staff       (20)     6547 2022-02-17 07:58:59.000000 seatconnect-1.1.6/seatconnect.egg-info/PKG-INFO
--rw-rw-r--   0 KINIL      (502) staff       (20)      454 2022-02-17 07:58:59.000000 seatconnect-1.1.6/seatconnect.egg-info/SOURCES.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)        1 2022-02-17 07:58:59.000000 seatconnect-1.1.6/seatconnect.egg-info/dependency_links.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)       57 2022-02-17 07:58:59.000000 seatconnect-1.1.6/seatconnect.egg-info/requires.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)       12 2022-02-17 07:58:59.000000 seatconnect-1.1.6/seatconnect.egg-info/top_level.txt
--rw-rw-r--   0 KINIL      (502) staff       (20)      438 2022-02-17 07:58:59.991604 seatconnect-1.1.6/setup.cfg
--rw-r--r--   0 KINIL      (502) staff       (20)      945 2022-02-03 08:08:32.000000 seatconnect-1.1.6/setup.py
+drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-07-04 18:32:49.348529 seatconnect-1.1.7/
+-rw-rw-r--   0 KINIL      (502) staff       (20)       66 2021-10-12 09:09:47.000000 seatconnect-1.1.7/.gitignore
+-rw-rw-r--   0 KINIL      (502) staff       (20)    11357 2021-06-03 09:37:48.000000 seatconnect-1.1.7/LICENSE
+-rw-r--r--   0 KINIL      (502) staff       (20)     6510 2023-07-04 18:32:49.348602 seatconnect-1.1.7/PKG-INFO
+-rw-rw-r--   0 KINIL      (502) staff       (20)     6234 2022-01-31 13:29:38.000000 seatconnect-1.1.7/README.md
+drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-07-04 18:32:49.346899 seatconnect-1.1.7/example/
+-rw-r--r--   0 KINIL      (502) staff       (20)    11980 2023-07-04 18:32:46.000000 seatconnect-1.1.7/example/example.py
+-rw-r--r--   0 KINIL      (502) staff       (20)       57 2022-02-03 08:08:32.000000 seatconnect-1.1.7/requirements.txt
+drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-07-04 18:32:49.347833 seatconnect-1.1.7/seatconnect/
+-rw-rw-r--   0 KINIL      (502) staff       (20)      223 2021-09-23 11:26:59.000000 seatconnect-1.1.7/seatconnect/__init__.py
+-rw-r--r--   0 KINIL      (502) staff       (20)      207 2023-07-04 18:31:55.000000 seatconnect-1.1.7/seatconnect/__version__.py
+-rw-r--r--   0 KINIL      (502) staff       (20)    79298 2023-07-04 18:31:55.000000 seatconnect-1.1.7/seatconnect/connection.py
+-rw-r--r--   0 KINIL      (502) staff       (20)     7675 2023-07-04 18:31:55.000000 seatconnect-1.1.7/seatconnect/const.py
+-rw-rw-r--   0 KINIL      (502) staff       (20)    32970 2022-01-31 13:05:56.000000 seatconnect-1.1.7/seatconnect/dashboard.py
+-rw-rw-r--   0 KINIL      (502) staff       (20)     2917 2021-09-23 11:53:58.000000 seatconnect-1.1.7/seatconnect/exceptions.py
+-rw-rw-r--   0 KINIL      (502) staff       (20)     2563 2021-06-03 09:37:48.000000 seatconnect-1.1.7/seatconnect/utilities.py
+-rw-rw-r--   0 KINIL      (502) staff       (20)   106232 2022-01-31 13:03:39.000000 seatconnect-1.1.7/seatconnect/vehicle.py
+drwxr-xr-x   0 KINIL      (502) staff       (20)        0 2023-07-04 18:32:49.348427 seatconnect-1.1.7/seatconnect.egg-info/
+-rw-rw-r--   0 KINIL      (502) staff       (20)     6510 2023-07-04 18:32:49.000000 seatconnect-1.1.7/seatconnect.egg-info/PKG-INFO
+-rw-rw-r--   0 KINIL      (502) staff       (20)      454 2023-07-04 18:32:49.000000 seatconnect-1.1.7/seatconnect.egg-info/SOURCES.txt
+-rw-rw-r--   0 KINIL      (502) staff       (20)        1 2023-07-04 18:32:49.000000 seatconnect-1.1.7/seatconnect.egg-info/dependency_links.txt
+-rw-rw-r--   0 KINIL      (502) staff       (20)       57 2023-07-04 18:32:49.000000 seatconnect-1.1.7/seatconnect.egg-info/requires.txt
+-rw-rw-r--   0 KINIL      (502) staff       (20)       12 2023-07-04 18:32:49.000000 seatconnect-1.1.7/seatconnect.egg-info/top_level.txt
+-rw-rw-r--   0 KINIL      (502) staff       (20)      438 2023-07-04 18:32:49.348875 seatconnect-1.1.7/setup.cfg
+-rw-r--r--   0 KINIL      (502) staff       (20)      945 2022-02-03 08:08:32.000000 seatconnect-1.1.7/setup.py
```

### Comparing `seatconnect-1.1.6/LICENSE` & `seatconnect-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/PKG-INFO` & `seatconnect-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: seatconnect
-Version: 1.1.6
+Version: 1.1.7
 Summary: Communicate with Seat Connect
 Home-page: https://github.com/farfar/seatconnect
 Author: Farfar
 Author-email: faekie@hotmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Provides: seatconnect
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Version](https://img.shields.io/github/v/release/farfar/seatconnect?include_prereleases)
 ![PyPi](https://img.shields.io/pypi/v/seatconnect?label=latest%20pypi)
 ![Downloads PyPi](https://img.shields.io/pypi/dm/seatconnect)
@@ -101,9 +99,7 @@
 conn.get<method>                                                        # The get methods calls on API endpoints and returns data. See example.
 conn.set<method>                                                        # The set methods calls on API endpoints to set config for vehicle.
 ```
 Refrain from using methods starting with _, they are intended for internal use only.
 
 ## Further help or contributions
 For questions, further help or contributions you can join the (Skoda Connect) Discord server at https://discord.gg/826X9jEtCh
-
-
```

### Comparing `seatconnect-1.1.6/README.md` & `seatconnect-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/example/example.py` & `seatconnect-1.1.7/example/example.py`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/seatconnect/connection.py` & `seatconnect-1.1.7/seatconnect/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
             _LOGGER.debug('Received authorization code, exchange for tokens.')
             # Extract code and tokens
             jwt_auth_code = parse_qs(urlparse(location).fragment).get('code')[0]
             jwt_id_token = parse_qs(urlparse(location).fragment).get('id_token')[0]
             tokenBody = {
                 'auth_code': jwt_auth_code,
                 'id_token':  jwt_id_token,
-                'brand': BRAND
+                'brand': 'cupra'
             }
             tokenURL = 'https://tokenrefreshservice.apps.emea.vwapps.io/exchangeAuthCode'
             req = await self._session.post(
                 url=tokenURL,
                 headers=self._session_auth_headers,
                 data = tokenBody,
                 allow_redirects=False
```

### Comparing `seatconnect-1.1.6/seatconnect/const.py` & `seatconnect-1.1.7/seatconnect/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 BASE_AUTH = 'https://identity.vwgroup.io'
 BRAND = 'seat'
 COUNTRY = 'ES'
 
 # Data used in communication
 CLIENT_LIST = {
     'seat': {
-        'CLIENT_ID': '50f215ac-4444-4230-9fb1-fe15cd1a9bcc@apps_vw-dilab_com',
+        'CLIENT_ID': '30e33736-c537-4c72-ab60-74a7b92cfe83@apps_vw-dilab_com',
         'SCOPE': 'openid profile address phone email birthdate nationalIdentifier cars mbb dealers badge nationality',
-        'TOKEN_TYPES': 'code id_token'
+        'TOKEN_TYPES': 'code id_token token'
     }
 }
 
 
 
 #XCLIENT_ID = '3516bc10-fabd-4eb2-b41c-b38e21e9d8f6'
-XCLIENT_ID = 'c34af3dc-f9d0-4bff-a5db-f0af674929f0'
+XCLIENT_ID = '9d183b70-d129-424f-9a26-c3778edf95e1'
 XAPPVERSION = '1.4.0'
 XAPPNAME = 'SEATConnect'
 USER_AGENT = 'okhttp/3.10.0'
-APP_URI = 'seatconnect://identity-kit/login'
+APP_URI = 'cupraconnect://identity-kit/login'
 
 HEADERS_SESSION = {
     'Connection': 'keep-alive',
     'Content-Type': 'application/json',
     'Accept-charset': 'UTF-8',
     'Accept': 'application/json',
     'X-Client-Id': XCLIENT_ID,
```

### Comparing `seatconnect-1.1.6/seatconnect/dashboard.py` & `seatconnect-1.1.7/seatconnect/dashboard.py`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/seatconnect/exceptions.py` & `seatconnect-1.1.7/seatconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/seatconnect/utilities.py` & `seatconnect-1.1.7/seatconnect/utilities.py`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/seatconnect/vehicle.py` & `seatconnect-1.1.7/seatconnect/vehicle.py`

 * *Files identical despite different names*

### Comparing `seatconnect-1.1.6/seatconnect.egg-info/PKG-INFO` & `seatconnect-1.1.7/seatconnect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: seatconnect
-Version: 1.1.6
+Version: 1.1.7
 Summary: Communicate with Seat Connect
 Home-page: https://github.com/farfar/seatconnect
 Author: Farfar
 Author-email: faekie@hotmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Provides: seatconnect
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Version](https://img.shields.io/github/v/release/farfar/seatconnect?include_prereleases)
 ![PyPi](https://img.shields.io/pypi/v/seatconnect?label=latest%20pypi)
 ![Downloads PyPi](https://img.shields.io/pypi/dm/seatconnect)
@@ -101,9 +99,7 @@
 conn.get<method>                                                        # The get methods calls on API endpoints and returns data. See example.
 conn.set<method>                                                        # The set methods calls on API endpoints to set config for vehicle.
 ```
 Refrain from using methods starting with _, they are intended for internal use only.
 
 ## Further help or contributions
 For questions, further help or contributions you can join the (Skoda Connect) Discord server at https://discord.gg/826X9jEtCh
-
-
```

### Comparing `seatconnect-1.1.6/setup.py` & `seatconnect-1.1.7/setup.py`

 * *Files identical despite different names*

