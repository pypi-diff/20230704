# Comparing `tmp/limberer-0.2.4.tar.gz` & `tmp/limberer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.2.4.tar", last modified: Mon Jul  3 20:55:18 2023, max compression
+gzip compressed data, was "limberer-0.2.5.tar", last modified: Mon Jul  3 22:29:02 2023, max compression
```

## Comparing `limberer-0.2.4.tar` & `limberer-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.4/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.4/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.4/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 20:55:18.307609 limberer-0.2.4/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.4/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1096 2023-07-03 19:36:54.000000 limberer-0.2.4/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 20:55:18.307609 limberer-0.2.4/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    10631 2023-07-03 19:20:56.000000 limberer-0.2.4/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6354 2023-07-03 20:44:58.000000 limberer-0.2.4/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1099 2023-07-03 20:53:29.000000 limberer-0.2.4/src/limberer/static/assets/base.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.2.4/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     4356 2023-07-03 20:53:23.000000 limberer-0.2.4/src/limberer/static/assets/theme.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.4/src/limberer/static/custom/custom.css
--rw-r--r--   0 jtd       (1000) jtd       (1000)      282 2023-06-28 04:38:31.000000 limberer-0.2.4/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3222 2023-07-03 20:53:41.000000 limberer-0.2.4/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 20:53:46.000000 limberer-0.2.4/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 07:49:58.000000 limberer-0.2.4/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.4/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-03 20:53:50.000000 limberer-0.2.4/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.4/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 20:55:18.307609 limberer-0.2.4/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 20:55:18.000000 limberer-0.2.4/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      738 2023-07-03 20:55:18.000000 limberer-0.2.4/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 20:55:18.000000 limberer-0.2.4/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 20:55:18.000000 limberer-0.2.4/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 20:55:18.000000 limberer-0.2.4/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 20:55:18.000000 limberer-0.2.4/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.5/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.5/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.5/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 22:29:02.651794 limberer-0.2.5/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.5/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1108 2023-07-03 22:21:38.000000 limberer-0.2.5/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 22:29:02.651794 limberer-0.2.5/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.647794 limberer-0.2.5/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    10974 2023-07-03 22:19:52.000000 limberer-0.2.5/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6354 2023-07-03 22:21:03.000000 limberer-0.2.5/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1099 2023-07-03 20:53:29.000000 limberer-0.2.5/src/limberer/static/assets/base.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.2.5/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     4331 2023-07-03 22:26:38.000000 limberer-0.2.5/src/limberer/static/assets/theme.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.5/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.2.5/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      355 2023-07-03 22:26:44.000000 limberer-0.2.5/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3246 2023-07-03 22:20:56.000000 limberer-0.2.5/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 20:53:46.000000 limberer-0.2.5/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 07:49:58.000000 limberer-0.2.5/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.5/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-03 20:53:50.000000 limberer-0.2.5/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.5/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.2.4/LICENSE` & `limberer-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/PKG-INFO` & `limberer-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.4
+Version: 0.2.5
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.4/README.md` & `limberer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/pyproject.toml` & `limberer-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
@@ -39,8 +39,8 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-"limberer.static" = ["*", "assets/*", "custom/*", "sections/*", "templates/*"]
+"limberer.static" = ["*", "assets/*", "custom/*", "sections/*", "templates/*", "images/*"]
```

### Comparing `limberer-0.2.4/src/limberer/__init__.py` & `limberer-0.2.5/src/limberer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from collections.abc import Callable
 import chevron
 import weasyprint
 import markdown # temporary
 import subprocess
 import io
 from bs4 import BeautifulSoup
+import re
 
 from .pf import entrypoint
 
 # disable remote url resolution and path traversal
 def fetcher(url):
   u = None
   if url.startswith("file://"):
@@ -72,14 +73,15 @@
 # >>> chevron.render('Hello, {{#mustache}}{{#__class__.__bases__}}{{#__subclasses__}}{{.}}{{/__subclasses__}}{{/__class__.__bases__}}{{/mustache}}!', {'mustache': 'World'})
 # 'Hello, no soup for you.!'
 # >>> chevron.render('Hello, {{#mustache}}{{#upper}}{{.}}{{/upper}}{{/mustache}}!', {'mustache': 'world'})
 # 'Hello, no soup for you!!'
 
 
 footnotecount = 1
+isheader = re.compile('h[1-9]')
 
 def convert(path, opts, toc, args):
   #print("convert(" + repr(path) + ")")
   proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
   if proc1.returncode != 0:
     sys.stderr.write("error running initial pandoc command: \n")
     sys.stderr.buffer.write(proc1.stderr)
@@ -226,14 +228,22 @@
       md = markdown.Markdown(extensions=["meta"])
       html = md.convert(content)
       opts = md.Meta | section
       opts['section_name'] = section_name
       html = convert(section_path, opts, toc, args)
       footnotes = ""
       soup = BeautifulSoup(html, 'html.parser')
+      _sns = soup.find_all(lambda e: e.name == 'section' and e.attrs.get('id')!=None)
+      for _sn in _sns:
+        _snc = [c for c in _sn.children if c != "\n"]
+        if len(_snc) > 0:
+          if re.match(isheader, _snc[0].name):
+            _snc[0]['id'] = _sn['id']
+            del _sn['id']
+
       _fns = soup.find(id="footnotes")
       if _fns is not None:
         _fns = _fns.extract()
         _fns.ol['start'] = str(footnotecount)
         _fns.ol['style'] = f"counter-reset:list-item {footnotecount}; counter-increment:list-item -1;"
         __fns = [c for c in _fns.ol.children if c != "\n"]
         del _fns['id']
```

### Comparing `limberer-0.2.4/src/limberer/pf.py` & `limberer-0.2.5/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/src/limberer/static/assets/base.css` & `limberer-0.2.5/src/limberer/static/assets/base.css`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/src/limberer/static/assets/logo.svg` & `limberer-0.2.5/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/src/limberer/static/assets/theme.css` & `limberer-0.2.5/src/limberer/static/assets/theme.css`

 * *Files 2% similar despite different names*

```diff
@@ -188,25 +188,26 @@
   justify-content: center;
   position: absolute;
   bottom: 0px;
   width: 100%;
 }
 
 article {
-  display: flex;
-  flex-direction: column;
   height: 8.5in;
   width: 6.5in;
-  align-items: flex-start;
+}
+
+article:not(#cover) {
+  display: flex;
+  flex-direction: column;
 }
 
 article>div.article-body {
   width: 6.5in;
   flex: 1 1 auto;
-  align-self: stretch;
 }
 
 article ul {
   list-style: none;
   padding-left: 0;
 }
```

### Comparing `limberer-0.2.4/src/limberer/static/sections/example.md` & `limberer-0.2.5/src/limberer/static/sections/example.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,30 +86,34 @@
 ![test](./images/test1.jpg){style="width: 30%;"}
 
 Test foo bar.
 
 <div class="two-col-fig">
 ![test](./images/test1.jpg)
 <div style="width: 40%">
-## Test
+## Test1
 
-Hello world. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
+Hello world1. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
 eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
 veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
 cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
 proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
+
+## Test1b
+
+Foo bar.
 </div>
 </div>
 
 <div class="two-col-fig">
 <div style="width: 60%">
 ## Test2
 
-Hello world. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
+Hello world2. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
 eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
 veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
 cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
 proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
 </div>
 ![test](./images/test1.jpg){style="width: 1.5in;" figstyle="color: red; width: 35%;" figclass="testing aaa"}
```

#### html2text {}

```diff
@@ -21,21 +21,22 @@
 sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
 minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
 commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
 esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
 non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. !
 [test](./images/test1.jpg){style="width: 30%;"} Test foo bar.
 ![test](./images/test1.jpg)
-## Test Hello world. Lorem ipsum dolor sit amet, consectetur adipiscing elit,
+## Test1 Hello world1. Lorem ipsum dolor sit amet, consectetur adipiscing elit,
 sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
 minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
 commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
 esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
-non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
-## Test2 Hello world. Lorem ipsum dolor sit amet, consectetur adipiscing elit,
+non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. ##
+Test1b Foo bar.
+## Test2 Hello world2. Lorem ipsum dolor sit amet, consectetur adipiscing elit,
 sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
 minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
 commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
 esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
 non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
 ![test](./images/test1.jpg){style="width: 1.5in;" figstyle="color: red; width:
 35%;" figclass="testing aaa"}
```

### Comparing `limberer-0.2.4/src/limberer/static/sections/example2.md` & `limberer-0.2.5/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/src/limberer/static/templates/cover.html` & `limberer-0.2.5/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/src/limberer/static/templates/toc.html` & `limberer-0.2.5/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.4/src/limberer.egg-info/PKG-INFO` & `limberer-0.2.5/src/limberer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.4
+Version: 0.2.5
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.4/src/limberer.egg-info/SOURCES.txt` & `limberer-0.2.5/src/limberer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 src/limberer.egg-info/requires.txt
 src/limberer.egg-info/top_level.txt
 src/limberer/static/project.toml
 src/limberer/static/assets/base.css
 src/limberer/static/assets/logo.svg
 src/limberer/static/assets/theme.css
 src/limberer/static/custom/custom.css
+src/limberer/static/images/test1.jpg
 src/limberer/static/sections/example.md
 src/limberer/static/sections/example2.md
 src/limberer/static/templates/base.html
 src/limberer/static/templates/cover.html
 src/limberer/static/templates/section.html
 src/limberer/static/templates/toc.html
```

