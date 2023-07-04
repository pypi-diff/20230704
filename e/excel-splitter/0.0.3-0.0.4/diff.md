# Comparing `tmp/excel_splitter-0.0.3.tar.gz` & `tmp/excel_splitter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Python Projects\General\Split_Excel\dist\.tmp-x266u1m3\excel_splitter-0.0.4.tar", last modified: Tue Jul  4 04:10:48 2023, max compression
```

## Comparing `excel_splitter-0.0.3.tar` & `excel_splitter-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/src/Split_Excel_Package/__init__.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/src/Split_Excel_Package/excel_splitter.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/LICENSE
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/README.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.752853 excel_splitter-0.0.4/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 excel_splitter-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1548 2023-07-04 04:10:48.751833 excel_splitter-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2023-07-03 04:50:27.000000 excel_splitter-0.0.4/README.md
+-rw-rw-rw-   0        0        0      764 2023-07-04 04:09:06.000000 excel_splitter-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 04:10:48.752853 excel_splitter-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.711347 excel_splitter-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.718001 excel_splitter-0.0.4/src/Split_Excel_Package/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 excel_splitter-0.0.4/src/Split_Excel_Package/__init__.py
+-rw-rw-rw-   0        0        0     4858 2023-07-03 04:45:27.000000 excel_splitter-0.0.4/src/Split_Excel_Package/excel_splitter.py
+drwxrwxrwx   0        0        0        0 2023-07-04 04:10:48.749787 excel_splitter-0.0.4/src/excel_splitter.egg-info/
+-rw-rw-rw-   0        0        0     1548 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-04 04:10:48.000000 excel_splitter-0.0.4/src/excel_splitter.egg-info/top_level.txt
```

### Comparing `excel_splitter-0.0.3/src/Split_Excel_Package/excel_splitter.py` & `excel_splitter-0.0.4/src/Split_Excel_Package/excel_splitter.py`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.3/LICENSE` & `excel_splitter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.3/README.md` & `excel_splitter-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.3/pyproject.toml` & `excel_splitter-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 [build-system]
-requires = ["hatchling", "openpyxl>=3.0.10"]
-build-backend = "hatchling.build"
+requires      = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "excel_splitter"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
+
+dependencies = [
+     "openpyxl>=3.0.10"
+    
+]
 description = "A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
 readme = "README.md"
 requires-python = ">=3.7"
+keywords = ["Excel", "Split", "opensource"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `excel_splitter-0.0.3/PKG-INFO` & `excel_splitter-0.0.4/src/excel_splitter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1
-Name: excel_splitter
-Version: 0.0.3
-Summary: A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
-Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
-Author-email: Jason Yearry <jasonyearry@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# Excel Splitter
-
-This is a package which will allow you to quickly split a single Excel sheet into either separate tabs of the same report or into different Excel reports.
-
-IMPORTANT: Your sheet must contain a header row to function properly!
-
-Once installed, you can call the split_sheet() function which contains the following parameters: 
-
-split_sheet(split_type, input_report_path, column_number_to_split_by)
-
-ACCEPTED PARAMETER VALUES:
-
-split_type = "separate_files" or "split_tabs"
-input_report_path = the path to the report to be split
-column_number_to_split_by = the # of the Excel column to split by (A = 1, B = 2, C =3, etc.)
-
-EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
-
-split_sheet(split_type='separate_files, input_report_path='PATH_TO_REPORT.xlsx', column_number_to_split_by=2)
-
-KNOWN ISSUE: 
-
-The current version of this script does not support transfer of formulas!!
+Metadata-Version: 2.1
+Name: excel-splitter
+Version: 0.0.4
+Summary: A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
+Author-email: Jason Yearry <jasonyearry@gmail.com>
+Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
+Keywords: Excel,Split,opensource
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Excel Splitter
+
+This is a package which will allow you to quickly split a single Excel sheet into either separate tabs of the same report or into different Excel reports.
+
+IMPORTANT: Your sheet must contain a header row to function properly!
+
+Once installed, you can call the split_sheet() function which contains the following parameters: 
+
+split_sheet(split_type, input_report_path, column_number_to_split_by)
+
+ACCEPTED PARAMETER VALUES:
+
+split_type = "separate_files" or "split_tabs"
+input_report_path = the path to the report to be split
+column_number_to_split_by = the # of the Excel column to split by (A = 1, B = 2, C =3, etc.)
+
+EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
+
+split_sheet(split_type='separate_files, input_report_path='PATH_TO_REPORT.xlsx', column_number_to_split_by=2)
+
+KNOWN ISSUE: 
+
+The current version of this script does not support transfer of formulas!!
```

