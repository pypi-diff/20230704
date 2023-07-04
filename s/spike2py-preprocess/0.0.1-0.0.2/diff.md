# Comparing `tmp/spike2py_preprocess-0.0.1.tar.gz` & `tmp/spike2py_preprocess-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spike2py_preprocess-0.0.1.tar", last modified: Tue Jul  4 05:02:09 2023, max compression
+gzip compressed data, was "spike2py_preprocess-0.0.2.tar", last modified: Tue Jul  4 06:06:01 2023, max compression
```

## Comparing `spike2py_preprocess-0.0.1.tar` & `spike2py_preprocess-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 05:02:09.479495 spike2py_preprocess-0.0.1/
--rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-07-02 04:35:06.000000 spike2py_preprocess-0.0.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     6052 2023-07-04 05:02:09.479495 spike2py_preprocess-0.0.1/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     5579 2023-07-04 04:06:53.000000 spike2py_preprocess-0.0.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-04 05:02:09.479495 spike2py_preprocess-0.0.1/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      975 2023-07-04 05:01:01.000000 spike2py_preprocess-0.0.1/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 05:02:09.479495 spike2py_preprocess-0.0.1/spike2py_preprocess/
--rw-r--r--   0 martin    (1000) martin    (1000)       22 2023-07-02 04:35:07.000000 spike2py_preprocess-0.0.1/spike2py_preprocess/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6700 2023-07-03 11:45:32.000000 spike2py_preprocess-0.0.1/spike2py_preprocess/preprocess.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 05:02:09.479495 spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     6052 2023-07-04 05:02:09.000000 spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      306 2023-07-04 05:02:09.000000 spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-04 05:02:09.000000 spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-07-04 05:02:09.000000 spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       20 2023-07-04 05:02:09.000000 spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/
+-rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-07-02 04:35:06.000000 spike2py_preprocess-0.0.2/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6052 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     5579 2023-07-04 04:06:53.000000 spike2py_preprocess-0.0.2/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      975 2023-07-04 06:04:37.000000 spike2py_preprocess-0.0.2/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/spike2py_preprocess/
+-rw-r--r--   0 martin    (1000) martin    (1000)       22 2023-07-02 04:35:07.000000 spike2py_preprocess-0.0.2/spike2py_preprocess/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6755 2023-07-04 05:41:14.000000 spike2py_preprocess-0.0.2/spike2py_preprocess/preprocess.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-04 06:06:01.070707 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6052 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      306 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       20 2023-07-04 06:06:01.000000 spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/top_level.txt
```

### Comparing `spike2py_preprocess-0.0.1/LICENSE` & `spike2py_preprocess-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spike2py_preprocess-0.0.1/PKG-INFO` & `spike2py_preprocess-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spike2py_preprocess
-Version: 0.0.1
+Version: 0.0.2
 Summary: Preprocess data with spike2py
 Home-page: https://github.com/MartinHeroux/spike2py_preprocess
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `spike2py_preprocess-0.0.1/README.md` & `spike2py_preprocess-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spike2py_preprocess-0.0.1/setup.py` & `spike2py_preprocess-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="spike2py_preprocess",
-    version="0.0.1",
+    version="0.0.2",
     description="Preprocess data with spike2py",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MartinHeroux/spike2py_preprocess",
     author="Martin Héroux",
     author_email="heroux.martin@gmail.com",
     license="GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `spike2py_preprocess-0.0.1/spike2py_preprocess/preprocess.py` & `spike2py_preprocess-0.0.2/spike2py_preprocess/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from pathlib import Path
+from typing import Union
 from dataclasses import dataclass
 
 from rich import print
 
 from spike2py.trial import Trial, TrialInfo
 
 
@@ -28,15 +29,15 @@
 
     def create(self):
         self.raw = self.home / "raw"
         self.proc = self.home / "proc"
         self.figures = self.home / "figures"
 
 
-def read_json(json_path: Path, strict: bool = True) -> dict | None:
+def read_json(json_path: Path, strict: bool = True) -> Union[dict, None]:
     """
     Read json file and return its content.
 
     If strict=True and file not found, program will stop.
     If strict=False and file note found, program will continue.
 
     Parameters
@@ -64,15 +65,15 @@
         message = f'{json_path.name} does not exist.'
         if strict:
             raise FileNotFoundError(message)
         print(message)
         return
 
 
-def trial(trial_info: TrialInfo, preprocess_info: dict | None = None):
+def trial(trial_info: TrialInfo, preprocess_info: Union[dict, None] = None):
     """
     Read, preprocess (if required) and pickle trial data.
 
     Parameters
     ----------
     trial_info: TrialInfo
         Instance of spike2py TrialInfo with info required to load data
@@ -115,16 +116,16 @@
         for preprocess_name, preprocess_arguments in preprocesses.items():
             exec(f"data.{channel}.{preprocess_name}({preprocess_arguments})")
     return data
 
 
 def subject(
     subject_path: Path,
-    preprocess_info: dict | None = None,
-    study_info: dict | None = None,
+    preprocess_info: Union[dict, None] = None,
+    study_info: Union[dict, None] = None,
 ):
     """
     Preprocess all trials for a given subject.
 
     Parameters
     ----------
     subject_path: Path
@@ -149,15 +150,15 @@
 
 def _gen_subject_paths(subject_path):
     paths = SubjectPaths(home=subject_path)
     paths.create()
     return paths
 
 
-def _get_subject_preprocess_info(paths: SubjectPaths, preprocess_info: dict | None):
+def _get_subject_preprocess_info(paths: SubjectPaths, preprocess_info: Union[dict, None]):
     preprocess_file = paths.home / SUBJECT_PREPROCESS_FILE
     info = _get_preprocess_info(preprocess_file, preprocess_info)
     return info
 
 
 def _preprocess_subject_trials(paths, subject_info, preprocess_info, study_info):
     for trial_ in subject_info["trials"].values():
```

### Comparing `spike2py_preprocess-0.0.1/spike2py_preprocess.egg-info/PKG-INFO` & `spike2py_preprocess-0.0.2/spike2py_preprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spike2py-preprocess
-Version: 0.0.1
+Version: 0.0.2
 Summary: Preprocess data with spike2py
 Home-page: https://github.com/MartinHeroux/spike2py_preprocess
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
```

