# Comparing `tmp/autodocumenter-test-0.1.1.tar.gz` & `tmp/autodocumenter-test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodocumenter-test-0.1.1.tar", last modified: Tue Jul  4 19:34:13 2023, max compression
+gzip compressed data, was "autodocumenter-test-0.1.2.tar", last modified: Tue Jul  4 19:56:58 2023, max compression
```

## Comparing `autodocumenter-test-0.1.1.tar` & `autodocumenter-test-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.407085 autodocumenter-test-0.1.1/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.1/LICENSE
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.1/MANIFEST.in
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:34:13.407155 autodocumenter-test-0.1.1/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.1/README.md
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.406120 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      511 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/SOURCES.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/dependency_links.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       60 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/entry_points.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/requires.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:34:13.000000 autodocumenter-test-0.1.1/autodocumenter_test.egg-info/top_level.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 19:34:13.407426 autodocumenter-test-0.1.1/setup.cfg
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1808 2023-07-04 19:33:58.000000 autodocumenter-test-0.1.1/setup.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404283 autodocumenter-test-0.1.1/src/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404446 autodocumenter-test-0.1.1/src/autodocumenter/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404378 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.406693 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/base.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/class.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/module.rst
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.404494 autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:34:13.406839 autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/utils/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/utils/config.yaml
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.087330 autodocumenter-test-0.1.2/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.2/LICENSE
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.2/MANIFEST.in
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:56:58.087392 autodocumenter-test-0.1.2/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.2/README.md
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.084300 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      848 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/SOURCES.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/dependency_links.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       64 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/entry_points.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/requires.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       15 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/top_level.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 19:56:58.088102 autodocumenter-test-0.1.2/setup.cfg
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1443 2023-07-04 19:56:35.000000 autodocumenter-test-0.1.2/setup.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.082520 autodocumenter-test-0.1.2/src/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.084702 autodocumenter-test-0.1.2/src/autodocumenter/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      183 2023-07-04 19:55:27.000000 autodocumenter-test-0.1.2/src/autodocumenter/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     4928 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.2/src/autodocumenter/__main__.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.085321 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      305 2023-07-04 17:30:51.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     2778 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/compile_doc.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.086066 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/base.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/class.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/module.rst
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.086897 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      506 2023-07-04 17:33:16.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     6913 2023-07-04 16:04:20.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/generate_doc.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     6655 2023-07-04 15:52:27.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/prepare_file.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.087109 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/utils/config.yaml
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1765 2023-07-04 13:46:08.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/write_file.py
```

### Comparing `autodocumenter-test-0.1.1/LICENSE` & `autodocumenter-test-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.1/src/autodocumenter/compile_doc/templates/module.rst` & `autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/module.rst`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.1/src/autodocumenter/generate_doc/utils/config.yaml` & `autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/utils/config.yaml`

 * *Files identical despite different names*

