# Comparing `tmp/screwhashesset-0.10.tar.gz` & `tmp/screwhashesset-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwhashesset-0.10.tar", last modified: Sun Jul  2 20:15:29 2023, max compression
+gzip compressed data, was "screwhashesset-0.11.tar", last modified: Tue Jul  4 06:12:50 2023, max compression
```

## Comparing `screwhashesset-0.10.tar` & `screwhashesset-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 20:15:29.975653 screwhashesset-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-02 20:15:24.000000 screwhashesset-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      113 2023-07-02 20:15:23.000000 screwhashesset-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2023-07-02 20:15:29.975653 screwhashesset-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2023-07-02 20:14:33.000000 screwhashesset-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 20:15:29.963683 screwhashesset-0.10/screwhashesset/
--rw-rw-rw-   0        0        0     1060 2023-07-02 20:14:33.000000 screwhashesset-0.10/screwhashesset/README.MD
--rw-rw-rw-   0        0        0     3306 2023-07-02 20:09:53.000000 screwhashesset-0.10/screwhashesset/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-02 20:15:28.000000 screwhashesset-0.10/screwhashesset/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-02 20:15:28.000000 screwhashesset-0.10/screwhashesset/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-02 20:15:29.974655 screwhashesset-0.10/screwhashesset.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-07-02 20:15:29.000000 screwhashesset-0.10/screwhashesset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-07-02 20:15:29.000000 screwhashesset-0.10/screwhashesset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 20:15:29.000000 screwhashesset-0.10/screwhashesset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-02 20:15:29.000000 screwhashesset-0.10/screwhashesset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-02 20:15:29.975653 screwhashesset-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1323 2023-07-02 20:15:28.000000 screwhashesset-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:12:50.981678 screwhashesset-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-04 06:12:46.000000 screwhashesset-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      113 2023-07-04 06:12:43.000000 screwhashesset-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0    25580 2023-07-04 06:12:50.981678 screwhashesset-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0    24896 2023-07-04 06:10:17.000000 screwhashesset-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 06:12:50.978686 screwhashesset-0.11/screwhashesset/
+-rw-rw-rw-   0        0        0    24896 2023-07-04 06:10:17.000000 screwhashesset-0.11/screwhashesset/README.MD
+-rw-rw-rw-   0        0        0    12813 2023-07-04 06:02:27.000000 screwhashesset-0.11/screwhashesset/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-04 06:12:50.980681 screwhashesset-0.11/screwhashesset.egg-info/
+-rw-rw-rw-   0        0        0    25580 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-04 06:12:50.000000 screwhashesset-0.11/screwhashesset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-04 06:12:50.982675 screwhashesset-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-07-04 06:12:50.000000 screwhashesset-0.11/setup.py
```

### Comparing `screwhashesset-0.10/LICENSE.rst` & `screwhashesset-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `screwhashesset-0.10/setup.py` & `screwhashesset-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''A set that handles all kinds of objects (hashable or not) and preserves the order of the elements'''
 
 # Setting up
 setup(
     name="screwhashesset",
     version=VERSION,
     license='MIT',
```

