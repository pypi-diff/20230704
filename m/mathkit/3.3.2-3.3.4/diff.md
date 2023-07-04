# Comparing `tmp/mathkit-3.3.2.tar.gz` & `tmp/mathkit-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-3.3.2.tar", last modified: Tue Jul  4 04:13:50 2023, max compression
+gzip compressed data, was "mathkit-3.3.4.tar", last modified: Tue Jul  4 04:16:18 2023, max compression
```

## Comparing `mathkit-3.3.2.tar` & `mathkit-3.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 04:13:50.383587 mathkit-3.3.2/
--rw-rw-rw-   0        0        0     3740 2023-07-04 04:13:50.382608 mathkit-3.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3295 2023-07-04 04:10:33.000000 mathkit-3.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 04:13:50.356610 mathkit-3.3.2/mathkit/
--rw-rw-rw-   0        0        0      558 2023-07-04 03:56:54.000000 mathkit-3.3.2/mathkit/__init__.py
--rw-rw-rw-   0        0        0    16102 2023-07-04 04:13:33.000000 mathkit-3.3.2/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:13:50.381708 mathkit-3.3.2/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3740 2023-07-04 04:13:50.000000 mathkit-3.3.2/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-04 04:13:50.000000 mathkit-3.3.2/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 04:13:50.000000 mathkit-3.3.2/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 04:13:50.000000 mathkit-3.3.2/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 04:13:50.383587 mathkit-3.3.2/setup.cfg
--rw-rw-rw-   0        0        0      712 2023-07-04 04:13:46.000000 mathkit-3.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:16:18.857222 mathkit-3.3.4/
+-rw-rw-rw-   0        0        0     3740 2023-07-04 04:16:18.855225 mathkit-3.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3295 2023-07-04 04:10:33.000000 mathkit-3.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 04:16:18.834801 mathkit-3.3.4/mathkit/
+-rw-rw-rw-   0        0        0      558 2023-07-04 03:56:54.000000 mathkit-3.3.4/mathkit/__init__.py
+-rw-rw-rw-   0        0        0    16376 2023-07-04 04:16:01.000000 mathkit-3.3.4/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:16:18.852214 mathkit-3.3.4/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3740 2023-07-04 04:16:18.000000 mathkit-3.3.4/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-04 04:16:18.000000 mathkit-3.3.4/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 04:16:18.000000 mathkit-3.3.4/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 04:16:18.000000 mathkit-3.3.4/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 04:16:18.857222 mathkit-3.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-07-04 04:16:13.000000 mathkit-3.3.4/setup.py
```

### Comparing `mathkit-3.3.2/PKG-INFO` & `mathkit-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 3.3.2
+Version: 3.3.4
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-3.3.2/README.md` & `mathkit-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mathkit-3.3.2/mathkit/__init__.py` & `mathkit-3.3.4/mathkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mathkit-3.3.2/mathkit/main.py` & `mathkit-3.3.4/mathkit/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
     Returns:
         None
 
 """
 import math
 import sys
+import time
 
 def add(num1=None, num2=None):
     """
     Add two numbers and print the result.
 
     Args:
         num1 (int or float): The first number (default: None).
@@ -478,43 +479,54 @@
     print("9. Percentage")
     print("10. Power")
     print("11. Trigonometry")
     print("12. Exit")
     choice = int(input("Enter your choice: "))
     if choice == 1:
         add()
+        time.sleep(2)
         main()
     elif choice == 2:
         sub()
+        time.sleep(2)
         main()
     elif choice == 3:
         mul()
+        time.sleep(2)
         main()
     elif choice == 4:
-        div()
+        div()        
+        time.sleep(2)
         main()
     elif choice == 5:
         sqr()
+        time.sleep(2)
         main()
     elif choice == 6:
         sqrt()
+        time.sleep(2)
         main()
     elif choice == 7:
         cube()
+        time.sleep(2)
         main()
     elif choice == 8:
         cbrt()
+        time.sleep(2)
         main()
     elif choice == 9:
         percentage()
+        time.sleep(2)
         main()
     elif choice == 10:
         power()
+        time.sleep(2)
         main()
     elif choice == 11:
         trig()
+        time.sleep(2)
         main()
     elif choice == 12:
         exit()
     else:
         print("Invalid choice!")
         main()
```

### Comparing `mathkit-3.3.2/mathkit.egg-info/PKG-INFO` & `mathkit-3.3.4/mathkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 3.3.2
+Version: 3.3.4
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-3.3.2/setup.py` & `mathkit-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="3.3.2",
+    version="3.3.4",
     author="TheUnkownHacker",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```

