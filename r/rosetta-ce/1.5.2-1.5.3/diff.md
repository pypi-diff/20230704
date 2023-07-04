# Comparing `tmp/rosetta-ce-1.5.2.tar.gz` & `tmp/rosetta-ce-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.5.2.tar", last modified: Tue Jul  4 04:46:04 2023, max compression
+gzip compressed data, was "rosetta-ce-1.5.3.tar", last modified: Tue Jul  4 05:00:22 2023, max compression
```

## Comparing `rosetta-ce-1.5.2.tar` & `rosetta-ce-1.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:46:04.223094 rosetta-ce-1.5.2/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.2/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 04:46:04.222655 rosetta-ce-1.5.2/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.2/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:46:04.215146 rosetta-ce-1.5.2/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.2/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:46:04.216688 rosetta-ce-1.5.2/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.2/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.2/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.2/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.5.2/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.2/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44278 2023-07-03 10:43:19.000000 rosetta-ce-1.5.2/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    10384 2023-07-04 04:45:51.000000 rosetta-ce-1.5.2/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:46:04.218751 rosetta-ce-1.5.2/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 04:46:04.000000 rosetta-ce-1.5.2/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-04 04:46:04.000000 rosetta-ce-1.5.2/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-04 04:46:04.000000 rosetta-ce-1.5.2/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-04 04:46:04.000000 rosetta-ce-1.5.2/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-04 04:46:04.000000 rosetta-ce-1.5.2/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-04 04:46:04.223138 rosetta-ce-1.5.2/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-04 04:45:59.000000 rosetta-ce-1.5.2/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 04:46:04.221333 rosetta-ce-1.5.2/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.2/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.2/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.2/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 05:00:22.462396 rosetta-ce-1.5.3/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.3/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 05:00:22.462078 rosetta-ce-1.5.3/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.3/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 05:00:22.456077 rosetta-ce-1.5.3/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.3/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 05:00:22.458064 rosetta-ce-1.5.3/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.3/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.3/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.3/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.5.3/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.3/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44278 2023-07-03 10:43:19.000000 rosetta-ce-1.5.3/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10463 2023-07-04 04:58:55.000000 rosetta-ce-1.5.3/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 05:00:22.460136 rosetta-ce-1.5.3/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 05:00:22.000000 rosetta-ce-1.5.3/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-04 05:00:22.000000 rosetta-ce-1.5.3/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-04 05:00:22.000000 rosetta-ce-1.5.3/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-04 05:00:22.000000 rosetta-ce-1.5.3/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-04 05:00:22.000000 rosetta-ce-1.5.3/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-04 05:00:22.462440 rosetta-ce-1.5.3/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-04 05:00:17.000000 rosetta-ce-1.5.3/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 05:00:22.461557 rosetta-ce-1.5.3/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.3/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.3/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.3/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.5.2/LICENSE` & `rosetta-ce-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/PKG-INFO` & `rosetta-ce-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.2
+Version: 1.5.3
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.2/README.md` & `rosetta-ce-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/rosetta/constants/sensors.py` & `rosetta-ce-1.5.3/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/rosetta/constants/sources.py` & `rosetta-ce-1.5.3/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/rosetta/constants/systems.py` & `rosetta-ce-1.5.3/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/rosetta/rconverter.py` & `rosetta-ce-1.5.3/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/rosetta/rfaker.py` & `rosetta-ce-1.5.3/rosetta/rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/rosetta/rsender.py` & `rosetta-ce-1.5.3/rosetta/rsender.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         self.vendor = vendor
         self.product = product
         self.version = version
         self.required_fields = required_fields
         self.destination = destination
         self.created_at = datetime.now()
         self.status = "Stopped"
+        self.response = None
         self.observables = observables
         self.fields = fields
         self.verify_ssl = verify_ssl
         self.datetime_obj = datetime_obj
         self.data_json = data_json
         self.data_text = data_text
 
@@ -200,14 +201,15 @@
                         url = 'http://' + self.destination
                     else:
                         url = self.destination
                     warnings.filterwarnings("ignore", category=InsecureRequestWarning)
                     print(f"Worker: {self.worker_name} sending log message to {url} ")
                     response = requests.post(url, json=fake_message[0], timeout=(2, 5), headers=self.headers,
                                              verify=self.verify_ssl)
+                    self.response = response.text
                     response.raise_for_status()
             except (ConnectionRefusedError, socket.timeout, requests.exceptions.RequestException) as e:
                 print(f"Connection error: {e}")
                 self.status = "Connection Error"
                 break
             except requests.exceptions.SSLError as e:
                 print(f"SSL error: {e}")
```

### Comparing `rosetta-ce-1.5.2/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.5.3/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.2
+Version: 1.5.3
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.2/setup.py` & `rosetta-ce-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.5.2",
+    version="1.5.3",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.5.2/tests/test_rconverter.py` & `rosetta-ce-1.5.3/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/tests/test_rfaker.py` & `rosetta-ce-1.5.3/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.2/tests/test_rsender.py` & `rosetta-ce-1.5.3/tests/test_rsender.py`

 * *Files identical despite different names*

