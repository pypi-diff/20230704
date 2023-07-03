# Comparing `tmp/nerdcore-0.0.4.tar.gz` & `tmp/nerdcore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdcore-0.0.4.tar", last modified: Mon Jul  3 22:00:02 2023, max compression
+gzip compressed data, was "nerdcore-0.0.5.tar", last modified: Mon Jul  3 22:14:53 2023, max compression
```

## Comparing `nerdcore-0.0.4.tar` & `nerdcore-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:00:02.071370 nerdcore-0.0.4/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:00:02.071370 nerdcore-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 21:59:44.000000 nerdcore-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:00:02.071370 nerdcore-0.0.4/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:00:02.000000 nerdcore-0.0.4/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 22:00:02.000000 nerdcore-0.0.4/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:00:02.000000 nerdcore-0.0.4/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 22:00:02.000000 nerdcore-0.0.4/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 22:00:02.000000 nerdcore-0.0.4/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:00:02.000000 nerdcore-0.0.4/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:00:02.071370 nerdcore-0.0.4/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 21:59:44.000000 nerdcore-0.0.4/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 21:59:44.000000 nerdcore-0.0.4/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:00:02.071370 nerdcore-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 21:59:44.000000 nerdcore-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:14:53.089931 nerdcore-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:14:35.000000 nerdcore-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/nerdcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/defs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/ncdefs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 22:14:35.000000 nerdcore-0.0.5/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 22:14:35.000000 nerdcore-0.0.5/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:14:53.089931 nerdcore-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 22:14:35.000000 nerdcore-0.0.5/setup.py
```

### Comparing `nerdcore-0.0.4/PKG-INFO` & `nerdcore-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.4/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.0.5/nerdcore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.4/scripts/nerd` & `nerdcore-0.0.5/scripts/nerd`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.4/scripts/nerd-new` & `nerdcore-0.0.5/scripts/nerd-new`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.4/setup.py` & `nerdcore-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.0.4',
+    version='0.0.5',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

