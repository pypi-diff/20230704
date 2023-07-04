# Comparing `tmp/mathkit-2.15.2.tar.gz` & `tmp/mathkit-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-2.15.2.tar", last modified: Mon Jul  3 06:57:50 2023, max compression
+gzip compressed data, was "mathkit-3.1.2.tar", last modified: Tue Jul  4 04:01:31 2023, max compression
```

## Comparing `mathkit-2.15.2.tar` & `mathkit-3.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:57:50.048018 mathkit-2.15.2/
--rw-rw-rw-   0        0        0     3467 2023-07-03 06:57:50.046967 mathkit-2.15.2/PKG-INFO
--rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-2.15.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 06:57:50.022351 mathkit-2.15.2/mathkit/
--rw-rw-rw-   0        0        0      527 2023-07-03 06:17:43.000000 mathkit-2.15.2/mathkit/__init__.py
--rw-rw-rw-   0        0        0    10036 2023-07-03 06:56:14.000000 mathkit-2.15.2/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:57:50.045044 mathkit-2.15.2/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3467 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 06:57:50.048018 mathkit-2.15.2/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-07-03 06:57:44.000000 mathkit-2.15.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:01:31.283736 mathkit-3.1.2/
+-rw-rw-rw-   0        0        0     3589 2023-07-04 04:01:31.282731 mathkit-3.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3144 2023-07-04 04:00:48.000000 mathkit-3.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 04:01:31.244934 mathkit-3.1.2/mathkit/
+-rw-rw-rw-   0        0        0      558 2023-07-04 03:56:54.000000 mathkit-3.1.2/mathkit/__init__.py
+-rw-rw-rw-   0        0        0    15926 2023-07-04 03:56:08.000000 mathkit-3.1.2/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:01:31.280811 mathkit-3.1.2/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3589 2023-07-04 04:01:31.000000 mathkit-3.1.2/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-04 04:01:31.000000 mathkit-3.1.2/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 04:01:31.000000 mathkit-3.1.2/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 04:01:31.000000 mathkit-3.1.2/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 04:01:31.284734 mathkit-3.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-07-04 04:01:02.000000 mathkit-3.1.2/setup.py
```

### Comparing `mathkit-2.15.2/PKG-INFO` & `mathkit-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 2.15.2
+Version: 3.1.2
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# MathKit
+# MathKit - A Mathematical Library Made Simple
 
 **MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.**
 
+## Example Short Usage
+
+```python
+from mathkit import main
+main()
+
+
+
+
+
+
 ## Example Usage
 
 ```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
@@ -59,15 +70,15 @@
 elif choice == 9:
     sqrt()  # You can predefine a number by looking at the syntax given below.
 elif choice == 10:
     cbrt()  # You can predefine a number by looking at the syntax given below.
 elif choice == 11:
     fact()  # You can predefine a number by looking at the syntax given below.
 elif choice == 12:
-    percent()  # You can predefine a number by looking at the syntax given below.
+    percentage()  # You can predefine a number by looking at the syntax given below.
 elif choice == 13:
     lcm()  # You can predefine a number by looking at the syntax given below.
 elif choice == 14:
     hcf()  # You can predefine a number by looking at the syntax given below.
 elif choice == 15:
     log()  # You can predefine a number by looking at the syntax given below.
 elif choice == 16:
```

### Comparing `mathkit-2.15.2/README.md` & `mathkit-3.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,22 @@
-# MathKit
+# MathKit - A Mathematical Library Made Simple
 
 **MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.**
 
+## Example Short Usage
+
+```python
+from mathkit import main
+main()
+
+
+
+
+
+
 ## Example Usage
 
 ```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
@@ -46,15 +57,15 @@
 elif choice == 9:
     sqrt()  # You can predefine a number by looking at the syntax given below.
 elif choice == 10:
     cbrt()  # You can predefine a number by looking at the syntax given below.
 elif choice == 11:
     fact()  # You can predefine a number by looking at the syntax given below.
 elif choice == 12:
-    percent()  # You can predefine a number by looking at the syntax given below.
+    percentage()  # You can predefine a number by looking at the syntax given below.
 elif choice == 13:
     lcm()  # You can predefine a number by looking at the syntax given below.
 elif choice == 14:
     hcf()  # You can predefine a number by looking at the syntax given below.
 elif choice == 15:
     log()  # You can predefine a number by looking at the syntax given below.
 elif choice == 16:
```

### Comparing `mathkit-2.15.2/mathkit/__init__.py` & `mathkit-3.1.2/mathkit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 from .main import mul
 from .main import percentage
 from .main import power
 from .main import sqrt
 from .main import sqr
 from .main import sub
 from .main import trig
+from .main import main
 
-__all__ = ['add', 'cube', 'cbrt', 'div', 'fact', 'hcf', 'lcm', 'log', 'mod', 'mul', 'percentage', 'power', 'sqrt', 'sqr', 'sub','trig']
+__all__ = ['add', 'cube', 'cbrt', 'div', 'fact', 'hcf', 'lcm', 'log', 'mod', 'mul', 'percentage', 'power', 'sqrt', 'sqr', 'sub','trig','main']
```

### Comparing `mathkit-2.15.2/mathkit.egg-info/PKG-INFO` & `mathkit-3.1.2/mathkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 2.15.2
+Version: 3.1.2
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# MathKit
+# MathKit - A Mathematical Library Made Simple
 
 **MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.**
 
+## Example Short Usage
+
+```python
+from mathkit import main
+main()
+
+
+
+
+
+
 ## Example Usage
 
 ```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
@@ -59,15 +70,15 @@
 elif choice == 9:
     sqrt()  # You can predefine a number by looking at the syntax given below.
 elif choice == 10:
     cbrt()  # You can predefine a number by looking at the syntax given below.
 elif choice == 11:
     fact()  # You can predefine a number by looking at the syntax given below.
 elif choice == 12:
-    percent()  # You can predefine a number by looking at the syntax given below.
+    percentage()  # You can predefine a number by looking at the syntax given below.
 elif choice == 13:
     lcm()  # You can predefine a number by looking at the syntax given below.
 elif choice == 14:
     hcf()  # You can predefine a number by looking at the syntax given below.
 elif choice == 15:
     log()  # You can predefine a number by looking at the syntax given below.
 elif choice == 16:
```

### Comparing `mathkit-2.15.2/setup.py` & `mathkit-3.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="2.15.2",
+    version="3.1.2",
     author="TheUnkownHacker",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```

