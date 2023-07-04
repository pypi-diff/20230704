# Comparing `tmp/goxlr-1.0.2.tar.gz` & `tmp/goxlr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.0.2.tar", last modified: Tue Jul  4 01:20:14 2023, max compression
+gzip compressed data, was "goxlr-1.0.3.tar", last modified: Tue Jul  4 11:26:49 2023, max compression
```

## Comparing `goxlr-1.0.2.tar` & `goxlr-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 01:20:14.922203 goxlr-1.0.2/
--rw-rw-rw-   0        0        0       52 2023-07-03 17:47:02.000000 goxlr-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      734 2023-07-04 01:20:14.922203 goxlr-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-07-04 01:18:58.000000 goxlr-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 01:20:14.918703 goxlr-1.0.2/goxlr/
--rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.2/goxlr/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.2/goxlr/error.py
--rw-rw-rw-   0        0        0    27172 2023-07-04 01:14:35.000000 goxlr-1.0.2/goxlr/goxlr.py
--rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.2/goxlr/types.py
--rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.2/goxlr/ws.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:20:14.921703 goxlr-1.0.2/goxlr.egg-info/
--rw-rw-rw-   0        0        0      734 2023-07-04 01:20:14.000000 goxlr-1.0.2/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-04 01:20:14.000000 goxlr-1.0.2/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 01:20:14.000000 goxlr-1.0.2/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 01:20:14.000000 goxlr-1.0.2/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 01:20:14.000000 goxlr-1.0.2/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 01:20:14.922702 goxlr-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      535 2023-07-04 01:19:04.000000 goxlr-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:26:49.834499 goxlr-1.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-07-04 11:05:46.000000 goxlr-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2278 2023-07-04 11:26:49.834499 goxlr-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1938 2023-07-04 11:26:03.000000 goxlr-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 11:26:49.830495 goxlr-1.0.3/goxlr/
+-rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.3/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.3/goxlr/error.py
+-rw-rw-rw-   0        0        0    27172 2023-07-04 01:14:35.000000 goxlr-1.0.3/goxlr/goxlr.py
+-rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.3/goxlr/types.py
+-rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.3/goxlr/ws.py
+drwxrwxrwx   0        0        0        0 2023-07-04 11:26:49.833996 goxlr-1.0.3/goxlr.egg-info/
+-rw-rw-rw-   0        0        0     2278 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 11:26:49.000000 goxlr-1.0.3/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-04 11:26:49.834996 goxlr-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      534 2023-07-04 11:26:25.000000 goxlr-1.0.3/setup.py
```

### Comparing `goxlr-1.0.2/goxlr/goxlr.py` & `goxlr-1.0.3/goxlr/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.2/goxlr/types.py` & `goxlr-1.0.3/goxlr/types.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.2/goxlr/ws.py` & `goxlr-1.0.3/goxlr/ws.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.2/setup.py` & `goxlr-1.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="goxlr",
-    version="1.0.2",
+    version="1.0.3",
     description="A Python wrapper for the GoXLR Utility API.",
     url="https://github.com/samcarsonx/goxlr",
     author="Sam Carson",
     author_email="sam@samcarson.co.uk",
-    license="None",
+    license="MIT",
     packages=find_packages(),
     install_requires=["asyncio", "websockets", "json", "ctypes", "enum"],
     python_requires=">=3.6",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
 )
```

