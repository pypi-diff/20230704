# Comparing `tmp/resfeci-0.0.12.tar.gz` & `tmp/resfeci-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-kjkjpst3\resfeci-0.0.12.tar", last modified: Tue Jul  4 08:17:23 2023, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-sw62cb_k\resfeci-0.0.13.tar", last modified: Tue Jul  4 08:29:27 2023, max compression
```

## Comparing `resfeci-0.0.12.tar` & `resfeci-0.0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:17:23.184334 resfeci-0.0.12/
--rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.12/LICENSE
--rw-rw-rw-   0        0        0     2080 2023-07-04 08:17:23.183827 resfeci-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2023-07-04 08:16:22.000000 resfeci-0.0.12/README.md
--rw-rw-rw-   0        0        0      797 2023-07-04 08:16:48.000000 resfeci-0.0.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 08:17:23.184840 resfeci-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:17:23.158430 resfeci-0.0.12/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:17:23.168107 resfeci-0.0.12/src/resfeci/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.12/src/resfeci/__init__.py
--rw-rw-rw-   0        0        0     4858 2023-07-04 07:56:04.000000 resfeci-0.0.12/src/resfeci/excel_split.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:17:23.182812 resfeci-0.0.12/src/resfeci.egg-info/
--rw-rw-rw-   0        0        0     2080 2023-07-04 08:17:23.000000 resfeci-0.0.12/src/resfeci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-04 08:17:23.000000 resfeci-0.0.12/src/resfeci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:17:23.000000 resfeci-0.0.12/src/resfeci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 08:17:23.000000 resfeci-0.0.12/src/resfeci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 08:29:27.600432 resfeci-0.0.13/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.13/LICENSE
+-rw-rw-rw-   0        0        0     2099 2023-07-04 08:29:27.599922 resfeci-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2023-07-04 08:28:43.000000 resfeci-0.0.13/README.md
+-rw-rw-rw-   0        0        0      809 2023-07-04 08:28:43.000000 resfeci-0.0.13/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:29:27.600432 resfeci-0.0.13/setup.cfg
+-rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:29:27.570448 resfeci-0.0.13/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:29:27.583669 resfeci-0.0.13/src/resfeci/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.13/src/resfeci/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-07-04 08:27:15.000000 resfeci-0.0.13/src/resfeci/excel_split.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:29:27.598396 resfeci-0.0.13/src/resfeci.egg-info/
+-rw-rw-rw-   0        0        0     2099 2023-07-04 08:29:27.000000 resfeci-0.0.13/src/resfeci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-04 08:29:27.000000 resfeci-0.0.13/src/resfeci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:29:27.000000 resfeci-0.0.13/src/resfeci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 08:29:27.000000 resfeci-0.0.13/src/resfeci.egg-info/top_level.txt
```

### Comparing `resfeci-0.0.12/LICENSE` & `resfeci-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `resfeci-0.0.12/PKG-INFO` & `resfeci-0.0.13/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.12
-Summary: A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
+Version: 0.0.13
+Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -18,27 +18,31 @@
 
 **IMPORTANT: Your sheet must contain a header row to function properly!**
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
 
 from resfeci import excel_split
+
 excel_split.split_sheet(split_type= 'separate_files' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT TABS OF THE SAME REPORT
 
 from resfeci import excel_split
+
 excel_split.split_sheet(split_type= 'split_tabs' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 **PARAMETER DESCRIPTIONS**
 
-split_type = must be either "separate_files" or "split_tabs";
+split_type = must be either "separate_files" or "split_tabs"
+
 input_report_path = the path to the report to be split
+
 column_number_to_split_by = the NUMBER of the Excel column to split by (A = 1, B = 2, C =3, etc.)
 
 **DEPENDENCIES**
 Openpyxl
 Pandas
 
 **KNOWN ISSUE**
```

### Comparing `resfeci-0.0.12/README.md` & `resfeci-0.0.13/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 
 **IMPORTANT: Your sheet must contain a header row to function properly!**
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
 
 from resfeci import excel_split
+
 excel_split.split_sheet(split_type= 'separate_files' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT TABS OF THE SAME REPORT
 
 from resfeci import excel_split
+
 excel_split.split_sheet(split_type= 'split_tabs' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 **PARAMETER DESCRIPTIONS**
 
-split_type = must be either "separate_files" or "split_tabs";
+split_type = must be either "separate_files" or "split_tabs"
+
 input_report_path = the path to the report to be split
+
 column_number_to_split_by = the NUMBER of the Excel column to split by (A = 1, B = 2, C =3, etc.)
 
 **DEPENDENCIES**
 Openpyxl
 Pandas
 
 **KNOWN ISSUE**
```

### Comparing `resfeci-0.0.12/pyproject.toml` & `resfeci-0.0.13/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires      = ["setuptools", "wheel", "openpyxl>=3.0.10", "pandas>=1.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resfeci"
-version = "0.0.12"
+version = "0.0.13"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
 
 
-description = "A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
+description = "Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Excel", "Split", "opensource"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `resfeci-0.0.12/src/resfeci/excel_split.py` & `resfeci-0.0.13/src/resfeci/excel_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
                     data=remove_formula_like_characters(str(i[cols+1]))
                     final_destination_ws.cell(row=row_counter, column=col_counter).value=data
                     final_destination_ws.cell(row=row_counter, column=col_counter).alignment =Alignment(horizontal='left', vertical='top', text_rotation=0, wrap_text=True, shrink_to_fit=False, indent=0)
                     col_counter=col_counter+1
 
                 row_counter=row_counter+1
 
+
+            unique_items=remove_illegal_characters(str(unique_items))
+
             final_destination_wb.save(f'text_{str(unique_items)}.xlsx')
             final_destination_wb.close()
 
     elif str(split_type).lower()=='split_tabs':
 
         final_destination_wb = Workbook()
```

### Comparing `resfeci-0.0.12/src/resfeci.egg-info/PKG-INFO` & `resfeci-0.0.13/src/resfeci.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.12
-Summary: A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
+Version: 0.0.13
+Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -18,27 +18,31 @@
 
 **IMPORTANT: Your sheet must contain a header row to function properly!**
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT REPORTS
 
 from resfeci import excel_split
+
 excel_split.split_sheet(split_type= 'separate_files' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 ## EXAMPLE OF SPLITTING AN EXCEL SHEET BY UNIQUE VALUES IN COLUMN B INTO DIFFERENT TABS OF THE SAME REPORT
 
 from resfeci import excel_split
+
 excel_split.split_sheet(split_type= 'split_tabs' , input_report_path= 'PATH_TO_REPORT.xlsx' , column_number_to_split_by=2)
 
 
 **PARAMETER DESCRIPTIONS**
 
-split_type = must be either "separate_files" or "split_tabs";
+split_type = must be either "separate_files" or "split_tabs"
+
 input_report_path = the path to the report to be split
+
 column_number_to_split_by = the NUMBER of the Excel column to split by (A = 1, B = 2, C =3, etc.)
 
 **DEPENDENCIES**
 Openpyxl
 Pandas
 
 **KNOWN ISSUE**
```

