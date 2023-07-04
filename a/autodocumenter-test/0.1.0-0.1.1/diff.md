# Comparing `tmp/autodocumenter-test-0.1.0.tar.gz` & `tmp/autodocumenter-test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodocumenter-test-0.1.0.tar", last modified: Tue Jul  4 19:31:54 2023, max compression
+gzip compressed data, was "autodocumenter-test-0.1.1.tar", last modified: Tue Jul  4 19:34:13 2023, max compression
```

## Comparing `autodocumenter-test-0.1.0.tar` & `autodocumenter-test-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.718015 autodocumenter-test-0.1.0/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.0/LICENSE
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.0/MANIFEST.in
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:31:54.718082 autodocumenter-test-0.1.0/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.0/README.md
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.716803 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:31:54.000000 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      511 2023-07-04 19:31:54.000000 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/SOURCES.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:31:54.000000 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/dependency_links.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       60 2023-07-04 19:31:54.000000 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/entry_points.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 19:31:54.000000 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/requires.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:31:54.000000 autodocumenter-test-0.1.0/autodocumenter_test.egg-info/top_level.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 19:31:54.718328 autodocumenter-test-0.1.0/setup.cfg
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1808 2023-07-04 19:31:09.000000 autodocumenter-test-0.1.0/setup.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.715057 autodocumenter-test-0.1.0/src/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.715242 autodocumenter-test-0.1.0/src/autodocumenter/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.715165 autodocumenter-test-0.1.0/src/autodocumenter/compile_doc/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.717596 autodocumenter-test-0.1.0/src/autodocumenter/compile_doc/templates/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.0/src/autodocumenter/compile_doc/templates/base.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.0/src/autodocumenter/compile_doc/templates/class.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.0/src/autodocumenter/compile_doc/templates/module.rst
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.715290 autodocumenter-test-0.1.0/src/autodocumenter/generate_doc/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:31:54.717765 autodocumenter-test-0.1.0/src/autodocumenter/generate_doc/utils/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.0/src/autodocumenter/generate_doc/utils/config.yaml
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.407085 autodocumenter-test-0.1.1/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.1/LICENSE
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.1/MANIFEST.in
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:34:13.407155 autodocumenter-test-0.1.1/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.1/README.md
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.406120 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      511 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/SOURCES.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/dependency_links.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       60 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/entry_points.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/requires.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/top_level.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 19:34:13.407426 autodocumenter-test-0.1.1/setup.cfg
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1808 2023-07-04 19:33:58.000000 autodocumenter-test-0.1.1/setup.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404283 autodocumenter-test-0.1.1/src/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404446 autodocumenter-test-0.1.1/src/autodocumenter/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404378 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.406693 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/base.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/class.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/module.rst
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404494 autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.406839 autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/utils/config.yaml
```

### Comparing `autodocumenter-test-0.1.0/LICENSE` & `autodocumenter-test-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.0/setup.py` & `autodocumenter-test-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = 'autodocumenter-test',         # How you named your package folder (MyLib)
     packages=find_packages(include=['autodocumenter', 'autodocumenter.*']),
     package_dir={'autodocumenter': 'src/autodocumenter'},
     package_data={'autodocumenter': ['autodocumenter/compile_doc/templates/*.rst', 'autodocumenter/generate_doc/utils/config.yaml']},
-    version = "0.1.0",      # Start with a small number and increase it with every change you make
+    version = "0.1.1",      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = ('Generate docstrings using ChatGPT and generate Sphinx documentation from the project structure.'),   # Give a short description about your library
     long_description=read('README.md'),
     author = 'Dusan Grujicic',                   # Type in your name
     author_email = 'dusangr22@gmail.com',      # Type in your E-Mail
     keywords = ["documentation", "ChatGPT", "Sphinx"],   # Keywords that define your package best
     python_requires='>3.9',
```

### Comparing `autodocumenter-test-0.1.0/src/autodocumenter/compile_doc/templates/module.rst` & `autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/module.rst`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.0/src/autodocumenter/generate_doc/utils/config.yaml` & `autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/utils/config.yaml`

 * *Files identical despite different names*

