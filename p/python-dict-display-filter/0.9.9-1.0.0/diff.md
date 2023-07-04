# Comparing `tmp/python-dict-display-filter-0.9.9.tar.gz` & `tmp/python-dict-display-filter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dict-display-filter-0.9.9.tar", last modified: Mon Jul  3 09:17:23 2023, max compression
+gzip compressed data, was "python-dict-display-filter-1.0.0.tar", last modified: Tue Jul  4 10:03:02 2023, max compression
```

## Comparing `python-dict-display-filter-0.9.9.tar` & `python-dict-display-filter-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/LICENSE
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4656 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4202 2023-07-03 09:14:46.000000 python-dict-display-filter-0.9.9/README.md
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/pydictdisplayfilter/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10804 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/display_filters.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/exceptions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/factories.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7661 2023-07-02 17:42:15.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/helpers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/models.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4311 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/pydictdisplayfilter/slicers.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4656 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      856 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       93 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/requires.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-03 09:17:23.000000 python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/top_level.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/setup.cfg
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1001 2023-07-02 17:35:40.000000 python-dict-display-filter-0.9.9/setup.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-03 09:17:23.863940 python-dict-display-filter-0.9.9/tests/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/tests/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10562 2023-06-30 09:43:27.000000 python-dict-display-filter-0.9.9/tests/test_dict_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/tests/test_display_filter_parser.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.9/tests/test_slicers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7550 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.9/tests/test_sql_display_filter.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/LICENSE
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4365 2023-07-03 10:05:45.000000 python-dict-display-filter-1.0.0/README.md
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/pydictdisplayfilter/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    11024 2023-07-04 09:39:48.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/display_filters.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/exceptions.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/factories.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8801 2023-07-03 21:07:45.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/helpers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/models.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4265 2023-07-03 22:31:59.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/pydictdisplayfilter/slicers.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4820 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1085 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      170 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/requires.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-04 10:03:02.000000 python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/top_level.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/setup.cfg
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1185 2023-07-04 10:01:31.000000 python-dict-display-filter-1.0.0/setup.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-04 10:03:02.053296 python-dict-display-filter-1.0.0/tests/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/tests/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1753 2023-07-03 22:36:44.000000 python-dict-display-filter-1.0.0/tests/test_csv_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    12488 2023-07-04 09:44:24.000000 python-dict-display-filter-1.0.0/tests/test_dict_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3237 2023-07-03 22:23:31.000000 python-dict-display-filter-1.0.0/tests/test_dict_display_filter_shell.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/tests/test_display_filter_parser.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1761 2023-07-03 13:37:42.000000 python-dict-display-filter-1.0.0/tests/test_json_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1762 2023-07-03 20:44:06.000000 python-dict-display-filter-1.0.0/tests/test_nmap_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-1.0.0/tests/test_slicers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7550 2023-07-02 14:04:11.000000 python-dict-display-filter-1.0.0/tests/test_sql_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3911 2023-07-03 13:44:39.000000 python-dict-display-filter-1.0.0/tests/test_sqlite_display_filter_example.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3072 2023-07-03 22:27:07.000000 python-dict-display-filter-1.0.0/tests/test_table.py
```

### Comparing `python-dict-display-filter-0.9.9/LICENSE` & `python-dict-display-filter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/PKG-INFO` & `python-dict-display-filter-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 0.9.9
+Version: 1.0.0
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 <p align="center">
     <img src="https://github.com/bytebutcher/python-dict-display-filter/raw/main/images/python_dict_display_filter_logo.png" alt="python_dict_display_filter Logo"/>
 </p>
 <h1 align="center" style="margin-top: 0px;">Python Dictionary Display Filter</h1>
 <div align="center">
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
+![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-display-filter)
+![Coverage](https://img.shields.io/codecov/c/github/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
 A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
 manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
 combining operators, membership operators, and more. 
 
 ## Table of Contents
 1. [Quick Start](#quick-start)
-2. [Usage](#usage)
-3. [Features](#features)
-4. [Examples](#examples)
-5. [Acknowledgements](#acknowledgements)
+2. [Features](#features)
+3. [Examples](#examples)
+4. [Acknowledgements](#acknowledgements)
 
 ## Quick Start
 
 Here's a simple example to get you started. First, install the package:
 
 ```commandline
 pip3 install python-dict-display-filter
@@ -92,9 +93,7 @@
 This project wouldn't be possible without these awesome projects:
 
 * <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
 * <a href="https://github.com/pyparsing/pyparsing/">pyparsing</a>: Creating PEG-parsers made easy
 * <a href="https://github.com/bytebutcher/ipranger/">ipranger</a>: Parsing and matching IPv4-addresses
 * <a href="https://pypi.org/project/python-dateutil/">python-dateutil</a>: Parsing and comparing dates 
-
-
```

#### html2text {}

```diff
@@ -1,43 +1,47 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.9 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.0.0 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
-email: thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Description-Content-Type: text/markdown License-File: LICENSE
+email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown Provides-Extra: test License-File:
+LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
+  ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-
+     display-filter) ![Coverage](https://img.shields.io/codecov/c/github/
+                    bytebutcher/python-dict-display-filter)
 
 A Wireshark-like display filter for Python dictionaries. This tool allows you
 to easily filter, analyze, and manipulate data in Python dictionaries. It
 offers a range of features including comparison operators, combining operators,
 membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
-start) 2. [Usage](#usage) 3. [Features](#features) 4. [Examples](#examples) 5.
-[Acknowledgements](#acknowledgements) ## Quick Start Here's a simple example to
-get you started. First, install the package: ```commandline pip3 install
-python-dict-display-filter ``` Then, use it to filter a list of dictionaries:
-``` from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
-["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
-["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
-["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
-"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
-"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) # This will
-filter the list to show only male actors born between 1960 and 1965 whose names
-end with 'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960
-and age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [
-{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
-``` For more details, please refer to the User_Guide. ## Features Python
-Dictionary Display Filter supports a wide range of features, including: *
-**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
-```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
-```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
-** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+start) 2. [Features](#features) 3. [Examples](#examples) 4. [Acknowledgements]
+(#acknowledgements) ## Quick Start Here's a simple example to get you started.
+First, install the package: ```commandline pip3 install python-dict-display-
+filter ``` Then, use it to filter a list of dictionaries: ``` from
+pydictdisplayfilter import DictDisplayFilter actors = [ {"name": ["Laurence",
+"Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name": ["Keanu",
+"Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight",
+"bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"},
+"gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"},
+"gender": "female"} ] ddf = DictDisplayFilter(actors) # This will filter the
+list to show only male actors born between 1960 and 1965 whose names end with
+'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960 and
+age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [{'name':
+['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For
+more details, please refer to the User_Guide. ## Features Python Dictionary
+Display Filter supports a wide range of features, including: * **Comparison
+Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```,
+```~=```, ```~```, ```&``` * **Combining Operators:** ```and```, ```or```,
+```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:**
+```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
 **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
 detailed description of the individual features check out the User_Guide. ##
 Examples For detailed examples of how the display filter can be utilized,
 please refer to the following: * [CSV Display Filter](https://github.com/
 bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
```

### Comparing `python-dict-display-filter-0.9.9/README.md` & `python-dict-display-filter-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 </p>
 <h1 align="center" style="margin-top: 0px;">Python Dictionary Display Filter</h1>
 <div align="center">
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
+![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-display-filter)
+![Coverage](https://img.shields.io/codecov/c/github/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
 A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
 manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
 combining operators, membership operators, and more. 
 
 ## Table of Contents
 1. [Quick Start](#quick-start)
-2. [Usage](#usage)
-3. [Features](#features)
-4. [Examples](#examples)
-5. [Acknowledgements](#acknowledgements)
+2. [Features](#features)
+3. [Examples](#examples)
+4. [Acknowledgements](#acknowledgements)
 
 ## Quick Start
 
 Here's a simple example to get you started. First, install the package:
 
 ```commandline
 pip3 install python-dict-display-filter
```

#### html2text {}

```diff
@@ -1,37 +1,40 @@
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
+  ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-
+     display-filter) ![Coverage](https://img.shields.io/codecov/c/github/
+                    bytebutcher/python-dict-display-filter)
 
 A Wireshark-like display filter for Python dictionaries. This tool allows you
 to easily filter, analyze, and manipulate data in Python dictionaries. It
 offers a range of features including comparison operators, combining operators,
 membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
-start) 2. [Usage](#usage) 3. [Features](#features) 4. [Examples](#examples) 5.
-[Acknowledgements](#acknowledgements) ## Quick Start Here's a simple example to
-get you started. First, install the package: ```commandline pip3 install
-python-dict-display-filter ``` Then, use it to filter a list of dictionaries:
-``` from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
-["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
-["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
-["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
-"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
-"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) # This will
-filter the list to show only male actors born between 1960 and 1965 whose names
-end with 'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960
-and age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [
-{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
-``` For more details, please refer to the User_Guide. ## Features Python
-Dictionary Display Filter supports a wide range of features, including: *
-**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
-```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
-```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
-** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+start) 2. [Features](#features) 3. [Examples](#examples) 4. [Acknowledgements]
+(#acknowledgements) ## Quick Start Here's a simple example to get you started.
+First, install the package: ```commandline pip3 install python-dict-display-
+filter ``` Then, use it to filter a list of dictionaries: ``` from
+pydictdisplayfilter import DictDisplayFilter actors = [ {"name": ["Laurence",
+"Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name": ["Keanu",
+"Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight",
+"bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"},
+"gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"},
+"gender": "female"} ] ddf = DictDisplayFilter(actors) # This will filter the
+list to show only male actors born between 1960 and 1965 whose names end with
+'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960 and
+age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [{'name':
+['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For
+more details, please refer to the User_Guide. ## Features Python Dictionary
+Display Filter supports a wide range of features, including: * **Comparison
+Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```,
+```~=```, ```~```, ```&``` * **Combining Operators:** ```and```, ```or```,
+```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:**
+```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
 **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
 detailed description of the individual features check out the User_Guide. ##
 Examples For detailed examples of how the display filter can be utilized,
 please refer to the following: * [CSV Display Filter](https://github.com/
 bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
```

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/__init__.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/display_filters.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/display_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,23 @@
                             there are no restrictions regarding specifying field names.
         :param functions: A dictionary of functions whereby the key specifies the name. If no functions are supplied
                           "len", "lower" and "upper" are used as default ones.
         :param slicers: A list of slicers. If no slicers are supplied the BasicSlicer is used per default.
         :param evaluator: The evaluator used to evaluate the expressions. If no evaluator is specified the
                           DefaultEvaluator is used.
         """
-        functions = functions if functions else {
+        self._slicer_factory = SlicerFactory(slicers)
+        self._evaluator = evaluator if evaluator else DefaultEvaluator()
+        self._functions = functions if functions is not None else {
             "len": lambda value: len(value),
             "lower": lambda value: value.lower(),
             "upper": lambda value: value.upper()
         }
-        self._slicer_factory = SlicerFactory(slicers)
-        self._evaluator = evaluator if evaluator else DefaultEvaluator()
-        self._functions = functions
-        self._field_names = field_names
-        self._display_filter_parser = DisplayFilterParser(field_names, functions)
+        self._field_names = field_names if field_names is not None else []
+        self._display_filter_parser = DisplayFilterParser(field_names=self._field_names, functions=self._functions)
 
     def _get_item_value(self, expression, item) -> str:
         """
         Returns the value found at the specified key in the item. Key can be dot-notated for retrieving values
         inside nested dicts. Returns a transformed value if a function is specified.
         """
         keys = expression.field.split('.')
@@ -99,24 +98,24 @@
     @property
     def field_names(self) -> List[str]:
         return self._field_names
 
     @field_names.setter
     def field_names(self, field_names: List[str] = None):
         self._field_names = field_names
-        self._display_filter_parser = DisplayFilterParser(self._field_names, self._functions)
+        self._display_filter_parser = DisplayFilterParser(field_names=self._field_names, functions=self._functions)
 
     @property
     def functions(self) -> Dict[str, Callable]:
         return self._functions
 
     @functions.setter
     def functions(self, functions: Dict[str, Callable]):
         self._functions = functions
-        self._display_filter_parser = DisplayFilterParser(self._field_names, self._functions)
+        self._display_filter_parser = DisplayFilterParser(field_names=self._field_names, functions=self._functions)
 
     @abstractmethod
     def filter(self, display_filter: str):
         raise NotImplementedError()
 
 
 class DictDisplayFilter(BaseDisplayFilter):
@@ -128,15 +127,15 @@
                  functions: Dict[str, Callable] = None,
                  slicers: List[BasicSlicer] = None,
                  evaluator: Evaluator = None):
         """
         Initializes the DictDisplayFilter.
         :param data: A list of dictionaries to filter on.
         """
-        super().__init__(field_names, functions, slicers, evaluator)
+        super().__init__(field_names=field_names, functions=functions, slicers=slicers, evaluator=evaluator)
         self._data = data
 
     def filter(self, display_filter: str):
         """ Filters the data using the display filter. """
         expressions = self._display_filter_parser.parse(display_filter)
         yield from self._filter_data(self._data, expressions)
 
@@ -150,17 +149,17 @@
                  functions: Dict[str, Callable] = None,
                  slicers: List[BasicSlicer] = None,
                  evaluator: Evaluator = None):
         """
         Initializes the ListDisplayFilter.
         :param data: A list of lists to filter on.
         """
-        super().__init__([
+        super().__init__(data=[
             dict(zip(field_names, item)) for item in data
-        ], field_names, functions, slicers, evaluator)
+        ], field_names=field_names, functions=functions, slicers=slicers, evaluator=evaluator)
 
     def filter(self, display_filter: str):
         """ Filters the data using the display filter. """
         for item in super().filter(display_filter):
             # Return each item as a list of values instead of a dictionary of key values.
             yield item.items()
 
@@ -186,15 +185,15 @@
         :param connection:
         :param table_name: The name of the database table where the display filter will be applied.
         :param column_names: A list of column names which are allowed in the display filter. If no column names are
                              given there are no restrictions regarding specifying column names.
         """
         self._connection = connection
         self.table_name = table_name
-        super().__init__(column_names, functions, slicers, evaluator)
+        super().__init__(field_names=column_names, functions=functions, slicers=slicers, evaluator=evaluator)
 
     def _validate_table_name(self, table_name: str) -> bool:
         """ Checks whether the table name contains invalid characters or keywords"""
         pattern = re.compile("^[a-zA-Z_][a-zA-Z0-9_]*$")
         if pattern.match(table_name) and not self._is_sql_keyword(table_name):
             return True
         else:
```

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/__init__.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/evaluators/common.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/evaluators/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/exceptions.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/factories.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/factories.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/helpers.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,50 +15,65 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import cmd
 import logging
 import os
 import time
 import traceback
-from typing import List
+from collections import OrderedDict
+from itertools import chain
+from typing import List, Dict, Callable
 
 from pydictdisplayfilter.display_filters import BaseDisplayFilter, DictDisplayFilter
+from pydictdisplayfilter.evaluators import Evaluator
 from pydictdisplayfilter.exceptions import ParserError, EvaluationError
+from pydictdisplayfilter.slicers import BasicSlicer
 
 
 class TableError(Exception):
     pass
 
 
+class TableColumnSizeCalculator:
+
+    @staticmethod
+    def calculate(data_store: List[dict], fields: List) -> List[int]:
+        """ Calculates and returns the necessary size of each column in the data store. """
+        field_sizes = OrderedDict()
+        for field in fields:
+            field_sizes[field] = len(field)
+        for item in data_store:
+            for key in field_sizes.keys():
+                if key in item:
+                    field_sizes[key] = max(len(str(item[key])), field_sizes[key])
+        return list(field_sizes.values())
+
+
 class Table:
     """ Data store with filter capabilities and pretty table printout. """
 
     def __init__(self, display_filter: BaseDisplayFilter):
         self._display_filter = display_filter
 
     def _make_table(self, data_store: List[dict]) -> List[str]:
         """ Creates a table including header from the data store. """
         if not data_store:
             return []
-        table = [self.fields()]
-        column_size = self._calculate_column_size(data_store)
+        fields = self.fields()
+        table = [fields]
+        column_size = self._calculate_column_size(data_store, fields)
         format_str = ' | '.join(["{{:<{}}}".format(i) for i in column_size])
         for item in data_store:
-            table.append(item.values())
-        column_size = self._calculate_column_size(data_store)
+            table.append([str(item[field]) if field in item else '' for field in fields])
         table.insert(1, ['-' * i for i in column_size]) # Separating line
         return [""] + [ format_str.format(*item) for item in table ]
 
-    def _calculate_column_size(self, data_store: List[dict]) -> List[int]:
+    def _calculate_column_size(self, data_store: List[dict], fields: List) -> List[int]:
         """ Calculates and returns the necessary size of each column in the data store. """
-        header = list(data_store[0].keys())
-        items = [list(item.values()) for item in data_store]
-        return [
-            max(len(str(item)) for item in column) for column in zip(*items + [header])
-        ]
+        return TableColumnSizeCalculator.calculate(data_store, fields)
 
     def _make_footer(self, items: List[dict], duration: float) -> List[str]:
         """ Creates a footer for the table which prints some statistics. """
         item_count = len(items)
         result = [""]
         if item_count == 0:
             result.append("Empty set ({:.2f} secs)".format(duration))
@@ -66,15 +81,15 @@
             type_name = "row" if item_count == 1 else "rows"
             result.append("{} {} in set ({:.2f} secs)".format(item_count, type_name, duration))
         result.append("")
         return result
 
     def fields(self) -> List[str]:
         """ Returns the field names used in the data store. """
-        raise NotImplementedError()
+        return self._display_filter.field_names
 
     def filter(self, display_filter: str) -> str:
         """
         Filters the items in the data store using the specified display filter and returns the result in a table.
         """
         start = time.time()
         result = list(self._display_filter.filter(display_filter))
@@ -173,26 +188,33 @@
         """ Exit application. """
         return True
 
 
 class DictTable(Table):
     """ Data store with filter capabilities and pretty table printout. """
 
-    def __init__(self, data_store: List[dict]):
+    def __init__(self,
+                 data_store: List[dict],
+                 field_names: List[str] = None,
+                 functions: Dict[str, Callable] = None,
+                 slicers: List[BasicSlicer] = None,
+                 evaluator: Evaluator = None):
         """ Initializes the DictTable with a data store. """
-        self._data_store = data_store
-        super().__init__(DictDisplayFilter(data_store))
+        field_names = field_names or self._extract_field_names(data_store)
+        super().__init__(DictDisplayFilter(data_store, field_names, functions, slicers, evaluator))
 
-    def fields(self) -> List[str]:
-        """ Returns the field names used in the data store. """
-        if not self._data_store:
-            # No items in data store, so there are no fields to query either.
-            return list()
-        return list(self._data_store[0].keys())
+    def _extract_field_names(self, data_store: List[dict]) -> List[str]:
+        """ Extracts the field names from the given data store. """
+        return sorted(set(chain.from_iterable(row.keys() for row in data_store)))
 
 
 class DictDisplayFilterShell(DisplayFilterShell):
     """ A little shell for querying a list of dictionaries using the display filter. """
 
-    def __init__(self, data_store: List[dict]):
+    def __init__(self,
+                 data_store: List[dict],
+                 field_names: List[str] = None,
+                 functions: Dict[str, Callable] = None,
+                 slicers: List[BasicSlicer] = None,
+                 evaluator: Evaluator = None):
         """ Initializes the DictDisplayFilterShell with a data store. """
-        super().__init__(DictTable(data_store))
+        super().__init__(DictTable(data_store, field_names, functions, slicers, evaluator))
```

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/models.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/models.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/__init__.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/common.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,18 +37,14 @@
 
 def _signed_float():
     return pp.Combine(pp.Optional('-') + pp.Word(pp.nums) + pp.Optional('.' + pp.Word(pp.nums))).setParseAction(
         lambda tokens: list(map(float, tokens.as_list()))
     )
 
 
-def _number():
-    return pp.common.integer
-
-
 def _string_list():
     return pp.delimitedList(
         _quoted_string()
     ).addParseAction(lambda tokens: [tokens.asList()])
 
 
 def _number_list():
```

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/parsers/display_filter.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/parsers/display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/pydictdisplayfilter/slicers.py` & `python-dict-display-filter-1.0.0/pydictdisplayfilter/slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/PKG-INFO` & `python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 0.9.9
+Version: 1.0.0
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 <p align="center">
     <img src="https://github.com/bytebutcher/python-dict-display-filter/raw/main/images/python_dict_display_filter_logo.png" alt="python_dict_display_filter Logo"/>
 </p>
 <h1 align="center" style="margin-top: 0px;">Python Dictionary Display Filter</h1>
 <div align="center">
 
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
 ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter)
 ![GitHub](https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
+![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-display-filter)
+![Coverage](https://img.shields.io/codecov/c/github/bytebutcher/python-dict-display-filter)
 </div>
 <br>
 
 A Wireshark-like display filter for Python dictionaries. This tool allows you to easily filter, analyze, and 
 manipulate data in Python dictionaries. It offers a range of features including comparison operators, 
 combining operators, membership operators, and more. 
 
 ## Table of Contents
 1. [Quick Start](#quick-start)
-2. [Usage](#usage)
-3. [Features](#features)
-4. [Examples](#examples)
-5. [Acknowledgements](#acknowledgements)
+2. [Features](#features)
+3. [Examples](#examples)
+4. [Acknowledgements](#acknowledgements)
 
 ## Quick Start
 
 Here's a simple example to get you started. First, install the package:
 
 ```commandline
 pip3 install python-dict-display-filter
@@ -92,9 +93,7 @@
 This project wouldn't be possible without these awesome projects:
 
 * <a href="https://wiki.wireshark.org/DisplayFilters">wireshark display filter</a>: Display filter for filtering network packages
 * <a href="https://github.com/wolever/parameterized">parameterized</a>: Parameterized testing with any Python test framework
 * <a href="https://github.com/pyparsing/pyparsing/">pyparsing</a>: Creating PEG-parsers made easy
 * <a href="https://github.com/bytebutcher/ipranger/">ipranger</a>: Parsing and matching IPv4-addresses
 * <a href="https://pypi.org/project/python-dateutil/">python-dateutil</a>: Parsing and comparing dates 
-
-
```

#### html2text {}

```diff
@@ -1,43 +1,47 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.9 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 1.0.0 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
-email: thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Description-Content-Type: text/markdown License-File: LICENSE
+email: thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown Provides-Extra: test License-File:
+LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
 ![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
   ![PyPI](https://img.shields.io/pypi/v/python-dict-display-filter) ![GitHub]
 (https://img.shields.io/github/license/bytebutcher/python-dict-display-filter)
+  ![Build Status](https://img.shields.io/travis/com/bytebutcher/python-dict-
+     display-filter) ![Coverage](https://img.shields.io/codecov/c/github/
+                    bytebutcher/python-dict-display-filter)
 
 A Wireshark-like display filter for Python dictionaries. This tool allows you
 to easily filter, analyze, and manipulate data in Python dictionaries. It
 offers a range of features including comparison operators, combining operators,
 membership operators, and more. ## Table of Contents 1. [Quick Start](#quick-
-start) 2. [Usage](#usage) 3. [Features](#features) 4. [Examples](#examples) 5.
-[Acknowledgements](#acknowledgements) ## Quick Start Here's a simple example to
-get you started. First, install the package: ```commandline pip3 install
-python-dict-display-filter ``` Then, use it to filter a list of dictionaries:
-``` from pydictdisplayfilter import DictDisplayFilter actors = [ {"name":
-["Laurence", "Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name":
-["Keanu", "Reeves"], "age": {"born": "1964"}, "gender": "male", "power":
-["flight", "bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born":
-"1951"}, "gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born":
-"1967"}, "gender": "female"} ] ddf = DictDisplayFilter(actors) # This will
-filter the list to show only male actors born between 1960 and 1965 whose names
-end with 'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960
-and age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [
-{'name': ['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}]
-``` For more details, please refer to the User_Guide. ## Features Python
-Dictionary Display Filter supports a wide range of features, including: *
-**Comparison Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```,
-```>```, ```~=```, ```~```, ```&``` * **Combining Operators:** ```and```,
-```or```, ```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:
-** ```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
+start) 2. [Features](#features) 3. [Examples](#examples) 4. [Acknowledgements]
+(#acknowledgements) ## Quick Start Here's a simple example to get you started.
+First, install the package: ```commandline pip3 install python-dict-display-
+filter ``` Then, use it to filter a list of dictionaries: ``` from
+pydictdisplayfilter import DictDisplayFilter actors = [ {"name": ["Laurence",
+"Fishburne"], "age": {"born": "1961"}, "gender": "male"}, {"name": ["Keanu",
+"Reeves"], "age": {"born": "1964"}, "gender": "male", "power": ["flight",
+"bullet-time"]}, {"name": ["Joe", "Pantoliano"], "age": {"born": "1951"},
+"gender": "male"}, {"name": ["Carrie-Anne", "Moss"], "age": {"born": "1967"},
+"gender": "female"} ] ddf = DictDisplayFilter(actors) # This will filter the
+list to show only male actors born between 1960 and 1965 whose names end with
+'e' filtered_actors = ddf.filter("gender == male and (age.born > 1960 and
+age.born < 1965) and name matches .*e$") print(list(filtered_actors)) [{'name':
+['Laurence', 'Fishburne'], 'age': {'born': '1961'}, 'gender': 'male'}] ``` For
+more details, please refer to the User_Guide. ## Features Python Dictionary
+Display Filter supports a wide range of features, including: * **Comparison
+Operators:** ```==```, ```!=```, ```<=```, ```<```, ```>=```, ```>```,
+```~=```, ```~```, ```&``` * **Combining Operators:** ```and```, ```or```,
+```xor```, ```not``` * **Membership Operators:** ```in``` * **Types:**
+```Text```, ```Number```, ```Date & Time```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Slicing:** ```Text```, ```Ethernet-```, ```IPv4-```,
 ```IPv6-Address``` * **Functions:** ```upper```, ```lower```, ```len``` *
 **Data Sources**: ```CSV```, ```Dictionaries```, ```JSON```, ```SQLite``` For a
 detailed description of the individual features check out the User_Guide. ##
 Examples For detailed examples of how the display filter can be utilized,
 please refer to the following: * [CSV Display Filter](https://github.com/
 bytebutcher/python-dict-display-filter/blob/main/docs/EXAMPLES.md#csv-display-
```

### Comparing `python-dict-display-filter-0.9.9/python_dict_display_filter.egg-info/SOURCES.txt` & `python-dict-display-filter-1.0.0/python_dict_display_filter.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,11 +15,17 @@
 pydictdisplayfilter/parsers/display_filter.py
 python_dict_display_filter.egg-info/PKG-INFO
 python_dict_display_filter.egg-info/SOURCES.txt
 python_dict_display_filter.egg-info/dependency_links.txt
 python_dict_display_filter.egg-info/requires.txt
 python_dict_display_filter.egg-info/top_level.txt
 tests/__init__.py
+tests/test_csv_display_filter_example.py
 tests/test_dict_display_filter.py
+tests/test_dict_display_filter_shell.py
 tests/test_display_filter_parser.py
+tests/test_json_display_filter_example.py
+tests/test_nmap_display_filter_example.py
 tests/test_slicers.py
-tests/test_sql_display_filter.py
+tests/test_sql_display_filter.py
+tests/test_sqlite_display_filter_example.py
+tests/test_table.py
```

### Comparing `python-dict-display-filter-0.9.9/setup.py` & `python-dict-display-filter-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="python-dict-display-filter",
-    version="0.9.9",
+    version="1.0.0",
     description="A Wireshark-like display filter for dictionaries.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bytebutcher/python-dict-display-filter",
     author="bytebutcher",
     author_email="thomas.engel.web@gmail.com",
     license="GPL-3.0",
@@ -27,9 +27,17 @@
     install_requires=[
         'packaging==23.1',
         'parameterized==0.8.1',
         'pyparsing==3.0.6',
         'ipranger==1.1.2',
         'python-dateutil==2.8.2'
     ],
+    extras_require={
+        'test': [
+            'pytest==7.3.1',
+            'pytest-cov==4.0.0',
+            'pexpect==4.8.0',
+            'python-libnmap==0.7.0'
+        ]
+    },
     include_package_data=True,
 )
```

### Comparing `python-dict-display-filter-0.9.9/tests/__init__.py` & `python-dict-display-filter-1.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/tests/test_dict_display_filter.py` & `python-dict-display-filter-1.0.0/tests/test_dict_display_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from parameterized import parameterized
 
 from pydictdisplayfilter.display_filters import DictDisplayFilter
+from pydictdisplayfilter.exceptions import ParserError
 
 
 class TestDictDisplayFilter(unittest.TestCase):
     # List of dictionaries representing the data to filter on.
     data = [
         {"name": "Morpheus", "age": 38, "gender": "male", "killed": False},
         {"name": "Neo", "age": 35, "gender": "male", "killed": False, "power": ["flight", "bullet-time"]},
@@ -261,11 +262,59 @@
         ['value <= 00:83:00:20:20:83', 0],
         ['value >= 00:83:00:20:20:83', 0],
         ['value < 00:83:00:20:20:83', 0],
         ['value > 00:83:00:20:20:83', 0],
     ])
     def test_mixed_data_display_filter_returns_correct_number_of_items(self, display_filter, no_items):
         items = list(DictDisplayFilter(self.mixed_data).filter(display_filter))
-        if len(items) != no_items:
-            list_difference = [item for item in self.mixed_data if item not in items]
-            print(list_difference)
         self.assertEqual(len(items), no_items)
+
+    @parameterized.expand([
+        # Fields
+        ["lower(value) == foobar", 2],
+        ["upper(value) == FOOBAR", 2],
+        ["upper(value) ~= FOO", 3],
+        ["lower(value) ~= foo", 3],
+        ["len(value) == 6", 2],
+        ["len(value) == 3", 2],
+    ])
+    def test_functions_default(self, display_filter, no_items):
+        data = [{'value': 'foobar'}, {'value': 'FOOBAR'}, {'value': 'FOO'}, {'value': 'BAR'}]
+        items = list(DictDisplayFilter(data).filter(display_filter))
+        self.assertEqual(len(items), no_items)
+
+    @parameterized.expand([
+        # Fields
+        ["ltrim(value) == foobar"],
+        ["rtrim(value) == foobar"],
+        ["trim(value) == foobar"],
+    ])
+    def test_functions_undefined_raises_parser_error(self, display_filter):
+        data = [{'value': 'foobar'}, {'value': 'FOOBAR'}, {'value': 'FOO'}, {'value': 'BAR'}]
+        self.assertRaises(ParserError, lambda: list(DictDisplayFilter(data).filter(display_filter)))
+
+    @parameterized.expand([
+        # Fields
+        ["value == foobar", 0],
+        ["ltrim(value) == foobar", 1],
+        ["rtrim(value) == foobar", 1],
+        ["trim(value) == foobar", 3]
+    ])
+    def test_functions_custom(self, display_filter, no_items):
+        data = [{'value': ' foobar'}, {'value': ' foobar '}, {'value': 'foobar '}]
+        functions = {
+            'ltrim': lambda v: v.lstrip(),
+            'rtrim': lambda v: v.rstrip(),
+            'trim': lambda v: v.strip()
+        }
+        items = list(DictDisplayFilter(data, functions=functions).filter(display_filter))
+        self.assertEqual(len(items), no_items)
+
+    @parameterized.expand([
+        # Fields
+        ["lower(value) == foobar"],
+        ["upper(value) == FOOBAR"],
+        ["len(value) == 6"],
+    ])
+    def test_functions_none(self, display_filter):
+        data = [{'value': 'foobar'}, {'value': 'FOOBAR'}, {'value': 'FOO'}, {'value': 'BAR'}]
+        self.assertRaises(ParserError, lambda: list(DictDisplayFilter(data, functions={}).filter(display_filter)))
```

### Comparing `python-dict-display-filter-0.9.9/tests/test_display_filter_parser.py` & `python-dict-display-filter-1.0.0/tests/test_display_filter_parser.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/tests/test_slicers.py` & `python-dict-display-filter-1.0.0/tests/test_slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.9/tests/test_sql_display_filter.py` & `python-dict-display-filter-1.0.0/tests/test_sql_display_filter.py`

 * *Files identical despite different names*

