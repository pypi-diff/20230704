# Comparing `tmp/shieldcloudapi-0.1.4.tar.gz` & `tmp/shieldcloudapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shieldcloudapi-0.1.4.tar", last modified: Fri Apr 14 01:49:48 2023, max compression
+gzip compressed data, was "shieldcloudapi-0.1.5.tar", last modified: Tue Jul  4 13:37:32 2023, max compression
```

## Comparing `shieldcloudapi-0.1.4.tar` & `shieldcloudapi-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-04-14 01:49:48.437787 shieldcloudapi-0.1.4/
--rw-r--r--   0 root         (0) wheel        (0)    11357 2022-09-23 00:22:05.000000 shieldcloudapi-0.1.4/LICENSE
--rw-r--r--   0 root         (0) wheel        (0)    13856 2023-04-14 01:49:48.437598 shieldcloudapi-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      319 2022-10-06 06:39:17.000000 shieldcloudapi-0.1.4/README.md
--rw-r--r--   0 root         (0) wheel        (0)      643 2023-04-14 01:48:00.000000 shieldcloudapi-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) wheel        (0)       38 2023-04-14 01:49:48.437831 shieldcloudapi-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) wheel        (0)      339 2023-03-21 03:40:14.000000 shieldcloudapi-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-04-14 01:49:48.436813 shieldcloudapi-0.1.4/shieldcloudapi/
--rw-r--r--   0 root         (0) wheel        (0)        0 2022-09-23 00:25:48.000000 shieldcloudapi-0.1.4/shieldcloudapi/__init__.py
--rw-r--r--   0 root         (0) wheel        (0)    20502 2023-04-14 01:47:28.000000 shieldcloudapi-0.1.4/shieldcloudapi/shieldcloudapi.py
-drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-04-14 01:49:48.437405 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/
--rw-r--r--   0 root         (0) wheel        (0)    13856 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) wheel        (0)      253 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) wheel        (0)        1 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) wheel        (0)       15 2023-04-14 01:49:48.000000 shieldcloudapi-0.1.4/shieldcloudapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-07-04 13:37:32.892731 shieldcloudapi-0.1.5/
+-rw-r--r--   0 root         (0) wheel        (0)    11357 2023-07-04 06:49:55.000000 shieldcloudapi-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) wheel        (0)    13856 2023-07-04 13:37:32.892518 shieldcloudapi-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      319 2023-07-04 06:49:55.000000 shieldcloudapi-0.1.5/README.md
+-rw-r--r--   0 root         (0) wheel        (0)      643 2023-07-04 13:33:59.000000 shieldcloudapi-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) wheel        (0)       38 2023-07-04 13:37:32.892777 shieldcloudapi-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) wheel        (0)      339 2023-07-04 06:49:55.000000 shieldcloudapi-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-07-04 13:37:32.891555 shieldcloudapi-0.1.5/shieldcloudapi/
+-rw-r--r--   0 root         (0) wheel        (0)        0 2023-07-04 06:49:55.000000 shieldcloudapi-0.1.5/shieldcloudapi/__init__.py
+-rw-r--r--   0 root         (0) wheel        (0)    20636 2023-07-04 07:11:45.000000 shieldcloudapi-0.1.5/shieldcloudapi/shieldcloudapi.py
+drwxr-xr-x   0 root         (0) wheel        (0)        0 2023-07-04 13:37:32.892298 shieldcloudapi-0.1.5/shieldcloudapi.egg-info/
+-rw-r--r--   0 root         (0) wheel        (0)    13856 2023-07-04 13:37:32.000000 shieldcloudapi-0.1.5/shieldcloudapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) wheel        (0)      253 2023-07-04 13:37:32.000000 shieldcloudapi-0.1.5/shieldcloudapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) wheel        (0)        1 2023-07-04 13:37:32.000000 shieldcloudapi-0.1.5/shieldcloudapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) wheel        (0)       15 2023-07-04 13:37:32.000000 shieldcloudapi-0.1.5/shieldcloudapi.egg-info/top_level.txt
```

### Comparing `shieldcloudapi-0.1.4/LICENSE` & `shieldcloudapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shieldcloudapi-0.1.4/PKG-INFO` & `shieldcloudapi-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shieldcloudapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Intrusion Inc Shield Cloud API package
 Author: John Edwards
 Author-email: John Edwards <john.edwards@intrusion.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `shieldcloudapi-0.1.4/pyproject.toml` & `shieldcloudapi-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shieldcloudapi"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="John Edwards", email="john.edwards@intrusion.com" },
 ]
 description = "Intrusion Inc Shield Cloud API package"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `shieldcloudapi-0.1.4/shieldcloudapi/shieldcloudapi.py` & `shieldcloudapi-0.1.5/shieldcloudapi/shieldcloudapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,26 +484,32 @@
     # print(q.to_text())
 
     # print("DNS: " + dns_server)
 
     maxretries = 3 # change to session variable
     retries = 0
     answer = False
-    
+    timeout = 3 # change to session variable
+
+
 
     while retries < maxretries and not answer:
         retries = retries + 1
         # run the query
         # implement timeout here later
 
         # change the server according to the load balance algo before each run
 
         # set a timer here
         try:
-            (r, tcp) = dns.query.udp_with_fallback(q, dns_server)
+            (r, tcp) = dns.query.udp_with_fallback(
+                    q, 
+                    dns_server,
+                    timeout
+                    )
             if not r.answer:
                 print("No answer from {} to attempt {}".format(dns_server,retries))
                 print("Query: {}".format(q))
 
                 print("Session: {}".format(session))
             else:
                 answer = True
```

### Comparing `shieldcloudapi-0.1.4/shieldcloudapi.egg-info/PKG-INFO` & `shieldcloudapi-0.1.5/shieldcloudapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shieldcloudapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Intrusion Inc Shield Cloud API package
 Author: John Edwards
 Author-email: John Edwards <john.edwards@intrusion.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

