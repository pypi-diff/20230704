# Comparing `tmp/autodocumenter-test-0.1.2.tar.gz` & `tmp/autodocumenter-test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodocumenter-test-0.1.2.tar", last modified: Tue Jul  4 19:56:58 2023, max compression
+gzip compressed data, was "autodocumenter-test-0.1.3.tar", last modified: Tue Jul  4 20:02:05 2023, max compression
```

## Comparing `autodocumenter-test-0.1.2.tar` & `autodocumenter-test-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,48 @@
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.087330 autodocumenter-test-0.1.2/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.2/LICENSE
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.2/MANIFEST.in
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:56:58.087392 autodocumenter-test-0.1.2/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.2/README.md
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.084300 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      848 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/SOURCES.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/dependency_links.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       64 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/entry_points.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/requires.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       15 2023-07-04 19:56:58.000000 autodocumenter-test-0.1.2/autodocumenter_test.egg-info/top_level.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 19:56:58.088102 autodocumenter-test-0.1.2/setup.cfg
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1443 2023-07-04 19:56:35.000000 autodocumenter-test-0.1.2/setup.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.082520 autodocumenter-test-0.1.2/src/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.084702 autodocumenter-test-0.1.2/src/autodocumenter/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      183 2023-07-04 19:55:27.000000 autodocumenter-test-0.1.2/src/autodocumenter/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     4928 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.2/src/autodocumenter/__main__.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.085321 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      305 2023-07-04 17:30:51.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     2778 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/compile_doc.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.086066 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/base.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/class.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/module.rst
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.086897 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      506 2023-07-04 17:33:16.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     6913 2023-07-04 16:04:20.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/generate_doc.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     6655 2023-07-04 15:52:27.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/prepare_file.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 19:56:58.087109 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/utils/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/utils/config.yaml
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1765 2023-07-04 13:46:08.000000 autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/write_file.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.741594 autodocumenter-test-0.1.3/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.3/LICENSE
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.3/MANIFEST.in
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 20:02:05.741690 autodocumenter-test-0.1.3/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.3/README.md
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.736014 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 20:02:05.000000 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1520 2023-07-04 20:02:05.000000 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/SOURCES.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 20:02:05.000000 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/dependency_links.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       64 2023-07-04 20:02:05.000000 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/entry_points.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 20:02:05.000000 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/requires.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       15 2023-07-04 20:02:05.000000 autodocumenter-test-0.1.3/autodocumenter_test.egg-info/top_level.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 20:02:05.741973 autodocumenter-test-0.1.3/setup.cfg
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1443 2023-07-04 20:01:48.000000 autodocumenter-test-0.1.3/setup.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.734147 autodocumenter-test-0.1.3/src/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.736415 autodocumenter-test-0.1.3/src/autodocumenter/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      183 2023-07-04 20:01:42.000000 autodocumenter-test-0.1.3/src/autodocumenter/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     4928 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.3/src/autodocumenter/__main__.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.736869 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      305 2023-07-04 17:30:51.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     2778 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/compile_doc.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.737492 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/templates/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/templates/base.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/templates/class.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/templates/module.rst
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.738388 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:00:21.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/utils/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     2967 2023-07-04 17:38:52.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/utils/edit_config.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      404 2023-07-04 17:39:01.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/utils/edit_index.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      579 2023-07-04 17:39:17.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/utils/edit_reference.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      139 2023-07-04 17:39:27.000000 autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/utils/edit_user_guide.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.739163 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      506 2023-07-04 17:33:16.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     6913 2023-07-04 16:04:20.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/generate_doc.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     6655 2023-07-04 15:52:27.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/prepare_file.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.740537 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:00:16.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/config.yaml
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1865 2023-07-04 16:40:57.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/generate_response.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      280 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/hashing.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     8712 2023-07-04 17:40:30.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/parse_file.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1222 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/token_counting.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1765 2023-07-04 13:46:08.000000 autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/write_file.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:02:05.741344 autodocumenter-test-0.1.3/src/autodocumenter/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:01:24.000000 autodocumenter-test-0.1.3/src/autodocumenter/utils/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      322 2023-07-04 14:48:59.000000 autodocumenter-test-0.1.3/src/autodocumenter/utils/constants.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      681 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.3/src/autodocumenter/utils/misc.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1343 2023-06-28 20:15:25.000000 autodocumenter-test-0.1.3/src/autodocumenter/utils/output.py
```

### Comparing `autodocumenter-test-0.1.2/LICENSE` & `autodocumenter-test-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/setup.py` & `autodocumenter-test-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = 'autodocumenter-test',   
     packages=find_packages(where='./src'),
     package_dir={'autodocumenter': 'src/autodocumenter'},
     # package_data={'autodocumenter': ['autodocumenter/compile_doc/templates/*.rst', 'autodocumenter/generate_doc/utils/config.yaml']},
-    version = "0.1.2",      
+    version = "0.1.3",      
     license='MIT',  
     description = ('Generate docstrings using ChatGPT and generate Sphinx documentation from the project structure.'),  
     long_description=read('README.md'),
     author = 'Dusan Grujicic',                  
     author_email = 'dusangr22@gmail.com',  
     keywords = ["documentation", "ChatGPT", "Sphinx"],   
     python_requires='>3.9',
```

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/__main__.py` & `autodocumenter-test-0.1.3/src/autodocumenter/__main__.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/compile_doc.py` & `autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/compile_doc.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/compile_doc/templates/module.rst` & `autodocumenter-test-0.1.3/src/autodocumenter/compile_doc/templates/module.rst`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/generate_doc.py` & `autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/prepare_file.py` & `autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/prepare_file.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/utils/config.yaml` & `autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/utils/config.yaml`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.2/src/autodocumenter/generate_doc/write_file.py` & `autodocumenter-test-0.1.3/src/autodocumenter/generate_doc/write_file.py`

 * *Files identical despite different names*

