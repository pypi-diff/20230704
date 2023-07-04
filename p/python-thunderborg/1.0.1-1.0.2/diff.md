# Comparing `tmp/python-thunderborg-1.0.1.tar.gz` & `tmp/python-thunderborg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-thunderborg-1.0.1.tar", last modified: Fri Aug 20 23:23:11 2021, max compression
+gzip compressed data, was "python-thunderborg-1.0.2.tar", last modified: Tue Jul  4 17:45:30 2023, max compression
```

## Comparing `python-thunderborg-1.0.1.tar` & `python-thunderborg-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2021-08-20 23:23:11.766757 python-thunderborg-1.0.1/
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1081 2017-10-22 13:20:12.000000 python-thunderborg-1.0.1/LICENSE.md
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2939 2021-08-20 23:23:11.766757 python-thunderborg-1.0.1/PKG-INFO
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1936 2021-08-20 23:17:40.000000 python-thunderborg-1.0.1/README.rst
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2021-08-20 23:23:11.766757 python-thunderborg-1.0.1/python_thunderborg.egg-info/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2939 2021-08-20 23:23:11.000000 python-thunderborg-1.0.1/python_thunderborg.egg-info/PKG-INFO
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      272 2021-08-20 23:23:11.000000 python-thunderborg-1.0.1/python_thunderborg.egg-info/SOURCES.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        1 2021-08-20 23:23:11.000000 python-thunderborg-1.0.1/python_thunderborg.egg-info/dependency_links.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        4 2021-08-20 23:23:11.000000 python-thunderborg-1.0.1/python_thunderborg.egg-info/requires.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        6 2021-08-20 23:23:11.000000 python-thunderborg-1.0.1/python_thunderborg.egg-info/top_level.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       38 2021-08-20 23:23:11.766757 python-thunderborg-1.0.1/setup.cfg
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1836 2021-08-20 23:20:09.000000 python-thunderborg-1.0.1/setup.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2021-08-20 23:23:11.766757 python-thunderborg-1.0.1/tborg/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2510 2019-02-03 20:07:49.000000 python-thunderborg-1.0.1/tborg/__init__.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)    44815 2021-08-20 22:22:13.000000 python-thunderborg-1.0.1/tborg/tborg.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-07-04 17:45:30.582549 python-thunderborg-1.0.2/
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1081 2017-10-22 13:20:12.000000 python-thunderborg-1.0.2/LICENSE.md
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2912 2023-07-04 17:45:30.582549 python-thunderborg-1.0.2/PKG-INFO
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     2072 2023-07-04 01:26:36.000000 python-thunderborg-1.0.2/README.rst
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-07-04 17:45:30.582549 python-thunderborg-1.0.2/python_thunderborg.egg-info/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2912 2023-07-04 17:45:30.000000 python-thunderborg-1.0.2/python_thunderborg.egg-info/PKG-INFO
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      272 2023-07-04 17:45:30.000000 python-thunderborg-1.0.2/python_thunderborg.egg-info/SOURCES.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        1 2023-07-04 17:45:30.000000 python-thunderborg-1.0.2/python_thunderborg.egg-info/dependency_links.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        4 2023-07-04 17:45:30.000000 python-thunderborg-1.0.2/python_thunderborg.egg-info/requires.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        6 2023-07-04 17:45:30.000000 python-thunderborg-1.0.2/python_thunderborg.egg-info/top_level.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       38 2023-07-04 17:45:30.582549 python-thunderborg-1.0.2/setup.cfg
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1822 2023-07-04 02:20:04.000000 python-thunderborg-1.0.2/setup.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-07-04 17:45:30.582549 python-thunderborg-1.0.2/tborg/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2510 2019-02-03 20:07:49.000000 python-thunderborg-1.0.2/tborg/__init__.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)    44815 2021-08-20 22:22:13.000000 python-thunderborg-1.0.2/tborg/tborg.py
```

### Comparing `python-thunderborg-1.0.1/LICENSE.md` & `python-thunderborg-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-thunderborg-1.0.1/PKG-INFO` & `python-thunderborg-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: python-thunderborg
-Version: 1.0.1
+Version: 1.0.2
 Summary: ThunderBorg Motor Controller API
-Home-page: https://github.com/cnobile2012/thunderborg
+Home-page: https://github.com/cnobile2012/python-thunderborg
 Author: Carl J. Nobile
 Author-email: carl.nobile@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE.md
 
 ********************************
 ThunderBorg Motor Controller API
 ********************************
@@ -49,15 +45,16 @@
 Overview
 ========
 
 This API for the
 `ThunderBorg <https://www.piborg.org/motor-control-1135/thunderborg>`_
 board has additional features that the original API does not have.
 
-1. Python 2.7.x and 3.4 and greater are supported in the same code base.
+1. Python 2.7.x and 3.8 are supported in the same code base. There is an issue
+   building the ``evdev`` package with all version or Python 3.8 and higher.
 
 2. Built in logging to a log file of your choice--**no print statements**.
 
 3. Auto **voltage in** settings.
 
 4. API initialization is done during class instantiation.
 
@@ -78,14 +75,14 @@
 An API (Application Programming Interface) for the ThunderBorg motor
 controller boards.
 
 `Installation Guide <INSTALL.rst>`_
 
 `Testing Guide <tborg/tests/README.rst>`_
 
+`Pair bluetooth Wireless Controller <PAIR-BT.rst>`_
+
 Feel free to contact me at: carl dot nobile at gmail.com
 
 Complete Documentation can be found on
 `Read the Docs <https://readthedocs.org/>`_ at:
 `Thunder Borg <http://python-thunderborg.readthedocs.io/en/latest/>`_
-
-
```

### Comparing `python-thunderborg-1.0.1/README.rst` & `python-thunderborg-1.0.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 Overview
 ========
 
 This API for the
 `ThunderBorg <https://www.piborg.org/motor-control-1135/thunderborg>`_
 board has additional features that the original API does not have.
 
-1. Python 2.7.x and 3.4 and greater are supported in the same code base.
+1. Python 2.7.x and 3.8 are supported in the same code base. There is an issue
+   building the ``evdev`` package with all version or Python 3.8 and higher.
 
 2. Built in logging to a log file of your choice--**no print statements**.
 
 3. Auto **voltage in** settings.
 
 4. API initialization is done during class instantiation.
 
@@ -52,12 +53,14 @@
 An API (Application Programming Interface) for the ThunderBorg motor
 controller boards.
 
 `Installation Guide <INSTALL.rst>`_
 
 `Testing Guide <tborg/tests/README.rst>`_
 
+`Pair bluetooth Wireless Controller <PAIR-BT.rst>`_
+
 Feel free to contact me at: carl dot nobile at gmail.com
 
 Complete Documentation can be found on
 `Read the Docs <https://readthedocs.org/>`_ at:
 `Thunder Borg <http://python-thunderborg.readthedocs.io/en/latest/>`_
```

### Comparing `python-thunderborg-1.0.1/python_thunderborg.egg-info/PKG-INFO` & `python-thunderborg-1.0.2/python_thunderborg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: python-thunderborg
-Version: 1.0.1
+Version: 1.0.2
 Summary: ThunderBorg Motor Controller API
-Home-page: https://github.com/cnobile2012/thunderborg
+Home-page: https://github.com/cnobile2012/python-thunderborg
 Author: Carl J. Nobile
 Author-email: carl.nobile@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE.md
 
 ********************************
 ThunderBorg Motor Controller API
 ********************************
@@ -49,15 +45,16 @@
 Overview
 ========
 
 This API for the
 `ThunderBorg <https://www.piborg.org/motor-control-1135/thunderborg>`_
 board has additional features that the original API does not have.
 
-1. Python 2.7.x and 3.4 and greater are supported in the same code base.
+1. Python 2.7.x and 3.8 are supported in the same code base. There is an issue
+   building the ``evdev`` package with all version or Python 3.8 and higher.
 
 2. Built in logging to a log file of your choice--**no print statements**.
 
 3. Auto **voltage in** settings.
 
 4. API initialization is done during class instantiation.
 
@@ -78,14 +75,14 @@
 An API (Application Programming Interface) for the ThunderBorg motor
 controller boards.
 
 `Installation Guide <INSTALL.rst>`_
 
 `Testing Guide <tborg/tests/README.rst>`_
 
+`Pair bluetooth Wireless Controller <PAIR-BT.rst>`_
+
 Feel free to contact me at: carl dot nobile at gmail.com
 
 Complete Documentation can be found on
 `Read the Docs <https://readthedocs.org/>`_ at:
 `Thunder Borg <http://python-thunderborg.readthedocs.io/en/latest/>`_
-
-
```

### Comparing `python-thunderborg-1.0.1/setup.py` & `python-thunderborg-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import os
 import re
 from setuptools import setup
 
 def version():
-    regex = r'^(?m){}[\s]*=[\s]*(?P<ver>\d*)$'
+    regex = r'(?m)(^{}[\s]*=[\s]*(?P<ver>\d*)$)'
 
     with open(os.path.join(os.path.dirname(__file__), 'include.mk')) as f:
         ver = f.read()
 
     major = re.search(regex.format('MAJORVERSION'), ver).group('ver')
     minor = re.search(regex.format('MINORVERSION'), ver).group('ver')
     patch = re.search(regex.format('PATCHLEVEL'), ver).group('ver')
-    return "{}.{}.{}".format(major, minor, patch)
+    # Look for a tag indicating a pre-release candidate. ex. rc1
+    env_value = os.environ.get('PR_TAG', '')
+    return "{}.{}.{}{}".format(major, minor, patch, env_value)
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
-# allow setup.py to be run from any path
+# Allow setup.py to be run from any path.
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='python-thunderborg',
     version=version(),
     packages=['tborg',],
     include_package_data=True,
     license='MIT',
     description=('ThunderBorg Motor Controller API'),
     long_description=README,
-    url='https://github.com/cnobile2012/thunderborg',
+    url='https://github.com/cnobile2012/python-thunderborg',
     author='Carl J. Nobile',
     author_email='carl.nobile@gmail.com',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         ],
     install_requires=[
         'six',
         ],
     )
```

### Comparing `python-thunderborg-1.0.1/tborg/__init__.py` & `python-thunderborg-1.0.2/tborg/__init__.py`

 * *Files identical despite different names*

### Comparing `python-thunderborg-1.0.1/tborg/tborg.py` & `python-thunderborg-1.0.2/tborg/tborg.py`

 * *Files identical despite different names*

