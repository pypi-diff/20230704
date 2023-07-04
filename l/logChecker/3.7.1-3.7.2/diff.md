# Comparing `tmp/logChecker-3.7.1.tar.gz` & `tmp/logChecker-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logChecker-3.7.1.tar", last modified: Wed May  3 16:39:30 2023, max compression
+gzip compressed data, was "logChecker-3.7.2.tar", last modified: Tue Jul  4 17:47:09 2023, max compression
```

## Comparing `logChecker-3.7.1.tar` & `logChecker-3.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.993637 logChecker-3.7.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1654 2022-11-28 15:01:26.000000 logChecker-3.7.1/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-05-03 16:39:29.993637 logChecker-3.7.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     4467 2022-11-28 15:01:26.000000 logChecker-3.7.1/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.993637 logChecker-3.7.1/logChecker.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      288 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       62 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       58 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       15 2023-05-03 16:39:29.000000 logChecker-3.7.1/logChecker.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-03 16:39:29.993637 logChecker-3.7.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1038 2023-05-03 16:38:51.000000 logChecker-3.7.1/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.989637 logChecker-3.7.1/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 16:39:29.993637 logChecker-3.7.1/src/logChecker/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-05-03 16:39:00.000000 logChecker-3.7.1/src/logChecker/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    30663 2023-05-03 15:04:12.000000 logChecker-3.7.1/src/logChecker/logChecker.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-04 17:47:09.746291 logChecker-3.7.2/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1654 2022-11-28 15:01:26.000000 logChecker-3.7.2/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-07-04 17:47:09.746291 logChecker-3.7.2/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     4467 2022-11-28 15:01:26.000000 logChecker-3.7.2/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-04 17:47:09.746291 logChecker-3.7.2/logChecker.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      611 2023-07-04 17:47:09.000000 logChecker-3.7.2/logChecker.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      288 2023-07-04 17:47:09.000000 logChecker-3.7.2/logChecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-07-04 17:47:09.000000 logChecker-3.7.2/logChecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       62 2023-07-04 17:47:09.000000 logChecker-3.7.2/logChecker.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       58 2023-07-04 17:47:09.000000 logChecker-3.7.2/logChecker.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       15 2023-07-04 17:47:09.000000 logChecker-3.7.2/logChecker.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-07-04 17:47:09.746291 logChecker-3.7.2/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1038 2023-07-04 17:42:45.000000 logChecker-3.7.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-04 17:47:09.746291 logChecker-3.7.2/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-04 17:47:09.746291 logChecker-3.7.2/src/logChecker/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-07-04 17:43:03.000000 logChecker-3.7.2/src/logChecker/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    30663 2023-07-04 17:41:38.000000 logChecker-3.7.2/src/logChecker/logChecker.py
```

### Comparing `logChecker-3.7.1/LICENSE` & `logChecker-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logChecker-3.7.1/PKG-INFO` & `logChecker-3.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logChecker
-Version: 3.7.1
+Version: 3.7.2
 Summary: A simple log analysis tool
 Home-page: https://github.com/laimaretto/logChecker
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Project-URL: Templates, https://github.com/laimaretto/logTemplates
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logChecker-3.7.1/README.md` & `logChecker-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `logChecker-3.7.1/logChecker.egg-info/PKG-INFO` & `logChecker-3.7.2/logChecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logChecker
-Version: 3.7.1
+Version: 3.7.2
 Summary: A simple log analysis tool
 Home-page: https://github.com/laimaretto/logChecker
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Project-URL: Templates, https://github.com/laimaretto/logTemplates
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logChecker-3.7.1/setup.py` & `logChecker-3.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='logChecker',
-    version='3.7.1',  
+    version='3.7.2',  
     description='A simple log analysis tool',
     long_description='A parsing tool to easily perform pre and post check comparisons after a maintenance window.',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/logChecker',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
     packages=['src/logChecker'],
-    install_requires=['textfsm==1.1.2',
+    install_requires=['textfsm==1.1.3',
                       'pandas==1.5.2',
                       'XlsxWriter==3.0.3',
                       'ttp==0.9.0',
                       ],
     python_requires='>=3.8',
     classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `logChecker-3.7.1/src/logChecker/logChecker.py` & `logChecker-3.7.2/src/logChecker/logChecker.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,15 +871,15 @@
 	parser1.add_argument('-json', '--formatJson',   type=str, default = 'yes', choices=['yes','no'], help='logs in json format: yes or no. Default=yes.')
 	parser1.add_argument('-tf', '--templateFolder', type=str, default='Templates/', help='Folder where templates reside. Used both for PRE and POST logs. Default=Templates/')
 	parser1.add_argument('-tf-post', '--templateFolderPost', type=str, default='', help='If set, use this folder of templates for POST logs.')
 	parser1.add_argument('-te', '--templateEngine', choices=['ttp','textFSM'], default='textFSM', type=str, help='Engine for parsing. Default=textFSM.')
 	parser1.add_argument('-ri', '--routerId',       choices=['name','ip','both'], default='name', type=str, help='Router Id to be used within the tables in the Excel report. Default=name.')
 	parser1.add_argument('-sr', '--showResults',    choices=['all','diff'], default='all', type=str, help='When comparison is done, show all variables or only the differences. Only available if --ri/--routerId=name. Default=all)')
 	parser1.add_argument('-ga', '--genAtp',        type=str, help='Generate ATP document in docx format, based on the contents of the json files from taskAutom. Default=no', default='no', choices=['no','yes'])
-	parser1.add_argument('-v'  ,'--version',        help='Version', action='version', version='Lucas Aimaretto - (c)2023 - Version: 3.7.1' )
+	parser1.add_argument('-v'  ,'--version',        help='Version', action='version', version='Lucas Aimaretto - (c)2023 - Version: 3.7.2' )
 
 	args               = parser1.parse_args()
 
 	dictParam = dict(
 		preFolder          = args.preFolder,
 		postFolder         = args.postFolder,
 		csvTemplate        = args.csvTemplate,
```

