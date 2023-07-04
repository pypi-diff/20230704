# Comparing `tmp/CORS-Analyzer-1.0.7.tar.gz` & `tmp/CORS-Analyzer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CORS-Analyzer-1.0.7.tar", last modified: Tue Jul  4 08:07:25 2023, max compression
+gzip compressed data, was "CORS-Analyzer-1.0.8.tar", last modified: Tue Jul  4 08:20:43 2023, max compression
```

## Comparing `CORS-Analyzer-1.0.7.tar` & `CORS-Analyzer-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 08:07:25.328550 CORS-Analyzer-1.0.7/
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 08:07:25.328550 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 08:07:25.000000 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      280 2023-07-04 08:07:25.000000 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-04 08:07:25.000000 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       49 2023-07-04 08:07:25.000000 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/entry_points.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-04 08:07:25.000000 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-04 08:07:25.000000 CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/top_level.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 08:07:25.328550 CORS-Analyzer-1.0.7/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     3395 2023-07-04 07:36:32.000000 CORS-Analyzer-1.0.7/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 08:07:25.328550 CORS-Analyzer-1.0.7/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 CORS-Analyzer-1.0.7/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     2805 2023-07-04 08:05:07.000000 CORS-Analyzer-1.0.7/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-04 08:07:25.328550 CORS-Analyzer-1.0.7/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      712 2023-07-04 08:07:08.000000 CORS-Analyzer-1.0.7/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 08:20:43.625286 CORS-Analyzer-1.0.8/
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 08:20:43.625286 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3735 2023-07-04 08:20:43.000000 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      280 2023-07-04 08:20:43.000000 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-04 08:20:43.000000 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       49 2023-07-04 08:20:43.000000 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-04 08:20:43.000000 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-04 08:20:43.000000 CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/top_level.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3735 2023-07-04 08:20:43.625286 CORS-Analyzer-1.0.8/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3389 2023-07-04 08:15:59.000000 CORS-Analyzer-1.0.8/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 08:20:43.625286 CORS-Analyzer-1.0.8/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 CORS-Analyzer-1.0.8/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2796 2023-07-04 08:17:53.000000 CORS-Analyzer-1.0.8/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-04 08:20:43.625286 CORS-Analyzer-1.0.8/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      712 2023-07-04 08:19:25.000000 CORS-Analyzer-1.0.8/setup.py
```

### Comparing `CORS-Analyzer-1.0.7/CORS_Analyzer.egg-info/PKG-INFO` & `CORS-Analyzer-1.0.8/CORS_Analyzer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CORS-Analyzer
-Version: 1.0.7
+Version: 1.0.8
 Summary: The cors-analyzer package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors-analyzer,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -45,17 +45,17 @@
 ### Python Version:
 * Python 3 (3.x.x) latest version
 
 ### How to Use CORS-Finder:
 
 ```
 For scanning:
-       cat <domain.txt> | xargs -n1 -P10 python3 corss.py                           
+       cat <domain.txt> | xargs -n1 -P10 cors-analyzer                           
 For scanning with output:  
-       cat <domain.txt> | xargs -n1 -P10 python3 corss.py | tee -a <output.txt>
+       cat <domain.txt> | xargs -n1 -P10 cors-analyzer | tee -a <output.txt>
 ```
 
 ### When its vulnerable:
 If the header returns the 
        Access-Control-Allow-Origin: https://vulnerable.com/
        Access-Control-Allow-Credentials: true
        its vulnerable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.7 Summary: The cors-
+Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.8 Summary: The cors-
 analyzer package is used to find the vulnerable CORS domains Home-page: UNKNOWN
 Author: Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors-
 analyzer,cors misconfiguration,cors exploit,cors vulnerability Platform:
 UNKNOWN Description-Content-Type: text/markdown # CORS-Analyzer ## This tools
 is developed for identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 ### How to install CORS-Analyzer: ``` git clone https://github.com/
@@ -13,16 +13,16 @@
 the following command, pip install cors-analyzer If you want to install the
 latest version of CORS-Analyzer just uninstall the old version using the
 following command, pip uninstall cors-analyzer pip install --upgrade cors-
 analyzer For upgrade, use the following command, pip install --upgrade cors-
 analyzer For ignore the cache, use the following command, pip install --ignore-
 cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x) latest version
 ### How to Use CORS-Finder: ``` For scanning: cat
-txt> | xargs -n1 -P10 python3 corss.py For scanning with output: cat
-txt> | xargs -n1 -P10 python3 corss.py | tee -a
+txt> | xargs -n1 -P10 cors-analyzer For scanning with output: cat
+txt> | xargs -n1 -P10 cors-analyzer | tee -a
 txt> ``` ### When its vulnerable: If the header returns the Access-Control-
 Allow-Origin: https://vulnerable.com/ Access-Control-Allow-Credentials: true
 its vulnerable Note: Not all the time its seems vulnerable, you have to check
 with cors payload and in the authenticated manner also. Try to exploit and this
 tool is only for indentifying the vulnerable domain Note: In this tool i used
 sample domain file but you have to choose your own url file which you recon
 using some other recon tool. ### Exploitation examples: Here is the Example
```

### Comparing `CORS-Analyzer-1.0.7/PKG-INFO` & `CORS-Analyzer-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CORS-Analyzer
-Version: 1.0.7
+Version: 1.0.8
 Summary: The cors-analyzer package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors-analyzer,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -45,17 +45,17 @@
 ### Python Version:
 * Python 3 (3.x.x) latest version
 
 ### How to Use CORS-Finder:
 
 ```
 For scanning:
-       cat <domain.txt> | xargs -n1 -P10 python3 corss.py                           
+       cat <domain.txt> | xargs -n1 -P10 cors-analyzer                           
 For scanning with output:  
-       cat <domain.txt> | xargs -n1 -P10 python3 corss.py | tee -a <output.txt>
+       cat <domain.txt> | xargs -n1 -P10 cors-analyzer | tee -a <output.txt>
 ```
 
 ### When its vulnerable:
 If the header returns the 
        Access-Control-Allow-Origin: https://vulnerable.com/
        Access-Control-Allow-Credentials: true
        its vulnerable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.7 Summary: The cors-
+Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.8 Summary: The cors-
 analyzer package is used to find the vulnerable CORS domains Home-page: UNKNOWN
 Author: Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors-
 analyzer,cors misconfiguration,cors exploit,cors vulnerability Platform:
 UNKNOWN Description-Content-Type: text/markdown # CORS-Analyzer ## This tools
 is developed for identifying the vulnerable cors domain ![alt text](https://
 raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 ### How to install CORS-Analyzer: ``` git clone https://github.com/
@@ -13,16 +13,16 @@
 the following command, pip install cors-analyzer If you want to install the
 latest version of CORS-Analyzer just uninstall the old version using the
 following command, pip uninstall cors-analyzer pip install --upgrade cors-
 analyzer For upgrade, use the following command, pip install --upgrade cors-
 analyzer For ignore the cache, use the following command, pip install --ignore-
 cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x) latest version
 ### How to Use CORS-Finder: ``` For scanning: cat
-txt> | xargs -n1 -P10 python3 corss.py For scanning with output: cat
-txt> | xargs -n1 -P10 python3 corss.py | tee -a
+txt> | xargs -n1 -P10 cors-analyzer For scanning with output: cat
+txt> | xargs -n1 -P10 cors-analyzer | tee -a
 txt> ``` ### When its vulnerable: If the header returns the Access-Control-
 Allow-Origin: https://vulnerable.com/ Access-Control-Allow-Credentials: true
 its vulnerable Note: Not all the time its seems vulnerable, you have to check
 with cors payload and in the authenticated manner also. Try to exploit and this
 tool is only for indentifying the vulnerable domain Note: In this tool i used
 sample domain file but you have to choose your own url file which you recon
 using some other recon tool. ### Exploitation examples: Here is the Example
```

### Comparing `CORS-Analyzer-1.0.7/README.md` & `CORS-Analyzer-1.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 ### Python Version:
 * Python 3 (3.x.x) latest version
 
 ### How to Use CORS-Finder:
 
 ```
 For scanning:
-       cat <domain.txt> | xargs -n1 -P10 python3 corss.py                           
+       cat <domain.txt> | xargs -n1 -P10 cors-analyzer                           
 For scanning with output:  
-       cat <domain.txt> | xargs -n1 -P10 python3 corss.py | tee -a <output.txt>
+       cat <domain.txt> | xargs -n1 -P10 cors-analyzer | tee -a <output.txt>
 ```
 
 ### When its vulnerable:
 If the header returns the 
        Access-Control-Allow-Origin: https://vulnerable.com/
        Access-Control-Allow-Credentials: true
        its vulnerable
```

#### html2text {}

```diff
@@ -8,16 +8,16 @@
 first time installation use the following command, pip install cors-analyzer If
 you want to install the latest version of CORS-Analyzer just uninstall the old
 version using the following command, pip uninstall cors-analyzer pip install --
 upgrade cors-analyzer For upgrade, use the following command, pip install --
 upgrade cors-analyzer For ignore the cache, use the following command, pip
 install --ignore-cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x)
 latest version ### How to Use CORS-Finder: ``` For scanning: cat
-txt> | xargs -n1 -P10 python3 corss.py For scanning with output: cat
-txt> | xargs -n1 -P10 python3 corss.py | tee -a
+txt> | xargs -n1 -P10 cors-analyzer For scanning with output: cat
+txt> | xargs -n1 -P10 cors-analyzer | tee -a
 txt> ``` ### When its vulnerable: If the header returns the Access-Control-
 Allow-Origin: https://vulnerable.com/ Access-Control-Allow-Credentials: true
 its vulnerable Note: Not all the time its seems vulnerable, you have to check
 with cors payload and in the authenticated manner also. Try to exploit and this
 tool is only for indentifying the vulnerable domain Note: In this tool i used
 sample domain file but you have to choose your own url file which you recon
 using some other recon tool. ### Exploitation examples: Here is the Example
```

### Comparing `CORS-Analyzer-1.0.7/lib/cors.py` & `CORS-Analyzer-1.0.8/lib/cors.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,23 +50,23 @@
 	for header, value in status.items():
 		print(header + ": " + value)"""
 
 def help():
 	print(Fore.WHITE)
 	banner()
 	print(Fore.GREEN + "USAGE: \n")
-	print(Fore.WHITE + "For scanning:  cat <domain.txt> | xargs -n1 -P10 python3 cors.py \n")
-	print(Fore.WHITE + "For scanning with output:  cat <domain.txt> | xargs -n1 -P10 python3 cors.py | tee -a <output.txt> \n")
+	print(Fore.WHITE + "For scanning:  cat <domain.txt> | xargs -n1 -P10 cors-analyzer \n")
+	print(Fore.WHITE + "For scanning with output:  cat <domain.txt> | xargs -n1 -P10 cors-analyzer | tee -a <output.txt> \n")
 	
 if (len(sys.argv)<=1):
 	os.system("clear")
 	banner()
 	print(Fore.WHITE)
 	print("You must provide a target. Use -h or --help for help. \n")
-	print("Usage: python3 cors.py -h or  python3 cors.py --help \n")
+	print("Usage: cors-analyzer -h or cors-analyzer --help \n")
 
 	print(" ")
 	sys.exit()        
 
 elif (str(sys.argv[1]) == "-h" or str(sys.argv[1]) == "--help"):
 	os.system("clear")
 	help()
```

### Comparing `CORS-Analyzer-1.0.7/setup.py` & `CORS-Analyzer-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="CORS-Analyzer",
-    version= '1.0.7',
+    version= '1.0.8',
     author= 'Hariharan',
     description= 'The cors-analyzer package is used to find the vulnerable CORS domains',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords= ['cors', 'cors-finder', 'cors-analyzer', 'cors misconfiguration', 'cors exploit', 'cors vulnerability'],
     packages=find_packages(),
     entry_points={
```

