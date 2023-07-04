# Comparing `tmp/bofire_converters-0.0.1.tar.gz` & `tmp/bofire_converters-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bofire_converters-0.0.1.tar", last modified: Tue Jul  4 11:44:07 2023, max compression
+gzip compressed data, was "bofire_converters-0.0.2.tar", last modified: Tue Jul  4 13:08:19 2023, max compression
```

## Comparing `bofire_converters-0.0.1.tar` & `bofire_converters-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 11:44:07.254810 bofire_converters-0.0.1/
--rw-rw-rw-   0        0        0      390 2023-06-21 18:09:51.000000 bofire_converters-0.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1534 2023-04-24 08:46:39.000000 bofire_converters-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3034 2023-07-04 11:44:07.254810 bofire_converters-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      710 2023-07-04 10:05:48.000000 bofire_converters-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 11:44:07.232810 bofire_converters-0.0.1/bofire_converters/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:01:22.000000 bofire_converters-0.0.1/bofire_converters/__init__.py
--rw-rw-rw-   0        0        0     8790 2023-07-04 10:22:09.000000 bofire_converters-0.0.1/bofire_converters/opti_to_domain.py
--rw-rw-rw-   0        0        0      195 2023-07-04 11:44:06.000000 bofire_converters-0.0.1/bofire_converters/version.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:44:07.248810 bofire_converters-0.0.1/bofire_converters.egg-info/
--rw-rw-rw-   0        0        0     3034 2023-07-04 11:44:07.000000 bofire_converters-0.0.1/bofire_converters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-07-04 11:44:07.000000 bofire_converters-0.0.1/bofire_converters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 11:44:07.000000 bofire_converters-0.0.1/bofire_converters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-04 11:44:07.000000 bofire_converters-0.0.1/bofire_converters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-04 11:44:07.000000 bofire_converters-0.0.1/bofire_converters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1197 2023-07-04 11:38:37.000000 bofire_converters-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-04-27 12:57:50.000000 bofire_converters-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 11:44:07.255812 bofire_converters-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 11:44:07.251816 bofire_converters-0.0.1/test/
--rw-rw-rw-   0        0        0     4322 2023-04-28 16:04:59.000000 bofire_converters-0.0.1/test/test_opti_to_domain.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/
+-rw-rw-rw-   0        0        0      390 2023-06-21 18:09:51.000000 bofire_converters-0.0.2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1534 2023-04-24 08:46:39.000000 bofire_converters-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3284 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2023-07-04 13:06:43.000000 bofire_converters-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.580090 bofire_converters-0.0.2/bofire_converters/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:01:22.000000 bofire_converters-0.0.2/bofire_converters/__init__.py
+-rw-rw-rw-   0        0        0     8790 2023-07-04 10:22:09.000000 bofire_converters-0.0.2/bofire_converters/opti_to_domain.py
+-rw-rw-rw-   0        0        0      215 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters/version.py
+drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.611348 bofire_converters-0.0.2/bofire_converters.egg-info/
+-rw-rw-rw-   0        0        0     3284 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1197 2023-07-04 13:07:43.000000 bofire_converters-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      119 2023-04-27 12:57:50.000000 bofire_converters-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/test/
+-rw-rw-rw-   0        0        0     4322 2023-04-28 16:04:59.000000 bofire_converters-0.0.2/test/test_opti_to_domain.py
```

### Comparing `bofire_converters-0.0.1/LICENSE` & `bofire_converters-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bofire_converters-0.0.1/PKG-INFO` & `bofire_converters-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bofire_converters
-Version: 0.0.1
+Version: 0.0.2
 License: BSD 3-Clause License
         
         Copyright (c) 2023, experimental-design
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -40,25 +40,25 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Mopti Problem to Bofire Domain Converter
 
-These tools are to help with migration of legacy applications from other Mopti to BoFire, and improve quality-of-life.
+These tools are to help with migration of legacy applications from [Mopti](https://github.com/basf/mopti) to [BoFire](https://github.com/experimental-design/bofire). Mopti is for defining optimization problems (inputs, outputs, constraints, ...) and has some sampling utilities. If you have a _problem_ defined in the Mopti format, `bofire_converters` can help you to create the corresponding BoFire object, which is called a _domain_.
 
 ## Quick start
 
-Clone this repo, then change to the directory you just cloned (the one containing setup.py) and do 
+Install via pip
 
-`pip install .`
+`pip install bofire-converters`
 
-Here is an example of converting a `Problem` object from [mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
+Here is an example of converting a `Problem` object from [Mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
 
 ```python
-from domainconverters.opti_to_domain import convert_problem
+from bofire_converters.opti_to_domain import convert_problem
 from opti.problems.multi import Daechert1
 
 # Use one of the opti built-in problems as an example
 my_opti_problem = Daechert1()                    
 my_bofire_domain = convert_problem(my_opti_problem)
 ```
```

### Comparing `bofire_converters-0.0.1/bofire_converters/opti_to_domain.py` & `bofire_converters-0.0.2/bofire_converters/opti_to_domain.py`

 * *Files identical despite different names*

### Comparing `bofire_converters-0.0.1/bofire_converters.egg-info/PKG-INFO` & `bofire_converters-0.0.2/bofire_converters.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bofire-converters
-Version: 0.0.1
+Version: 0.0.2
 License: BSD 3-Clause License
         
         Copyright (c) 2023, experimental-design
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -40,25 +40,25 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Mopti Problem to Bofire Domain Converter
 
-These tools are to help with migration of legacy applications from other Mopti to BoFire, and improve quality-of-life.
+These tools are to help with migration of legacy applications from [Mopti](https://github.com/basf/mopti) to [BoFire](https://github.com/experimental-design/bofire). Mopti is for defining optimization problems (inputs, outputs, constraints, ...) and has some sampling utilities. If you have a _problem_ defined in the Mopti format, `bofire_converters` can help you to create the corresponding BoFire object, which is called a _domain_.
 
 ## Quick start
 
-Clone this repo, then change to the directory you just cloned (the one containing setup.py) and do 
+Install via pip
 
-`pip install .`
+`pip install bofire-converters`
 
-Here is an example of converting a `Problem` object from [mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
+Here is an example of converting a `Problem` object from [Mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
 
 ```python
-from domainconverters.opti_to_domain import convert_problem
+from bofire_converters.opti_to_domain import convert_problem
 from opti.problems.multi import Daechert1
 
 # Use one of the opti built-in problems as an example
 my_opti_problem = Daechert1()                    
 my_bofire_domain = convert_problem(my_opti_problem)
 ```
```

### Comparing `bofire_converters-0.0.1/pyproject.toml` & `bofire_converters-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 select = ["B", "C", "E", "F", "W", "I"]
 
 [tool.ruff.mccabe]
 max-complexity = 18
 
 [project]
 name = "bofire_converters"
-version = "0.0.1"
+version = "0.0.2"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = ["Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: BSD License",
         "Topic :: Scientific/Engineering",
```

### Comparing `bofire_converters-0.0.1/test/test_opti_to_domain.py` & `bofire_converters-0.0.2/test/test_opti_to_domain.py`

 * *Files identical despite different names*

