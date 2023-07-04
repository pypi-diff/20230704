# Comparing `tmp/qubuilders-0.0.1.tar.gz` & `tmp/qubuilders-0.0.2.tar.gz`

## Comparing `qubuilders-0.0.1.tar` & `qubuilders-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.1/__main__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 qubuilders-0.0.1/setup.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/QuBu.iml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    32480 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qubuilders-0.0.1/NchTan/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.1/NchTan/form.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.1/NchTan/formd.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 qubuilders-0.0.1/NchTan/quseq.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 qubuilders-0.0.1/generators/stament/Asghar_S.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 qubuilders-0.0.1/generators/stament/Mode_S.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.1/generators/stament/Rostam_S.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 qubuilders-0.0.1/generators/stament/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.1/generators/stament/checker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quloaders/__init__.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quloaders/csv_loader.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quloaders/json_loader.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quwriter/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quwriter/csv_writer.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quwriter/json_writer.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 qubuilders-0.0.1/quwriter/type_checker.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/NchTan/test_NchTan_From.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/NchTan/test_NchTan_quseq.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/generators/test_Mode_S.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/generators/test_asghar_S.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/generators/test_checkers.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/generators/test_rostam_s.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quloaders/test_csv_loader.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quloaders/test_json_loader.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quloaders/data_sample/exam.csv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quloaders/data_sample/eq/exa.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quloaders/data_sample/eq/exam.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quwriter/test_json_writer.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quwriter/test_type_checker.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quwriter/data_sample/exam.csv
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quwriter/data_sample/eq/exa.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.1/tests/quwriter/data_sample/eq/exam.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.1/LICENSE
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 qubuilders-0.0.1/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 qubuilders-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 qubuilders-0.0.2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qubuilders-0.0.2/__main__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 qubuilders-0.0.2/setup.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/QuBu.iml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    32131 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 qubuilders-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/form.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/formd.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 qubuilders-0.0.2/NchTan/quseq.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/Asghar_S.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/Mode_S.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/Rostam_S.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 qubuilders-0.0.2/generators/stament/checker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quloaders/__init__.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quloaders/csv_loader.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quloaders/json_loader.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/csv_writer.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/json_writer.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 qubuilders-0.0.2/quwriter/type_checker.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/NchTan/test_NchTan_From.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/NchTan/test_NchTan_quseq.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_Mode_S.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_asghar_S.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_checkers.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/generators/test_rostam_s.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/test_csv_loader.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/test_json_loader.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/data_sample/exam.csv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quloaders/data_sample/eq/exam.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/test_json_writer.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/test_type_checker.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/data_sample/exam.csv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/data_sample/eq/exa.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qubuilders-0.0.2/tests/quwriter/data_sample/eq/exam.json
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 qubuilders-0.0.2/LICENSE
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 qubuilders-0.0.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 qubuilders-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 qubuilders-0.0.2/PKG-INFO
```

### Comparing `qubuilders-0.0.1/setup.py` & `qubuilders-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
-  name = 'QuestionBuilders',         # How you named your package folder (MyLib)
-  packages = ['QuestionBuilders'],   # Chose the same as "name"
-  version = '0.0.1',      # Start with a small number and increase it with every change you make
+  name = 'QuBuilders',         # How you named your package folder (MyLib)
+  packages = ['QuBuilders'],   # Chose the same as "name"
+  version = '0.0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'this is a python package help you to make n choice questions',   # Give a short description about your library
   author = 'Amirreza Zahraei',                   # Type in your name
   author_email = 'amir.reza.zahraei@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/AmirrezaZahraei1387/QuBu',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/AmirrezaZahraei1387/QuBu/blob/master/dist/qubu-0.0.1.tar.gz',    # I explain this later on
   keywords = ['Question', 'multiple choice questions', 'creating questions'],   # Keywords that define your package best
```

### Comparing `qubuilders-0.0.1/.github/workflows/python-package.yml` & `qubuilders-0.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/.idea/workspace.xml` & `qubuilders-0.0.2/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `qubuilders-0.0.1/.idea/workspace.xml` & `qubuilders-0.0.2/.idea/workspace.xml`

```diff
@@ -1,18 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="0643fa01-c989-4e6e-8770-b93352bd1ffb" name="Changes" comment="main added">
-      <change beforePath="$PROJECT_DIR$/dist/qubu-0.0.1-py3-none-any.whl" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/qubu-0.0.1.tar.gz" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-    </list>
+    <list default="true" id="0643fa01-c989-4e6e-8770-b93352bd1ffb" name="Changes" comment="main added"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -174,43 +170,16 @@
       <workItem from="1687900023461" duration="1000"/>
       <workItem from="1687915335686" duration="4350000"/>
       <workItem from="1687968438893" duration="21000"/>
       <workItem from="1688355828490" duration="1283000"/>
       <workItem from="1688438837264" duration="1767000"/>
       <workItem from="1688440730652" duration="67000"/>
       <workItem from="1688441098575" duration="14000"/>
-      <workItem from="1688441113905" duration="1063000"/>
-    </task>
-    <task id="LOCAL-00036" summary="a docstring is added to json_writer.py file">
-      <created>1687731425311</created>
-      <option name="number" value="00036"/>
-      <option name="presentableId" value="LOCAL-00036"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687731425311</updated>
-    </task>
-    <task id="LOCAL-00037" summary="the type_checker.py is more compatible">
-      <created>1687732604886</created>
-      <option name="number" value="00037"/>
-      <option name="presentableId" value="LOCAL-00037"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687732604886</updated>
-    </task>
-    <task id="LOCAL-00038" summary="the formd is added">
-      <created>1687732864956</created>
-      <option name="number" value="00038"/>
-      <option name="presentableId" value="LOCAL-00038"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687732864956</updated>
-    </task>
-    <task id="LOCAL-00039" summary="the form is created">
-      <created>1687732990590</created>
-      <option name="number" value="00039"/>
-      <option name="presentableId" value="LOCAL-00039"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687732990590</updated>
+      <workItem from="1688441113905" duration="1271000"/>
+      <workItem from="1688442413504" duration="70000"/>
     </task>
     <task id="LOCAL-00040" summary="the option of closing files is added to all loaders and writers">
       <created>1687733336460</created>
       <option name="number" value="00040"/>
       <option name="presentableId" value="LOCAL-00040"/>
       <option name="project" value="LOCAL"/>
       <updated>1687733336460</updated>
@@ -519,15 +488,43 @@
     <task id="LOCAL-00084" summary="main added">
       <created>1688441813436</created>
       <option name="number" value="00084"/>
       <option name="presentableId" value="LOCAL-00084"/>
       <option name="project" value="LOCAL"/>
       <updated>1688441813436</updated>
     </task>
-    <option name="localTasksCounter" value="85"/>
+    <task id="LOCAL-00085" summary="main added">
+      <created>1688442213323</created>
+      <option name="number" value="00085"/>
+      <option name="presentableId" value="LOCAL-00085"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688442213323</updated>
+    </task>
+    <task id="LOCAL-00086" summary="main added">
+      <created>1688442225574</created>
+      <option name="number" value="00086"/>
+      <option name="presentableId" value="LOCAL-00086"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688442225575</updated>
+    </task>
+    <task id="LOCAL-00087" summary="main added">
+      <created>1688442389547</created>
+      <option name="number" value="00087"/>
+      <option name="presentableId" value="LOCAL-00087"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688442389547</updated>
+    </task>
+    <task id="LOCAL-00088" summary="main added">
+      <created>1688442440591</created>
+      <option name="number" value="00088"/>
+      <option name="presentableId" value="LOCAL-00088"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688442440592</updated>
+    </task>
+    <option name="localTasksCounter" value="89"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
```

### Comparing `qubuilders-0.0.1/NchTan/form.py` & `qubuilders-0.0.2/NchTan/form.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/NchTan/quseq.py` & `qubuilders-0.0.2/NchTan/quseq.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/generators/stament/Asghar_S.py` & `qubuilders-0.0.2/generators/stament/Asghar_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/generators/stament/Mode_S.py` & `qubuilders-0.0.2/generators/stament/Mode_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/generators/stament/Rostam_S.py` & `qubuilders-0.0.2/generators/stament/Rostam_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/generators/stament/checker.py` & `qubuilders-0.0.2/generators/stament/checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/quloaders/csv_loader.py` & `qubuilders-0.0.2/quloaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/quloaders/json_loader.py` & `qubuilders-0.0.2/quloaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/quwriter/csv_writer.py` & `qubuilders-0.0.2/quwriter/csv_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/quwriter/json_writer.py` & `qubuilders-0.0.2/quwriter/json_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/quwriter/type_checker.py` & `qubuilders-0.0.2/quwriter/type_checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/NchTan/test_NchTan_From.py` & `qubuilders-0.0.2/tests/NchTan/test_NchTan_From.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/NchTan/test_NchTan_quseq.py` & `qubuilders-0.0.2/tests/NchTan/test_NchTan_quseq.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/generators/test_Mode_S.py` & `qubuilders-0.0.2/tests/generators/test_Mode_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/generators/test_asghar_S.py` & `qubuilders-0.0.2/tests/generators/test_asghar_S.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/generators/test_checkers.py` & `qubuilders-0.0.2/tests/generators/test_checkers.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/generators/test_rostam_s.py` & `qubuilders-0.0.2/tests/generators/test_rostam_s.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/quloaders/test_json_loader.py` & `qubuilders-0.0.2/tests/quloaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/quwriter/test_json_writer.py` & `qubuilders-0.0.2/tests/quwriter/test_json_writer.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/tests/quwriter/test_type_checker.py` & `qubuilders-0.0.2/tests/quwriter/test_type_checker.py`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/LICENSE` & `qubuilders-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/README.md` & `qubuilders-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qubuilders-0.0.1/pyproject.toml` & `qubuilders-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling",'validators', 'beautifulsoup4',]
 build-backend = "hatchling.build"
 [project]
 name = "QuBuilders"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Amirrza Zahraei", email="amir.reza.zahraei@gmail.com" },
 ]
 description = "a pakage that help you to make n choice questions faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qubuilders-0.0.1/PKG-INFO` & `qubuilders-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuBuilders
-Version: 0.0.1
+Version: 0.0.2
 Summary: a pakage that help you to make n choice questions faster
 Project-URL: Homepage, https://github.com/AmirrezaZahraei1387/QuBu
 Project-URL: Bug Tracker, https://github.com/AmirrezaZahraei1387/QuBu/issues
 Author-email: Amirrza Zahraei <amir.reza.zahraei@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

