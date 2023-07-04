# Comparing `tmp/limberer-0.2.6.tar.gz` & `tmp/limberer-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.2.6.tar", last modified: Mon Jul  3 23:37:27 2023, max compression
+gzip compressed data, was "limberer-0.3.tar", last modified: Tue Jul  4 01:58:34 2023, max compression
```

## Comparing `limberer-0.2.6.tar` & `limberer-0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.6/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.6/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.6/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 23:37:27.715332 limberer-0.2.6/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.6/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1108 2023-07-03 23:37:04.000000 limberer-0.2.6/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 23:37:27.715332 limberer-0.2.6/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    10974 2023-07-03 22:19:52.000000 limberer-0.2.6/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6354 2023-07-03 22:21:03.000000 limberer-0.2.6/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5164 2023-07-03 23:34:10.000000 limberer-0.2.6/src/limberer/static/assets/core.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.2.6/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-03 23:36:07.000000 limberer-0.2.6/src/limberer/static/assets/style.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.6/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.2.6/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      355 2023-07-03 22:26:44.000000 limberer-0.2.6/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3246 2023-07-03 22:20:56.000000 limberer-0.2.6/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 20:53:46.000000 limberer-0.2.6/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.2.6/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.6/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-03 20:53:50.000000 limberer-0.2.6/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.6/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.3/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.3/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.3/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     8384 2023-07-04 01:58:34.167821 limberer-0.3/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6324 2023-07-04 01:31:34.000000 limberer-0.3/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1092 2023-07-04 01:57:18.000000 limberer-0.3/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-04 01:58:34.167821 limberer-0.3/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.163821 limberer-0.3/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11728 2023-07-04 01:56:49.000000 limberer-0.3/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6548 2023-07-04 01:49:09.000000 limberer-0.3/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5164 2023-07-03 23:34:10.000000 limberer-0.3/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.3/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-03 23:36:07.000000 limberer-0.3/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.3/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.3/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      363 2023-07-04 00:11:03.000000 limberer-0.3/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3269 2023-07-04 00:13:53.000000 limberer-0.3/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 20:53:46.000000 limberer-0.3/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.3/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.3/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-04 01:55:47.000000 limberer-0.3/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.3/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-04 01:58:34.167821 limberer-0.3/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     8384 2023-07-04 01:58:34.000000 limberer-0.3/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-04 01:58:34.000000 limberer-0.3/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-04 01:58:34.000000 limberer-0.3/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-04 01:58:34.000000 limberer-0.3/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-04 01:58:34.000000 limberer-0.3/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-04 01:58:34.000000 limberer-0.3/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.2.6/LICENSE` & `limberer-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/pyproject.toml` & `limberer-0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.2.6"
+version = "0.3"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
@@ -17,15 +17,14 @@
   "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
   "panflute",
   "chevron",
   "weasyprint",
   "toml",
-  "markdown",
   "pillow",
   "beautifulsoup4",
 ]
 
 [project.urls]
 repository = "https://github.com/ChaosData/limberer"
```

### Comparing `limberer-0.2.6/src/limberer/__init__.py` & `limberer-0.3/src/limberer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 import os.path
 import shutil
 import toml
 from collections.abc import Callable
 import chevron
 import weasyprint
-import markdown # temporary
+#import markdown # temporary
 import subprocess
 import io
 from bs4 import BeautifulSoup
 import re
 
 from .pf import entrypoint
 
@@ -71,14 +71,21 @@
   return r
 chevron.renderer._get_key = fake_get_key
 # >>> chevron.render('Hello, {{#mustache}}{{#__class__.__bases__}}{{#__subclasses__}}{{.}}{{/__subclasses__}}{{/__class__.__bases__}}{{/mustache}}!', {'mustache': 'World'})
 # 'Hello, no soup for you.!'
 # >>> chevron.render('Hello, {{#mustache}}{{#upper}}{{.}}{{/upper}}{{/mustache}}!', {'mustache': 'world'})
 # 'Hello, no soup for you!!'
 
+def open_subpath(path, mode='r'):
+  cwd = os.path.abspath(".")
+  target = os.path.abspath(path)
+  if not target.startswith(cwd + os.sep):
+    print(f"error: invalid path {repr(path)} references outside of project directory.")
+    sys.exit(1)
+  return open(path, mode)
 
 footnotecount = 1
 isheader = re.compile('h[1-9]')
 
 def convert(path, opts, toc, args):
   #print("convert(" + repr(path) + ")")
   proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
@@ -95,15 +102,17 @@
   # run the panflute filter
   sys.argv = ["html"]
   iw = io.StringIO(o1)
   ow = io.StringIO("")
 
   headers = []
   _headers = []
-  r = entrypoint(iw, ow, _headers)
+  _meta = []
+  r = entrypoint(iw, ow, _headers, _meta)
+  opts.update(_meta[0][0])
   ow.seek(0)
   o2 = ow.read()
 
   if len(_headers) == 1:
     headers = _headers[0]
 
   if "columns" in opts:
@@ -213,77 +222,86 @@
   toc_template = open('templates/toc.html', 'r').read()
 
   body = ''
 
   sections = []
   toc = []
 
-  for section in config['sections']:
+  for i in range(len(config['sections'])):
+    section = config['sections'][i]
     if section['type'] == 'section':
       # markdown
       section_name = section['name']
       section_path = 'sections/{}.md'.format(section['name'])
-      content = open(section_path, 'rb').read()
+      content = open_subpath(section_path, 'rb').read()
       #print(repr(content))
-      content = content.decode('utf-8')
-      md = markdown.Markdown(extensions=["meta"])
-      html = md.convert(content)
-      opts = md.Meta | section
+      #content = content.decode('utf-8')
+      #md = markdown.Markdown(extensions=["meta"])
+      #html = md.convert(content)
+      #opts = md.Meta | section
+      opts = {} | section
       opts['section_name'] = section_name
       html = convert(section_path, opts, toc, args)
+      #print("opts: " + repr(opts))
       footnotes = ""
       soup = BeautifulSoup(html, 'html.parser')
       _sns = soup.find_all(lambda e: e.name == 'section' and e.attrs.get('id')!=None)
       for _sn in _sns:
         _snc = [c for c in _sn.children if c != "\n"]
         if len(_snc) > 0:
           if re.match(isheader, _snc[0].name):
             _snc[0]['id'] = _sn['id']
             del _sn['id']
+      #_iders = soup.find_all(lambda e: e.attrs.get('id')!=None)
+      #for _ider in _iders:
 
       _fns = soup.find(id="footnotes")
       if _fns is not None:
         _fns = _fns.extract()
         _fns.ol['start'] = str(footnotecount)
         _fns.ol['style'] = f"counter-reset:list-item {footnotecount}; counter-increment:list-item -1;"
         __fns = [c for c in _fns.ol.children if c != "\n"]
         del _fns['id']
         for __fn in __fns:
           id = __fn['id']
-          nid = section_name + "-" + id
+          #nid = f"{i}-{section_name}-{id}"
+          nid = f"{section_name}-{id}"
           __fn['id'] = nid
           __fnx = soup.find(id=id)
           if __fnx is not None:
             __fnx['id'] = nid
         for _a in soup.find_all(class_="footnote-ref"):
-          _a['id'] = section_name + "-" + _a['id']
-          _a['href'] = '#' + section_name + "-" + _a['href'][1:]
+          #_a['id'] = f"{i}-{section_name}-{_a['id']}"
+          _a['id'] = f"{section_name}-{_a['id']}"
+          #_a['href'] = f"#{i}-{section_name}-{_a['href'][1:]}"
+          _a['href'] = f"#{section_name}-{_a['href'][1:]}"
           _a.sup.string = str(footnotecount - 1 + int(_a.sup.string))
         for _a in _fns.find_all(class_="footnote-back"):
-          _a['href'] = '#' + section_name + "-" + _a['href'][1:]
+          #_a['href'] = f"#{i}-{section_name}-{_a['href'][1:]}"
+          _a['href'] = f"#{section_name}-{_a['href'][1:]}"
         _fns.name = 'div'
         footnotecount += len(__fns)
 
         footnotes = str(_fns)
         html = str(soup)
 
       opts['html'] = html
       opts['footnotes'] = footnotes
       opts['opts'] = opts # we occasionally need top.down.variable.paths to resolve abiguity
       template = section_template
       if "alt" in section:
-        template = open('templates/{}.html'.format(section['alt']), 'r').read()
+        template = open_subpath('templates/{}.html'.format(section['alt']), 'r').read()
       r = chevron.render(template, opts)
       sections.append(r)
     elif section['type'] == 'toc':
       # defer until after we get through everything else
       sections.append(section)
     else:
       # assume in templates/
-      template = open('templates/{}.html'.format(section['type']), 'r').read()
+      template = open_subpath('templates/{}.html'.format(section['type']), 'r').read()
       r = chevron.render(template, config)
       sections.append(r)
       if section['type'] != 'cover' and "title" in section:
         toc.append(opts | {"name": section['type'], "issubsection": False})
 
   for section in sections:
     if type(section) == str:
```

### Comparing `limberer-0.2.6/src/limberer/pf.py` & `limberer-0.3/src/limberer/pf.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import os
 import platform
 import base64
 from PIL import Image
 
 titlecounter = 0
 headers = []
+metadata = []
 figurecount = 1
 
 def stringify(content):
   out = []
   for part in content:
     if isinstance(part, pf.Str):
       out.append(str(part)[4:-1])
@@ -48,15 +49,16 @@
 
 def header(elem, doc):
   global titlecounter
   global checkboxcounter
   global figurecount
 
   if isinstance(elem, pf.Doc):
-    pass
+    m = {k: elem.get_metadata(k) for k in elem.metadata.content}
+    metadata.append(m)
   elif isinstance(elem, pf.Header):
     #with open("/tmp/log.txt", "a") as fd:
     #  fd.write(repr(elem) + "\n")
     headers.append(elem)
     elem.identifier = elem.identifier + str(len(headers))
   #elif isinstance(elem, pf.Note):
   #  print("footnote: " + repr(elem))
@@ -163,19 +165,23 @@
         return pf.RawInline(html, format='html')
       else:
         sys.stderr.write("image path bad: " + f + "\n")
         sys.stderr.write(os.path.realpath(f) + "\n")
         sys.stderr.write(os.path.join(os.path.realpath('.'), f) + "\n")
   return elem
 
-def entrypoint(_in=None, _out=None, _headers=None):
+def entrypoint(_in=None, _out=None, _headers=None, _meta=None):
   global headers
+  global metadata
   headers = []
   if _in is None:
     pf.run_filter(header)
   else:
     if _headers != None:
       _headers.append(headers)
+    if _meta != None:
+      metadata = []
+      _meta.append(metadata)
     return pf.run_filter(header, input_stream=_in, output_stream=_out)
 
 if __name__ == "__main__":
   entrypoint()
```

### Comparing `limberer-0.2.6/src/limberer/static/assets/core.css` & `limberer-0.3/src/limberer/static/assets/core.css`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer/static/assets/logo.svg` & `limberer-0.3/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer/static/assets/style.css` & `limberer-0.3/src/limberer/static/assets/style.css`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer/static/images/test1.jpg` & `limberer-0.3/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer/static/sections/example.md` & `limberer-0.3/src/limberer/static/sections/example.md`

 * *Files 3% similar despite different names*

```diff
@@ -112,10 +112,10 @@
 Hello world2. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
 eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
 veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
 cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
 proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
 </div>
-![test](./images/test1.jpg){style="width: 1.5in;" figstyle="color: red; width: 35%;" figclass="testing aaa"}
+![test](./images/test1.jpg){style="width: 1.5in; border: 1px solid red;" figstyle="color: red; width: 35%;" figclass="testing aaa"}
 </div>
```

#### html2text {}

```diff
@@ -34,9 +34,9 @@
 Test1b Foo bar.
 ## Test2 Hello world2. Lorem ipsum dolor sit amet, consectetur adipiscing elit,
 sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
 minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
 commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit
 esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
 non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
-![test](./images/test1.jpg){style="width: 1.5in;" figstyle="color: red; width:
-35%;" figclass="testing aaa"}
+![test](./images/test1.jpg){style="width: 1.5in; border: 1px solid red;"
+figstyle="color: red; width: 35%;" figclass="testing aaa"}
```

### Comparing `limberer-0.2.6/src/limberer/static/sections/example2.md` & `limberer-0.3/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer/static/templates/cover.html` & `limberer-0.3/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer/static/templates/toc.html` & `limberer-0.3/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.6/src/limberer.egg-info/SOURCES.txt` & `limberer-0.3/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

