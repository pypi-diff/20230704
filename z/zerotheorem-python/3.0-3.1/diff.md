# Comparing `tmp/zerotheorem-python-3.0.tar.gz` & `tmp/zerotheorem-python-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerotheorem-python-3.0.tar", last modified: Tue Jul  4 13:45:59 2023, max compression
+gzip compressed data, was "zerotheorem-python-3.1.tar", last modified: Tue Jul  4 14:14:44 2023, max compression
```

## Comparing `zerotheorem-python-3.0.tar` & `zerotheorem-python-3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        0 2023-07-04 13:45:59.591704 zerotheorem-python-3.0/
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)     1052 2023-03-29 08:13:06.000000 zerotheorem-python-3.0/LICENSE.txt
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      396 2023-07-04 13:45:59.591704 zerotheorem-python-3.0/PKG-INFO
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      105 2023-07-04 11:07:42.000000 zerotheorem-python-3.0/README.md
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)       38 2023-07-04 13:45:59.591704 zerotheorem-python-3.0/setup.cfg
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      373 2023-07-04 13:45:03.000000 zerotheorem-python-3.0/setup.py
-drwxrwxr-x   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        0 2023-07-04 13:45:59.591704 zerotheorem-python-3.0/zerotheorem/
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)     2544 2023-07-04 12:56:55.000000 zerotheorem-python-3.0/zerotheorem/__init__.py
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      186 2023-07-04 12:33:09.000000 zerotheorem-python-3.0/zerotheorem/test.py
-drwxrwxr-x   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        0 2023-07-04 13:45:59.591704 zerotheorem-python-3.0/zerotheorem_python.egg-info/
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      396 2023-07-04 13:45:59.000000 zerotheorem-python-3.0/zerotheorem_python.egg-info/PKG-INFO
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      242 2023-07-04 13:45:59.000000 zerotheorem-python-3.0/zerotheorem_python.egg-info/SOURCES.txt
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        1 2023-07-04 13:45:59.000000 zerotheorem-python-3.0/zerotheorem_python.egg-info/dependency_links.txt
--rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)       12 2023-07-04 13:45:59.000000 zerotheorem-python-3.0/zerotheorem_python.egg-info/top_level.txt
+drwxrwxr-x   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        0 2023-07-04 14:14:44.631666 zerotheorem-python-3.1/
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)     1052 2023-03-29 08:13:06.000000 zerotheorem-python-3.1/LICENSE.txt
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      396 2023-07-04 14:14:44.631666 zerotheorem-python-3.1/PKG-INFO
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      105 2023-07-04 11:07:42.000000 zerotheorem-python-3.1/README.md
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)       38 2023-07-04 14:14:44.631666 zerotheorem-python-3.1/setup.cfg
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      373 2023-07-04 14:14:30.000000 zerotheorem-python-3.1/setup.py
+drwxrwxr-x   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        0 2023-07-04 14:14:44.631666 zerotheorem-python-3.1/zerotheorem/
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)     2544 2023-07-04 14:13:46.000000 zerotheorem-python-3.1/zerotheorem/__init__.py
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      186 2023-07-04 14:12:16.000000 zerotheorem-python-3.1/zerotheorem/test.py
+drwxrwxr-x   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        0 2023-07-04 14:14:44.631666 zerotheorem-python-3.1/zerotheorem_python.egg-info/
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      396 2023-07-04 14:14:44.000000 zerotheorem-python-3.1/zerotheorem_python.egg-info/PKG-INFO
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)      242 2023-07-04 14:14:44.000000 zerotheorem-python-3.1/zerotheorem_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)        1 2023-07-04 14:14:44.000000 zerotheorem-python-3.1/zerotheorem_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahmood-yousaf  (1000) mahmood-yousaf  (1000)       12 2023-07-04 14:14:44.000000 zerotheorem-python-3.1/zerotheorem_python.egg-info/top_level.txt
```

### Comparing `zerotheorem-python-3.0/LICENSE.txt` & `zerotheorem-python-3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerotheorem-python-3.0/zerotheorem/__init__.py` & `zerotheorem-python-3.1/zerotheorem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 #     global key
 #     endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get_stats"
 #     headers = {"Authorization": "Bearer " + key}
 #     return requests.get(endpoint, headers=headers).json()
 def get_stats(model_name=""):
     global key
     if model_name == "":
+        endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get_stats"
+        headers = {"Authorization": "Bearer " + key}
+        return requests.get(endpoint, headers=headers).json()
+    else:
         if len(model_name.split("_")) == 3:
             endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get/live_stats/" + model_name
             headers = {"Authorization": "Bearer " + key}
             return requests.get(endpoint, headers=headers).json()
         else:
-            endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get_stats"
+            endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get_stats/" + model_name
             headers = {"Authorization": "Bearer " + key}
-            return requests.get(endpoint, headers=headers).json()     
-    else:
-        endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get_stat/"+model_name
-        headers = {"Authorization": "Bearer " + key}
-        return requests.get(endpoint, headers=headers).json()
+            return requests.get(endpoint, headers=headers).json()  
 
 def get_forecast(model_name=""):
     global key
     if model_name == "":
         endpoint = "https://zt-rest-api-rmkp2vbpqq-uc.a.run.app/get_strategies"
         headers = {"Authorization": "Bearer " + key}
         return requests.get(endpoint, headers=headers).json()
```

