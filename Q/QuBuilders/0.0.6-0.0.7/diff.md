# Comparing `tmp/qubuilders-0.0.6.tar.gz` & `tmp/qubuilders-0.0.7.tar.gz`

## Comparing `qubuilders-0.0.6.tar` & `qubuilders-0.0.7.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 qubuilders-0.0.6/setup.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/QuBu.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0    27880 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/__main__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/form.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/formd.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/NchTan/quseq.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/Asghar_S.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/Mode_S.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/Rostam_S.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/generators/stament/checker.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quloaders/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quloaders/csv_loader.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quloaders/json_loader.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/csv_writer.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/json_writer.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qubuilders-0.0.6/QuBuilders/quwriter/type_checker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/NchTan/__init__.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/NchTan/test_NchTan_From.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/NchTan/test_NchTan_quseq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_Mode_S.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_asghar_S.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_checkers.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/generators/test_rostam_s.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/test_csv_loader.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/test_json_loader.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/data_sample/exam.csv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/data_sample/eq/exa.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quloaders/data_sample/eq/exam.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/test_json_writer.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/test_type_checker.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/data_sample/exam.csv
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/data_sample/eq/exa.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.6/tests/quwriter/data_sample/eq/exam.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.6/LICENSE
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 qubuilders-0.0.6/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 qubuilders-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 qubuilders-0.0.7/setup.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/QuBu.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0    32329 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/__main__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/form.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/formd.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/quseq.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/Asghar_S.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/Mode_S.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/Rostam_S.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/checker.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quloaders/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quloaders/csv_loader.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quloaders/json_loader.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/csv_writer.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/json_writer.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/type_checker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/NchTan/__init__.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_From.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_quseq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_Mode_S.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_asghar_S.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_checkers.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_rostam_s.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/test_csv_loader.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/test_json_loader.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/data_sample/exam.csv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/data_sample/eq/exam.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/test_json_writer.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/test_type_checker.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/data_sample/exam.csv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/data_sample/eq/exam.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 qubuilders-0.0.7/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 qubuilders-0.0.7/PKG-INFO
```

### Comparing `qubuilders-0.0.6/setup.py` & `qubuilders-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 
 from distutils.core import setup
 setup(
   name = 'QuBuilders',         # How you named your package folder (MyLib)
   packages = ['QuBuilders'],   # Chose the same as "name"
-  version = '0.0.6',      # Start with a small number and increase it with every change you make
+  version = '0.0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'this is a python package help you to make n choice questions',   # Give a short description about your library
   author = 'Amirreza Zahraei',                   # Type in your name
   author_email = 'amir.reza.zahraei@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AmirrezaZahraei1387/QuBu',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubuilders-0.0.7.tar.gz',    # I explain this later on
   keywords = ['Question', 'multiple choice questions', 'creating questions'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
           'hatchling',
       ],
   classifiers=[
```

### Comparing `qubuilders-0.0.6/.idea/QuBu.iml` & `qubuilders-0.0.7/.idea/QuBu.iml`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/.idea/workspace.xml` & `qubuilders-0.0.7/.idea/workspace.xml`

 * *Files 19% similar despite different names*

#### Comparing `qubuilders-0.0.6/.idea/workspace.xml` & `qubuilders-0.0.7/.idea/workspace.xml`

```diff
@@ -1,15 +1,37 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="0643fa01-c989-4e6e-8770-b93352bd1ffb" name="Changes" comment="the version 0.0.6">
-      <change beforePath="$PROJECT_DIR$/setup.py" beforeDir="false" afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/.idea/workspace.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/workspace.xml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/NchTan/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/NchTan/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/NchTan/test_NchTan_From.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/NchTan/test_NchTan_From.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/NchTan/test_NchTan_quseq.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/NchTan/test_NchTan_quseq.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/generators/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/generators/test_Mode_S.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_Mode_S.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/generators/test_asghar_S.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_asghar_S.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/generators/test_checkers.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_checkers.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/generators/test_rostam_s.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_rostam_s.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quloaders/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quloaders/data_sample/eq/exa.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/data_sample/eq/exa.json" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quloaders/data_sample/eq/exam.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/data_sample/eq/exam.json" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quloaders/data_sample/exam.csv" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/data_sample/exam.csv" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quloaders/test_csv_loader.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/test_csv_loader.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quloaders/test_json_loader.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/test_json_loader.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quwriter/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quwriter/data_sample/eq/exa.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/data_sample/eq/exa.json" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quwriter/data_sample/eq/exam.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/data_sample/eq/exam.json" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quwriter/data_sample/exam.csv" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/data_sample/exam.csv" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quwriter/test_json_writer.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/test_json_writer.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/quwriter/test_type_checker.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/test_type_checker.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -18,14 +40,17 @@
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
+  <component name="HighlightingSettingsPerFile">
+    <setting file="file://$PROJECT_DIR$/../AppData/Local/Programs/Python/Python311/Lib/site-packages/QuBuilders/__init__.py" root0="FORCE_HIGHLIGHTING"/>
+  </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2RcS5ShzqHPzikurVLUjRtRVVfU"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
@@ -34,117 +59,118 @@
   "keyToString": {
     "ASKED_SHARE_PROJECT_CONFIGURATION_FILES": "true",
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "SHARE_PROJECT_CONFIGURATION_FILES": "true",
     "WebServerToolWindowFactoryState": "false",
     "database.data.extractors.current.export.id": "Comma-separated (CSV)_id",
-    "last_opened_file_path": "C:/Users/mzx776/QuBuilders",
+    "last_opened_file_path": "C:/Users/mzx776/Desktop/New folder",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="E:\Github Repos\QuBu\tests\quwriter"/>
       <recent name="E:\Github Repos\QuBu\quloaders\data_sample\eq"/>
       <recent name="E:\Github Repos\QuBu\quloaders\data_sample\questions"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\mzx776\QuBuilders\QuBuilders"/>
+      <recent name="C:\Users\mzx776\QuBuilders"/>
       <recent name="E:\Github Repos\QuBu\tests\quloaders"/>
       <recent name="E:\Github Repos\QuBu\quloaders\data_sample\eq"/>
       <recent name="E:\Github Repos\QuBu\quloaders\data_sample"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.Python tests for tests.generators.test_checkers.test.test_length_save">
-    <configuration name="Python tests for tests.generators.test_checkers.test.test_length_save" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+  <component name="RunManager" selected="Python tests.Python tests for QuBuilders.tests.generators.test_checkers.test.test_length_save">
+    <configuration name="Python tests for QuBuilders.tests.generators.test_checkers.test.test_length_save" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="QuBu"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value="C:\Users\mzx776\AppData\Local\Programs\Python\Python311\python.exe"/>
       <option name="SDK_NAME" value="Python 3.11"/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/generators"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/QuBuilders/tests/generators"/>
       <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.generators.test_checkers.test.test_length_save&quot;"/>
+      <option name="_new_target" value="&quot;QuBuilders.tests.generators.test_checkers.test.test_length_save&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for tests.quloaders.test_json_loader.test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for QuBuilders.tests.quloaders.test_json_loader.test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="QuBu"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/quloaders"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/QuBuilders/tests/quloaders"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.quloaders.test_json_loader.test&quot;"/>
+      <option name="_new_target" value="&quot;QuBuilders.tests.quloaders.test_json_loader.test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for tests.quwriter.test_json_writer.test.test_write_all" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for QuBuilders.tests.quwriter.test_json_writer.test.test_write_all" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="QuBu"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/quwriter"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/QuBuilders/tests/quwriter"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.quwriter.test_json_writer.test.test_write_all&quot;"/>
+      <option name="_new_target" value="&quot;QuBuilders.tests.quwriter.test_json_writer.test.test_write_all&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for tests.quwriter.test_json_writer.test.test_write_single" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for QuBuilders.tests.quwriter.test_json_writer.test.test_write_single" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="QuBu"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/quwriter"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/QuBuilders/tests/quwriter"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.quwriter.test_json_writer.test.test_write_single&quot;"/>
+      <option name="_new_target" value="&quot;QuBuilders.tests.quwriter.test_json_writer.test.test_write_single&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Python tests in test_json_loader.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="QuBu"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/quloaders"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/QuBuilders/tests/quloaders"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/quloaders/test_json_loader.py&quot;"/>
+      <option name="_new_target" value="&quot;$PROJECT_DIR$/QuBuilders/tests/quloaders/test_json_loader.py&quot;"/>
       <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python tests.Python tests for QuBuilders.tests.generators.test_checkers.test.test_length_save"/>
         <item itemvalue="Python tests.Python tests in test_json_loader.py"/>
-        <item itemvalue="Python tests.Python tests for tests.generators.test_checkers.test.test_length_save"/>
-        <item itemvalue="Python tests.Python tests for tests.quwriter.test_json_writer.test.test_write_all"/>
-        <item itemvalue="Python tests.Python tests for tests.quwriter.test_json_writer.test.test_write_single"/>
-        <item itemvalue="Python tests.Python tests for tests.quloaders.test_json_loader.test"/>
+        <item itemvalue="Python tests.Python tests for QuBuilders.tests.quwriter.test_json_writer.test.test_write_all"/>
+        <item itemvalue="Python tests.Python tests for QuBuilders.tests.quwriter.test_json_writer.test.test_write_single"/>
+        <item itemvalue="Python tests.Python tests for QuBuilders.tests.quloaders.test_json_loader.test"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="0643fa01-c989-4e6e-8770-b93352bd1ffb" name="Changes" comment=""/>
@@ -176,35 +202,14 @@
       <workItem from="1688355828490" duration="1283000"/>
       <workItem from="1688438837264" duration="1767000"/>
       <workItem from="1688440730652" duration="67000"/>
       <workItem from="1688441098575" duration="14000"/>
       <workItem from="1688441113905" duration="1271000"/>
       <workItem from="1688442413504" duration="70000"/>
     </task>
-    <task id="LOCAL-00050" summary="the Asghar_S.py is debugged">
-      <created>1687809687028</created>
-      <option name="number" value="00050"/>
-      <option name="presentableId" value="LOCAL-00050"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687809687028</updated>
-    </task>
-    <task id="LOCAL-00051" summary="the option for same questions or no added">
-      <created>1687809978387</created>
-      <option name="number" value="00051"/>
-      <option name="presentableId" value="LOCAL-00051"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687809978387</updated>
-    </task>
-    <task id="LOCAL-00052" summary="the __init__ of class State is crated">
-      <created>1687810915883</created>
-      <option name="number" value="00052"/>
-      <option name="presentableId" value="LOCAL-00052"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687810915883</updated>
-    </task>
     <task id="LOCAL-00053" summary="the __init__ of class State is got better by adding some checking">
       <created>1687811231508</created>
       <option name="number" value="00053"/>
       <option name="presentableId" value="LOCAL-00053"/>
       <option name="project" value="LOCAL"/>
       <updated>1687811231508</updated>
     </task>
@@ -519,15 +524,36 @@
     <task id="LOCAL-00098" summary="the version 0.0.6">
       <created>1688497331080</created>
       <option name="number" value="00098"/>
       <option name="presentableId" value="LOCAL-00098"/>
       <option name="project" value="LOCAL"/>
       <updated>1688497331081</updated>
     </task>
-    <option name="localTasksCounter" value="99"/>
+    <task id="LOCAL-00099" summary="the version 0.0.6">
+      <created>1688497498845</created>
+      <option name="number" value="00099"/>
+      <option name="presentableId" value="LOCAL-00099"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688497498845</updated>
+    </task>
+    <task id="LOCAL-00100" summary="the version 0.0.6">
+      <created>1688497512269</created>
+      <option name="number" value="00100"/>
+      <option name="presentableId" value="LOCAL-00100"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688497512269</updated>
+    </task>
+    <task id="LOCAL-00101" summary="the version 0.0.6">
+      <created>1688497750527</created>
+      <option name="number" value="00101"/>
+      <option name="presentableId" value="LOCAL-00101"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688497750527</updated>
+    </task>
+    <option name="localTasksCounter" value="102"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
```

### Comparing `qubuilders-0.0.6/QuBuilders/.github/workflows/python-package.yml` & `qubuilders-0.0.7/QuBuilders/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/NchTan/form.py` & `qubuilders-0.0.7/QuBuilders/NchTan/form.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/NchTan/quseq.py` & `qubuilders-0.0.7/QuBuilders/NchTan/quseq.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/generators/stament/Asghar_S.py` & `qubuilders-0.0.7/QuBuilders/generators/stament/Asghar_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/generators/stament/Mode_S.py` & `qubuilders-0.0.7/QuBuilders/generators/stament/Mode_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/generators/stament/Rostam_S.py` & `qubuilders-0.0.7/QuBuilders/generators/stament/Rostam_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/generators/stament/checker.py` & `qubuilders-0.0.7/QuBuilders/generators/stament/checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/quloaders/csv_loader.py` & `qubuilders-0.0.7/QuBuilders/quloaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/quloaders/json_loader.py` & `qubuilders-0.0.7/QuBuilders/quloaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/quwriter/csv_writer.py` & `qubuilders-0.0.7/QuBuilders/quwriter/csv_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/QuBuilders/quwriter/json_writer.py` & `qubuilders-0.0.7/QuBuilders/quwriter/json_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/NchTan/test_NchTan_From.py` & `qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_From.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/NchTan/test_NchTan_quseq.py` & `qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_quseq.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/generators/test_Mode_S.py` & `qubuilders-0.0.7/QuBuilders/tests/generators/test_Mode_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/generators/test_asghar_S.py` & `qubuilders-0.0.7/QuBuilders/tests/generators/test_asghar_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/generators/test_checkers.py` & `qubuilders-0.0.7/QuBuilders/tests/generators/test_checkers.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/generators/test_rostam_s.py` & `qubuilders-0.0.7/QuBuilders/tests/generators/test_rostam_s.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/quloaders/test_json_loader.py` & `qubuilders-0.0.7/QuBuilders/tests/quloaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/quwriter/test_json_writer.py` & `qubuilders-0.0.7/QuBuilders/tests/quwriter/test_json_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/tests/quwriter/test_type_checker.py` & `qubuilders-0.0.7/QuBuilders/tests/quwriter/test_type_checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/LICENSE` & `qubuilders-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.6/pyproject.toml` & `qubuilders-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling",'validators', 'beautifulsoup4',]
 build-backend = "hatchling.build"
 [project]
 name = "QuBuilders"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Amirrza Zahraei", email="amir.reza.zahraei@gmail.com" },
 ]
 description = "a pakage that help you to make n choice questions faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qubuilders-0.0.6/PKG-INFO` & `qubuilders-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuBuilders
-Version: 0.0.6
+Version: 0.0.7
 Summary: a pakage that help you to make n choice questions faster
 Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
 Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
 Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,16 +38,34 @@
 the only different is this that some words and some numbers and
 symbols are different, however the pattern, concept and the solution
 of all of them is the same.
 
 Now this is a little project named QuBu that will help you to generate
 such questions.
 
-installation:
+# installation:
 
 for installing the project you can simply use pip and your cmd:
 
-pip install QuBuilders
-
+```cmd
+# for Uix/MacOS
+python3 -m pip install QuBuilders
+
+# for windows
+py -m pip install QuBuilders
+```
+
+# How to use
+
+to use this project first let's go to talk about how to make 
+a simple question:
+
+For making a question you can simply use QuestionDataSaver class to save 
+your questions and manage them in an appropriate way. to save your question 
+you can do like the following code:
+
+``` python
+from QuBuilders.NchTan import QuestionDataSaver
+```
```

