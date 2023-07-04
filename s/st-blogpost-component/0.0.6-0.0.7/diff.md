# Comparing `tmp/st_blogpost_component-0.0.6.tar.gz` & `tmp/st_blogpost_component-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_blogpost_component-0.0.6.tar", last modified: Tue Jul  4 18:46:57 2023, max compression
+gzip compressed data, was "st_blogpost_component-0.0.7.tar", last modified: Tue Jul  4 18:47:48 2023, max compression
```

## Comparing `st_blogpost_component-0.0.6.tar` & `st_blogpost_component-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.526106 st_blogpost_component-0.0.6/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.6/LICENSE
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.6/MANIFEST.in
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 18:46:57.526106 st_blogpost_component-0.0.6/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 18:46:57.526106 st_blogpost_component-0.0.6/setup.cfg
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 18:46:43.000000 st_blogpost_component-0.0.6/setup.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.518106 st_blogpost_component-0.0.6/st_blogpost_component/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3635 2023-07-04 18:45:40.000000 st_blogpost_component-0.0.6/st_blogpost_component/__init__.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.514106 st_blogpost_component-0.0.6/st_blogpost_component/frontend/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.518106 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/asset-manifest.json
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 18:45:47.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/bootstrap.min.css
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/index.html
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.514106 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.526106 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141267 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1769 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     5320 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:46:57.518106 st_blogpost_component-0.0.6/st_blogpost_component.egg-info/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 18:46:57.000000 st_blogpost_component-0.0.6/st_blogpost_component.egg-info/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 18:46:57.000000 st_blogpost_component-0.0.6/st_blogpost_component.egg-info/SOURCES.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 18:46:57.000000 st_blogpost_component-0.0.6/st_blogpost_component.egg-info/dependency_links.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 18:46:57.000000 st_blogpost_component-0.0.6/st_blogpost_component.egg-info/requires.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 18:46:57.000000 st_blogpost_component-0.0.6/st_blogpost_component.egg-info/top_level.txt
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.030937 st_blogpost_component-0.0.7/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.7/LICENSE
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.7/MANIFEST.in
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 18:47:48.030937 st_blogpost_component-0.0.7/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 18:47:48.030937 st_blogpost_component-0.0.7/setup.cfg
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 18:47:41.000000 st_blogpost_component-0.0.7/setup.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.022937 st_blogpost_component-0.0.7/st_blogpost_component/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3634 2023-07-04 18:47:27.000000 st_blogpost_component-0.0.7/st_blogpost_component/__init__.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.022937 st_blogpost_component-0.0.7/st_blogpost_component/frontend/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.026937 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/asset-manifest.json
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 18:45:47.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/index.html
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.022937 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.030937 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141267 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1769 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     5320 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 18:46:06.000000 st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 18:47:48.026937 st_blogpost_component-0.0.7/st_blogpost_component.egg-info/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 18:47:47.000000 st_blogpost_component-0.0.7/st_blogpost_component.egg-info/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 18:47:47.000000 st_blogpost_component-0.0.7/st_blogpost_component.egg-info/SOURCES.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 18:47:47.000000 st_blogpost_component-0.0.7/st_blogpost_component.egg-info/dependency_links.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 18:47:47.000000 st_blogpost_component-0.0.7/st_blogpost_component.egg-info/requires.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 18:47:47.000000 st_blogpost_component-0.0.7/st_blogpost_component.egg-info/top_level.txt
```

### Comparing `st_blogpost_component-0.0.6/LICENSE` & `st_blogpost_component-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/setup.py` & `st_blogpost_component-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_blogpost_component",
-    version="0.0.6",
+    version="0.0.7",
     author="YM",
     author_email="",
     description="",
     long_description="custom component to display blog post card for personal blog",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/__init__.py` & `st_blogpost_component-0.0.7/st_blogpost_component/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 import requests
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 import os import streamlit.components.v1 as components import requests # Create
 a _RELEASE constant. We'll set this to False while we're developing # the
 component, and True when we're ready to package and distribute it. # (This is,
 of course, optional - there are innumerable ways to manage your # release
-process.) _RELEASE = False # Declare a Streamlit component. `declare_component`
+process.) _RELEASE = True # Declare a Streamlit component. `declare_component`
 returns a function # that is used to create instances of the component. We're
 naming this # function "_component_func", with an underscore prefix, because we
 don't want # to expose it directly to users. Instead, we will create a custom
 wrapper # function, below, that will serve as our component's public API. #
 It's worth noting that this call to `declare_component` is the # *only thing*
 you need to do to create the binding between Streamlit and # your component
 frontend. Everything else we do in this file is simply a # best practice. if
```

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/asset-manifest.json` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/bootstrap.min.css` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/index.html` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js.map` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/main.19002e51.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map` & `st_blogpost_component-0.0.7/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.6/st_blogpost_component.egg-info/SOURCES.txt` & `st_blogpost_component-0.0.7/st_blogpost_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

