# Comparing `tmp/limberer-0.2.5.tar.gz` & `tmp/limberer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.2.5.tar", last modified: Mon Jul  3 22:29:02 2023, max compression
+gzip compressed data, was "limberer-0.2.6.tar", last modified: Mon Jul  3 23:37:27 2023, max compression
```

## Comparing `limberer-0.2.5.tar` & `limberer-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.5/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.5/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.5/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 22:29:02.651794 limberer-0.2.5/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.5/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1108 2023-07-03 22:21:38.000000 limberer-0.2.5/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 22:29:02.651794 limberer-0.2.5/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.647794 limberer-0.2.5/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    10974 2023-07-03 22:19:52.000000 limberer-0.2.5/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6354 2023-07-03 22:21:03.000000 limberer-0.2.5/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1099 2023-07-03 20:53:29.000000 limberer-0.2.5/src/limberer/static/assets/base.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.2.5/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     4331 2023-07-03 22:26:38.000000 limberer-0.2.5/src/limberer/static/assets/theme.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.5/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.2.5/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      355 2023-07-03 22:26:44.000000 limberer-0.2.5/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3246 2023-07-03 22:20:56.000000 limberer-0.2.5/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 20:53:46.000000 limberer-0.2.5/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 07:49:58.000000 limberer-0.2.5/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.5/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-03 20:53:50.000000 limberer-0.2.5/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.5/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 22:29:02.651794 limberer-0.2.5/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 22:29:02.000000 limberer-0.2.5/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.2.6/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.2.6/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.2.6/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 23:37:27.715332 limberer-0.2.6/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1347 2023-06-28 11:10:47.000000 limberer-0.2.6/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1108 2023-07-03 23:37:04.000000 limberer-0.2.6/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-03 23:37:27.715332 limberer-0.2.6/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    10974 2023-07-03 22:19:52.000000 limberer-0.2.6/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6354 2023-07-03 22:21:03.000000 limberer-0.2.6/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5164 2023-07-03 23:34:10.000000 limberer-0.2.6/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.2.6/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-03 23:36:07.000000 limberer-0.2.6/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.2.6/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.2.6/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      355 2023-07-03 22:26:44.000000 limberer-0.2.6/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3246 2023-07-03 22:20:56.000000 limberer-0.2.6/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1605 2023-07-03 20:53:46.000000 limberer-0.2.6/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.2.6/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.2.6/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      346 2023-07-03 20:53:50.000000 limberer-0.2.6/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      810 2023-06-28 13:19:57.000000 limberer-0.2.6/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-03 23:37:27.715332 limberer-0.2.6/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     3409 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       64 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-03 23:37:27.000000 limberer-0.2.6/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.2.5/LICENSE` & `limberer-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/PKG-INFO` & `limberer-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.5
+Version: 0.2.6
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.5/README.md` & `limberer-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/pyproject.toml` & `limberer-0.2.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.2.5/src/limberer/__init__.py` & `limberer-0.2.6/src/limberer/__init__.py`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/pf.py` & `limberer-0.2.6/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/static/assets/logo.svg` & `limberer-0.2.6/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/static/assets/theme.css` & `limberer-0.2.6/src/limberer/static/assets/core.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,88 @@
 @page {
   @top-left {
+    /* logo */
     background: url(logo.svg) no-repeat center;
     background-size: 1in;
     width: 1.75in;
     height: auto;
     content: '';
     display: inline-block;
     float: left;
     margin-left: -0.6in;
   }
   @top-center {
-    background: #000000;
+    /* header line */
+    background: black;
     content: '';
-    height: .01in;
-    opacity: .5;
+    height: 0.01in;
+    opacity: 0.5;
     width: 7.4375in;
     margin-bottom: 0.25in;
     margin-left: 0in;
   }
   @bottom-right {
-    background: #B57EDC;
+    /* page number */
+    background: black;
     color: #ffffff;
     content: counter(page);
     height: 0.4in;
     text-align: center;
     width: 0.4in;
   }
   @bottom-center {
-    /*content: "© <year> Example Corp.",*/
-    color: #000000;
+    content: none;
+    color: black;
+    opacity: 0.5;
     font-size: 6pt;
     text-align: left;
     margin-top: 0.25in;
     margin-left: -0.25in;
     margin-right: -0.25in;
   }
   size: Letter;
   margin-top: 1.5in;
   margin-left: 1in;
   margin-right: 1in;
   margin-bottom: 1in;
 }
 @page cover {
   @top-left {
-    background: url(logo.svg) no-repeat center;
-    background-size: 1in;
-    width: 1.75in;
-    height: auto;
-    content: '';
-    display: inline-block;
-    float: left;
+    /* fixup logo placement due to different margins on cover */
     margin-left: 0.4in;
   }
   @top-right { content: none }
   @bottom-left { content: none }
-  @bottom-center { background: #ff0000; width: 100%; content: none }
+  @bottom-center { width: 100%; content: none }
   @bottom-right { content: none }
   margin-left: 0;
   margin-right: 0;
   margin-bottom: 0;
 }
 
 html {
-  color: #393939;
+  color: black;
   font-family: Arial;
   font-size: 10pt;
   font-weight: 300;
   line-height: 1.0;
 }
 
 strong {
-  font-family: Arial;
   font-weight: bold;
 }
 
 body {
   margin: 0;
   counter-reset: figurecount;
 }
 
 #title {
   page: cover;
-  margin: 0.5in 1in 0 1in;
+  margin: 0.5in 1in 0in 1in;
 }
 
 article {
   break-before: always;
 }
 article.nobreak {
   break-before: avoid;
@@ -106,31 +103,31 @@
 }
 h3, h4 {
   color: black;
   font-weight: bold;
   margin-top: 0.5rem;
   margin-bottom: 0.5rem;
 }
-p {
-  font-size: 10pt;
-}
 h1 {
   font-size: 30pt;
   string-set: heading content();
 }
 h2 {
   font-size: 20pt;
   string-set: heading content();
 }
 h3 {
   font-size: 16pt;
 }
 h4 {
   font-size: 11pt;
 }
+p {
+  font-size: 10pt;
+}
 
 table {
   width: 100%;
 }
 table, th, td {
   border-collapse: collapse;
   border-spacing: 0;
@@ -174,27 +171,76 @@
   width: 100%;
   height: 100%;
 }
 
 #cover>div#title {
 }
 #cover>div#who {
-  background: #B57EDC;
+  background: black;
   color: white;
   white-space: pre-wrap;
   min-height: 2in;
   padding: 0px;
   display: flex;
   align-items: flex-start;
   justify-content: center;
   position: absolute;
   bottom: 0px;
   width: 100%;
 }
 
+ul.toc {
+  padding-left: 0px;
+  list-style-type: none;
+}
+ul.toc>ul {
+  padding-left: 1rem;
+  list-style-type: none;
+}
+
+ul.toc li {
+  margin-top: 0.25em;
+}
+ul.toc li::before {
+  content: none;
+}
+a.toc {
+  display: flex;
+  text-decoration: none;
+  color: black;
+}
+div.toctext::before {
+  content: target-text(attr(href));
+}
+div.toctext {
+  display: flex;
+}
+div.tocpagenr {
+  border-bottom: 1pt dotted black;
+  display: flex;
+  flex: 1;
+  justify-content: flex-end;
+}
+div.tocpagenr::after {
+  content: target-counter(attr(href), page);
+}
+
+li a.title {
+  color: inherit;
+  text-decoration-line: inherit;
+}
+li a.title::before {
+  content: target-text(attr(href));
+}
+li a.title::after {
+  color: black;
+  content: target-counter(attr(href), page);
+  float: right;
+}
+
 article {
   height: 8.5in;
   width: 6.5in;
 }
 
 article:not(#cover) {
   display: flex;
@@ -222,20 +268,56 @@
 }
 
 article li {
   line-height: 1.5;
 }
 
 article ul li::before {
-  color: #E6E6FA;
+  color: black;
   content: '• ';
   font-size: 10pt;
   padding-right: 1em;
 }
 
+.columns section {
+  columns: 2;
+  column-gap: 1cm;
+  padding-top: 0;
+}
+.columns section p {
+  text-align: justify;
+}
+.columns section p:first-of-type {
+  font-weight: 700;
+}
+
+article figure {
+  text-align: center;
+}
+
+article figure>figcaption::before {
+  counter-increment: figurecount;
+  content: "Figure " counter(figurecount) ": ";
+}
+
+article figure>img {
+  width: 100%;
+}
+
+div .two-col-fig {
+  width: 100%;
+  display: flex;
+  align-items: flex-start;
+  justify-content: center;
+}
+
+div .two-col-fig>figure {
+  width: 40%;
+}
+
 .footnotes {
   width: 6.5in;
   flex: 0 1in auto;
   min-height: 4rem;
 }
 
 .footnotes hr {
@@ -260,31 +342,9 @@
   color: inherit;
 }
 .footnote-back {
   text-decoration: none;
   color: inherit;
 }
 
-article figure {
-  text-align: center;
-}
-
-article figure>figcaption::before {
-  counter-increment: figurecount;
-  content: "Figure " counter(figurecount) ": ";
-}
-
-article figure>img {
-  width: 100%;
-}
 
-div .two-col-fig {
-  width: 100%;
-  display: flex;
-  align-items: flex-start;
-  justify-content: center;
-}
-
-div .two-col-fig>figure {
-  width: 40%;
-}
```

### Comparing `limberer-0.2.5/src/limberer/static/images/test1.jpg` & `limberer-0.2.6/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/static/sections/example.md` & `limberer-0.2.6/src/limberer/static/sections/example.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/static/sections/example2.md` & `limberer-0.2.6/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/static/templates/cover.html` & `limberer-0.2.6/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer/static/templates/toc.html` & `limberer-0.2.6/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.2.5/src/limberer.egg-info/PKG-INFO` & `limberer-0.2.6/src/limberer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.2.5
+Version: 0.2.6
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.2.5/src/limberer.egg-info/SOURCES.txt` & `limberer-0.2.6/src/limberer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 src/limberer.egg-info/PKG-INFO
 src/limberer.egg-info/SOURCES.txt
 src/limberer.egg-info/dependency_links.txt
 src/limberer.egg-info/entry_points.txt
 src/limberer.egg-info/requires.txt
 src/limberer.egg-info/top_level.txt
 src/limberer/static/project.toml
-src/limberer/static/assets/base.css
+src/limberer/static/assets/core.css
 src/limberer/static/assets/logo.svg
-src/limberer/static/assets/theme.css
+src/limberer/static/assets/style.css
 src/limberer/static/custom/custom.css
 src/limberer/static/images/test1.jpg
 src/limberer/static/sections/example.md
 src/limberer/static/sections/example2.md
 src/limberer/static/templates/base.html
 src/limberer/static/templates/cover.html
 src/limberer/static/templates/section.html
```

