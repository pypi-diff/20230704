# Comparing `tmp/pycof-1.5.5.tar.gz` & `tmp/pycof-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycof-1.5.5.tar", last modified: Tue Jul  4 10:03:35 2023, max compression
+gzip compressed data, was "pycof-1.5.6.tar", last modified: Tue Jul  4 11:00:03 2023, max compression
```

## Comparing `pycof-1.5.5.tar` & `pycof-1.5.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 10:03:35.128156 pycof-1.5.5/
--rw-r--r--   0 florian   (1000) florian   (1000)     1071 2020-10-01 18:30:50.000000 pycof-1.5.5/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-07-04 10:03:35.128156 pycof-1.5.5/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     4067 2022-09-25 17:41:11.000000 pycof-1.5.5/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 10:03:35.128156 pycof-1.5.5/pycof/
--rw-r--r--   0 florian   (1000) florian   (1000)      178 2023-07-04 10:03:34.000000 pycof-1.5.5/pycof/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14439 2023-01-26 16:12:36.000000 pycof-1.5.5/pycof/data.py
--rw-r--r--   0 florian   (1000) florian   (1000)    30792 2023-07-04 10:03:08.000000 pycof-1.5.5/pycof/format.py
--rw-r--r--   0 florian   (1000) florian   (1000)      182 2021-06-27 12:32:45.000000 pycof-1.5.5/pycof/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)    15161 2023-07-04 09:14:03.000000 pycof-1.5.5/pycof/misc.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10308 2022-09-25 17:49:57.000000 pycof-1.5.5/pycof/sql.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14117 2023-07-04 08:44:49.000000 pycof-1.5.5/pycof/sqlhelper.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 10:03:35.128156 pycof-1.5.5/pycof.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      300 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      313 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-04 10:03:35.128156 pycof-1.5.5/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     1170 2023-03-12 10:48:27.000000 pycof-1.5.5/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1216 2023-07-04 10:03:34.000000 pycof-1.5.5/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 11:00:03.566727 pycof-1.5.6/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1071 2020-10-01 18:30:50.000000 pycof-1.5.6/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-07-04 11:00:03.566727 pycof-1.5.6/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     4067 2022-09-25 17:41:11.000000 pycof-1.5.6/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 11:00:03.555893 pycof-1.5.6/pycof/
+-rw-r--r--   0 florian   (1000) florian   (1000)      178 2023-07-04 11:00:03.000000 pycof-1.5.6/pycof/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14439 2023-01-26 16:12:36.000000 pycof-1.5.6/pycof/data.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    30803 2023-07-04 10:56:50.000000 pycof-1.5.6/pycof/format.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      182 2021-06-27 12:32:45.000000 pycof-1.5.6/pycof/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15161 2023-07-04 09:14:03.000000 pycof-1.5.6/pycof/misc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10308 2022-09-25 17:49:57.000000 pycof-1.5.6/pycof/sql.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14117 2023-07-04 08:44:49.000000 pycof-1.5.6/pycof/sqlhelper.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 11:00:03.566727 pycof-1.5.6/pycof.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-07-04 11:00:03.000000 pycof-1.5.6/pycof.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      300 2023-07-04 11:00:03.000000 pycof-1.5.6/pycof.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-04 11:00:03.000000 pycof-1.5.6/pycof.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      313 2023-07-04 11:00:03.000000 pycof-1.5.6/pycof.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-04 11:00:03.000000 pycof-1.5.6/pycof.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-04 11:00:03.566727 pycof-1.5.6/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1170 2023-03-12 10:48:27.000000 pycof-1.5.6/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1216 2023-07-04 11:00:03.000000 pycof-1.5.6/setup_new.py
```

### Comparing `pycof-1.5.5/LICENSE` & `pycof-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/PKG-INFO` & `pycof-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycof
-Version: 1.5.5
+Version: 1.5.6
 Summary: A package for commonly used functions
 Home-page: https://www.florianfelice.com/pycof
 Author: Florian Felice
 Author-email: admin@florianfelice.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycof-1.5.5/README.md` & `pycof-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/pycof/data.py` & `pycof-1.5.6/pycof/data.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/pycof/format.py` & `pycof-1.5.6/pycof/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     msg = MIMEMultipart()
     msg['From'] = config.get('EMAIL_USER')
     msg['To'] = to
     # msg['Cc'] = '' if cc == '' else cc
     msg['Subject'] = subject
 
     mail_type = 'html' if '</' in body else 'plain'
-    msg.attach(MIMEText(body))
+    msg.attach(MIMEText(body), mail_type)
 
     text = msg.as_string()
 
     with EmailSSHTunnel(config=config, connection=connection) as tunnel:
         conn = tunnel.connector()
         conn.sendmail(config.get('EMAIL_USER'), [to, '', cc], text)
         conn.quit()
```

### Comparing `pycof-1.5.5/pycof/misc.py` & `pycof-1.5.6/pycof/misc.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/pycof/sql.py` & `pycof-1.5.6/pycof/sql.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/pycof/sqlhelper.py` & `pycof-1.5.6/pycof/sqlhelper.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/pycof.egg-info/PKG-INFO` & `pycof-1.5.6/pycof.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycof
-Version: 1.5.5
+Version: 1.5.6
 Summary: A package for commonly used functions
 Home-page: https://www.florianfelice.com/pycof
 Author: Florian Felice
 Author-email: admin@florianfelice.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycof-1.5.5/setup.py` & `pycof-1.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.5/setup_new.py` & `pycof-1.5.6/setup_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycof",
-    version="1.5.5",
+    version="1.5.6",
     author="Florian Felice",
     author_email="admin@florianfelice.com",
     description="A package for commonly used functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/pycof",
     packages=setuptools.find_packages(),
```

