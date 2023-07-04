# Comparing `tmp/azure_recommendations-0.3.3.tar.gz` & `tmp/azure_recommendations-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_recommendations-0.3.3.tar", last modified: Sat May 13 15:13:50 2023, max compression
+gzip compressed data, was "azure_recommendations-0.3.4.tar", last modified: Tue Jul  4 13:15:52 2023, max compression
```

## Comparing `azure_recommendations-0.3.3.tar` & `azure_recommendations-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 15:13:50.821438 azure_recommendations-0.3.3/
--rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.3/LICENCE
--rw-rw-rw-   0        0        0      533 2023-05-13 15:13:50.819440 azure_recommendations-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 15:13:50.724440 azure_recommendations-0.3.3/azure_recommendations/
--rw-rw-rw-   0        0        0      602 2023-05-13 15:13:20.000000 azure_recommendations-0.3.3/azure_recommendations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:13:50.815438 azure_recommendations-0.3.3/azure_recommendations/recommendation/
--rw-rw-rw-   0        0        0     7333 2023-05-13 15:13:20.000000 azure_recommendations-0.3.3/azure_recommendations/recommendation/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.3/azure_recommendations/recommendation/advisor_recommendations.py
--rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.3/azure_recommendations/recommendation/network_recommendations.py
--rw-rw-rw-   0        0        0    10152 2023-05-13 14:55:05.000000 azure_recommendations-0.3.3/azure_recommendations/recommendation/utils.py
--rw-rw-rw-   0        0        0    21178 2023-05-13 14:50:12.000000 azure_recommendations-0.3.3/azure_recommendations/recommendation/vm_recommendations.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:13:50.739439 azure_recommendations-0.3.3/azure_recommendations.egg-info/
--rw-rw-rw-   0        0        0      533 2023-05-13 15:13:50.000000 azure_recommendations-0.3.3/azure_recommendations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-05-13 15:13:50.000000 azure_recommendations-0.3.3/azure_recommendations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 15:13:50.000000 azure_recommendations-0.3.3/azure_recommendations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-05-13 15:13:50.000000 azure_recommendations-0.3.3/azure_recommendations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-13 15:13:50.000000 azure_recommendations-0.3.3/azure_recommendations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2023-05-13 15:13:20.000000 azure_recommendations-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 15:13:50.821438 azure_recommendations-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.880880 azure_recommendations-0.3.4/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.4/LICENCE
+-rw-rw-rw-   0        0        0      533 2023-07-04 13:15:52.879902 azure_recommendations-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.749052 azure_recommendations-0.3.4/azure_recommendations/
+-rw-rw-rw-   0        0        0      602 2023-07-04 13:12:54.000000 azure_recommendations-0.3.4/azure_recommendations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.875022 azure_recommendations-0.3.4/azure_recommendations/recommendation/
+-rw-rw-rw-   0        0        0     7333 2023-05-13 15:13:20.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/advisor_recommendations.py
+-rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/network_recommendations.py
+-rw-rw-rw-   0        0        0    10152 2023-05-13 14:55:05.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/utils.py
+-rw-rw-rw-   0        0        0    21578 2023-07-04 13:12:54.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/vm_recommendations.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.771517 azure_recommendations-0.3.4/azure_recommendations.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-07-04 13:12:54.000000 azure_recommendations-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 13:15:52.881856 azure_recommendations-0.3.4/setup.cfg
```

### Comparing `azure_recommendations-0.3.3/PKG-INFO` & `azure_recommendations-0.3.4/azure_recommendations.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: azure_recommendations
-Version: 0.3.3
+Name: azure-recommendations
+Version: 0.3.4
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.3/azure_recommendations/__init__.py` & `azure_recommendations-0.3.4/azure_recommendations/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from azure_recommendations.recommendation import recommendation
 
 import logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 
 class az_session(recommendation):
     def __init__(self, tenant_id: str, client_id: str, client_secret: str):
         """
         :param tenant_id: tenant Id from Azure
         :param client_id: Access ID
```

### Comparing `azure_recommendations-0.3.3/azure_recommendations/recommendation/__init__.py` & `azure_recommendations-0.3.4/azure_recommendations/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.3/azure_recommendations/recommendation/advisor_recommendations.py` & `azure_recommendations-0.3.4/azure_recommendations/recommendation/advisor_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.3/azure_recommendations/recommendation/network_recommendations.py` & `azure_recommendations-0.3.4/azure_recommendations/recommendation/network_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.3/azure_recommendations/recommendation/utils.py` & `azure_recommendations-0.3.4/azure_recommendations/recommendation/utils.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.3/azure_recommendations/recommendation/vm_recommendations.py` & `azure_recommendations-0.3.4/azure_recommendations/recommendation/vm_recommendations.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,14 +400,25 @@
 
                 response = requests.request("GET", url, headers=headers, data=payload)
 
                 data = json.loads(response.text)
                 # print(json.dumps(data, indent=2))
                 # print(rg)
                 # print(json.dumps(data))
+
+                try:
+                    temp = data['value']
+                except KeyError:
+                    try:
+                        response = requests.request("GET", url, headers=headers, data=payload)
+                        data = json.loads(response.text)
+                        temp = data['value']
+                    except KeyError:
+                        continue
+
                 for item in data['value']:
                     lookback_period = item['properties']['lookBackPeriod']
 
                     current_cost = item['properties']['costWithNoReservedInstances']
 
                     effective_cost = item['properties']['totalCostWithReservedInstances']
```

### Comparing `azure_recommendations-0.3.3/azure_recommendations.egg-info/PKG-INFO` & `azure_recommendations-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: azure-recommendations
-Version: 0.3.3
+Name: azure_recommendations
+Version: 0.3.4
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.3/azure_recommendations.egg-info/SOURCES.txt` & `azure_recommendations-0.3.4/azure_recommendations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.3/pyproject.toml` & `azure_recommendations-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "azure_recommendations"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
 ]
 description = "Provides Azure recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

