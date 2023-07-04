# Comparing `tmp/tier_sdk-0.1.0.tar.gz` & `tmp/tier_sdk-0.1.1.tar.gz`

## Comparing `tier_sdk-0.1.0.tar` & `tier_sdk-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.DS_Store
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.editorconfig
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.gitattributes
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/tier-python-sdk.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/tier/.DS_Store
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/tier/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/tier/py.typed
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/tier/tier.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/tier/types.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/README.md
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 tier_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/py.typed
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/tier.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/types.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/PKG-INFO
```

### Comparing `tier_sdk-0.1.0/tier/tier.py` & `tier_sdk-0.1.1/tier/tier.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,17 +50,17 @@
             response = requests.post(
                 self.base_uri + url, json=params, headers=self.headers
             )
         else:
             raise RuntimeError("Invalid request method provided")
 
         if response.status_code == 401:
-            raise UnauthorizedException(response.json().get("error"))
+            raise UnauthorizedException()
         if response.status_code == 404:
-            raise NotFoundException(response.json().get("error"))
+            raise NotFoundException(response.json().get("title"))
         if response.status_code >= 400:
             raise TIERException(response.json().get("error") or "Unknown error")
         return response.json()
 
 
 class Vehicles:
     def __init__(self, client: TIER):
```

### Comparing `tier_sdk-0.1.0/LICENSE.md` & `tier_sdk-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tier_sdk-0.1.0/README.md` & `tier_sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tier_sdk-0.1.0/pyproject.toml` & `tier_sdk-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tier_sdk-0.1.0/PKG-INFO` & `tier_sdk-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tier-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: TIER Python SDK
 Project-URL: Source Code, https://github.com/owenvoke/tier-python-sdk
 Project-URL: Issues, https://github.com/owenvoke/tier-python-sdk/issues
 Author-email: Owen Voke <development@voke.dev>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: sdk,tier
```

