# Comparing `tmp/taibun-0.0.1.tar.gz` & `tmp/taibun-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taibun-0.0.1.tar", last modified: Thu Jun 15 08:36:31 2023, max compression
+gzip compressed data, was "taibun-0.0.2.tar", last modified: Tue Jul  4 05:04:22 2023, max compression
```

## Comparing `taibun-0.0.1.tar` & `taibun-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:36:31.113151 taibun-0.0.1/
--rw-rw-rw-   0        0        0      534 2023-06-15 08:36:31.111156 taibun-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-15 08:36:31.114149 taibun-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-06-15 08:36:16.000000 taibun-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:36:31.047148 taibun-0.0.1/taibun/
--rw-rw-rw-   0        0        0       19 2023-06-15 08:01:53.000000 taibun-0.0.1/taibun/__init__.py
--rw-rw-rw-   0        0        0      106 2023-06-15 08:12:04.000000 taibun-0.0.1/taibun/taibun.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:36:31.104160 taibun-0.0.1/taibun.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-15 08:36:30.000000 taibun-0.0.1/taibun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-06-15 08:36:30.000000 taibun-0.0.1/taibun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:36:30.000000 taibun-0.0.1/taibun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 08:36:30.000000 taibun-0.0.1/taibun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 05:04:22.388658 taibun-0.0.2/
+-rw-rw-rw-   0        0        0    10993 2023-07-04 05:04:22.387689 taibun-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 taibun-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 05:04:22.389642 taibun-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-07-04 05:04:01.000000 taibun-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:04:22.356731 taibun-0.0.2/taibun/
+-rw-rw-rw-   0        0        0       20 2023-06-15 08:41:22.000000 taibun-0.0.2/taibun/__init__.py
+-rw-rw-rw-   0        0        0    19874 2023-07-04 01:32:21.000000 taibun-0.0.2/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:04:22.382660 taibun-0.0.2/taibun.egg-info/
+-rw-rw-rw-   0        0        0    10993 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/top_level.txt
```

### Comparing `taibun-0.0.1/setup.py` & `taibun-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from setuptools import setup, find_packages
+import codecs
+import os
 
-VERSION = '0.0.1'
-DESCRIPTION = 'A basic hello package'
-LONG_DESCRIPTION = 'A basic hello package long desc.'
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding='utf-8') as fh:
+    LONG_DESCRIPTION = '\n' + fh.read()
+
+VERSION = '0.0.2'
+DESCRIPTION = 'Convert Chinese characters to Taiwanese'
+#LONG_DESCRIPTION = 'Taiwanese Hokkien transliterator from Chinese characters.'
 
 # Setting up
 setup(
     name="taibun",
     version=VERSION,
     author="Andrei Harbachov",
     author_email="<andrei.harbachov@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=['python'],
+    keywords=['python', 'taiwan', 'taiwanese', 'taigi', 'hokkien', 'romanization'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

