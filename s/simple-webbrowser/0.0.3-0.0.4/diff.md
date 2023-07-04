# Comparing `tmp/simple_webbrowser-0.0.3.tar.gz` & `tmp/simple_webbrowser-0.0.4.tar.gz`

## Comparing `simple_webbrowser-0.0.3.tar` & `simple_webbrowser-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.3/src/simple_webbrowser/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.3/src/simple_webbrowser/simple_webbrowser.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.3/LICENSE
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.3/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/src/simple_webbrowser/__init__.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/src/simple_webbrowser/simple_webbrowser.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/PKG-INFO
```

### Comparing `simple_webbrowser-0.0.3/src/simple_webbrowser/simple_webbrowser.py` & `simple_webbrowser-0.0.4/src/simple_webbrowser/simple_webbrowser.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,60 +9,77 @@
     if platform == "win32":
         webbrowser.open(url)
         # trust me: this part is not a total waste
     elif platform == "linux" or "darwin":
         webbrowser.open(url)
         
 def Google(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open('https://www.google.com/search?q='+typed)
+
+def Brave(query):
+    query = str(query)
+    for i in query:
+        typed = query.replace(' ', '+')
+    webbrowser.open('https://search.brave.com/search?q='+typed)
                 
 def Bing(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open('https://www.bing.com/search?q='+typed)
                 
 def Yahoo(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open("https://search.yahoo.com/search?p="+typed)
                 
 def DuckDuckGo(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open("https://duckduckgo.com/?q="+typed)
                 
 def YouTube(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open("https://www.youtube.com/results?search_query="+typed)
                 
 def Ecosia(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '%20')
     webbrowser.open("https://www.ecosia.org/search?method=index&q="+typed)
         
 def StackOverflow(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open("https://stackoverflow.com/search?q="+typed)
                 
 def SoundCloud(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '%20')
     webbrowser.open("https://soundcloud.com/search?q="+typed)
                 
 def Archive(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open("https://archive.org/search?query="+typed)
                 
 def Qwant(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open("https://www.qwant.com/?q="+typed)
                 
 def SpotifyOnline(query):
+    query = str(query)
     for i in query:
         typed = query.replace(' ', '%20')
     webbrowser.open("https://open.spotify.com/search/"+typed)
```

### Comparing `simple_webbrowser-0.0.3/LICENSE` & `simple_webbrowser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_webbrowser-0.0.3/pyproject.toml` & `simple_webbrowser-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple_webbrowser"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="MF366", email="real_mf366@yahoo.com" },
 ]
 description = "A better webbrowser. Just. For. You."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_webbrowser-0.0.3/PKG-INFO` & `simple_webbrowser-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_webbrowser
-Version: 0.0.3
+Version: 0.0.4
 Summary: A better webbrowser. Just. For. You.
 Project-URL: Homepage, https://github.com/MF366-Coding/simple_webbrowser
 Project-URL: Bug Tracker, https://github.com/MF366-Coding/simple_webbrowser/issues
 Author-email: MF366 <real_mf366@yahoo.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,10 +15,22 @@
 # simple_webbrowser
 `simple_webbrowser` is a module that makes `webbrowser` module way more simple to work with.
 
 # License
 This module is licensed under the MIT License.
 
 # PyPI
-This module is not available on PyPI.
+This module is also available on PyPI.
 
-Instead, it's here, on GitHub... 
+# How to install?
+Use the following command on the commandline:
+```
+pip install simple_webbrowser
+```
+
+# How to use?
+Import it like this:
+```
+from simple_webbrowser import simple_webbrowser
+
+# Afterwards, just use it :)
+```
```

