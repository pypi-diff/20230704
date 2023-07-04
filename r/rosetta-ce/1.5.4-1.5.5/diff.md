# Comparing `tmp/rosetta-ce-1.5.4.tar.gz` & `tmp/rosetta-ce-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.5.4.tar", last modified: Tue Jul  4 08:14:58 2023, max compression
+gzip compressed data, was "rosetta-ce-1.5.5.tar", last modified: Tue Jul  4 08:30:00 2023, max compression
```

## Comparing `rosetta-ce-1.5.4.tar` & `rosetta-ce-1.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:14:58.844084 rosetta-ce-1.5.4/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.4/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 08:14:58.843548 rosetta-ce-1.5.4/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.4/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:14:58.837193 rosetta-ce-1.5.4/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.4/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:14:58.839546 rosetta-ce-1.5.4/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.4/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)      269 2023-07-04 08:04:58.000000 rosetta-ce-1.5.4/rosetta/constants/attributes.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.4/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.4/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6478 2023-07-04 08:03:50.000000 rosetta-ce-1.5.4/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.4/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44324 2023-07-04 08:14:22.000000 rosetta-ce-1.5.4/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    10463 2023-07-04 04:58:55.000000 rosetta-ce-1.5.4/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:14:58.841539 rosetta-ce-1.5.4/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 08:14:58.000000 rosetta-ce-1.5.4/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      491 2023-07-04 08:14:58.000000 rosetta-ce-1.5.4/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-04 08:14:58.000000 rosetta-ce-1.5.4/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-04 08:14:58.000000 rosetta-ce-1.5.4/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-04 08:14:58.000000 rosetta-ce-1.5.4/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-04 08:14:58.844134 rosetta-ce-1.5.4/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-04 08:14:29.000000 rosetta-ce-1.5.4/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:14:58.843013 rosetta-ce-1.5.4/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.4/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.4/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.4/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.910155 rosetta-ce-1.5.5/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.5/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 08:30:00.909845 rosetta-ce-1.5.5/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.5/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.905484 rosetta-ce-1.5.5/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.5/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.907241 rosetta-ce-1.5.5/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.5/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)      269 2023-07-04 08:04:58.000000 rosetta-ce-1.5.5/rosetta/constants/attributes.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.5/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.5/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6478 2023-07-04 08:03:50.000000 rosetta-ce-1.5.5/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.5/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44325 2023-07-04 08:28:39.000000 rosetta-ce-1.5.5/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10463 2023-07-04 04:58:55.000000 rosetta-ce-1.5.5/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.908522 rosetta-ce-1.5.5/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      491 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-04 08:30:00.910222 rosetta-ce-1.5.5/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-04 08:29:04.000000 rosetta-ce-1.5.5/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.909438 rosetta-ce-1.5.5/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.5/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.5/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.5/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.5.4/LICENSE` & `rosetta-ce-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/PKG-INFO` & `rosetta-ce-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.4
+Version: 1.5.5
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.4/README.md` & `rosetta-ce-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/rosetta/constants/sensors.py` & `rosetta-ce-1.5.5/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/rosetta/constants/sources.py` & `rosetta-ce-1.5.5/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/rosetta/constants/systems.py` & `rosetta-ce-1.5.5/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/rosetta/rconverter.py` & `rosetta-ce-1.5.5/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/rosetta/rfaker.py` & `rosetta-ce-1.5.5/rosetta/rfaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
             field_value = random.choice(observables.unix_process) if observables and observables.unix_process \
                 else "sudo"
         if field == "unix_cmd":
             field_value = random.choice(observables.unix_cmd) if observables and observables.unix_cmd \
                 else random.choice(UNIX_CMD)
         if field == "severity":
             field_value = random.choice(observables.severity) if observables and observables.severity \
-                else faker.choice(SEVERITIES)
+                else random.choice(SEVERITIES)
         if field == "local_ip":
             field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
                     else faker.ipv4()
         if field == "local_port":
             field_value = faker.random_int(min=1024, max=65535)
         if field == "remote_ip":
             field_value = random.choice(observables.remote_ip) if observables and observables.remote_ip \
```

### Comparing `rosetta-ce-1.5.4/rosetta/rsender.py` & `rosetta-ce-1.5.5/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.5.5/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.4
+Version: 1.5.5
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.4/setup.py` & `rosetta-ce-1.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.5.4",
+    version="1.5.5",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.5.4/tests/test_rconverter.py` & `rosetta-ce-1.5.5/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/tests/test_rfaker.py` & `rosetta-ce-1.5.5/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.4/tests/test_rsender.py` & `rosetta-ce-1.5.5/tests/test_rsender.py`

 * *Files identical despite different names*

