# Comparing `tmp/autodocumenter-test-0.1.5.tar.gz` & `tmp/autodocumenter-test-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodocumenter-test-0.1.5.tar", last modified: Tue Jul  4 20:26:14 2023, max compression
+gzip compressed data, was "autodocumenter-test-0.1.6.tar", last modified: Tue Jul  4 20:30:15 2023, max compression
```

## Comparing `autodocumenter-test-0.1.5.tar` & `autodocumenter-test-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.757384 autodocumenter-test-0.1.5/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.5/LICENSE
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 19:31:50.000000 autodocumenter-test-0.1.5/MANIFEST.in
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 20:26:14.757467 autodocumenter-test-0.1.5/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.5/README.md
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.751242 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 20:26:14.000000 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/PKG-INFO
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1520 2023-07-04 20:26:14.000000 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/SOURCES.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 20:26:14.000000 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/dependency_links.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       64 2023-07-04 20:26:14.000000 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/entry_points.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 20:26:14.000000 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/requires.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)       15 2023-07-04 20:26:14.000000 autodocumenter-test-0.1.5/autodocumenter_test.egg-info/top_level.txt
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 20:26:14.757709 autodocumenter-test-0.1.5/setup.cfg
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1449 2023-07-04 20:26:05.000000 autodocumenter-test-0.1.5/setup.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.749421 autodocumenter-test-0.1.5/src/
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.751479 autodocumenter-test-0.1.5/src/autodocumenter/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      183 2023-07-04 20:26:10.000000 autodocumenter-test-0.1.5/src/autodocumenter/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     4928 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.5/src/autodocumenter/__main__.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.752067 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      305 2023-07-04 17:30:51.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     2778 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/compile_doc.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.752869 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/templates/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/templates/base.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/templates/class.rst
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/templates/module.rst
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.753855 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:00:21.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     2967 2023-07-04 17:38:52.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/edit_config.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      404 2023-07-04 17:39:01.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/edit_index.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      578 2023-07-04 20:08:21.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/edit_reference.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      139 2023-07-04 17:39:27.000000 autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/edit_user_guide.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.754753 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      506 2023-07-04 17:33:16.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     6913 2023-07-04 16:04:20.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/generate_doc.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     6656 2023-07-04 20:05:40.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/prepare_file.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.756262 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:00:16.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/config.yaml
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1865 2023-07-04 16:40:57.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/generate_response.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      280 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/hashing.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     8712 2023-07-04 17:40:30.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/parse_file.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1222 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/token_counting.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1765 2023-07-04 13:46:08.000000 autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/write_file.py
-drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:26:14.757157 autodocumenter-test-0.1.5/src/autodocumenter/utils/
--rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:01:24.000000 autodocumenter-test-0.1.5/src/autodocumenter/utils/__init__.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      322 2023-07-04 14:48:59.000000 autodocumenter-test-0.1.5/src/autodocumenter/utils/constants.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)      681 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.5/src/autodocumenter/utils/misc.py
--rw-r--r--   0 dusangrujicic   (501) staff       (20)     1343 2023-06-28 20:15:25.000000 autodocumenter-test-0.1.5/src/autodocumenter/utils/output.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.339567 autodocumenter-test-0.1.6/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1061 2023-07-04 16:01:11.000000 autodocumenter-test-0.1.6/LICENSE
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      148 2023-07-04 20:29:25.000000 autodocumenter-test-0.1.6/MANIFEST.in
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 20:30:15.339626 autodocumenter-test-0.1.6/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       80 2023-07-04 16:00:51.000000 autodocumenter-test-0.1.6/README.md
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.333892 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      402 2023-07-04 20:30:15.000000 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/PKG-INFO
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1520 2023-07-04 20:30:15.000000 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/SOURCES.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        1 2023-07-04 20:30:15.000000 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/dependency_links.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       64 2023-07-04 20:30:15.000000 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/entry_points.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      162 2023-07-04 20:30:15.000000 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/requires.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)       15 2023-07-04 20:30:15.000000 autodocumenter-test-0.1.6/autodocumenter_test.egg-info/top_level.txt
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      103 2023-07-04 20:30:15.340322 autodocumenter-test-0.1.6/setup.cfg
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1484 2023-07-04 20:29:51.000000 autodocumenter-test-0.1.6/setup.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.332042 autodocumenter-test-0.1.6/src/
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.334120 autodocumenter-test-0.1.6/src/autodocumenter/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      183 2023-07-04 20:30:01.000000 autodocumenter-test-0.1.6/src/autodocumenter/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     4928 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.6/src/autodocumenter/__main__.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.334676 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      305 2023-07-04 17:30:51.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     2778 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/compile_doc.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.335445 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/templates/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      121 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/templates/base.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      483 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/templates/class.rst
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1824 2023-06-26 19:25:22.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/templates/module.rst
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.336354 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:00:21.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     2967 2023-07-04 17:38:52.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/edit_config.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      404 2023-07-04 17:39:01.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/edit_index.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      578 2023-07-04 20:08:21.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/edit_reference.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      139 2023-07-04 17:39:27.000000 autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/edit_user_guide.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.337240 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      506 2023-07-04 17:33:16.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     6913 2023-07-04 16:04:20.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/generate_doc.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     6656 2023-07-04 20:05:40.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/prepare_file.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.338472 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:00:16.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1618 2023-07-01 15:07:10.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/config.yaml
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1865 2023-07-04 16:40:57.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/generate_response.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      280 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/hashing.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     8712 2023-07-04 17:40:30.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/parse_file.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1222 2023-07-04 15:33:54.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/token_counting.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1765 2023-07-04 13:46:08.000000 autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/write_file.py
+drwxr-xr-x   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:30:15.339349 autodocumenter-test-0.1.6/src/autodocumenter/utils/
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)        0 2023-07-04 20:01:24.000000 autodocumenter-test-0.1.6/src/autodocumenter/utils/__init__.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      322 2023-07-04 14:48:59.000000 autodocumenter-test-0.1.6/src/autodocumenter/utils/constants.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)      681 2023-07-03 19:32:49.000000 autodocumenter-test-0.1.6/src/autodocumenter/utils/misc.py
+-rw-r--r--   0 dusangrujicic   (501) staff       (20)     1343 2023-06-28 20:15:25.000000 autodocumenter-test-0.1.6/src/autodocumenter/utils/output.py
```

### Comparing `autodocumenter-test-0.1.5/LICENSE` & `autodocumenter-test-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/autodocumenter_test.egg-info/SOURCES.txt` & `autodocumenter-test-0.1.6/autodocumenter_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/setup.py` & `autodocumenter-test-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = 'autodocumenter-test',   
     packages=find_packages(where='./src'),
     package_dir={'autodocumenter': 'src/autodocumenter'},
-    package_data={'autodocumenter': ['src/autodocumenter/compile_doc/templates/*.rst', 'src/autodocumenter/generate_doc/utils/config.yaml']},
-    version = "0.1.5",      
+    # package_data={'autodocumenter': ['src/autodocumenter/compile_doc/templates/*.rst', 'src/autodocumenter/generate_doc/utils/config.yaml']},
+    version = "0.1.6",      
     license='MIT',  
     description = ('Generate docstrings using ChatGPT and generate Sphinx documentation from the project structure.'),  
     long_description=read('README.md'),
     author = 'Dusan Grujicic',                  
     author_email = 'dusangr22@gmail.com',  
     keywords = ["documentation", "ChatGPT", "Sphinx"],   
     python_requires='>3.9',
@@ -31,9 +31,10 @@
         "aiomisc>=17.3.2",
         "alive_progress>=3.1.4",
         "openlimit>=0.2.7",
         "PyYAML>=6.0"
     ],
     entry_points={
         'console_scripts': ['autodocumenter = autodocumenter.__main__:main']
-    }
+    },
+    include_package_data = True
 )
```

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/__main__.py` & `autodocumenter-test-0.1.6/src/autodocumenter/__main__.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/compile_doc.py` & `autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/compile_doc.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/templates/module.rst` & `autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/templates/module.rst`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/edit_config.py` & `autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/edit_config.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/compile_doc/utils/edit_reference.py` & `autodocumenter-test-0.1.6/src/autodocumenter/compile_doc/utils/edit_reference.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/generate_doc.py` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/prepare_file.py` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/prepare_file.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/config.yaml` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/config.yaml`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/generate_response.py` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/generate_response.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/parse_file.py` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/parse_file.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/utils/token_counting.py` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/utils/token_counting.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/generate_doc/write_file.py` & `autodocumenter-test-0.1.6/src/autodocumenter/generate_doc/write_file.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/utils/misc.py` & `autodocumenter-test-0.1.6/src/autodocumenter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autodocumenter-test-0.1.5/src/autodocumenter/utils/output.py` & `autodocumenter-test-0.1.6/src/autodocumenter/utils/output.py`

 * *Files identical despite different names*

