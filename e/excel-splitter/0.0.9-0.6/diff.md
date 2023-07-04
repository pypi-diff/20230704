# Comparing `tmp/excel_splitter-0.0.9.tar.gz` & `tmp/excel-splitter-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-62k_5try\excel_splitter-0.0.9.tar", last modified: Tue Jul  4 07:17:32 2023, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-5gxhu12x\excel-splitter-0.6.tar", last modified: Tue Jul  4 04:41:08 2023, max compression
```

## Comparing `excel_splitter-0.0.9.tar` & `excel-splitter-0.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 07:17:32.965706 excel_splitter-0.0.9/
--rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 excel_splitter-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1548 2023-07-04 07:17:32.965200 excel_splitter-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      949 2023-07-03 04:50:27.000000 excel_splitter-0.0.9/README.md
--rw-rw-rw-   0        0        0      786 2023-07-04 07:16:09.000000 excel_splitter-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 07:17:32.966214 excel_splitter-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 excel_splitter-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:17:32.940846 excel_splitter-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 07:17:32.949987 excel_splitter-0.0.9/src/excel_splitter/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 excel_splitter-0.0.9/src/excel_splitter/__init__.py
--rw-rw-rw-   0        0        0     4858 2023-07-03 04:45:27.000000 excel_splitter-0.0.9/src/excel_splitter/excel_splitter.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:17:32.964187 excel_splitter-0.0.9/src/excel_splitter.egg-info/
--rw-rw-rw-   0        0        0     1548 2023-07-04 07:17:32.000000 excel_splitter-0.0.9/src/excel_splitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-07-04 07:17:32.000000 excel_splitter-0.0.9/src/excel_splitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 07:17:32.000000 excel_splitter-0.0.9/src/excel_splitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-04 07:17:32.000000 excel_splitter-0.0.9/src/excel_splitter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 04:41:08.850621 excel-splitter-0.6/
+-rw-rw-rw-   0        0        0      241 2023-07-04 04:41:08.850621 excel-splitter-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2023-07-03 04:50:27.000000 excel-splitter-0.6/README.md
+-rw-rw-rw-   0        0        0      115 2023-07-04 04:41:08.852654 excel-splitter-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-07-04 04:40:45.000000 excel-splitter-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:41:08.828388 excel-splitter-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 04:41:08.833511 excel-splitter-0.6/src/Split_Excel_Package/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 excel-splitter-0.6/src/Split_Excel_Package/__init__.py
+-rw-rw-rw-   0        0        0     4858 2023-07-03 04:45:27.000000 excel-splitter-0.6/src/Split_Excel_Package/excel_splitter.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:41:08.850112 excel-splitter-0.6/src/excel_splitter.egg-info/
+-rw-rw-rw-   0        0        0      241 2023-07-04 04:41:08.000000 excel-splitter-0.6/src/excel_splitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-04 04:41:08.000000 excel-splitter-0.6/src/excel_splitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 04:41:08.000000 excel-splitter-0.6/src/excel_splitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 04:41:08.000000 excel-splitter-0.6/src/excel_splitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-04 04:41:08.000000 excel-splitter-0.6/src/excel_splitter.egg-info/top_level.txt
```

### Comparing `excel_splitter-0.0.9/README.md` & `excel-splitter-0.6/README.md`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.9/src/excel_splitter/excel_splitter.py` & `excel-splitter-0.6/src/Split_Excel_Package/excel_splitter.py`

 * *Files identical despite different names*

