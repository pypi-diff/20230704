# Comparing `tmp/luucy_python-0.3.0.tar.gz` & `tmp/luucy_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luucy_python-0.3.0.tar", last modified: Tue Jul  4 18:38:14 2023, max compression
+gzip compressed data, was "luucy_python-0.4.0.tar", last modified: Tue Jul  4 19:28:59 2023, max compression
```

## Comparing `luucy_python-0.3.0.tar` & `luucy_python-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      182 2023-07-04 18:37:48.311589 luucy_python-0.3.0/README.md
--rw-r--r--   0        0        0     1446 2023-07-04 18:38:14.543809 luucy_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-04 18:37:48.312589 luucy_python-0.3.0/src/luucy/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 18:37:48.312589 luucy_python-0.3.0/src/luucy/__version__.py
--rw-r--r--   0        0        0     1391 2023-07-04 18:37:48.312589 luucy_python-0.3.0/src/luucy/core.py
--rw-r--r--   0        0        0     2407 2023-07-04 18:37:48.312589 luucy_python-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      844 2023-07-04 18:37:48.312589 luucy_python-0.3.0/tests/features/login/init.feature
--rw-r--r--   0        0        0      628 2023-07-04 18:37:48.312589 luucy_python-0.3.0/tests/test_init_with_username_and_password.py
--rw-r--r--   0        0        0      582 2023-07-04 18:37:48.313589 luucy_python-0.3.0/tests/test_init_without_username_and_password copy.py
--rw-r--r--   0        0        0      661 2023-07-04 18:37:48.313589 luucy_python-0.3.0/tests/test_initi_with_env_username_and_password.py
--rw-r--r--   0        0        0      474 2023-07-04 18:37:48.313589 luucy_python-0.3.0/tests/test_returns_logged_in_user_data.py
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 luucy_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      182 2023-07-04 19:28:32.099363 luucy_python-0.4.0/README.md
+-rw-r--r--   0        0        0     1446 2023-07-04 19:28:59.021057 luucy_python-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-04 19:28:32.100363 luucy_python-0.4.0/src/luucy/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-04 19:28:32.100363 luucy_python-0.4.0/src/luucy/__version__.py
+-rw-r--r--   0        0        0     1791 2023-07-04 19:28:32.100363 luucy_python-0.4.0/src/luucy/core.py
+-rw-r--r--   0        0        0     2460 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1144 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/features/login/init.feature
+-rw-r--r--   0        0        0      628 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/test_init_with_username_and_password.py
+-rw-r--r--   0        0        0      582 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/test_init_without_username_and_password copy.py
+-rw-r--r--   0        0        0      661 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/test_initi_with_env_username_and_password.py
+-rw-r--r--   0        0        0      479 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/test_production_environment.py
+-rw-r--r--   0        0        0      474 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/test_returns_logged_in_user_data.py
+-rw-r--r--   0        0        0      543 2023-07-04 19:28:32.101363 luucy_python-0.4.0/tests/test_staging_environment.py
+-rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 luucy_python-0.4.0/PKG-INFO
```

### Comparing `luucy_python-0.3.0/pyproject.toml` & `luucy_python-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "luucy-python"
-version = "0.3.0"
+version = "0.4.0"
 description = "LUUCY Python APIs"
 authors = [
     { name = "Thorben Westerhuys", email = "thorben.westerhuys@luucy.ch" },
 ]
 dependencies = [
     "requests>=2.31.0",
 ]
```

### Comparing `luucy_python-0.3.0/src/luucy/core.py` & `luucy_python-0.4.0/src/luucy/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 from typing import Optional
 import os
+import json
 import requests
 
 
 class LUUCY:
     """A high level object to initiate a client.
 
     Parameters:
         username: LUUCY username.
         password: LUCUY password.
 
     Raises:
         ValueError: When no `username` and `password` are supplied
     """
 
-    def __init__(self, username: Optional[str] = None, password: Optional[str] = None):
+    def __init__(
+        self,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        base_url: str = "app.luucy.ch",
+    ):
         self._username = username
         self._password = password
+        self._base_url = base_url
         self._user_id = None
 
         if os.environ.get("LUUCY_USERNAME", None) and os.environ.get(
             "LUUCY_PASSWORD", None
         ):
             self._username = os.environ["LUUCY_USERNAME"]
             self._password = os.environ["LUUCY_PASSWORD"]
 
         if self._username and self._password:
             account = requests.post(
-                url="https://www.luucy.ch/api/login",
-                data={"username": self._username, "password": self._password},
+                url=f"https://{self._base_url}/api/login",
+                headers={
+                    "Content-Type": "application/json; charset=utf-8",
+                },
+                data=json.dumps(
+                    {
+                        "login": self._username,
+                        "password": self._password,
+                        "rememberMe": True,
+                    }
+                ),
                 timeout=300,
             )
             if account.status_code == 200:
                 self._user_id = account.json()["person"]["id"]
                 self._api_token = account.json()["apiKey"]
 
             return None
```

### Comparing `luucy_python-0.3.0/tests/conftest.py` & `luucy_python-0.4.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
     def json(self):
         return self.json_data
 
 
 @pytest.fixture
 def mock_login_request(monkeypatch):
-    def mock_login_request_func(*args, **kwargs):
+    def mock_login_request_func(url, *args, **kwargs):
+        monkeypatch.setenv("REQUEST_URL", url)
+
         return MockResponse(
             {
                 "apiKey": "18b8c9a1234599b5043e654321e0c870956aga09",
                 "person": {
                     "id": 1234,
                     "name": "Luucy",
                     "surname": "Tester",
```

### Comparing `luucy_python-0.3.0/tests/features/login/init.feature` & `luucy_python-0.4.0/tests/features/login/init.feature`

 * *Files 18% similar despite different names*

```diff
@@ -20,7 +20,19 @@
     Then it loads successfully
 
   Scenario: Returns user data
 
     Given the client is logged in
     When user_data is called
     Then user data of logged in user is returned
+
+  Scenario: Can be used with different environments
+
+    Given the baseUrl is set to staging
+    When initiating the client
+    Then staging is used
+
+  Scenario: Can be used with production environment
+
+    Given the baseUrl is set not set
+    When initiating the client
+    Then production is used
```

### Comparing `luucy_python-0.3.0/tests/test_init_with_username_and_password.py` & `luucy_python-0.4.0/tests/test_init_with_username_and_password.py`

 * *Files identical despite different names*

### Comparing `luucy_python-0.3.0/tests/test_init_without_username_and_password copy.py` & `luucy_python-0.4.0/tests/test_init_without_username_and_password copy.py`

 * *Files identical despite different names*

### Comparing `luucy_python-0.3.0/tests/test_initi_with_env_username_and_password.py` & `luucy_python-0.4.0/tests/test_initi_with_env_username_and_password.py`

 * *Files identical despite different names*

