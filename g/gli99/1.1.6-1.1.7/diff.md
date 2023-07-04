# Comparing `tmp/gli99-1.1.6.tar.gz` & `tmp/gli99-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gli99-1.1.6.tar", last modified: Tue Jun 13 18:41:06 2023, max compression
+gzip compressed data, was "gli99-1.1.7.tar", last modified: Tue Jul  4 19:54:53 2023, max compression
```

## Comparing `gli99-1.1.6.tar` & `gli99-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.261517 gli99-1.1.6/
--rw-rw-rw-   0        0        0     1085 2023-03-04 20:16:16.000000 gli99-1.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0       24 2023-03-07 22:58:15.000000 gli99-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1082 2023-06-13 18:41:06.261517 gli99-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-06-13 18:41:05.000000 gli99-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 18:41:06.262518 gli99-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-06-13 18:40:58.000000 gli99-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.235669 gli99-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.243650 gli99-1.1.6/src/gli99/
--rw-rw-rw-   0        0        0        0 2023-03-06 23:39:49.000000 gli99-1.1.6/src/gli99/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-09 03:29:00.000000 gli99-1.1.6/src/gli99/browser_options.json
--rw-rw-rw-   0        0        0     4892 2023-03-10 19:25:37.000000 gli99-1.1.6/src/gli99/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.259611 gli99-1.1.6/src/gli99.egg-info/
--rw-rw-rw-   0        0        0     1082 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:53.047682 gli99-1.1.7/
+-rw-rw-rw-   0        0        0     1085 2023-03-04 20:16:16.000000 gli99-1.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       24 2023-03-07 22:58:15.000000 gli99-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1082 2023-07-04 19:54:53.047682 gli99-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-07-04 19:54:52.000000 gli99-1.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:54:53.047682 gli99-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-07-04 19:48:44.000000 gli99-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:53.015679 gli99-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:53.031679 gli99-1.1.7/src/gli99/
+-rw-rw-rw-   0        0        0        0 2023-03-06 23:39:49.000000 gli99-1.1.7/src/gli99/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-09 03:29:00.000000 gli99-1.1.7/src/gli99/browser_options.json
+-rw-rw-rw-   0        0        0     4951 2023-07-04 19:53:49.000000 gli99-1.1.7/src/gli99/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:54:53.047682 gli99-1.1.7/src/gli99.egg-info/
+-rw-rw-rw-   0        0        0     1082 2023-07-04 19:54:52.000000 gli99-1.1.7/src/gli99.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-04 19:54:52.000000 gli99-1.1.7/src/gli99.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:54:52.000000 gli99-1.1.7/src/gli99.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-04 19:54:52.000000 gli99-1.1.7/src/gli99.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 19:54:52.000000 gli99-1.1.7/src/gli99.egg-info/top_level.txt
```

### Comparing `gli99-1.1.6/LICENSE.txt` & `gli99-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gli99-1.1.6/PKG-INFO` & `gli99-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gli99
-Version: 1.1.6
+Version: 1.1.7
 Summary: Web scraper for gifcities.org
 Home-page: https://github.com/TomTkacz/gli99
 Author: Tom Tkacz
 Author-email: thomasatkacz@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-***Do NOT use this repo for professional use, this was a personal project to practice version control, web scraping, and readme design. The correct way to access GifCities.org is through its (admittedly slow) [API](https://gifcities.archive.org/api/v1/gifsearch?q=hamster).***
+***Do NOT use this repo for professional use. This was a personal project to practice version control, web scraping, and readme design. The correct way to access GifCities.org is through its (admittedly slow) [API](https://gifcities.archive.org/api/v1/gifsearch?q=hamster).***
 
 ---
 
 
 
 ## Installation
```

### Comparing `gli99-1.1.6/README.md` & `gli99-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-***Do NOT use this repo for professional use, this was a personal project to practice version control, web scraping, and readme design. The correct way to access GifCities.org is through its (admittedly slow) [API](https://gifcities.archive.org/api/v1/gifsearch?q=hamster).***
+***Do NOT use this repo for professional use. This was a personal project to practice version control, web scraping, and readme design. The correct way to access GifCities.org is through its (admittedly slow) [API](https://gifcities.archive.org/api/v1/gifsearch?q=hamster).***
 
 ---
 
 
 
 ## Installation
```

### Comparing `gli99-1.1.6/setup.py` & `gli99-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gli99",
-    version='1.1.6',
+    version='1.1.7',
     description="Web scraper for gifcities.org",
     package_dir={'':'src'},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     python_requires=">3.10.0",
     classifiers=[
         "Programming Language :: Python",
```

### Comparing `gli99-1.1.6/src/gli99/browser_options.json` & `gli99-1.1.7/src/gli99/browser_options.json`

 * *Files identical despite different names*

### Comparing `gli99-1.1.6/src/gli99/tools.py` & `gli99-1.1.7/src/gli99/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 
 class GifScraper():
 
     def __init__(self,browser="edge"):
         self.browser=browser
         self.sources = []
         self.options = None
+        
         abspath = os.path.abspath(__file__)
-        dname = os.path.dirname(abspath)
-        os.chdir(dname)
+        root = os.path.dirname(abspath)
+        options_path = os.path.normpath(root + "/browser_options.json")
+
         options_json = json.load(open('browser_options.json','r'))
         
         print(f"attempting to create {browser} driver ",end="... ")
         
         def set_browser_options():
             if self.browser.lower() in options_json:
                 [self.options.add_argument(arg) for arg in options_json[self.browser.lower()]["arguments"]]
```

### Comparing `gli99-1.1.6/src/gli99.egg-info/PKG-INFO` & `gli99-1.1.7/src/gli99.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gli99
-Version: 1.1.6
+Version: 1.1.7
 Summary: Web scraper for gifcities.org
 Home-page: https://github.com/TomTkacz/gli99
 Author: Tom Tkacz
 Author-email: thomasatkacz@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-***Do NOT use this repo for professional use, this was a personal project to practice version control, web scraping, and readme design. The correct way to access GifCities.org is through its (admittedly slow) [API](https://gifcities.archive.org/api/v1/gifsearch?q=hamster).***
+***Do NOT use this repo for professional use. This was a personal project to practice version control, web scraping, and readme design. The correct way to access GifCities.org is through its (admittedly slow) [API](https://gifcities.archive.org/api/v1/gifsearch?q=hamster).***
 
 ---
 
 
 
 ## Installation
```

