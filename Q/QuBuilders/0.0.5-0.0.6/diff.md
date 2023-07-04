# Comparing `tmp/QuBuilders-0.0.5.tar.gz` & `tmp/qubuilders-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuBuilders-0.0.5.tar", last modified: Tue Jul  4 18:49:33 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `QuBuilders-0.0.5.tar` & `qubuilders-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:49:33.974313 QuBuilders-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-07-04 18:22:08.000000 QuBuilders-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1820 2023-07-04 18:49:33.973313 QuBuilders-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 18:49:33.950280 QuBuilders-0.0.5/QuBuilders/
--rw-rw-rw-   0        0        0       69 2023-07-04 18:48:47.000000 QuBuilders-0.0.5/QuBuilders/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-04 18:22:08.000000 QuBuilders-0.0.5/QuBuilders/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:49:33.966309 QuBuilders-0.0.5/QuBuilders.egg-info/
--rw-rw-rw-   0        0        0     1820 2023-07-04 18:49:33.000000 QuBuilders-0.0.5/QuBuilders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-07-04 18:49:33.000000 QuBuilders-0.0.5/QuBuilders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:49:33.000000 QuBuilders-0.0.5/QuBuilders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 18:49:33.000000 QuBuilders-0.0.5/QuBuilders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-04 18:49:33.000000 QuBuilders-0.0.5/QuBuilders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-07-04 18:22:08.000000 QuBuilders-0.0.5/README.md
--rw-rw-rw-   0        0        0      669 2023-07-04 18:49:11.000000 QuBuilders-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 18:49:33.974313 QuBuilders-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1811 2023-07-04 18:49:11.000000 QuBuilders-0.0.5/setup.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 qubuilders-0.0.6/setup.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/QuBu.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    27880 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/__main__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/form.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/formd.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/quseq.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/Asghar_S.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/Mode_S.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/Rostam_S.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/checker.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quloaders/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quloaders/csv_loader.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quloaders/json_loader.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/csv_writer.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/json_writer.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/type_checker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/NchTan/__init__.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/NchTan/test_NchTan_From.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/NchTan/test_NchTan_quseq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_Mode_S.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_asghar_S.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_checkers.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_rostam_s.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/test_csv_loader.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/test_json_loader.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/data_sample/exam.csv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/data_sample/eq/exam.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/test_json_writer.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/test_type_checker.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/data_sample/exam.csv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/data_sample/eq/exam.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.6/LICENSE
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 qubuilders-0.0.6/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 qubuilders-0.0.6/PKG-INFO
```

### Comparing `QuBuilders-0.0.5/LICENSE` & `qubuilders-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QuBuilders-0.0.5/PKG-INFO` & `qubuilders-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,53 @@
-Metadata-Version: 2.1
-Name: QuBuilders
-Version: 0.0.5
-Summary: a pakage that help you to make n choice questions faster
-Home-page: https://github.com/AmirrezaZahraei1387/QuBu
-Download-URL: https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz
-Author: Amirreza Zahraei
-Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
-Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
-Keywords: Question,multiple choice questions,creating questions
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# QuBu
-The qubu is an open source project that is created to help people 
-especially teachers to make n choice questions with t answers faster
-and quicly. The idea comes from the situation when you have a lot of questions that 
-they all look to have the same pattern. Like these questions.
-
-1-What is the simplified polynomial of the following polynomial?
-5*x+3+7*x+5+23
-
-2-What is the simplified polynomial of the following polynomial?
-90*x+3+7*x+5+2
-
-or 
-
-1-how to say hello word in german?
-
-2-how to say good word in german?
-
-3-how to say hello word in Farsi?
-
-...
-
-they all look the same right?
-the only different is this that some words and some numbers and
-symbols are different, however the pattern, concept and the solution
-of all of them is the same.
-
-Now this is a little project named QuBu that will help you to generate
-such questions.
-
-installation:
-
-for installing the project you can simply use pip and your cmd:
-
-pip install QuBuilders
-
-
-
-
+Metadata-Version: 2.1
+Name: QuBuilders
+Version: 0.0.6
+Summary: a pakage that help you to make n choice questions faster
+Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
+Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
+Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# QuBu
+The qubu is an open source project that is created to help people 
+especially teachers to make n choice questions with t answers faster
+and quicly. The idea comes from the situation when you have a lot of questions that 
+they all look to have the same pattern. Like these questions.
+
+1-What is the simplified polynomial of the following polynomial?
+5*x+3+7*x+5+23
+
+2-What is the simplified polynomial of the following polynomial?
+90*x+3+7*x+5+2
+
+or 
+
+1-how to say hello word in german?
+
+2-how to say good word in german?
+
+3-how to say hello word in Farsi?
+
+...
+
+they all look the same right?
+the only different is this that some words and some numbers and
+symbols are different, however the pattern, concept and the solution
+of all of them is the same.
+
+Now this is a little project named QuBu that will help you to generate
+such questions.
+
+installation:
+
+for installing the project you can simply use pip and your cmd:
+
+pip install QuBuilders
+
+
+
+
```

### Comparing `QuBuilders-0.0.5/README.md` & `qubuilders-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `QuBuilders-0.0.5/pyproject.toml` & `qubuilders-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling",'validators', 'beautifulsoup4',]
 build-backend = "hatchling.build"
 [project]
 name = "QuBuilders"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Amirrza Zahraei", email="amir.reza.zahraei@gmail.com" },
 ]
 description = "a pakage that help you to make n choice questions faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QuBuilders-0.0.5/setup.py` & `qubuilders-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 from distutils.core import setup
 setup(
   name = 'QuBuilders',         # How you named your package folder (MyLib)
   packages = ['QuBuilders'],   # Chose the same as "name"
-  version = '0.0.5',      # Start with a small number and increase it with every change you make
+  version = '0.0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'this is a python package help you to make n choice questions',   # Give a short description about your library
   author = 'Amirreza Zahraei',                   # Type in your name
   author_email = 'amir.reza.zahraei@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AmirrezaZahraei1387/QuBu',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz',    # I explain this later on
   keywords = ['Question', 'multiple choice questions', 'creating questions'],   # Keywords that define your package best
```

