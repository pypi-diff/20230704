# Comparing `tmp/swarms-0.0.7.tar.gz` & `tmp/swarms-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.7.tar", last modified: Mon Jul  3 22:09:07 2023, max compression
+gzip compressed data, was "swarms-0.0.8.tar", last modified: Mon Jul  3 22:16:19 2023, max compression
```

## Comparing `swarms-0.0.7.tar` & `swarms-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:08:54.000000 swarms-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:09:07.389770 swarms-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:08:54.000000 swarms-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:09:07.389770 swarms-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-03 22:08:54.000000 swarms-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:08:54.000000 swarms-0.0.7/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:08:54.000000 swarms-0.0.7/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-03 22:08:54.000000 swarms-0.0.7/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:09:07.389770 swarms-0.0.7/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:09:07.000000 swarms-0.0.7/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:16:09.000000 swarms-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:16:19.368694 swarms-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 22:16:09.000000 swarms-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:16:19.368694 swarms-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 22:16:09.000000 swarms-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 22:16:09.000000 swarms-0.0.8/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:09.000000 swarms-0.0.8/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-03 22:16:09.000000 swarms-0.0.8/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:16:19.368694 swarms-0.0.8/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:16:19.000000 swarms-0.0.8/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.7/LICENSE` & `swarms-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.7/PKG-INFO` & `swarms-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.7
+Version: 0.0.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.7/README.md` & `swarms-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.0.7/setup.py` & `swarms-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -15,15 +15,15 @@
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
         "transformers",
         "openai",
-        "langchain==0.0.101",
+        "langchain",
         "torch==1.13.1",
         "torchvision==0.14.1",
         "asyncio",
         "nest_asyncio",
         "bs4",
         "playwright",
         "duckduckgo_search",
```

### Comparing `swarms-0.0.7/swarms/agents/swarms.py` & `swarms-0.0.8/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.0.7/swarms.egg-info/PKG-INFO` & `swarms-0.0.8/swarms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.7
+Version: 0.0.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.7/swarms.egg-info/requires.txt` & `swarms-0.0.8/swarms.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 transformers
 openai
-langchain==0.0.101
+langchain
 torch==1.13.1
 torchvision==0.14.1
 asyncio
 nest_asyncio
 bs4
 playwright
 duckduckgo_search
```

