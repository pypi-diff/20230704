# Comparing `tmp/textbasedlib-1.0.tar.gz` & `tmp/textbasedlib-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbasedlib-1.0.tar", last modified: Tue Jul  4 12:01:11 2023, max compression
+gzip compressed data, was "textbasedlib-1.2.tar", last modified: Tue Jul  4 12:08:55 2023, max compression
```

## Comparing `textbasedlib-1.0.tar` & `textbasedlib-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 12:01:11.761152 textbasedlib-1.0/
--rw-rw-rw-   0        0        0     1099 2023-07-03 23:21:18.000000 textbasedlib-1.0/LICENSE
--rw-rw-rw-   0        0        0     1386 2023-07-04 12:01:11.757156 textbasedlib-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-07-04 11:05:11.000000 textbasedlib-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 12:01:11.761152 textbasedlib-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1009 2023-07-04 12:00:37.000000 textbasedlib-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:01:11.733193 textbasedlib-1.0/textbasedlib/
--rw-rw-rw-   0        0        0       34 2023-07-04 11:55:43.000000 textbasedlib-1.0/textbasedlib/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-07-03 23:19:59.000000 textbasedlib-1.0/textbasedlib/plugin_manager.py
--rw-rw-rw-   0        0        0     7672 2023-07-04 10:58:19.000000 textbasedlib-1.0/textbasedlib/tblib.py
-drwxrwxrwx   0        0        0        0 2023-07-04 12:01:11.757156 textbasedlib-1.0/textbasedlib.egg-info/
--rw-rw-rw-   0        0        0     1386 2023-07-04 12:01:11.000000 textbasedlib-1.0/textbasedlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-04 12:01:11.000000 textbasedlib-1.0/textbasedlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 12:01:11.000000 textbasedlib-1.0/textbasedlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 12:01:11.000000 textbasedlib-1.0/textbasedlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 12:01:11.000000 textbasedlib-1.0/textbasedlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 12:08:55.462142 textbasedlib-1.2/
+-rw-rw-rw-   0        0        0     1099 2023-07-03 23:21:18.000000 textbasedlib-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1386 2023-07-04 12:08:55.461144 textbasedlib-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-07-04 11:05:11.000000 textbasedlib-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 12:08:55.462142 textbasedlib-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2023-07-04 12:06:32.000000 textbasedlib-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:08:55.444189 textbasedlib-1.2/textbasedlib/
+-rw-rw-rw-   0        0        0       34 2023-07-04 11:55:43.000000 textbasedlib-1.2/textbasedlib/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-07-03 23:19:59.000000 textbasedlib-1.2/textbasedlib/plugin_manager.py
+-rw-rw-rw-   0        0        0     7676 2023-07-04 12:04:03.000000 textbasedlib-1.2/textbasedlib/tblib.py
+drwxrwxrwx   0        0        0        0 2023-07-04 12:08:55.458151 textbasedlib-1.2/textbasedlib.egg-info/
+-rw-rw-rw-   0        0        0     1386 2023-07-04 12:08:55.000000 textbasedlib-1.2/textbasedlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-04 12:08:55.000000 textbasedlib-1.2/textbasedlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 12:08:55.000000 textbasedlib-1.2/textbasedlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 12:08:55.000000 textbasedlib-1.2/textbasedlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 12:08:55.000000 textbasedlib-1.2/textbasedlib.egg-info/top_level.txt
```

### Comparing `textbasedlib-1.0/LICENSE` & `textbasedlib-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textbasedlib-1.0/PKG-INFO` & `textbasedlib-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textbasedlib
-Version: 1.0
+Version: 1.2
 Summary: A library for creating text-based games in the terminal
 Home-page: https://tblib-docs.devplodocus.repl.co
 Author: gugu256 (Gustave Dufresne-Walter)
 Author-email: gugu256@mail.com
 License: MIT License
 Keywords: python,lightweight,game-development,terminal-based,terminal-game,text-based-game
 Classifier: Intended Audience :: Developers
```

### Comparing `textbasedlib-1.0/README.md` & `textbasedlib-1.2/README.md`

 * *Files identical despite different names*

### Comparing `textbasedlib-1.0/setup.py` & `textbasedlib-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0'
+VERSION = '1.2'
 DESCRIPTION = 'A library for creating text-based games in the terminal'
 LONG_DESCRIPTION = open("README.md").read()
 # Setting up
 setup(
     name="textbasedlib",
     version=VERSION,
     author="gugu256 (Gustave Dufresne-Walter)",
```

### Comparing `textbasedlib-1.0/textbasedlib/plugin_manager.py` & `textbasedlib-1.2/textbasedlib/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `textbasedlib-1.0/textbasedlib/tblib.py` & `textbasedlib-1.2/textbasedlib/tblib.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 try:
   arg_ = sys.argv[1]
   if arg_ == "new_project":
     os.mkdir(sys.argv[2])
     os.chdir(sys.argv[2])
     ostype = platform.system()
-    cmd('echo ' + "from textbasedlib import tblib" + " > main.py")
+    cmd('echo ' + "import textbasedlib.tblib as tblib" + " > main.py")
     cmd('echo ' + "Our adventure is set in the fair town of Reinsburg.. " + '> dialogs.txt')
     print(f"{sys.argv[2]} Project created !")
     input("Press enter to continue./")
 except:
   pass
 
 files = listdir(getcwd())
```

### Comparing `textbasedlib-1.0/textbasedlib.egg-info/PKG-INFO` & `textbasedlib-1.2/textbasedlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textbasedlib
-Version: 1.0
+Version: 1.2
 Summary: A library for creating text-based games in the terminal
 Home-page: https://tblib-docs.devplodocus.repl.co
 Author: gugu256 (Gustave Dufresne-Walter)
 Author-email: gugu256@mail.com
 License: MIT License
 Keywords: python,lightweight,game-development,terminal-based,terminal-game,text-based-game
 Classifier: Intended Audience :: Developers
```

