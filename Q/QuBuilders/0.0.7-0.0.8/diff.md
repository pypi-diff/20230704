# Comparing `tmp/qubuilders-0.0.7.tar.gz` & `tmp/qubuilders-0.0.8.tar.gz`

## Comparing `qubuilders-0.0.7.tar` & `qubuilders-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 qubuilders-0.0.7/setup.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/QuBu.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0    32329 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/__main__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/form.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/formd.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/NchTan/quseq.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/Asghar_S.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/Mode_S.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/Rostam_S.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/generators/stament/checker.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quloaders/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quloaders/csv_loader.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quloaders/json_loader.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/csv_writer.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/json_writer.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/quwriter/type_checker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/NchTan/__init__.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_From.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_quseq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_Mode_S.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_asghar_S.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_checkers.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/generators/test_rostam_s.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/test_csv_loader.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/test_json_loader.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/data_sample/exam.csv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/data_sample/eq/exa.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quloaders/data_sample/eq/exam.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/test_json_writer.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/test_type_checker.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/data_sample/exam.csv
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/data_sample/eq/exa.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.7/QuBuilders/tests/quwriter/data_sample/eq/exam.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.7/LICENSE
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 qubuilders-0.0.7/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 qubuilders-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 qubuilders-0.0.8/setup.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/QuBu.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0    28494 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/__main__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/NchTan/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/NchTan/form.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/NchTan/formd.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/NchTan/quseq.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/generators/stament/Asghar_S.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/generators/stament/Mode_S.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/generators/stament/Rostam_S.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/generators/stament/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/generators/stament/checker.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quloaders/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quloaders/csv_loader.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quloaders/json_loader.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quwriter/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quwriter/csv_writer.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quwriter/json_writer.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/quwriter/type_checker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/NchTan/__init__.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/NchTan/test_NchTan_From.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/NchTan/test_NchTan_quseq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/generators/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/generators/test_Mode_S.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/generators/test_asghar_S.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/generators/test_checkers.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/generators/test_rostam_s.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quloaders/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quloaders/test_csv_loader.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quloaders/test_json_loader.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quloaders/data_sample/exam.csv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quloaders/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quloaders/data_sample/eq/exam.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quwriter/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quwriter/test_json_writer.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quwriter/test_type_checker.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quwriter/data_sample/exam.csv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quwriter/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.8/QuBuilders/tests/quwriter/data_sample/eq/exam.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 qubuilders-0.0.8/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 qubuilders-0.0.8/PKG-INFO
```

### Comparing `qubuilders-0.0.7/setup.py` & `qubuilders-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 from distutils.core import setup
 setup(
   name = 'QuBuilders',         # How you named your package folder (MyLib)
   packages = ['QuBuilders'],   # Chose the same as "name"
-  version = '0.0.7',      # Start with a small number and increase it with every change you make
+  version = '0.0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'this is a python package help you to make n choice questions',   # Give a short description about your library
   author = 'Amirreza Zahraei',                   # Type in your name
   author_email = 'amir.reza.zahraei@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AmirrezaZahraei1387/QuBu',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubuilders-0.0.7.tar.gz',    # I explain this later on
   keywords = ['Question', 'multiple choice questions', 'creating questions'],   # Keywords that define your package best
```

### Comparing `qubuilders-0.0.7/.idea/QuBu.iml` & `qubuilders-0.0.8/.idea/QuBu.iml`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/.idea/workspace.xml` & `qubuilders-0.0.8/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `qubuilders-0.0.7/.idea/workspace.xml` & `qubuilders-0.0.8/.idea/workspace.xml`

```diff
@@ -1,37 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="0643fa01-c989-4e6e-8770-b93352bd1ffb" name="Changes" comment="the version 0.0.6">
+    <list default="true" id="0643fa01-c989-4e6e-8770-b93352bd1ffb" name="Changes" comment="the version 0.0.7">
       <change beforePath="$PROJECT_DIR$/.idea/workspace.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/workspace.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/NchTan/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/NchTan/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/NchTan/test_NchTan_From.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/NchTan/test_NchTan_From.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/NchTan/test_NchTan_quseq.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/NchTan/test_NchTan_quseq.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/generators/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/generators/test_Mode_S.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_Mode_S.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/generators/test_asghar_S.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_asghar_S.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/generators/test_checkers.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_checkers.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/generators/test_rostam_s.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/generators/test_rostam_s.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quloaders/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quloaders/data_sample/eq/exa.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/data_sample/eq/exa.json" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quloaders/data_sample/eq/exam.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/data_sample/eq/exam.json" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quloaders/data_sample/exam.csv" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/data_sample/exam.csv" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quloaders/test_csv_loader.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/test_csv_loader.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quloaders/test_json_loader.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quloaders/test_json_loader.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quwriter/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quwriter/data_sample/eq/exa.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/data_sample/eq/exa.json" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quwriter/data_sample/eq/exam.json" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/data_sample/eq/exam.json" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quwriter/data_sample/exam.csv" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/data_sample/exam.csv" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quwriter/test_json_writer.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/test_json_writer.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/quwriter/test_type_checker.py" beforeDir="false" afterPath="$PROJECT_DIR$/QuBuilders/tests/quwriter/test_type_checker.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -51,29 +29,29 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2RcS5ShzqHPzikurVLUjRtRVVfU"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "ASKED_SHARE_PROJECT_CONFIGURATION_FILES": "true",
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "SHARE_PROJECT_CONFIGURATION_FILES": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "database.data.extractors.current.export.id": "Comma-separated (CSV)_id",
-    "last_opened_file_path": "C:/Users/mzx776/Desktop/New folder",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;ASKED_SHARE_PROJECT_CONFIGURATION_FILES&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;SHARE_PROJECT_CONFIGURATION_FILES&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;database.data.extractors.current.export.id&quot;: &quot;Comma-separated (CSV)_id&quot;,
+    &quot;last_opened_file_path&quot;: &quot;C:/Users/mzx776/Desktop/New folder&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="E:\Github Repos\QuBu\tests\quwriter"/>
       <recent name="E:\Github Repos\QuBu\quloaders\data_sample\eq"/>
       <recent name="E:\Github Repos\QuBu\quloaders\data_sample\questions"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
@@ -202,28 +180,14 @@
       <workItem from="1688355828490" duration="1283000"/>
       <workItem from="1688438837264" duration="1767000"/>
       <workItem from="1688440730652" duration="67000"/>
       <workItem from="1688441098575" duration="14000"/>
       <workItem from="1688441113905" duration="1271000"/>
       <workItem from="1688442413504" duration="70000"/>
     </task>
-    <task id="LOCAL-00053" summary="the __init__ of class State is got better by adding some checking">
-      <created>1687811231508</created>
-      <option name="number" value="00053"/>
-      <option name="presentableId" value="LOCAL-00053"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687811231508</updated>
-    </task>
-    <task id="LOCAL-00054" summary="the class state seem done">
-      <created>1687812157610</created>
-      <option name="number" value="00054"/>
-      <option name="presentableId" value="LOCAL-00054"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687812157610</updated>
-    </task>
     <task id="LOCAL-00055" summary="the Rostam_S.py is tested">
       <created>1687812600760</created>
       <option name="number" value="00055"/>
       <option name="presentableId" value="LOCAL-00055"/>
       <option name="project" value="LOCAL"/>
       <updated>1687812600760</updated>
     </task>
@@ -545,15 +509,29 @@
     <task id="LOCAL-00101" summary="the version 0.0.6">
       <created>1688497750527</created>
       <option name="number" value="00101"/>
       <option name="presentableId" value="LOCAL-00101"/>
       <option name="project" value="LOCAL"/>
       <updated>1688497750527</updated>
     </task>
-    <option name="localTasksCounter" value="102"/>
+    <task id="LOCAL-00102" summary="the version 0.0.7">
+      <created>1688498674143</created>
+      <option name="number" value="00102"/>
+      <option name="presentableId" value="LOCAL-00102"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688498674143</updated>
+    </task>
+    <task id="LOCAL-00103" summary="the version 0.0.7">
+      <created>1688498726104</created>
+      <option name="number" value="00103"/>
+      <option name="presentableId" value="LOCAL-00103"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688498726104</updated>
+    </task>
+    <option name="localTasksCounter" value="104"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -563,15 +541,14 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="the Rostam_S.py is tested"/>
     <MESSAGE value="the __init__.py is added to the generators"/>
     <MESSAGE value="the files are debugged and some new options are added"/>
     <MESSAGE value="a option  for checing all the lengths is added to Rostam_S.py."/>
     <MESSAGE value="the test requrements for quwriters is added"/>
     <MESSAGE value="__init__ created"/>
     <MESSAGE value="a new class named check_length is added to avoid same codes"/>
     <MESSAGE value="the codes are checked"/>
@@ -588,10 +565,11 @@
     <MESSAGE value="the setup.py"/>
     <MESSAGE value="main added"/>
     <MESSAGE value="the version 0.0.3 of the pakage released"/>
     <MESSAGE value="the __init__.pys resolved"/>
     <MESSAGE value="the version 0.0.4"/>
     <MESSAGE value="the version 0.0.5"/>
     <MESSAGE value="the version 0.0.6"/>
-    <option name="LAST_COMMIT_MESSAGE" value="the version 0.0.6"/>
+    <MESSAGE value="the version 0.0.7"/>
+    <option name="LAST_COMMIT_MESSAGE" value="the version 0.0.7"/>
   </component>
 </project>
```

### Comparing `qubuilders-0.0.7/QuBuilders/.github/workflows/python-package.yml` & `qubuilders-0.0.8/QuBuilders/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/NchTan/form.py` & `qubuilders-0.0.8/QuBuilders/NchTan/form.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/NchTan/quseq.py` & `qubuilders-0.0.8/QuBuilders/NchTan/quseq.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/generators/stament/Asghar_S.py` & `qubuilders-0.0.8/QuBuilders/generators/stament/Asghar_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/generators/stament/Mode_S.py` & `qubuilders-0.0.8/QuBuilders/generators/stament/Mode_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/generators/stament/Rostam_S.py` & `qubuilders-0.0.8/QuBuilders/generators/stament/Rostam_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/generators/stament/checker.py` & `qubuilders-0.0.8/QuBuilders/generators/stament/checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/quloaders/csv_loader.py` & `qubuilders-0.0.8/QuBuilders/quloaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/quloaders/json_loader.py` & `qubuilders-0.0.8/QuBuilders/quloaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/quwriter/csv_writer.py` & `qubuilders-0.0.8/QuBuilders/quwriter/csv_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/quwriter/json_writer.py` & `qubuilders-0.0.8/QuBuilders/quwriter/json_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_From.py` & `qubuilders-0.0.8/QuBuilders/tests/NchTan/test_NchTan_From.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/NchTan/test_NchTan_quseq.py` & `qubuilders-0.0.8/QuBuilders/tests/NchTan/test_NchTan_quseq.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/generators/test_Mode_S.py` & `qubuilders-0.0.8/QuBuilders/tests/generators/test_Mode_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/generators/test_asghar_S.py` & `qubuilders-0.0.8/QuBuilders/tests/generators/test_asghar_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/generators/test_checkers.py` & `qubuilders-0.0.8/QuBuilders/tests/generators/test_checkers.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/generators/test_rostam_s.py` & `qubuilders-0.0.8/QuBuilders/tests/generators/test_rostam_s.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/quloaders/test_json_loader.py` & `qubuilders-0.0.8/QuBuilders/tests/quloaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/quwriter/test_json_writer.py` & `qubuilders-0.0.8/QuBuilders/tests/quwriter/test_json_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/QuBuilders/tests/quwriter/test_type_checker.py` & `qubuilders-0.0.8/QuBuilders/tests/quwriter/test_type_checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/LICENSE` & `qubuilders-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/README.md` & `qubuilders-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.7/pyproject.toml` & `qubuilders-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling",'validators', 'beautifulsoup4',]
 build-backend = "hatchling.build"
 [project]
 name = "QuBuilders"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Amirrza Zahraei", email="amir.reza.zahraei@gmail.com" },
 ]
 description = "a pakage that help you to make n choice questions faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qubuilders-0.0.7/PKG-INFO` & `qubuilders-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuBuilders
-Version: 0.0.7
+Version: 0.0.8
 Summary: a pakage that help you to make n choice questions faster
 Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
 Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
 Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

