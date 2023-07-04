# Comparing `tmp/QuBuilders-0.0.3.tar.gz` & `tmp/QuBuilders-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuBuilders-0.0.3.tar", last modified: Tue Jul  4 18:28:22 2023, max compression
+gzip compressed data, was "QuBuilders-0.0.4.tar", last modified: Tue Jul  4 18:43:17 2023, max compression
```

## Comparing `QuBuilders-0.0.3.tar` & `QuBuilders-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:28:22.868782 QuBuilders-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1820 2023-07-04 18:28:22.867782 QuBuilders-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 18:28:22.848255 QuBuilders-0.0.3/QuBuilders/
--rw-rw-rw-   0        0        0        0 2023-07-04 18:27:26.000000 QuBuilders-0.0.3/QuBuilders/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/QuBuilders/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:28:22.865134 QuBuilders-0.0.3/QuBuilders.egg-info/
--rw-rw-rw-   0        0        0     1820 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/README.md
--rw-rw-rw-   0        0        0      669 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 18:28:22.868782 QuBuilders-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1807 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:43:17.208802 QuBuilders-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-07-04 18:22:08.000000 QuBuilders-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1820 2023-07-04 18:43:17.207801 QuBuilders-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 18:43:17.189878 QuBuilders-0.0.4/QuBuilders/
+-rw-rw-rw-   0        0        0       17 2023-07-04 18:41:40.000000 QuBuilders-0.0.4/QuBuilders/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-04 18:22:08.000000 QuBuilders-0.0.4/QuBuilders/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:43:17.205806 QuBuilders-0.0.4/QuBuilders.egg-info/
+-rw-rw-rw-   0        0        0     1820 2023-07-04 18:43:17.000000 QuBuilders-0.0.4/QuBuilders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-07-04 18:43:17.000000 QuBuilders-0.0.4/QuBuilders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 18:43:17.000000 QuBuilders-0.0.4/QuBuilders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-04 18:43:17.000000 QuBuilders-0.0.4/QuBuilders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-04 18:43:17.000000 QuBuilders-0.0.4/QuBuilders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-07-04 18:22:08.000000 QuBuilders-0.0.4/README.md
+-rw-rw-rw-   0        0        0      669 2023-07-04 18:43:01.000000 QuBuilders-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 18:43:17.208802 QuBuilders-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2023-07-04 18:43:01.000000 QuBuilders-0.0.4/setup.py
```

### Comparing `QuBuilders-0.0.3/LICENSE` & `QuBuilders-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `QuBuilders-0.0.3/PKG-INFO` & `QuBuilders-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuBuilders
-Version: 0.0.3
+Version: 0.0.4
 Summary: a pakage that help you to make n choice questions faster
 Home-page: https://github.com/AmirrezaZahraei1387/QuBu
 Download-URL: https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz
 Author: Amirreza Zahraei
 Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
```

### Comparing `QuBuilders-0.0.3/QuBuilders.egg-info/PKG-INFO` & `QuBuilders-0.0.4/QuBuilders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuBuilders
-Version: 0.0.3
+Version: 0.0.4
 Summary: a pakage that help you to make n choice questions faster
 Home-page: https://github.com/AmirrezaZahraei1387/QuBu
 Download-URL: https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz
 Author: Amirreza Zahraei
 Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
```

### Comparing `QuBuilders-0.0.3/README.md` & `QuBuilders-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `QuBuilders-0.0.3/pyproject.toml` & `QuBuilders-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling",'validators', 'beautifulsoup4',]
 build-backend = "hatchling.build"
 [project]
 name = "QuBuilders"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Amirrza Zahraei", email="amir.reza.zahraei@gmail.com" },
 ]
 description = "a pakage that help you to make n choice questions faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QuBuilders-0.0.3/setup.py` & `QuBuilders-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+
+
 from distutils.core import setup
 setup(
   name = 'QuBuilders',         # How you named your package folder (MyLib)
   packages = ['QuBuilders'],   # Chose the same as "name"
-  version = '0.0.3',      # Start with a small number and increase it with every change you make
+  version = '0.0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'this is a python package help you to make n choice questions',   # Give a short description about your library
   author = 'Amirreza Zahraei',                   # Type in your name
   author_email = 'amir.reza.zahraei@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AmirrezaZahraei1387/QuBu',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz',    # I explain this later on
   keywords = ['Question', 'multiple choice questions', 'creating questions'],   # Keywords that define your package best
```

