# Comparing `tmp/st_blogpost_component-0.0.2.tar.gz` & `tmp/st_blogpost_component-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_blogpost_component-0.0.2.tar", last modified: Tue Jul  4 04:58:30 2023, max compression
+gzip compressed data, was "st_blogpost_component-0.0.3.tar", last modified: Tue Jul  4 05:14:05 2023, max compression
```

## Comparing `st_blogpost_component-0.0.2.tar` & `st_blogpost_component-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.212345 st_blogpost_component-0.0.2/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.2/LICENSE
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.2/MANIFEST.in
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 04:58:30.212345 st_blogpost_component-0.0.2/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 04:58:30.212345 st_blogpost_component-0.0.2/setup.cfg
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 04:55:53.000000 st_blogpost_component-0.0.2/setup.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.204345 st_blogpost_component-0.0.2/st_blogpost_component/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3475 2023-07-04 04:55:26.000000 st_blogpost_component-0.0.2/st_blogpost_component/__init__.py
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.204345 st_blogpost_component-0.0.2/st_blogpost_component/frontend/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.204345 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/asset-manifest.json
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 04:56:31.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/bootstrap.min.css
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/index.html
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.204345 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.212345 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141267 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1351 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3930 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js.map
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
-drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 04:58:30.204345 st_blogpost_component-0.0.2/st_blogpost_component.egg-info/
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 04:58:30.000000 st_blogpost_component-0.0.2/st_blogpost_component.egg-info/PKG-INFO
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 04:58:30.000000 st_blogpost_component-0.0.2/st_blogpost_component.egg-info/SOURCES.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 04:58:30.000000 st_blogpost_component-0.0.2/st_blogpost_component.egg-info/dependency_links.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 04:58:30.000000 st_blogpost_component-0.0.2/st_blogpost_component.egg-info/requires.txt
--rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 04:58:30.000000 st_blogpost_component-0.0.2/st_blogpost_component.egg-info/top_level.txt
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.629818 st_blogpost_component-0.0.3/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1063 2023-07-04 03:12:34.000000 st_blogpost_component-0.0.3/LICENSE
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       57 2023-07-04 04:48:07.000000 st_blogpost_component-0.0.3/MANIFEST.in
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 05:14:05.629818 st_blogpost_component-0.0.3/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       38 2023-07-04 05:14:05.629818 st_blogpost_component-0.0.3/setup.cfg
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      628 2023-07-04 05:13:58.000000 st_blogpost_component-0.0.3/setup.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.621817 st_blogpost_component-0.0.3/st_blogpost_component/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3471 2023-07-04 05:11:33.000000 st_blogpost_component-0.0.3/st_blogpost_component/__init__.py
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.617817 st_blogpost_component-0.0.3/st_blogpost_component/frontend/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.621817 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      691 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/asset-manifest.json
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   197459 2023-07-04 04:56:31.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2087 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/index.html
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.621817 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.629818 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)   557241 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     2243 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)  2141267 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1351 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     3930 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js.map
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     1584 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)     8369 2023-07-04 04:56:49.000000 st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
+drwxrwxr-x   0 ymhedhbi  (1000) ymhedhbi  (1000)        0 2023-07-04 05:14:05.621817 st_blogpost_component-0.0.3/st_blogpost_component.egg-info/
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      307 2023-07-04 05:14:05.000000 st_blogpost_component-0.0.3/st_blogpost_component.egg-info/PKG-INFO
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)      955 2023-07-04 05:14:05.000000 st_blogpost_component-0.0.3/st_blogpost_component.egg-info/SOURCES.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)        1 2023-07-04 05:14:05.000000 st_blogpost_component-0.0.3/st_blogpost_component.egg-info/dependency_links.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       16 2023-07-04 05:14:05.000000 st_blogpost_component-0.0.3/st_blogpost_component.egg-info/requires.txt
+-rw-rw-r--   0 ymhedhbi  (1000) ymhedhbi  (1000)       22 2023-07-04 05:14:05.000000 st_blogpost_component-0.0.3/st_blogpost_component.egg-info/top_level.txt
```

### Comparing `st_blogpost_component-0.0.2/LICENSE` & `st_blogpost_component-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/setup.py` & `st_blogpost_component-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_blogpost_component",
-    version="0.0.2",
+    version="0.0.3",
     author="YM",
     author_email="",
     description="",
     long_description="custom component to display blog post card for personal blog",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/__init__.py` & `st_blogpost_component-0.0.3/st_blogpost_component/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     # There's no need to do this in our simple example - but it's an option.
     return component_value
 
 
 # Add some test code to play with the component while it's in development.
 # During development, we can run this just as we would any other Streamlit
 # app: `$ streamlit run my_component/__init__.py`
-if not _RELEASE:
+if _RELEASE:
     import streamlit as st
 
     st.subheader("Component with constant args")
 
     # Create an instance of our component with a constant `name` arg, and
     # print its output value.
     url = blog_card_component("World", "example", "test", "urltesttest")
```

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/asset-manifest.json` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/bootstrap.min.css` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/index.html` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/2.cc3b77fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js.map` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/main.a8adb8b7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map` & `st_blogpost_component-0.0.3/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map`

 * *Files identical despite different names*

### Comparing `st_blogpost_component-0.0.2/st_blogpost_component.egg-info/SOURCES.txt` & `st_blogpost_component-0.0.3/st_blogpost_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

