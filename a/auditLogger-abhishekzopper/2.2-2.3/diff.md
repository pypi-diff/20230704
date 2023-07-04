# Comparing `tmp/auditLogger-abhishekzopper-2.2.tar.gz` & `tmp/auditLogger-abhishekzopper-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auditLogger-abhishekzopper-2.2.tar", last modified: Tue Jul  4 13:07:49 2023, max compression
+gzip compressed data, was "auditLogger-abhishekzopper-2.3.tar", last modified: Tue Jul  4 13:10:09 2023, max compression
```

## Comparing `auditLogger-abhishekzopper-2.2.tar` & `auditLogger-abhishekzopper-2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:07:49.349249 auditLogger-abhishekzopper-2.2/
--rw-r--r--   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 07:21:25.000000 auditLogger-abhishekzopper-2.2/LICENSE
--rw-r--r--   0 abhishekratnam   (501) staff       (20)      424 2023-07-04 13:07:49.349314 auditLogger-abhishekzopper-2.2/PKG-INFO
--rw-r--r--   0 abhishekratnam   (501) staff       (20)       28 2023-07-04 07:26:57.000000 auditLogger-abhishekzopper-2.2/README.md
--rw-r--r--   0 abhishekratnam   (501) staff       (20)      232 2023-07-04 13:07:31.000000 auditLogger-abhishekzopper-2.2/pyproject.toml
--rw-r--r--   0 abhishekratnam   (501) staff       (20)      520 2023-07-04 13:07:49.349582 auditLogger-abhishekzopper-2.2/setup.cfg
-drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:07:49.346160 auditLogger-abhishekzopper-2.2/src/
-drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:07:49.348005 auditLogger-abhishekzopper-2.2/src/auditLogger/
--rw-r--r--   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 07:23:17.000000 auditLogger-abhishekzopper-2.2/src/auditLogger/__init__.py
--rw-r--r--   0 abhishekratnam   (501) staff       (20)     2844 2023-07-04 12:59:42.000000 auditLogger-abhishekzopper-2.2/src/auditLogger/custom_logging.py
--rw-r--r--   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 07:23:59.000000 auditLogger-abhishekzopper-2.2/src/auditLogger/main.py
--rw-r--r--   0 abhishekratnam   (501) staff       (20)     6942 2023-07-04 12:46:22.000000 auditLogger-abhishekzopper-2.2/src/auditLogger/req_resp_middleware.py
--rw-r--r--   0 abhishekratnam   (501) staff       (20)    10324 2023-07-04 08:51:48.000000 auditLogger-abhishekzopper-2.2/src/auditLogger/requests_logging.py
-drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:07:49.349103 auditLogger-abhishekzopper-2.2/src/auditLogger_abhishekzopper.egg-info/
--rw-r--r--   0 abhishekratnam   (501) staff       (20)      424 2023-07-04 13:07:49.000000 auditLogger-abhishekzopper-2.2/src/auditLogger_abhishekzopper.egg-info/PKG-INFO
--rw-r--r--   0 abhishekratnam   (501) staff       (20)      419 2023-07-04 13:07:49.000000 auditLogger-abhishekzopper-2.2/src/auditLogger_abhishekzopper.egg-info/SOURCES.txt
--rw-r--r--   0 abhishekratnam   (501) staff       (20)        1 2023-07-04 13:07:49.000000 auditLogger-abhishekzopper-2.2/src/auditLogger_abhishekzopper.egg-info/dependency_links.txt
--rw-r--r--   0 abhishekratnam   (501) staff       (20)       12 2023-07-04 13:07:49.000000 auditLogger-abhishekzopper-2.2/src/auditLogger_abhishekzopper.egg-info/top_level.txt
+drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:10:09.520447 auditLogger-abhishekzopper-2.3/
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 07:21:25.000000 auditLogger-abhishekzopper-2.3/LICENSE
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)      424 2023-07-04 13:10:09.520517 auditLogger-abhishekzopper-2.3/PKG-INFO
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)       28 2023-07-04 07:26:57.000000 auditLogger-abhishekzopper-2.3/README.md
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)      239 2023-07-04 13:09:34.000000 auditLogger-abhishekzopper-2.3/pyproject.toml
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)      520 2023-07-04 13:10:09.520792 auditLogger-abhishekzopper-2.3/setup.cfg
+drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:10:09.517358 auditLogger-abhishekzopper-2.3/src/
+drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:10:09.519168 auditLogger-abhishekzopper-2.3/src/auditLogger/
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 07:23:17.000000 auditLogger-abhishekzopper-2.3/src/auditLogger/__init__.py
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)     2844 2023-07-04 12:59:42.000000 auditLogger-abhishekzopper-2.3/src/auditLogger/custom_logging.py
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 07:23:59.000000 auditLogger-abhishekzopper-2.3/src/auditLogger/main.py
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)     6942 2023-07-04 12:46:22.000000 auditLogger-abhishekzopper-2.3/src/auditLogger/req_resp_middleware.py
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)    10324 2023-07-04 08:51:48.000000 auditLogger-abhishekzopper-2.3/src/auditLogger/requests_logging.py
+drwxr-xr-x   0 abhishekratnam   (501) staff       (20)        0 2023-07-04 13:10:09.520290 auditLogger-abhishekzopper-2.3/src/auditLogger_abhishekzopper.egg-info/
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)      424 2023-07-04 13:10:09.000000 auditLogger-abhishekzopper-2.3/src/auditLogger_abhishekzopper.egg-info/PKG-INFO
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)      419 2023-07-04 13:10:09.000000 auditLogger-abhishekzopper-2.3/src/auditLogger_abhishekzopper.egg-info/SOURCES.txt
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)        1 2023-07-04 13:10:09.000000 auditLogger-abhishekzopper-2.3/src/auditLogger_abhishekzopper.egg-info/dependency_links.txt
+-rw-r--r--   0 abhishekratnam   (501) staff       (20)       12 2023-07-04 13:10:09.000000 auditLogger-abhishekzopper-2.3/src/auditLogger_abhishekzopper.egg-info/top_level.txt
```

### Comparing `auditLogger-abhishekzopper-2.2/setup.cfg` & `auditLogger-abhishekzopper-2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = auditLogger-abhishekzopper
-version = 2.2
+version = 2.3
 author = AbhishekRatnam
 author_email = abhishek.ratnam@zopper.com
 description = Custom Logger package
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `auditLogger-abhishekzopper-2.2/src/auditLogger/custom_logging.py` & `auditLogger-abhishekzopper-2.3/src/auditLogger/custom_logging.py`

 * *Files identical despite different names*

### Comparing `auditLogger-abhishekzopper-2.2/src/auditLogger/req_resp_middleware.py` & `auditLogger-abhishekzopper-2.3/src/auditLogger/req_resp_middleware.py`

 * *Files identical despite different names*

### Comparing `auditLogger-abhishekzopper-2.2/src/auditLogger/requests_logging.py` & `auditLogger-abhishekzopper-2.3/src/auditLogger/requests_logging.py`

 * *Files identical despite different names*

