# Comparing `tmp/nlp_service-1.4.7.tar.gz` & `tmp/nlp_service-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.7.tar", max compression
+gzip compressed data, was "nlp_service-1.4.8.tar", max compression
```

## Comparing `nlp_service-1.4.7.tar` & `nlp_service-1.4.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-07-03 12:11:40.033243 nlp_service-1.4.7/LICENSE
--rw-r--r--   0        0        0     7887 2023-07-03 12:11:40.033243 nlp_service-1.4.7/README.md
--rw-r--r--   0        0        0      226 2023-07-03 12:11:40.033243 nlp_service-1.4.7/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-07-03 12:11:40.033243 nlp_service-1.4.7/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-07-03 12:11:40.033243 nlp_service-1.4.7/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-07-03 12:11:40.033243 nlp_service-1.4.7/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-07-03 12:11:40.033243 nlp_service-1.4.7/nlp_service/py.typed
--rw-r--r--   0        0        0    17139 2023-07-03 12:11:40.037243 nlp_service-1.4.7/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-07-03 12:11:40.037243 nlp_service-1.4.7/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-07-03 12:11:40.037243 nlp_service-1.4.7/nlp_service/typing.py
--rw-r--r--   0        0        0     1361 2023-07-03 12:12:57.201624 nlp_service-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     9517 1970-01-01 00:00:00.000000 nlp_service-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 08:58:58.874066 nlp_service-1.4.8/LICENSE
+-rw-r--r--   0        0        0     7887 2023-07-04 08:58:58.874066 nlp_service-1.4.8/README.md
+-rw-r--r--   0        0        0      226 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/py.typed
+-rw-r--r--   0        0        0    17139 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/typing.py
+-rw-r--r--   0        0        0     1361 2023-07-04 09:00:12.671492 nlp_service-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 nlp_service-1.4.8/setup.py
+-rw-r--r--   0        0        0     9517 1970-01-01 00:00:00.000000 nlp_service-1.4.8/PKG-INFO
```

### Comparing `nlp_service-1.4.7/LICENSE` & `nlp_service-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.7/README.md` & `nlp_service-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.7/nlp_service/client.py` & `nlp_service-1.4.8/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.7/nlp_service/infersent.py` & `nlp_service-1.4.8/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.7/nlp_service/server.py` & `nlp_service-1.4.8/nlp_service/server.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.7/nlp_service/similarity.py` & `nlp_service-1.4.8/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.7/pyproject.toml` & `nlp_service-1.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.7"
+version = "1.4.8"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
```

### Comparing `nlp_service-1.4.7/PKG-INFO` & `nlp_service-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.7
+Version: 1.4.8
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

