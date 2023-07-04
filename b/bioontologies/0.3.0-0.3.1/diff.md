# Comparing `tmp/bioontologies-0.3.0.tar.gz` & `tmp/bioontologies-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioontologies-0.3.0.tar", last modified: Thu Jun 29 10:00:21 2023, max compression
+gzip compressed data, was "bioontologies-0.3.1.tar", last modified: Tue Jul  4 17:51:08 2023, max compression
```

## Comparing `bioontologies-0.3.0.tar` & `bioontologies-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.980429 bioontologies-0.3.0/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-04-28 07:50:12.000000 bioontologies-0.3.0/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      342 2022-04-29 11:08:00.000000 bioontologies-0.3.0/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     8050 2023-06-29 10:00:21.980575 bioontologies-0.3.0/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     6660 2022-04-29 09:27:24.000000 bioontologies-0.3.0/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.956660 bioontologies-0.3.0/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.962445 bioontologies-0.3.0/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      246 2022-04-28 07:50:12.000000 bioontologies-0.3.0/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7050 2023-06-29 10:00:21.000000 bioontologies-0.3.0/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1780 2022-04-28 08:25:25.000000 bioontologies-0.3.0/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      548 2022-04-28 07:50:12.000000 bioontologies-0.3.0/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2022-04-29 12:14:06.000000 bioontologies-0.3.0/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-04-28 07:50:12.000000 bioontologies-0.3.0/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2645 2023-06-29 10:00:21.981571 bioontologies-0.3.0/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.957141 bioontologies-0.3.0/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.969795 bioontologies-0.3.0/src/bioontologies/
--rw-r--r--   0 cthoyt     (501) staff       (20)      383 2023-06-21 09:33:32.000000 bioontologies-0.3.0/src/bioontologies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      330 2022-04-28 07:50:12.000000 bioontologies-0.3.0/src/bioontologies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3192 2023-06-14 12:47:47.000000 bioontologies-0.3.0/src/bioontologies/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      963 2023-06-21 11:30:52.000000 bioontologies-0.3.0/src/bioontologies/constants.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3317 2023-06-26 22:54:32.000000 bioontologies-0.3.0/src/bioontologies/gilda_utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    34494 2023-06-29 09:15:08.000000 bioontologies-0.3.0/src/bioontologies/obograph.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:50:12.000000 bioontologies-0.3.0/src/bioontologies/py.typed
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.974474 bioontologies-0.3.0/src/bioontologies/relations/
--rw-r--r--   0 cthoyt     (501) staff       (20)      189 2023-06-27 10:44:19.000000 bioontologies-0.3.0/src/bioontologies/relations/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5242 2023-06-29 09:22:44.000000 bioontologies-0.3.0/src/bioontologies/relations/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    96122 2023-06-29 08:55:57.000000 bioontologies-0.3.0/src/bioontologies/relations/data.json
--rw-r--r--   0 cthoyt     (501) staff       (20)    15567 2023-06-29 08:50:06.000000 bioontologies-0.3.0/src/bioontologies/robot.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.977536 bioontologies-0.3.0/src/bioontologies/upgrade/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1592 2023-05-16 11:21:41.000000 bioontologies-0.3.0/src/bioontologies/upgrade/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9556 2023-06-27 07:35:18.000000 bioontologies-0.3.0/src/bioontologies/upgrade/data.tsv
--rw-r--r--   0 cthoyt     (501) staff       (20)      814 2022-09-09 14:23:13.000000 bioontologies-0.3.0/src/bioontologies/upgrade/import_debio.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1033 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.972414 bioontologies-0.3.0/src/bioontologies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     8050 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1005 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       57 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:56:41.000000 bioontologies-0.3.0/src/bioontologies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      206 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       14 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.979595 bioontologies-0.3.0/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       63 2022-04-28 07:50:12.000000 bioontologies-0.3.0/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      903 2022-06-06 11:57:54.000000 bioontologies-0.3.0/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      760 2023-06-29 09:16:38.000000 bioontologies-0.3.0/tests/test_relations.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.126181 bioontologies-0.3.1/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-04-28 07:50:12.000000 bioontologies-0.3.1/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      342 2022-04-29 11:08:00.000000 bioontologies-0.3.1/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8051 2023-07-04 17:51:08.126303 bioontologies-0.3.1/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6660 2022-04-29 09:27:24.000000 bioontologies-0.3.1/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.110400 bioontologies-0.3.1/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.115809 bioontologies-0.3.1/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      246 2022-04-28 07:50:12.000000 bioontologies-0.3.1/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7050 2023-07-04 17:51:07.000000 bioontologies-0.3.1/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1780 2022-04-28 08:25:25.000000 bioontologies-0.3.1/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      548 2022-04-28 07:50:12.000000 bioontologies-0.3.1/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2022-04-29 12:14:06.000000 bioontologies-0.3.1/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-07-02 15:57:52.000000 bioontologies-0.3.1/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2650 2023-07-04 17:51:08.127240 bioontologies-0.3.1/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.110903 bioontologies-0.3.1/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.119338 bioontologies-0.3.1/src/bioontologies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      383 2023-06-21 09:33:32.000000 bioontologies-0.3.1/src/bioontologies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      330 2022-04-28 07:50:12.000000 bioontologies-0.3.1/src/bioontologies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3192 2023-06-14 12:47:47.000000 bioontologies-0.3.1/src/bioontologies/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      963 2023-06-21 11:30:52.000000 bioontologies-0.3.1/src/bioontologies/constants.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3317 2023-06-26 22:54:32.000000 bioontologies-0.3.1/src/bioontologies/gilda_utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    34503 2023-07-04 17:50:25.000000 bioontologies-0.3.1/src/bioontologies/obograph.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:50:12.000000 bioontologies-0.3.1/src/bioontologies/py.typed
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.122830 bioontologies-0.3.1/src/bioontologies/relations/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      189 2023-06-27 10:44:19.000000 bioontologies-0.3.1/src/bioontologies/relations/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5242 2023-06-29 09:22:44.000000 bioontologies-0.3.1/src/bioontologies/relations/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    96122 2023-06-29 08:55:57.000000 bioontologies-0.3.1/src/bioontologies/relations/data.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)    15567 2023-06-29 08:50:06.000000 bioontologies-0.3.1/src/bioontologies/robot.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.124936 bioontologies-0.3.1/src/bioontologies/upgrade/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1592 2023-05-16 11:21:41.000000 bioontologies-0.3.1/src/bioontologies/upgrade/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9556 2023-06-27 07:35:18.000000 bioontologies-0.3.1/src/bioontologies/upgrade/data.tsv
+-rw-r--r--   0 cthoyt     (501) staff       (20)      814 2022-09-09 14:23:13.000000 bioontologies-0.3.1/src/bioontologies/upgrade/import_debio.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1033 2023-07-04 17:51:07.000000 bioontologies-0.3.1/src/bioontologies/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.121711 bioontologies-0.3.1/src/bioontologies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8051 2023-07-04 17:51:08.000000 bioontologies-0.3.1/src/bioontologies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1005 2023-07-04 17:51:08.000000 bioontologies-0.3.1/src/bioontologies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-07-04 17:51:08.000000 bioontologies-0.3.1/src/bioontologies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       57 2023-07-04 17:51:08.000000 bioontologies-0.3.1/src/bioontologies.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:56:41.000000 bioontologies-0.3.1/src/bioontologies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      210 2023-07-04 17:51:08.000000 bioontologies-0.3.1/src/bioontologies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       14 2023-07-04 17:51:08.000000 bioontologies-0.3.1/src/bioontologies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-04 17:51:08.125916 bioontologies-0.3.1/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       63 2022-04-28 07:50:12.000000 bioontologies-0.3.1/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      903 2022-06-06 11:57:54.000000 bioontologies-0.3.1/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      760 2023-06-29 09:16:38.000000 bioontologies-0.3.1/tests/test_relations.py
```

### Comparing `bioontologies-0.3.0/LICENSE` & `bioontologies-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/PKG-INFO` & `bioontologies-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioontologies
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tools for biomedical ontologies.
 Home-page: https://github.com/biopragmatics/bioontologies
 Download-URL: https://github.com/biopragmatics/bioontologies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -17,20 +17,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 <!--
 <p align="center">
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: bioontologies Version: 0.3.0 Summary: Tools for
+Metadata-Version: 2.1 Name: bioontologies Version: 0.3.1 Summary: Tools for
 biomedical ontologies. Home-page: https://github.com/biopragmatics/
 bioontologies Download-URL: https://github.com/biopragmatics/bioontologies/
 releases Author: Charles Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer:
 Charles Tapley Hoyt Maintainer-email: cthoyt@gmail.com License: MIT Project-
 URL: Bug Tracker, https://github.com/biopragmatics/bioontologies/issues
 Project-URL: Source Code, https://github.com/biopragmatics/bioontologies
 Keywords: snekpack,cookiecutter,ontologies,OBO Foundry,knowledge
 graphs,biomedicine,biology,systems biology,networks biology Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests Provides-Extra: docs License-File: LICENSE
                           ****** Bioontologies ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                             [Contributor_Covenant]
 Tools for biomedical ontologies. ## ðª Getting Started This package lets you
 get OBO Graphs from ontologies based on their OWL files, OBO files, or
```

### Comparing `bioontologies-0.3.0/README.md` & `bioontologies-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/docs/source/conf.py` & `bioontologies-0.3.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "bioontologies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.3.0"
+release = "0.3.1"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `bioontologies-0.3.0/docs/source/index.rst` & `bioontologies-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/docs/source/installation.rst` & `bioontologies-0.3.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/setup.cfg` & `bioontologies-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bioontologies
-version = 0.3.0
+version = 0.3.1
 description = Tools for biomedical ontologies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/bioontologies
 download_url = https://github.com/biopragmatics/bioontologies/releases
 project_urls = 
 	Bug Tracker = https://github.com/biopragmatics/bioontologies/issues
@@ -21,18 +21,18 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Framework :: Pytest
 	Framework :: tox
 	Framework :: Sphinx
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 keywords = 
 	snekpack
 	cookiecutter
 	ontologies
 	OBO Foundry
 	knowledge graphs
@@ -42,21 +42,21 @@
 	networks biology
 
 [options]
 install_requires = 
 	bioregistry>=0.6.13
 	curies>=0.5.5
 	requests
-	pydantic
+	pydantic<2.0
 	typing_extensions
 	pystow
 	pandas
 zip_safe = false
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
```

### Comparing `bioontologies-0.3.0/src/bioontologies/cli.py` & `bioontologies-0.3.1/src/bioontologies/cli.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/constants.py` & `bioontologies-0.3.1/src/bioontologies/constants.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/gilda_utils.py` & `bioontologies-0.3.1/src/bioontologies/gilda_utils.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/obograph.py` & `bioontologies-0.3.1/src/bioontologies/obograph.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,19 +98,20 @@
         if self.xrefs_raw:
             self.references = _get_references(self.xrefs_raw)
         if self.value:
             self.value = self.value.strip().replace("  ", " ").replace("\n", " ")
         self.standardized = True
         return self
 
-    def from_parsed(self, value: str, references: Optional[List[Reference]] = None) -> "Definition":
+    @classmethod
+    def from_parsed(cls, value: str, references: Optional[List[Reference]] = None) -> "Definition":
         """Construct a definition object from pre-standardized content."""
         if not references:
             references = []
-        return Definition(
+        return cls(
             value=value,
             xrefs_raw=[r.curie for r in references],
             references=references,
             standardize=True,
         )
```

### Comparing `bioontologies-0.3.0/src/bioontologies/relations/api.py` & `bioontologies-0.3.1/src/bioontologies/relations/api.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/relations/data.json` & `bioontologies-0.3.1/src/bioontologies/relations/data.json`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/robot.py` & `bioontologies-0.3.1/src/bioontologies/robot.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/upgrade/__init__.py` & `bioontologies-0.3.1/src/bioontologies/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/upgrade/data.tsv` & `bioontologies-0.3.1/src/bioontologies/upgrade/data.tsv`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/upgrade/import_debio.py` & `bioontologies-0.3.1/src/bioontologies/upgrade/import_debio.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/src/bioontologies/version.py` & `bioontologies-0.3.1/src/bioontologies/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`bioontologies` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `bioontologies-0.3.0/src/bioontologies.egg-info/PKG-INFO` & `bioontologies-0.3.1/src/bioontologies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioontologies
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tools for biomedical ontologies.
 Home-page: https://github.com/biopragmatics/bioontologies
 Download-URL: https://github.com/biopragmatics/bioontologies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -17,20 +17,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 <!--
 <p align="center">
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: bioontologies Version: 0.3.0 Summary: Tools for
+Metadata-Version: 2.1 Name: bioontologies Version: 0.3.1 Summary: Tools for
 biomedical ontologies. Home-page: https://github.com/biopragmatics/
 bioontologies Download-URL: https://github.com/biopragmatics/bioontologies/
 releases Author: Charles Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer:
 Charles Tapley Hoyt Maintainer-email: cthoyt@gmail.com License: MIT Project-
 URL: Bug Tracker, https://github.com/biopragmatics/bioontologies/issues
 Project-URL: Source Code, https://github.com/biopragmatics/bioontologies
 Keywords: snekpack,cookiecutter,ontologies,OBO Foundry,knowledge
 graphs,biomedicine,biology,systems biology,networks biology Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
 Extra: tests Provides-Extra: docs License-File: LICENSE
                           ****** Bioontologies ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                             [Contributor_Covenant]
 Tools for biomedical ontologies. ## ðª Getting Started This package lets you
 get OBO Graphs from ontologies based on their OWL files, OBO files, or
```

### Comparing `bioontologies-0.3.0/src/bioontologies.egg-info/SOURCES.txt` & `bioontologies-0.3.1/src/bioontologies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/tests/test_api.py` & `bioontologies-0.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.3.0/tests/test_relations.py` & `bioontologies-0.3.1/tests/test_relations.py`

 * *Files identical despite different names*

