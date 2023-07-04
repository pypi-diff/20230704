# Comparing `tmp/simpler_py-1.0.0.tar.gz` & `tmp/simpler_py-1.0.1.tar.gz`

## Comparing `simpler_py-1.0.0.tar` & `simpler_py-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpler_py-1.0.0/src/simpler_py/__init__.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 simpler_py-1.0.0/src/simpler_py/simpler.py
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 simpler_py-1.0.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 simpler_py-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 simpler_py-1.0.0/README.md
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 simpler_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 simpler_py-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 simpler_py-1.0.1/Publish.bat
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 simpler_py-1.0.1/src/simpler_py/__init__.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 simpler_py-1.0.1/src/simpler_py/simpler.py
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 simpler_py-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 simpler_py-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 simpler_py-1.0.1/README.md
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 simpler_py-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 simpler_py-1.0.1/PKG-INFO
```

### Comparing `simpler_py-1.0.0/src/simpler_py/simpler.py` & `simpler_py-1.0.1/src/simpler_py/simpler.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,24 +53,29 @@
         response = self._session.request(method, self._server + self._endpoints[endpoint], json = data)
       self._setLastMessage(response)
       if response.status_code == 200:
         self._setLastResult(response)
         succeeded = True
     else:
       print('Endpoint not found: ' + endpoint)
+      for key in self._endpoints:
+        print(key)
 
     return succeeded
 
   @property
   def lastContent(self):
     return self._lastContent
 
   @property
   def lastMessage(self):
-    return self._lastMessage
+    if self._lastMessage != None:
+      return self._lastMessage
+    else:
+      return ''
 
   @property
   def lastResult(self):
     return self._lastResult
 
   def post(self, endpoint, data = None):
     return self._invoke('POST', endpoint, data)
```

### Comparing `simpler_py-1.0.0/.gitignore` & `simpler_py-1.0.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -361,8 +361,8 @@
 
 # Fody - auto-generated XML schema
 FodyWeavers.xsd
 
 # Custom
 Simpler.sln
 Test/
-Simpler/Properties/launchSettings.json
+launchSettings.json
```

### Comparing `simpler_py-1.0.0/LICENSE.txt` & `simpler_py-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

