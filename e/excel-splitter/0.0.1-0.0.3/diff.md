# Comparing `tmp/excel_splitter-0.0.1.tar.gz` & `tmp/excel_splitter-0.0.3.tar.gz`

## Comparing `excel_splitter-0.0.1.tar` & `excel_splitter-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_splitter-0.0.1/src/Split_Excel_Package/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 excel_splitter-0.0.1/src/Split_Excel_Package/excel_splitter.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 excel_splitter-0.0.1/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 excel_splitter-0.0.1/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 excel_splitter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 excel_splitter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/src/Split_Excel_Package/__init__.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/src/Split_Excel_Package/excel_splitter.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/LICENSE
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 excel_splitter-0.0.3/PKG-INFO
```

### Comparing `excel_splitter-0.0.1/src/Split_Excel_Package/excel_splitter.py` & `excel_splitter-0.0.3/src/Split_Excel_Package/excel_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         # Currently this doesnt do formulas, this remove the = sign from the beginning so as not to cause errors when opening new file.
 
         if string[0]=='=':
             string=string[1:]
         
         return string 
 
-def split_report_test(split_type, input_report_path, column_number_to_split_by):
+def split_sheet(split_type, input_report_path, column_number_to_split_by):
     
     df = pd.read_excel(input_report_path)
     selected_col_values=df.iloc[:,int(column_number_to_split_by)-1].unique()
 
-    if str(split_type)=='Separate_Files':
+    if str(split_type).lower()=='separate_files':
 
         for unique_items in selected_col_values:
 
             final_destination_wb = Workbook()
             final_destination_ws = final_destination_wb['Sheet']
 
             row_counter=2
@@ -65,15 +65,15 @@
                     col_counter=col_counter+1
 
                 row_counter=row_counter+1
 
             final_destination_wb.save(f'text_{str(unique_items)}.xlsx')
             final_destination_wb.close()
 
-    elif str(split_type)=='Split_Tabs':
+    elif str(split_type).lower()=='split_tabs':
 
         final_destination_wb = Workbook()
             
         for unique_items in selected_col_values:
 
             if unique_items not in df.columns:
```

### Comparing `excel_splitter-0.0.1/LICENSE` & `excel_splitter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_splitter-0.0.1/pyproject.toml` & `excel_splitter-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "openpyxl>=3.0.10"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excel_splitter"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
-description = "A Tool to Quickly Split an Excel Sheet into Multiple Sheets or Separate Files"
+description = "A packge to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = [
-  "openpyxl>=3.0.10"
-]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+
+
 [project.urls]
 "Homepage" = "https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter"
```

