# Comparing `tmp/qubuilders-0.0.2.tar.gz` & `tmp/QuBuilders-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "QuBuilders-0.0.3.tar", last modified: Tue Jul  4 18:28:22 2023, max compression
```

## Comparing `qubuilders-0.0.2.tar` & `QuBuilders-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,16 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 qubuilders-0.0.2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.2/__main__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 qubuilders-0.0.2/setup.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/QuBu.iml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0    32131 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/form.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/formd.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/quseq.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/Asghar_S.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/Mode_S.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/Rostam_S.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/checker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quloaders/__init__.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quloaders/csv_loader.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quloaders/json_loader.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/csv_writer.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/json_writer.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/type_checker.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/NchTan/test_NchTan_From.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/NchTan/test_NchTan_quseq.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_Mode_S.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_asghar_S.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_checkers.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_rostam_s.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/test_csv_loader.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/test_json_loader.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/data_sample/exam.csv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/data_sample/eq/exa.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/data_sample/eq/exam.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/test_json_writer.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/test_type_checker.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/data_sample/exam.csv
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/data_sample/eq/exa.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/data_sample/eq/exam.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.2/LICENSE
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 qubuilders-0.0.2/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 qubuilders-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:22.868782 QuBuilders-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1820 2023-07-04 18:28:22.867782 QuBuilders-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:22.848255 QuBuilders-0.0.3/QuBuilders/
+-rw-rw-rw-   0        0        0        0 2023-07-04 18:27:26.000000 QuBuilders-0.0.3/QuBuilders/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/QuBuilders/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:22.865134 QuBuilders-0.0.3/QuBuilders.egg-info/
+-rw-rw-rw-   0        0        0     1820 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-04 18:28:22.000000 QuBuilders-0.0.3/QuBuilders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/README.md
+-rw-rw-rw-   0        0        0      669 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 18:28:22.868782 QuBuilders-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1807 2023-07-04 18:22:08.000000 QuBuilders-0.0.3/setup.py
```

### Comparing `qubuilders-0.0.2/setup.py` & `QuBuilders-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'QuBuilders',         # How you named your package folder (MyLib)
   packages = ['QuBuilders'],   # Chose the same as "name"
-  version = '0.0.2',      # Start with a small number and increase it with every change you make
+  version = '0.0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'this is a python package help you to make n choice questions',   # Give a short description about your library
   author = 'Amirreza Zahraei',                   # Type in your name
   author_email = 'amir.reza.zahraei@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AmirrezaZahraei1387/QuBu',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz',    # I explain this later on
   keywords = ['Question', 'multiple choice questions', 'creating questions'],   # Keywords that define your package best
```

### Comparing `qubuilders-0.0.2/LICENSE` & `QuBuilders-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.2/README.md` & `QuBuilders-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,10 +24,16 @@
 the only different is this that some words and some numbers and
 symbols are different, however the pattern, concept and the solution
 of all of them is the same.
 
 Now this is a little project named QuBu that will help you to generate
 such questions.
 
+installation:
+
+for installing the project you can simply use pip and your cmd:
+
+pip install QuBuilders
+
```

### Comparing `qubuilders-0.0.2/pyproject.toml` & `QuBuilders-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling",'validators', 'beautifulsoup4',]
 build-backend = "hatchling.build"
 [project]
 name = "QuBuilders"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Amirrza Zahraei", email="amir.reza.zahraei@gmail.com" },
 ]
 description = "a pakage that help you to make n choice questions faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qubuilders-0.0.2/PKG-INFO` & `QuBuilders-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-Metadata-Version: 2.1
-Name: QuBuilders
-Version: 0.0.2
-Summary: a pakage that help you to make n choice questions faster
-Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
-Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
-Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
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
-
-
-
+Metadata-Version: 2.1
+Name: QuBuilders
+Version: 0.0.3
+Summary: a pakage that help you to make n choice questions faster
+Home-page: https://github.com/AmirrezaZahraei1387/QuBu
+Download-URL: https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz
+Author: Amirreza Zahraei
+Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
+Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
+Keywords: Question,multiple choice questions,creating questions
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
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

