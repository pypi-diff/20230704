# Comparing `tmp/rosetta-ce-1.5.0.tar.gz` & `tmp/rosetta-ce-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.5.0.tar", last modified: Mon Jul  3 13:20:01 2023, max compression
+gzip compressed data, was "rosetta-ce-1.5.1.tar", last modified: Tue Jul  4 04:18:41 2023, max compression
```

## Comparing `rosetta-ce-1.5.0.tar` & `rosetta-ce-1.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.854515 rosetta-ce-1.5.0/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.0/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 13:20:01.854013 rosetta-ce-1.5.0/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.0/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.848455 rosetta-ce-1.5.0/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.0/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.850162 rosetta-ce-1.5.0/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.0/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.0/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.0/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.5.0/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.0/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44278 2023-07-03 10:43:19.000000 rosetta-ce-1.5.0/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    10384 2023-07-03 13:19:23.000000 rosetta-ce-1.5.0/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.852131 rosetta-ce-1.5.0/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-03 13:20:01.000000 rosetta-ce-1.5.0/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-03 13:20:01.854565 rosetta-ce-1.5.0/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-03 13:19:23.000000 rosetta-ce-1.5.0/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 13:20:01.853595 rosetta-ce-1.5.0/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.0/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.0/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.0/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:18:41.758816 rosetta-ce-1.5.1/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.1/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 04:18:41.758434 rosetta-ce-1.5.1/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.1/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:18:41.751582 rosetta-ce-1.5.1/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.1/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:18:41.753392 rosetta-ce-1.5.1/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.1/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.1/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.1/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.5.1/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.1/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44278 2023-07-03 10:43:19.000000 rosetta-ce-1.5.1/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10385 2023-07-04 04:18:19.000000 rosetta-ce-1.5.1/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:18:41.755347 rosetta-ce-1.5.1/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 04:18:41.000000 rosetta-ce-1.5.1/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-04 04:18:41.000000 rosetta-ce-1.5.1/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-04 04:18:41.000000 rosetta-ce-1.5.1/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-04 04:18:41.000000 rosetta-ce-1.5.1/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-04 04:18:41.000000 rosetta-ce-1.5.1/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-04 04:18:41.758860 rosetta-ce-1.5.1/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-04 04:18:32.000000 rosetta-ce-1.5.1/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:18:41.757877 rosetta-ce-1.5.1/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.1/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.1/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.1/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.5.0/LICENSE` & `rosetta-ce-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/PKG-INFO` & `rosetta-ce-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.0
+Version: 1.5.1
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.0/README.md` & `rosetta-ce-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/rosetta/constants/sensors.py` & `rosetta-ce-1.5.1/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/rosetta/constants/sources.py` & `rosetta-ce-1.5.1/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/rosetta/constants/systems.py` & `rosetta-ce-1.5.1/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/rosetta/rconverter.py` & `rosetta-ce-1.5.1/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/rosetta/rfaker.py` & `rosetta-ce-1.5.1/rosetta/rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/rosetta/rsender.py` & `rosetta-ce-1.5.1/rosetta/rsender.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def __init__(self, data_type: str, destination: str, headers: Optional[dict] = None,
                  worker_name: Optional[str] = 'worker_'+str(datetime.now()), count: Optional[int] = 1,
                  interval: Optional[int] = 1, vendor: Optional[str] = None, product: Optional[str] = None,
                  version: Optional[str] = None, required_fields: Optional[str] = None,
                  observables: Optional[Observables] = None, fields: Optional[str] = None,
                  verify_ssl: Optional[bool] = None, datetime_obj: Optional[datetime] = None,
-                 data_json: Optional[dict] = None, data_text: Optional[str] = None):
+                 data_json: Optional[list] = None, data_text: Optional[list] = None):
         """
         Constructor for DataSenderWorker class.
 
         :param data_type: A value from the WorkerTypeEnum indicating the type of data to send. Options include:
             - SYSLOG
             - CEF
             - LEEF
```

### Comparing `rosetta-ce-1.5.0/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.5.1/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.0
+Version: 1.5.1
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.0/setup.py` & `rosetta-ce-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.5.0",
+    version="1.5.1",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.5.0/tests/test_rconverter.py` & `rosetta-ce-1.5.1/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/tests/test_rfaker.py` & `rosetta-ce-1.5.1/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.0/tests/test_rsender.py` & `rosetta-ce-1.5.1/tests/test_rsender.py`

 * *Files identical despite different names*

