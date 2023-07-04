# Comparing `tmp/CORS-Analyzer-1.0.5.tar.gz` & `tmp/CORS-Analyzer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CORS-Analyzer-1.0.5.tar", last modified: Tue Jul  4 07:38:31 2023, max compression
+gzip compressed data, was "CORS-Analyzer-1.0.6.tar", last modified: Tue Jul  4 07:57:57 2023, max compression
```

## Comparing `CORS-Analyzer-1.0.5.tar` & `CORS-Analyzer-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      280 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       49 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/entry_points.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/top_level.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     3395 2023-07-04 07:36:32.000000 CORS-Analyzer-1.0.5/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 CORS-Analyzer-1.0.5/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-04 07:08:35.000000 CORS-Analyzer-1.0.5/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      712 2023-07-04 07:38:11.000000 CORS-Analyzer-1.0.5/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:57:57.195580 CORS-Analyzer-1.0.6/
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:57:57.195580 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 07:57:57.000000 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      280 2023-07-04 07:57:57.000000 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-04 07:57:57.000000 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       49 2023-07-04 07:57:57.000000 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-04 07:57:57.000000 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-04 07:57:57.000000 CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/top_level.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 07:57:57.195580 CORS-Analyzer-1.0.6/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3395 2023-07-04 07:36:32.000000 CORS-Analyzer-1.0.6/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:57:57.195580 CORS-Analyzer-1.0.6/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 CORS-Analyzer-1.0.6/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2755 2023-07-04 07:53:21.000000 CORS-Analyzer-1.0.6/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-04 07:57:57.195580 CORS-Analyzer-1.0.6/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      712 2023-07-04 07:56:25.000000 CORS-Analyzer-1.0.6/setup.py
```

### Comparing `CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/PKG-INFO` & `CORS-Analyzer-1.0.6/CORS_Analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CORS-Analyzer
-Version: 1.0.5
+Version: 1.0.6
 Summary: The cors-analyzer package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors-analyzer,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.5 Summary: The cors-
+Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.6 Summary: The cors-
 analyzer package is used to find the vulnerable CORS domains Home-page: UNKNOWN
 Author: Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors-
 analyzer,cors misconfiguration,cors exploit,cors vulnerability Platform:
 UNKNOWN Description-Content-Type: text/markdown # CORS-Analyzer ## This tools
 is developed for identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 ### How to install CORS-Analyzer: ``` git clone https://github.com/
```

### Comparing `CORS-Analyzer-1.0.5/PKG-INFO` & `CORS-Analyzer-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CORS-Analyzer
-Version: 1.0.5
+Version: 1.0.6
 Summary: The cors-analyzer package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors-analyzer,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.5 Summary: The cors-
+Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.6 Summary: The cors-
 analyzer package is used to find the vulnerable CORS domains Home-page: UNKNOWN
 Author: Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors-
 analyzer,cors misconfiguration,cors exploit,cors vulnerability Platform:
 UNKNOWN Description-Content-Type: text/markdown # CORS-Analyzer ## This tools
 is developed for identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 ### How to install CORS-Analyzer: ``` git clone https://github.com/
```

### Comparing `CORS-Analyzer-1.0.5/README.md` & `CORS-Analyzer-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `CORS-Analyzer-1.0.5/lib/cors.py` & `CORS-Analyzer-1.0.6/lib/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 		print(header + ": " + value)"""
 
 def help():
 	print(Fore.WHITE)
 	banner()
 	print(Fore.GREEN + "USAGE: \n")
 	print(Fore.WHITE + "For scanning:  cat <domain.txt> | xargs -n1 -P10 python3 cors.py \n")
-	print(Fore.WHITE + "For scanning with output:  cat <domain.txt> | xargs -n1 -P10 python3 corss.py | tee -a <output.txt> \n")
+	print(Fore.WHITE + "For scanning with output:  cat <domain.txt> | xargs -n1 -P10 python3 cors.py | tee -a <output.txt> \n")
 	
 if (len(sys.argv)<=1):
 	os.system("clear")
 	banner()
 	print(Fore.WHITE)
 	print("You must provide a target. Use -h or --help for help. \n")
 	print("Usage: python3 cors.py -h or  python3 cors.py --help \n")
@@ -69,10 +69,8 @@
 
 elif (str(sys.argv[1]) == "-h" or str(sys.argv[1]) == "--help"):
 	os.system("clear")
 	help()
 	sys.exit()
 	
 elif (len(sys.argv)>=1):
-	os.system("clear")
-	banner()
 	action()
```

### Comparing `CORS-Analyzer-1.0.5/setup.py` & `CORS-Analyzer-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="CORS-Analyzer",
-    version= '1.0.5',
+    version= '1.0.6',
     author= 'Hariharan',
     description= 'The cors-analyzer package is used to find the vulnerable CORS domains',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords= ['cors', 'cors-finder', 'cors-analyzer', 'cors misconfiguration', 'cors exploit', 'cors vulnerability'],
     packages=find_packages(),
     entry_points={
```

