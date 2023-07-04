# Comparing `tmp/CORS-Analyzer-1.0.4.tar.gz` & `tmp/CORS-Analyzer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CORS-Analyzer-1.0.4.tar", last modified: Tue Jul  4 07:21:11 2023, max compression
+gzip compressed data, was "CORS-Analyzer-1.0.5.tar", last modified: Tue Jul  4 07:38:31 2023, max compression
```

## Comparing `CORS-Analyzer-1.0.4.tar` & `CORS-Analyzer-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:21:11.739698 CORS-Analyzer-1.0.4/
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:21:11.735697 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/
--rw-rw-r--   0 hari      (1000) hari      (1000)     3688 2023-07-04 07:21:11.000000 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)      280 2023-07-04 07:21:11.000000 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-04 07:21:11.000000 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       49 2023-07-04 07:21:11.000000 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/entry_points.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-04 07:21:11.000000 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/requires.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-04 07:21:11.000000 CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/top_level.txt
--rw-rw-r--   0 hari      (1000) hari      (1000)     3688 2023-07-04 07:21:11.739698 CORS-Analyzer-1.0.4/PKG-INFO
--rw-rw-r--   0 hari      (1000) hari      (1000)     3342 2023-07-04 07:19:28.000000 CORS-Analyzer-1.0.4/README.md
-drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:21:11.739698 CORS-Analyzer-1.0.4/lib/
--rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 CORS-Analyzer-1.0.4/lib/__init__.py
--rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-04 07:08:35.000000 CORS-Analyzer-1.0.4/lib/cors.py
--rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-04 07:21:11.739698 CORS-Analyzer-1.0.4/setup.cfg
--rw-rw-r--   0 hari      (1000) hari      (1000)      712 2023-07-04 07:15:08.000000 CORS-Analyzer-1.0.4/setup.py
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)      280 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        1 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       49 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)       18 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/requires.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)        4 2023-07-04 07:38:31.000000 CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/top_level.txt
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3741 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/PKG-INFO
+-rw-rw-r--   0 hari      (1000) hari      (1000)     3395 2023-07-04 07:36:32.000000 CORS-Analyzer-1.0.5/README.md
+drwxrwxr-x   0 hari      (1000) hari      (1000)        0 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/lib/
+-rw-rw-r--   0 hari      (1000) hari      (1000)        0 2023-07-02 16:59:46.000000 CORS-Analyzer-1.0.5/lib/__init__.py
+-rwxrwxr-x   0 hari      (1000) hari      (1000)     2786 2023-07-04 07:08:35.000000 CORS-Analyzer-1.0.5/lib/cors.py
+-rw-rw-r--   0 hari      (1000) hari      (1000)       96 2023-07-04 07:38:31.614223 CORS-Analyzer-1.0.5/setup.cfg
+-rw-rw-r--   0 hari      (1000) hari      (1000)      712 2023-07-04 07:38:11.000000 CORS-Analyzer-1.0.5/setup.py
```

### Comparing `CORS-Analyzer-1.0.4/CORS_Analyzer.egg-info/PKG-INFO` & `CORS-Analyzer-1.0.5/CORS_Analyzer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: CORS-Analyzer
-Version: 1.0.4
+Version: 1.0.5
 Summary: The cors-analyzer package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors-analyzer,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # CORS-Analyzer
 ## This tools is developed for identifying the vulnerable cors domain
 
-![alt text](lib/banner/cors-analyzer.png)
+![alt text](https://raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 
 ### How to install CORS-Analyzer:
 ```
 git clone https://github.com/hariharan005/CORS.git     
 ls    
 cd CORS
 sudo pip3 install -r requirements.txt 
@@ -34,15 +34,15 @@
 
 If you want to install the latest version of CORS-Analyzer just uninstall the old version using the following command,
     pip uninstall cors-analyzer
     pip install --upgrade cors-analyzer
 
 For upgrade, use the following command,
     pip install --upgrade cors-analyzer
-    
+
 For ignore the cache, use the following command,
     pip install --ignore-cache cors-analyzer
 ```
 ### Python Version:
 * Python 3 (3.x.x) latest version
 
 ### How to Use CORS-Finder:
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.4 Summary: The cors-
+Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.5 Summary: The cors-
 analyzer package is used to find the vulnerable CORS domains Home-page: UNKNOWN
 Author: Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors-
 analyzer,cors misconfiguration,cors exploit,cors vulnerability Platform:
 UNKNOWN Description-Content-Type: text/markdown # CORS-Analyzer ## This tools
-is developed for identifying the vulnerable cors domain ![alt text](lib/banner/
-cors-analyzer.png) ### How to install CORS-Analyzer: ``` git clone https://
-github.com/hariharan005/CORS.git ls cd CORS sudo pip3 install -
-r requirements.txt cd lib && chmod +x cors.py sudo ln -s "$(pwd)/cors.py" /usr/
-local/bin/cors-analyzer cors-analyzer ``` Now type "cors-analyzer" to access
-the CORS analyzer tool from anywhere ### How to install using pip: ``` For
-first time installation use the following command, pip install cors-analyzer If
-you want to install the latest version of CORS-Analyzer just uninstall the old
-version using the following command, pip uninstall cors-analyzer pip install --
-upgrade cors-analyzer For upgrade, use the following command, pip install --
-upgrade cors-analyzer For ignore the cache, use the following command, pip
-install --ignore-cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x)
-latest version ### How to Use CORS-Finder: ``` For scanning: cat
+is developed for identifying the vulnerable cors domain ![alt text](https://
+raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
+### How to install CORS-Analyzer: ``` git clone https://github.com/
+hariharan005/CORS.git ls cd CORS sudo pip3 install -r requirements.txt cd lib
+&& chmod +x cors.py sudo ln -s "$(pwd)/cors.py" /usr/local/bin/cors-analyzer
+cors-analyzer ``` Now type "cors-analyzer" to access the CORS analyzer tool
+from anywhere ### How to install using pip: ``` For first time installation use
+the following command, pip install cors-analyzer If you want to install the
+latest version of CORS-Analyzer just uninstall the old version using the
+following command, pip uninstall cors-analyzer pip install --upgrade cors-
+analyzer For upgrade, use the following command, pip install --upgrade cors-
+analyzer For ignore the cache, use the following command, pip install --ignore-
+cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x) latest version
+### How to Use CORS-Finder: ``` For scanning: cat
 txt> | xargs -n1 -P10 python3 corss.py For scanning with output: cat
 txt> | xargs -n1 -P10 python3 corss.py | tee -a
 txt> ``` ### When its vulnerable: If the header returns the Access-Control-
 Allow-Origin: https://vulnerable.com/ Access-Control-Allow-Credentials: true
 its vulnerable Note: Not all the time its seems vulnerable, you have to check
 with cors payload and in the authenticated manner also. Try to exploit and this
 tool is only for indentifying the vulnerable domain Note: In this tool i used
```

### Comparing `CORS-Analyzer-1.0.4/PKG-INFO` & `CORS-Analyzer-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: CORS-Analyzer
-Version: 1.0.4
+Version: 1.0.5
 Summary: The cors-analyzer package is used to find the vulnerable CORS domains
 Home-page: UNKNOWN
 Author: Hariharan
 License: UNKNOWN
 Keywords: cors,cors-finder,cors-analyzer,cors misconfiguration,cors exploit,cors vulnerability
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # CORS-Analyzer
 ## This tools is developed for identifying the vulnerable cors domain
 
-![alt text](lib/banner/cors-analyzer.png)
+![alt text](https://raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 
 ### How to install CORS-Analyzer:
 ```
 git clone https://github.com/hariharan005/CORS.git     
 ls    
 cd CORS
 sudo pip3 install -r requirements.txt 
@@ -34,15 +34,15 @@
 
 If you want to install the latest version of CORS-Analyzer just uninstall the old version using the following command,
     pip uninstall cors-analyzer
     pip install --upgrade cors-analyzer
 
 For upgrade, use the following command,
     pip install --upgrade cors-analyzer
-    
+
 For ignore the cache, use the following command,
     pip install --ignore-cache cors-analyzer
 ```
 ### Python Version:
 * Python 3 (3.x.x) latest version
 
 ### How to Use CORS-Finder:
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.4 Summary: The cors-
+Metadata-Version: 2.1 Name: CORS-Analyzer Version: 1.0.5 Summary: The cors-
 analyzer package is used to find the vulnerable CORS domains Home-page: UNKNOWN
 Author: Hariharan License: UNKNOWN Keywords: cors,cors-finder,cors-
 analyzer,cors misconfiguration,cors exploit,cors vulnerability Platform:
 UNKNOWN Description-Content-Type: text/markdown # CORS-Analyzer ## This tools
-is developed for identifying the vulnerable cors domain ![alt text](lib/banner/
-cors-analyzer.png) ### How to install CORS-Analyzer: ``` git clone https://
-github.com/hariharan005/CORS.git ls cd CORS sudo pip3 install -
-r requirements.txt cd lib && chmod +x cors.py sudo ln -s "$(pwd)/cors.py" /usr/
-local/bin/cors-analyzer cors-analyzer ``` Now type "cors-analyzer" to access
-the CORS analyzer tool from anywhere ### How to install using pip: ``` For
-first time installation use the following command, pip install cors-analyzer If
-you want to install the latest version of CORS-Analyzer just uninstall the old
-version using the following command, pip uninstall cors-analyzer pip install --
-upgrade cors-analyzer For upgrade, use the following command, pip install --
-upgrade cors-analyzer For ignore the cache, use the following command, pip
-install --ignore-cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x)
-latest version ### How to Use CORS-Finder: ``` For scanning: cat
+is developed for identifying the vulnerable cors domain ![alt text](https://
+raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
+### How to install CORS-Analyzer: ``` git clone https://github.com/
+hariharan005/CORS.git ls cd CORS sudo pip3 install -r requirements.txt cd lib
+&& chmod +x cors.py sudo ln -s "$(pwd)/cors.py" /usr/local/bin/cors-analyzer
+cors-analyzer ``` Now type "cors-analyzer" to access the CORS analyzer tool
+from anywhere ### How to install using pip: ``` For first time installation use
+the following command, pip install cors-analyzer If you want to install the
+latest version of CORS-Analyzer just uninstall the old version using the
+following command, pip uninstall cors-analyzer pip install --upgrade cors-
+analyzer For upgrade, use the following command, pip install --upgrade cors-
+analyzer For ignore the cache, use the following command, pip install --ignore-
+cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x) latest version
+### How to Use CORS-Finder: ``` For scanning: cat
 txt> | xargs -n1 -P10 python3 corss.py For scanning with output: cat
 txt> | xargs -n1 -P10 python3 corss.py | tee -a
 txt> ``` ### When its vulnerable: If the header returns the Access-Control-
 Allow-Origin: https://vulnerable.com/ Access-Control-Allow-Credentials: true
 its vulnerable Note: Not all the time its seems vulnerable, you have to check
 with cors payload and in the authenticated manner also. Try to exploit and this
 tool is only for indentifying the vulnerable domain Note: In this tool i used
```

### Comparing `CORS-Analyzer-1.0.4/README.md` & `CORS-Analyzer-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CORS-Analyzer
 ## This tools is developed for identifying the vulnerable cors domain
 
-![alt text](lib/banner/cors-analyzer.png)
+![alt text](https://raw.githubusercontent.com/hariharan005/CORS/main/lib/banner/cors-analyzer.png)
 
 ### How to install CORS-Analyzer:
 ```
 git clone https://github.com/hariharan005/CORS.git     
 ls    
 cd CORS
 sudo pip3 install -r requirements.txt 
@@ -23,15 +23,15 @@
 
 If you want to install the latest version of CORS-Analyzer just uninstall the old version using the following command,
     pip uninstall cors-analyzer
     pip install --upgrade cors-analyzer
 
 For upgrade, use the following command,
     pip install --upgrade cors-analyzer
-    
+
 For ignore the cache, use the following command,
     pip install --ignore-cache cors-analyzer
 ```
 ### Python Version:
 * Python 3 (3.x.x) latest version
 
 ### How to Use CORS-Finder:
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # CORS-Analyzer ## This tools is developed for identifying the vulnerable cors
-domain ![alt text](lib/banner/cors-analyzer.png) ### How to install CORS-
-Analyzer: ``` git clone https://github.com/hariharan005/CORS.git ls cd CORS
-sudo pip3 install -r requirements.txt cd lib && chmod +x cors.py sudo ln -s "$
-(pwd)/cors.py" /usr/local/bin/cors-analyzer cors-analyzer ``` Now type "cors-
-analyzer" to access the CORS analyzer tool from anywhere ### How to install
-using pip: ``` For first time installation use the following command, pip
-install cors-analyzer If you want to install the latest version of CORS-
-Analyzer just uninstall the old version using the following command, pip
-uninstall cors-analyzer pip install --upgrade cors-analyzer For upgrade, use
-the following command, pip install --upgrade cors-analyzer For ignore the
-cache, use the following command, pip install --ignore-cache cors-analyzer ```
-### Python Version: * Python 3 (3.x.x) latest version ### How to Use CORS-
-Finder: ``` For scanning: cat
+domain ![alt text](https://raw.githubusercontent.com/hariharan005/CORS/main/
+lib/banner/cors-analyzer.png) ### How to install CORS-Analyzer: ``` git clone
+https://github.com/hariharan005/CORS.git ls cd CORS sudo pip3 install -
+r requirements.txt cd lib && chmod +x cors.py sudo ln -s "$(pwd)/cors.py" /usr/
+local/bin/cors-analyzer cors-analyzer ``` Now type "cors-analyzer" to access
+the CORS analyzer tool from anywhere ### How to install using pip: ``` For
+first time installation use the following command, pip install cors-analyzer If
+you want to install the latest version of CORS-Analyzer just uninstall the old
+version using the following command, pip uninstall cors-analyzer pip install --
+upgrade cors-analyzer For upgrade, use the following command, pip install --
+upgrade cors-analyzer For ignore the cache, use the following command, pip
+install --ignore-cache cors-analyzer ``` ### Python Version: * Python 3 (3.x.x)
+latest version ### How to Use CORS-Finder: ``` For scanning: cat
 txt> | xargs -n1 -P10 python3 corss.py For scanning with output: cat
 txt> | xargs -n1 -P10 python3 corss.py | tee -a
 txt> ``` ### When its vulnerable: If the header returns the Access-Control-
 Allow-Origin: https://vulnerable.com/ Access-Control-Allow-Credentials: true
 its vulnerable Note: Not all the time its seems vulnerable, you have to check
 with cors payload and in the authenticated manner also. Try to exploit and this
 tool is only for indentifying the vulnerable domain Note: In this tool i used
```

### Comparing `CORS-Analyzer-1.0.4/lib/cors.py` & `CORS-Analyzer-1.0.5/lib/cors.py`

 * *Files identical despite different names*

### Comparing `CORS-Analyzer-1.0.4/setup.py` & `CORS-Analyzer-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name="CORS-Analyzer",
-    version= '1.0.4',
+    version= '1.0.5',
     author= 'Hariharan',
     description= 'The cors-analyzer package is used to find the vulnerable CORS domains',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords= ['cors', 'cors-finder', 'cors-analyzer', 'cors misconfiguration', 'cors exploit', 'cors vulnerability'],
     packages=find_packages(),
     entry_points={
```

