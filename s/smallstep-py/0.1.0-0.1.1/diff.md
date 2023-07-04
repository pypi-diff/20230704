# Comparing `tmp/smallstep_py-0.1.0.tar.gz` & `tmp/smallstep_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallstep_py-0.1.0.tar", last modified: Mon Jul  3 21:27:21 2023, max compression
+gzip compressed data, was "smallstep_py-0.1.1.tar", last modified: Tue Jul  4 02:06:18 2023, max compression
```

## Comparing `smallstep_py-0.1.0.tar` & `smallstep_py-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-29 23:32:15.071843 smallstep_py-0.1.0/LICENSE
--rw-r--r--   0        0        0       48 2023-06-29 23:32:15.072009 smallstep_py-0.1.0/README.md
--rw-r--r--   0        0        0      734 2023-07-03 21:27:21.866437 smallstep_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      921 2023-07-03 21:21:53.507597 smallstep_py-0.1.0/step/__init__.py
--rw-r--r--   0        0        0     2965 2023-07-03 21:21:58.248568 smallstep_py-0.1.0/step/models.py
--rw-r--r--   0        0        0     7068 2023-07-03 21:22:05.372785 smallstep_py-0.1.0/step/step_cli.py
--rwxr-xr-x   0        0        0     8660 2023-07-03 21:22:01.259668 smallstep_py-0.1.0/step/step_cli_parser.py
--rw-r--r--   0        0        0     1936 2023-07-03 18:25:42.846827 smallstep_py-0.1.0/tests/testing_step_cli.py
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 smallstep_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-29 23:32:15.071843 smallstep_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0      707 2023-07-04 01:51:30.702927 smallstep_py-0.1.1/README.md
+-rw-r--r--   0        0        0     1041 2023-07-04 02:06:18.890530 smallstep_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-07-04 01:55:27.202847 smallstep_py-0.1.1/step/__init__.py
+-rw-r--r--   0        0        0     2965 2023-07-04 01:23:40.835605 smallstep_py-0.1.1/step/models.py
+-rw-r--r--   0        0        0     7068 2023-07-03 21:22:05.372785 smallstep_py-0.1.1/step/step_cli.py
+-rwxr-xr-x   0        0        0     8660 2023-07-03 21:22:01.259668 smallstep_py-0.1.1/step/step_cli_parser.py
+-rw-r--r--   0        0        0     1936 2023-07-03 18:25:42.846827 smallstep_py-0.1.1/tests/testing_step_cli.py
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 smallstep_py-0.1.1/PKG-INFO
```

### Comparing `smallstep_py-0.1.0/LICENSE` & `smallstep_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smallstep_py-0.1.0/step/__init__.py` & `smallstep_py-0.1.1/step/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2023 Clayton Rosenthal
+Copyright (C) 2023 Clayton Rosenthal.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -12,20 +12,18 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # Python package to interact with (small)step ca through python
 
-from .models import (
-    StepAdmin,
-    StepSshHost
-)
+from .models import StepAdmin, StepSshHost, StepVersion
 from .step_cli import StepCli
 from .step_cli_parser import StepCliParser
 
 __all__ = [
     "StepAdmin",
     "StepSshHost",
+    "StepVersion",
     "StepCli",
     "StepCliParser",
-]
+]
```

### Comparing `smallstep_py-0.1.0/step/models.py` & `smallstep_py-0.1.1/step/models.py`

 * *Files identical despite different names*

### Comparing `smallstep_py-0.1.0/step/step_cli.py` & `smallstep_py-0.1.1/step/step_cli.py`

 * *Files identical despite different names*

### Comparing `smallstep_py-0.1.0/step/step_cli_parser.py` & `smallstep_py-0.1.1/step/step_cli_parser.py`

 * *Files identical despite different names*

### Comparing `smallstep_py-0.1.0/tests/testing_step_cli.py` & `smallstep_py-0.1.1/tests/testing_step_cli.py`

 * *Files identical despite different names*

