# Comparing `tmp/re_it-0.0.1.tar.gz` & `tmp/re_it-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\re_it-0.0.1.tar", last modified: Tue Jul  4 08:35:34 2023, max compression
+gzip compressed data, was "dist\re_it-1.0.0.0.tar", last modified: Tue Jul  4 08:45:02 2023, max compression
```

## Comparing `re_it-0.0.1.tar` & `re_it-1.0.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:35:34.000000 re_it-0.0.1/
--rw-rw-rw-   0        0        0      284 2023-07-04 08:35:34.000000 re_it-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-04 08:30:22.000000 re_it-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:35:34.000000 re_it-0.0.1/re_it/
--rw-rw-rw-   0        0        0        0 2023-07-04 08:28:05.000000 re_it-0.0.1/re_it/__init__.py
--rw-rw-rw-   0        0        0      754 2023-07-04 08:29:10.000000 re_it-0.0.1/re_it/请求.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:35:34.000000 re_it-0.0.1/re_it.egg-info/
--rw-rw-rw-   0        0        0      284 2023-07-04 08:35:33.000000 re_it-0.0.1/re_it.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-04 08:35:33.000000 re_it-0.0.1/re_it.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:35:33.000000 re_it-0.0.1/re_it.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 08:35:33.000000 re_it-0.0.1/re_it.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:35:34.000000 re_it-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-07-04 08:31:25.000000 re_it-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:45:02.000000 re_it-1.0.0.0/
+-rw-rw-rw-   0        0        0     1737 2023-07-04 08:45:02.000000 re_it-1.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1234 2023-07-04 08:44:53.000000 re_it-1.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 08:45:02.000000 re_it-1.0.0.0/re_it/
+-rw-rw-rw-   0        0        0        0 2023-07-04 08:28:05.000000 re_it-1.0.0.0/re_it/__init__.py
+-rw-rw-rw-   0        0        0      754 2023-07-04 08:29:10.000000 re_it-1.0.0.0/re_it/请求.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:45:02.000000 re_it-1.0.0.0/re_it.egg-info/
+-rw-rw-rw-   0        0        0     1737 2023-07-04 08:45:02.000000 re_it-1.0.0.0/re_it.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-04 08:45:02.000000 re_it-1.0.0.0/re_it.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:45:02.000000 re_it-1.0.0.0/re_it.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 08:45:02.000000 re_it-1.0.0.0/re_it.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:45:02.000000 re_it-1.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      527 2023-07-04 08:44:53.000000 re_it-1.0.0.0/setup.py
```

### Comparing `re_it-0.0.1/re_it/请求.py` & `re_it-1.0.0.0/re_it/请求.py`

 * *Files identical despite different names*

### Comparing `re_it-0.0.1/setup.py` & `re_it-1.0.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='re_it',
-    version='0.0.1',
+    version='1.0.0.0',
     author='SuiBo',
     author_email='534047068@qq.com',
     description='中文的python网络请求库！',
     install_requires=[
 
     ],
     py_modules=["re_it"],
```

