# Comparing `tmp/colab-xterm-0.1.2.tar.gz` & `tmp/colab-xterm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/colab-xterm/colab-xterm/dist/tmpwiztwafo/colab-xterm-0.1.2.tar", last modified: Fri Feb 11 09:46:30 2022, max compression
+gzip compressed data, was "colab-xterm-0.2.0.tar", last modified: Tue Jul  4 14:39:02 2023, max compression
```

## Comparing `colab-xterm-0.1.2.tar` & `colab-xterm-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colabxterm/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/xterm.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colabxterm/client/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colabxterm/client/dist/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/client/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/client/dist/main.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)   426644 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/client/dist/main.js
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/colabxterm/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colab_xterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colab_xterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colab_xterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colab_xterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colab_xterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/colab_xterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-02-11 09:46:30.000000 colab-xterm-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-02-11 09:46:01.000000 colab-xterm-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/colab_xterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-04 14:39:01.000000 colab-xterm-0.2.0/colab_xterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-04 14:39:01.000000 colab-xterm-0.2.0/colab_xterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:39:01.000000 colab-xterm-0.2.0/colab_xterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 14:39:01.000000 colab-xterm-0.2.0/colab_xterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 14:39:01.000000 colab-xterm-0.2.0/colab_xterm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/colabxterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/colabxterm/client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/colabxterm/client/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/client/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   426644 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/client/dist/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/client/dist/main.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/colabxterm/xterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:39:02.003524 colab-xterm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-04 14:38:25.000000 colab-xterm-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `colab-xterm-0.1.2/colabxterm/xterm.py` & `colab-xterm-0.2.0/colabxterm/xterm.py`

 * *Files identical despite different names*

### Comparing `colab-xterm-0.1.2/colabxterm/client/dist/main.js` & `colab-xterm-0.2.0/colabxterm/client/dist/main.js`

 * *Files identical despite different names*

### Comparing `colab-xterm-0.1.2/colabxterm/manager.py` & `colab-xterm-0.2.0/colabxterm/manager.py`

 * *Files identical despite different names*

### Comparing `colab-xterm-0.1.2/colabxterm/notebook.py` & `colab-xterm-0.2.0/colabxterm/notebook.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,14 +72,30 @@
         import socket
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             return s.connect_ex(('localhost', port)) == 0
 
     parsed_args = shlex.split(args_string, comments=True, posix=True)
     height = 800
     port = 10000
+
+    # Setup parameter from parsed_args to support the following format.
+    # %xterm height=300 port=10001
+    for parameter in parsed_args:
+        kv_pair:list[str] = str(parameter).split('=')
+        if len(kv_pair) == 2:
+            k = kv_pair[0]
+            v = kv_pair[1]
+            if v.isdigit():
+                if k == "height":
+                    height = int(v)
+                elif k == "port":
+                    port = int(v)
+    # Clean parsed_args as an empty list to avoid the disability of the magic line command.
+    parsed_args=[]
+
     while True:
         if not is_port_in_use(port):
             break
         port = port+1
 
     manager.start(parsed_args, port)
     fn = {
```

### Comparing `colab-xterm-0.1.2/LICENSE` & `colab-xterm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `colab-xterm-0.1.2/setup.py` & `colab-xterm-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `colab-xterm-0.1.2/colab_xterm.egg-info/PKG-INFO` & `colab-xterm-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: colab-xterm
-Version: 0.1.2
-Summary: Open a terminal in colab, including the free tier.
-Home-page: https://github.com/InfuseAI/colab-xterm
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/InfuseAI/colab-xterm/issues
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # colab-xterm
 Colab-xterm allows you to open a terminal in a cell.
 
 # Usage
 
 1. Install package and load the extension
     ```
@@ -31,10 +18,20 @@
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/infuseai/colab-xterm/blob/main/demo.ipynb)
 
 # Features
 - TTY support
 - Does not block your kernel
 
-# Screenshots
-![](assets/colab-xterm.png)
+# Options
 
+```
+%xterm height=1000 port=10001
+```
+
+option | description
+-------|-----------
+height | The height of the terminal panel
+port | The server port
+
+# Screenshots
+![](assets/colab-xterm.png)
```

