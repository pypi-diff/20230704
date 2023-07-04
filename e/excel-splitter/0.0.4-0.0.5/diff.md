# Comparing `tmp/excel_splitter-0.0.4.tar.gz` & `tmp/excel_splitter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jason\Desktop\Python Projects\General\Split_Excel\dist\.tmp-x266u1m3\excel_splitter-0.0.4.tar", last modified: Tue Jul  4 04:10:48 2023, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-tzdlkib8\excel_splitter-0.0.5.tar", last modified: Tue Jul  4 04:19:45 2023, max compression
```

## Comparing `excel_splitter-0.0.4.tar` & `excel_splitter-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.752853 excel_splitter-0.0.4/
--rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 excel_splitter-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1548 2023-07-04 04:10:48.751833 excel_splitter-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      949 2023-07-03 04:50:27.000000 excel_splitter-0.0.4/README.md
--rw-rw-rw-   0        0        0      764 2023-07-04 04:09:06.000000 excel_splitter-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 04:10:48.752853 excel_splitter-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.711347 excel_splitter-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.718001 excel_splitter-0.0.4/src/Split_Excel_Package/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 excel_splitter-0.0.4/src/Split_Excel_Package/__init__.py
--rw-rw-rw-   0        0        0     4858 2023-07-03 04:45:27.000000 excel_splitter-0.0.4/src/Split_Excel_Package/excel_splitter.py
-drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.749787 excel_splitter-0.0.4/src/excel_splitter.egg-info/
--rw-rw-rw-   0        0        0     1548 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 04:19:45.836034 excel_splitter-0.0.5/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 excel_splitter-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1548 2023-07-04 04:19:45.835016 excel_splitter-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2023-07-03 04:50:27.000000 excel_splitter-0.0.5/README.md
+-rw-rw-rw-   0        0        0      764 2023-07-04 04:19:32.000000 excel_splitter-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 04:19:45.836034 excel_splitter-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 04:19:45.807639 excel_splitter-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 04:19:45.813743 excel_splitter-0.0.5/src/Split_Excel_Package/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 excel_splitter-0.0.5/src/Split_Excel_Package/__init__.py
+-rw-rw-rw-   0        0        0     4858 2023-07-03 04:45:27.000000 excel_splitter-0.0.5/src/Split_Excel_Package/excel_splitter.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:19:45.833974 excel_splitter-0.0.5/src/excel_splitter.egg-info/
+-rw-rw-rw-   0        0        0     1548 2023-07-04 04:19:45.000000 excel_splitter-0.0.5/src/excel_splitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-04 04:19:45.000000 excel_splitter-0.0.5/src/excel_splitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 04:19:45.000000 excel_splitter-0.0.5/src/excel_splitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 04:19:45.000000 excel_splitter-0.0.5/src/excel_splitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-04 04:19:45.000000 excel_splitter-0.0.5/src/excel_splitter.egg-info/top_level.txt
```

### Comparing `excel_splitter-0.0.4/LICENSE` & `excel_splitter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.4/PKG-INFO` & `excel_splitter-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_splitter
-Version: 0.0.4
+Version: 0.0.5
 Summary: A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `excel_splitter-0.0.4/README.md` & `excel_splitter-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.4/pyproject.toml` & `excel_splitter-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "excel_splitter"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
 
 dependencies = [
      "openpyxl>=3.0.10"
```

### Comparing `excel_splitter-0.0.4/src/Split_Excel_Package/excel_splitter.py` & `excel_splitter-0.0.5/src/Split_Excel_Package/excel_splitter.py`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.4/src/excel_splitter.egg-info/PKG-INFO` & `excel_splitter-0.0.5/src/excel_splitter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-splitter
-Version: 0.0.4
+Version: 0.0.5
 Summary: A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

