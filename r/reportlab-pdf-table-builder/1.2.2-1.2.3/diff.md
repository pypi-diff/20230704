# Comparing `tmp/reportlab-pdf-table-builder-1.2.2.tar.gz` & `tmp/reportlab-pdf-table-builder-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab-pdf-table-builder-1.2.2.tar", last modified: Tue Oct 11 13:51:00 2022, max compression
+gzip compressed data, was "reportlab-pdf-table-builder-1.2.3.tar", last modified: Tue Jul  4 08:07:08 2023, max compression
```

## Comparing `reportlab-pdf-table-builder-1.2.2.tar` & `reportlab-pdf-table-builder-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-10-11 13:51:00.222661 reportlab-pdf-table-builder-1.2.2/
--rw-rw-rw-   0        0        0     1091 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       39 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3151 2022-10-11 13:51:00.221659 reportlab-pdf-table-builder-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2635 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-10-11 13:51:00.211100 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/
--rw-rw-rw-   0        0        0        0 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-11 13:51:00.213096 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__pycache__/
--rw-rw-rw-   0        0        0      204 2022-07-14 10:06:18.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     8532 2022-10-11 13:50:30.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__pycache__/builder.cpython-38.pyc
--rw-rw-rw-   0        0        0      561 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__pycache__/helpers.cpython-38.pyc
--rw-rw-rw-   0        0        0    12302 2022-10-11 13:50:27.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/builder.py
--rw-rw-rw-   0        0        0      710 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/consts.py
-drwxrwxrwx   0        0        0        0 2022-10-11 13:51:00.215091 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/fonts/
--rw-rw-rw-   0        0        0   455164 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/fonts/NotoSans-Bold.ttf
--rw-rw-rw-   0        0        0   455188 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/fonts/NotoSans-Regular.ttf
--rw-rw-rw-   0        0        0     1000 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/helpers.py
-drwxrwxrwx   0        0        0        0 2022-10-11 13:51:00.216837 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/utils/
--rw-rw-rw-   0        0        0     1388 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.2/pdf_table_builder/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2022-10-11 13:51:00.221659 reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/
--rw-rw-rw-   0        0        0     3151 2022-10-11 13:51:00.000000 reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2022-10-11 13:51:00.000000 reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-11 13:51:00.000000 reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-10-11 13:51:00.000000 reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-10-11 13:51:00.000000 reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-11 13:51:00.222661 reportlab-pdf-table-builder-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      857 2022-10-11 13:50:56.000000 reportlab-pdf-table-builder-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.101185 reportlab-pdf-table-builder-1.2.3/
+-rw-rw-rw-   0        0        0     1091 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       39 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3274 2023-07-04 08:07:08.101185 reportlab-pdf-table-builder-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2717 2023-07-04 08:02:39.000000 reportlab-pdf-table-builder-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.080257 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/
+-rw-rw-rw-   0        0        0        0 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.090157 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/
+-rw-rw-rw-   0        0        0      204 2022-07-14 10:06:18.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      225 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8532 2022-10-11 13:50:30.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-38.pyc
+-rw-rw-rw-   0        0        0     8555 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-39.pyc
+-rw-rw-rw-   0        0        0      561 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-38.pyc
+-rw-rw-rw-   0        0        0      582 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12302 2022-10-11 13:50:27.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/builder.py
+-rw-rw-rw-   0        0        0      710 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.093226 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/
+-rw-rw-rw-   0        0        0   455164 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Bold.ttf
+-rw-rw-rw-   0        0        0   455188 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Regular.ttf
+-rw-rw-rw-   0        0        0     1000 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.094759 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/utils/
+-rw-rw-rw-   0        0        0     1388 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.100188 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/
+-rw-rw-rw-   0        0        0     3274 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:07:08.101185 reportlab-pdf-table-builder-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-07-04 08:06:38.000000 reportlab-pdf-table-builder-1.2.3/setup.py
```

### Comparing `reportlab-pdf-table-builder-1.2.2/LICENSE` & `reportlab-pdf-table-builder-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/PKG-INFO` & `reportlab-pdf-table-builder-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: reportlab-pdf-table-builder
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple pdf table builder using the ReportLab Toolkit
 Home-page: https://github.com/timossavva/reportlab-pdf-table-builder
 Author: Timotheos Savva
 Author-email: timotheos.savva12@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # reportlab-pdf-table-builder
 
 A simple pdf table builder using the ReportLab Toolkit
 
 # Example usage
 
+You can run the example.py file to see the result
+```
+python example.py
+```
+
 ```python
 import datetime
 
 from reportlab.lib import colors
 from reportlab.lib.enums import TA_RIGHT, TA_CENTER, TA_LEFT
 from reportlab.platypus import Spacer
 
@@ -77,7 +84,9 @@
 
 table = pfd_table_builder(data)
 
 pdfbuilder = ReportLabPDFBuilder()
 pdfbuilder.add_to_story(table)
 pdfbuilder.save_pdf_file('a.pdf')
 ```
+
+
```

### Comparing `reportlab-pdf-table-builder-1.2.2/README.md` & `reportlab-pdf-table-builder-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # reportlab-pdf-table-builder
 
 A simple pdf table builder using the ReportLab Toolkit
 
 # Example usage
 
+You can run the example.py file to see the result
+```
+python example.py
+```
+
 ```python
 import datetime
 
 from reportlab.lib import colors
 from reportlab.lib.enums import TA_RIGHT, TA_CENTER, TA_LEFT
 from reportlab.platypus import Spacer
```

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__pycache__/builder.cpython-38.pyc` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/__pycache__/helpers.cpython-38.pyc` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/builder.py` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/builder.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/consts.py` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/consts.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/fonts/NotoSans-Bold.ttf` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/fonts/NotoSans-Regular.ttf` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/helpers.py` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/pdf_table_builder/utils/helpers.py` & `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/PKG-INFO` & `reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: reportlab-pdf-table-builder
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple pdf table builder using the ReportLab Toolkit
 Home-page: https://github.com/timossavva/reportlab-pdf-table-builder
 Author: Timotheos Savva
 Author-email: timotheos.savva12@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # reportlab-pdf-table-builder
 
 A simple pdf table builder using the ReportLab Toolkit
 
 # Example usage
 
+You can run the example.py file to see the result
+```
+python example.py
+```
+
 ```python
 import datetime
 
 from reportlab.lib import colors
 from reportlab.lib.enums import TA_RIGHT, TA_CENTER, TA_LEFT
 from reportlab.platypus import Spacer
 
@@ -77,7 +84,9 @@
 
 table = pfd_table_builder(data)
 
 pdfbuilder = ReportLabPDFBuilder()
 pdfbuilder.add_to_story(table)
 pdfbuilder.save_pdf_file('a.pdf')
 ```
+
+
```

### Comparing `reportlab-pdf-table-builder-1.2.2/reportlab_pdf_table_builder.egg-info/SOURCES.txt` & `reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 README.md
 setup.py
 pdf_table_builder/__init__.py
 pdf_table_builder/builder.py
 pdf_table_builder/consts.py
 pdf_table_builder/helpers.py
 pdf_table_builder/__pycache__/__init__.cpython-38.pyc
+pdf_table_builder/__pycache__/__init__.cpython-39.pyc
 pdf_table_builder/__pycache__/builder.cpython-38.pyc
+pdf_table_builder/__pycache__/builder.cpython-39.pyc
 pdf_table_builder/__pycache__/helpers.cpython-38.pyc
+pdf_table_builder/__pycache__/helpers.cpython-39.pyc
 pdf_table_builder/fonts/NotoSans-Bold.ttf
 pdf_table_builder/fonts/NotoSans-Regular.ttf
 pdf_table_builder/utils/helpers.py
 reportlab_pdf_table_builder.egg-info/PKG-INFO
 reportlab_pdf_table_builder.egg-info/SOURCES.txt
 reportlab_pdf_table_builder.egg-info/dependency_links.txt
 reportlab_pdf_table_builder.egg-info/requires.txt
```

### Comparing `reportlab-pdf-table-builder-1.2.2/setup.py` & `reportlab-pdf-table-builder-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reportlab-pdf-table-builder",
-    version="1.2.2",
+    version="1.2.3",
     author="Timotheos Savva",
     author_email="timotheos.savva12@gmail.com",
     description="A simple pdf table builder using the ReportLab Toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timossavva/reportlab-pdf-table-builder",
     packages=setuptools.find_packages(),
```

