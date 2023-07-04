# Comparing `tmp/MechanicalSoup-1.2.0.tar.gz` & `tmp/MechanicalSoup-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MechanicalSoup-1.2.0.tar", last modified: Sat Sep 17 20:00:52 2022, max compression
+gzip compressed data, was "MechanicalSoup-1.3.0.tar", last modified: Tue Jul  4 19:22:00 2023, max compression
```

## Comparing `MechanicalSoup-1.2.0.tar` & `MechanicalSoup-1.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 20:00:52.733233 MechanicalSoup-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 20:00:52.729232 MechanicalSoup-1.2.0/MechanicalSoup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-09-17 20:00:52.000000 MechanicalSoup-1.2.0/MechanicalSoup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-09-17 20:00:52.000000 MechanicalSoup-1.2.0/MechanicalSoup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-17 20:00:52.000000 MechanicalSoup-1.2.0/MechanicalSoup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-17 20:00:52.000000 MechanicalSoup-1.2.0/MechanicalSoup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-17 20:00:52.000000 MechanicalSoup-1.2.0/MechanicalSoup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-09-17 20:00:52.733233 MechanicalSoup-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 20:00:52.729232 MechanicalSoup-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    13058 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/ChangeLog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7003 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8282 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/external-resources.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8647 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6475 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/mechanicalsoup.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 20:00:52.729232 MechanicalSoup-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/examples/example_manual.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 20:00:52.729232 MechanicalSoup-1.2.0/mechanicalsoup/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/mechanicalsoup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/mechanicalsoup/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14822 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/mechanicalsoup/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)    15502 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/mechanicalsoup/form.py
--rw-r--r--   0 runner    (1001) docker     (121)    16833 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/mechanicalsoup/stateful_browser.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/mechanicalsoup/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-17 20:00:52.733233 MechanicalSoup-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-17 20:00:52.733233 MechanicalSoup-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/setpath.py
--rw-r--r--   0 runner    (1001) docker     (121)    11998 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19685 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (121)    29385 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/test_stateful_browser.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-09-17 20:00:43.000000 MechanicalSoup-1.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 19:22:00.731923 MechanicalSoup-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 19:22:00.727923 MechanicalSoup-1.3.0/MechanicalSoup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5951 2023-07-04 19:22:00.000000 MechanicalSoup-1.3.0/MechanicalSoup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-07-04 19:22:00.000000 MechanicalSoup-1.3.0/MechanicalSoup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 19:22:00.000000 MechanicalSoup-1.3.0/MechanicalSoup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-04 19:22:00.000000 MechanicalSoup-1.3.0/MechanicalSoup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-04 19:22:00.000000 MechanicalSoup-1.3.0/MechanicalSoup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5951 2023-07-04 19:22:00.731923 MechanicalSoup-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4736 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 19:22:00.727923 MechanicalSoup-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)    13948 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/ChangeLog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     8282 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/external-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8647 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6475 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/mechanicalsoup.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8519 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 19:22:00.727923 MechanicalSoup-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/examples/example_manual.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 19:22:00.731923 MechanicalSoup-1.3.0/mechanicalsoup/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/mechanicalsoup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/mechanicalsoup/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14987 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/mechanicalsoup/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16470 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/mechanicalsoup/form.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17065 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/mechanicalsoup/stateful_browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/mechanicalsoup/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-04 19:22:00.731923 MechanicalSoup-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 19:22:00.731923 MechanicalSoup-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/setpath.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19685 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31783 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/test_stateful_browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-07-04 19:21:51.000000 MechanicalSoup-1.3.0/tests/utils.py
```

### Comparing `MechanicalSoup-1.2.0/LICENSE` & `MechanicalSoup-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/MechanicalSoup.egg-info/PKG-INFO` & `MechanicalSoup-1.3.0/MechanicalSoup.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: MechanicalSoup
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python library for automating interaction with websites
 Home-page: https://mechanicalsoup.readthedocs.io/
 License: MIT
 Project-URL: Source, https://github.com/MechanicalSoup/MechanicalSoup
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/MechanicalSoup/MechanicalSoup/main/assets/mechanical-soup-logo.png
    :alt: MechanicalSoup. A Python library for automating website interaction.
 
@@ -118,19 +119,18 @@
 For an example with a more complex form (checkboxes, radio buttons and
 textareas), read `tests/test_browser.py <https://github.com/MechanicalSoup/MechanicalSoup/blob/main/tests/test_browser.py>`__
 and `tests/test_form.py <https://github.com/MechanicalSoup/MechanicalSoup/blob/main/tests/test_form.py>`__.
 
 Development
 -----------
 
-|Build Status| |Coverage Status|
-|Requirements Status| |Documentation Status|
+|Build Status|
+|Coverage Status|
+|Documentation Status|
 |CII Best Practices|
-|LGTM Alerts|
-|LGTM Grade|
 
 Instructions for building, testing and contributing to MechanicalSoup:
 see `CONTRIBUTING.rst <https://github.com/MechanicalSoup/MechanicalSoup/blob/main/CONTRIBUTING.rst>`__.
 
 Common problems
 ---------------
 
@@ -141,19 +141,13 @@
    :target: https://pypi.python.org/pypi/MechanicalSoup/
 .. |Supported Versions| image:: https://img.shields.io/pypi/pyversions/mechanicalsoup.svg
    :target: https://pypi.python.org/pypi/MechanicalSoup/
 .. |Build Status| image:: https://github.com/MechanicalSoup/MechanicalSoup/actions/workflows/python-package.yml/badge.svg?branch=main
    :target: https://github.com/MechanicalSoup/MechanicalSoup/actions/workflows/python-package.yml?query=branch%3Amain
 .. |Coverage Status| image:: https://codecov.io/gh/MechanicalSoup/MechanicalSoup/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/MechanicalSoup/MechanicalSoup
-.. |Requirements Status| image:: https://requires.io/github/MechanicalSoup/MechanicalSoup/requirements.svg?branch=main
-   :target: https://requires.io/github/MechanicalSoup/MechanicalSoup/requirements/?branch=main
 .. |Documentation Status| image:: https://readthedocs.org/projects/mechanicalsoup/badge/?version=latest
    :target: https://mechanicalsoup.readthedocs.io/en/latest/?badge=latest
 .. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/1334/badge
    :target: https://bestpractices.coreinfrastructure.org/projects/1334
 .. |Gitter Chat| image:: https://badges.gitter.im/MechanicalSoup/MechanicalSoup.svg
    :target: https://gitter.im/MechanicalSoup/Lobby
-.. |LGTM Alerts| image:: https://img.shields.io/lgtm/alerts/g/MechanicalSoup/MechanicalSoup.svg
-   :target: https://lgtm.com/projects/g/MechanicalSoup/MechanicalSoup/
-.. |LGTM Grade| image:: https://img.shields.io/lgtm/grade/python/g/MechanicalSoup/MechanicalSoup.svg
-   :target: https://lgtm.com/projects/g/MechanicalSoup/MechanicalSoup/
```

### Comparing `MechanicalSoup-1.2.0/MechanicalSoup.egg-info/SOURCES.txt` & `MechanicalSoup-1.3.0/MechanicalSoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/PKG-INFO` & `MechanicalSoup-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: MechanicalSoup
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python library for automating interaction with websites
 Home-page: https://mechanicalsoup.readthedocs.io/
 License: MIT
 Project-URL: Source, https://github.com/MechanicalSoup/MechanicalSoup
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/MechanicalSoup/MechanicalSoup/main/assets/mechanical-soup-logo.png
    :alt: MechanicalSoup. A Python library for automating website interaction.
 
@@ -118,19 +119,18 @@
 For an example with a more complex form (checkboxes, radio buttons and
 textareas), read `tests/test_browser.py <https://github.com/MechanicalSoup/MechanicalSoup/blob/main/tests/test_browser.py>`__
 and `tests/test_form.py <https://github.com/MechanicalSoup/MechanicalSoup/blob/main/tests/test_form.py>`__.
 
 Development
 -----------
 
-|Build Status| |Coverage Status|
-|Requirements Status| |Documentation Status|
+|Build Status|
+|Coverage Status|
+|Documentation Status|
 |CII Best Practices|
-|LGTM Alerts|
-|LGTM Grade|
 
 Instructions for building, testing and contributing to MechanicalSoup:
 see `CONTRIBUTING.rst <https://github.com/MechanicalSoup/MechanicalSoup/blob/main/CONTRIBUTING.rst>`__.
 
 Common problems
 ---------------
 
@@ -141,19 +141,13 @@
    :target: https://pypi.python.org/pypi/MechanicalSoup/
 .. |Supported Versions| image:: https://img.shields.io/pypi/pyversions/mechanicalsoup.svg
    :target: https://pypi.python.org/pypi/MechanicalSoup/
 .. |Build Status| image:: https://github.com/MechanicalSoup/MechanicalSoup/actions/workflows/python-package.yml/badge.svg?branch=main
    :target: https://github.com/MechanicalSoup/MechanicalSoup/actions/workflows/python-package.yml?query=branch%3Amain
 .. |Coverage Status| image:: https://codecov.io/gh/MechanicalSoup/MechanicalSoup/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/MechanicalSoup/MechanicalSoup
-.. |Requirements Status| image:: https://requires.io/github/MechanicalSoup/MechanicalSoup/requirements.svg?branch=main
-   :target: https://requires.io/github/MechanicalSoup/MechanicalSoup/requirements/?branch=main
 .. |Documentation Status| image:: https://readthedocs.org/projects/mechanicalsoup/badge/?version=latest
    :target: https://mechanicalsoup.readthedocs.io/en/latest/?badge=latest
 .. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/1334/badge
    :target: https://bestpractices.coreinfrastructure.org/projects/1334
 .. |Gitter Chat| image:: https://badges.gitter.im/MechanicalSoup/MechanicalSoup.svg
    :target: https://gitter.im/MechanicalSoup/Lobby
-.. |LGTM Alerts| image:: https://img.shields.io/lgtm/alerts/g/MechanicalSoup/MechanicalSoup.svg
-   :target: https://lgtm.com/projects/g/MechanicalSoup/MechanicalSoup/
-.. |LGTM Grade| image:: https://img.shields.io/lgtm/grade/python/g/MechanicalSoup/MechanicalSoup.svg
-   :target: https://lgtm.com/projects/g/MechanicalSoup/MechanicalSoup/
```

### Comparing `MechanicalSoup-1.2.0/docs/ChangeLog.rst` & `MechanicalSoup-1.3.0/docs/ChangeLog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,41 @@
 =============
 Release Notes
 =============
 
+Version 1.3
+===========
+
+Breaking changes
+----------------
+
+* To prevent malicious web servers from reading arbitrary files from the
+  client, files must now be opened explicitly by the user in order to
+  upload their contents in form submission. For example, instead of:
+
+    browser["upload"] = "/path/to/file"
+
+  you would now use:
+
+    browser["upload"] = open("/path/to/file", "rb")
+
+  This remediates
+  `CVE-2023-34457 <https://github.com/MechanicalSoup/MechanicalSoup/security/advisories/GHSA-x456-3ccm-m6j4>`__.
+  Our thanks to @e-c-d for reporting and helping to fix the vulnerability!
+
+Main changes
+------------
+
+* Added support for Python 3.11.
+
+* Allow submitting a form with no submit element. This can be achieved by
+  passing ``submit=False`` to ``StatefulBrowser.submit_selected``. Thanks
+  @alexreg!
+  [`#480 <https://github.com/MechanicalSoup/MechanicalSoup/pull/411`__]
+
 Version 1.2
 ===========
 
 Main changes
 ------------
 
 * Added support for Python 3.10.
```

### Comparing `MechanicalSoup-1.2.0/docs/Makefile` & `MechanicalSoup-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/conf.py` & `MechanicalSoup-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/external-resources.rst` & `MechanicalSoup-1.3.0/docs/external-resources.rst`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/faq.rst` & `MechanicalSoup-1.3.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/index.rst` & `MechanicalSoup-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/introduction.rst` & `MechanicalSoup-1.3.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/make.bat` & `MechanicalSoup-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/mechanicalsoup.rst` & `MechanicalSoup-1.3.0/docs/mechanicalsoup.rst`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/docs/tutorial.rst` & `MechanicalSoup-1.3.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/examples/example.py` & `MechanicalSoup-1.3.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/examples/example_manual.py` & `MechanicalSoup-1.3.0/examples/example_manual.py`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/mechanicalsoup/browser.py` & `MechanicalSoup-1.3.0/mechanicalsoup/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import io
 import os
 import tempfile
 import urllib
 import weakref
 import webbrowser
 
 import bs4
 import bs4.dammit
 import requests
 
 from .__version__ import __title__, __version__
 from .form import Form
-from .utils import LinkNotFoundError
+from .utils import LinkNotFoundError, is_multipart_file_upload
 
 
 class Browser:
     """Builds a low-level Browser.
 
     It is recommended to use :class:`StatefulBrowser` for most applications,
     since it offers more advanced features and conveniences than Browser.
@@ -224,26 +225,28 @@
                     value = tag.get("value", "on")
                 else:
                     # browsers use empty string for inputs with missing values
                     value = tag.get("value", "")
 
                 # If the enctype is not multipart, the filename is put in
                 # the form as a text input and the file is not sent.
-                if tag.get("type", "").lower() == "file" and multipart:
-                    filepath = value
-                    if filepath != "" and isinstance(filepath, str):
-                        content = open(filepath, "rb")
+                if is_multipart_file_upload(form, tag):
+                    if isinstance(value, io.IOBase):
+                        content = value
+                        filename = os.path.basename(getattr(value, "name", ""))
                     else:
                         content = ""
-                    filename = os.path.basename(filepath)
-                    # If value is the empty string, we still pass it
+                        filename = os.path.basename(value)
+                    # If content is the empty string, we still pass it
                     # for consistency with browsers (see
                     # https://github.com/MechanicalSoup/MechanicalSoup/issues/250).
                     files[name] = (filename, content)
                 else:
+                    if isinstance(value, io.IOBase):
+                        value = os.path.basename(getattr(value, "name", ""))
                     data.append((name, value))
 
             elif tag.name == "button":
                 if tag.get("type", "").lower() in ("button", "reset"):
                     continue
                 else:
                     data.append((name, tag.get("value", "")))
```

### Comparing `MechanicalSoup-1.2.0/mechanicalsoup/form.py` & `MechanicalSoup-1.3.0/mechanicalsoup/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
+import io
 import warnings
 
 from bs4 import BeautifulSoup
 
-from .utils import LinkNotFoundError
+from .utils import LinkNotFoundError, is_multipart_file_upload
 
 
 class InvalidFormMethod(LinkNotFoundError):
     """This exception is raised when a method of :class:`Form` is used
     for an HTML element that is of the wrong type (or is malformed).
     It is caught within :func:`Form.set` to perform element type deduction.
 
@@ -64,14 +65,15 @@
         give it the value ``password``.
         """
 
         for (name, value) in data.items():
             i = self.form.find("input", {"name": name})
             if not i:
                 raise InvalidFormMethod("No input field named " + name)
+            self._assert_valid_file_upload(i, value)
             i["value"] = value
 
     def uncheck_all(self, name):
         """Remove the *checked*-attribute of all input elements with
         a *name*-attribute given by ``name``.
         """
         for option in self.form.find_all("input", {"name": name}):
@@ -257,20 +259,20 @@
         .. code-block:: python
 
             form.set("login", username)
             form.set("password", password)
             form.set("eula-checkbox", True)
 
         Example: uploading a file through a ``<input type="file"
-        name="tagname">`` field (provide the path to the local file,
+        name="tagname">`` field (provide an open file object,
         and its content will be uploaded):
 
         .. code-block:: python
 
-            form.set("tagname", path_to_local_file)
+            form.set("tagname", open(path_to_local_file, "rb"))
 
         """
         for func in ("checkbox", "radio", "input", "textarea", "select"):
             try:
                 getattr(self, "set_" + func)({name: value})
                 return
             except InvalidFormMethod:
@@ -296,23 +298,26 @@
         # included in Python to avoid having dependency issue.
         control = BeautifulSoup("", "html.parser").new_tag('input')
         control['type'] = type
         control['name'] = name
         control['value'] = value
         for k, v in kwargs.items():
             control[k] = v
+        self._assert_valid_file_upload(control, value)
         self.form.append(control)
         return control
 
     def choose_submit(self, submit):
         """Selects the input (or button) element to use for form submission.
 
-        :param submit: The bs4.element.Tag (or just its *name*-attribute) that
-            identifies the submit element to use. If ``None``, will choose the
-            first valid submit element in the form, if one exists.
+        :param submit: The :class:`bs4.element.Tag` (or just its
+            *name*-attribute) that identifies the submit element to use. If
+            ``None``, will choose the first valid submit element in the form,
+            if one exists. If ``False``, will not use any submit element;
+            this is useful for simulating AJAX requests, for example.
 
         To simulate a normal web browser, only one submit element must be
         sent. Therefore, this does not need to be called if there is only
         one submit element in the form.
 
         If the element is not found or if multiple elements match, raise a
         :class:`LinkNotFoundError` exception.
@@ -357,15 +362,15 @@
                     del inp['name']
                 found = True
             else:
                 # Delete any non-matching element's name so that it will be
                 # omitted from the submitted form data.
                 del inp['name']
 
-        if not found and submit is not None:
+        if not found and submit is not None and submit is not False:
             raise LinkNotFoundError(
                 f"Specified submit element not found: {submit}"
             )
         self._submit_chosen = True
 
     def print_summary(self):
         """Print a summary of the form.
@@ -377,7 +382,21 @@
             input_copy = copy.copy(input)
             # Text between the opening tag and the closing tag often
             # contains a lot of spaces that we don't want here.
             for subtag in input_copy.find_all() + [input_copy]:
                 if subtag.string:
                     subtag.string = subtag.string.strip()
             print(input_copy)
+
+    def _assert_valid_file_upload(self, tag, value):
+        """Raise an exception if a multipart file input is not an open file."""
+        if (
+            is_multipart_file_upload(self.form, tag) and
+            not isinstance(value, io.IOBase)
+        ):
+            raise ValueError(
+                "From v1.3.0 onwards, you must pass an open file object "
+                'directly, e.g. `form["name"] = open("/path/to/file", "rb")`. '
+                "This change is to remediate a security vulnerability where "
+                "a malicious web server could read arbitrary files from the "
+                "client (CVE-2023-34457)."
+            )
```

### Comparing `MechanicalSoup-1.2.0/mechanicalsoup/stateful_browser.py` & `MechanicalSoup-1.3.0/mechanicalsoup/stateful_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,20 +264,25 @@
 
     def submit_selected(self, btnName=None, update_state=True,
                         **kwargs):
         """Submit the form that was selected with :func:`select_form`.
 
         :return: Forwarded from :func:`Browser.submit`.
 
-        If there are multiple submit input/button elements, passes ``btnName``
-        to :func:`Form.choose_submit` on the current form to choose between
-        them. If `update_state` is False, form will be submitted but the
-        browser state will remain unchanged. This is useful for forms that
-        result in a download of a file. All other arguments are forwarded to
-        :func:`Browser.submit`.
+        :param btnName: Passed to :func:`Form.choose_submit` to choose the
+            element of the current form to use for submission. If ``None``,
+            will choose the first valid submit element in the form, if one
+            exists. If ``False``, will not use any submit element; this is
+            useful for simulating AJAX requests, for example.
+
+        :param update_state: If False, the form will be submitted but the
+            browser state will remain unchanged; this is useful for forms that
+            result in a download of a file, for example.
+
+        All other arguments are forwarded to :func:`Browser.submit`.
         """
         self.form.choose_submit(btnName)
 
         kwargs = self._merge_referer(**kwargs)
         resp = self.submit(self.__state.form, url=self.__state.url,
                            **kwargs)
         if update_state:
```

### Comparing `MechanicalSoup-1.2.0/mechanicalsoup/utils.py` & `MechanicalSoup-1.3.0/mechanicalsoup/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,7 +10,14 @@
       error is triggered while browsing.
 
     * The user tried to fill-in a field which doesn't exist in a form
       (e.g. browser["name"] = "val" with browser being a
       StatefulBrowser).
     """
     pass
+
+
+def is_multipart_file_upload(form, tag):
+    return (
+        form.get("enctype", "") == "multipart/form-data" and
+        tag.get("type", "").lower() == "file"
+    )
```

### Comparing `MechanicalSoup-1.2.0/setup.py` & `MechanicalSoup-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from os import path
 
 from setuptools import setup  # Always prefer setuptools over distutils
 
 
 def requirements_from_file(filename):
     """Parses a pip requirements file into a list."""
-    return [line.strip() for line in open(filename, 'r')
-            if line.strip() and not line.strip().startswith('--')]
+    with open(filename, 'r') as fd:
+        return [line.strip() for line in fd
+                if line.strip() and not line.strip().startswith('--')]
 
 
 def read(fname, URL, URLImage):
     """Read the content of a file."""
-    readme = open(path.join(path.dirname(__file__), fname)).read()
+    with open(path.join(path.dirname(__file__), fname)) as fd:
+        readme = fd.read()
     if hasattr(readme, 'decode'):
         # In Python 3, turn bytes into str.
         readme = readme.decode('utf8')
     # turn relative links into absolute ones
     readme = re.sub(r'`<([^>]*)>`__',
                     r'`\1 <' + URL + r"/blob/main/\1>`__",
                     readme)
@@ -27,16 +29,16 @@
     return readme
 
 
 here = path.abspath(path.dirname(__file__))
 
 about = {}
 with open(path.join(here, 'mechanicalsoup', '__version__.py'),
-          'r', 'utf-8') as f:
-    exec(f.read(), about)
+          'r', 'utf-8') as fd:
+    exec(fd.read(), about)
 
 # Don't install pytest-runner on every setup.py run, just for tests.
 # See https://pypi.org/project/pytest-runner/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
@@ -64,14 +66,15 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
 
     packages=['mechanicalsoup'],
 
     # List run-time dependencies here. These will be installed by pip
     # when your project is installed. For an analysis of
```

### Comparing `MechanicalSoup-1.2.0/tests/test_browser.py` & `MechanicalSoup-1.3.0/tests/test_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,17 @@
         os.close(pic_filedescriptor)
         if valid_enctype:
             # Correct encoding => send the content
             expected_content = file_content
         else:
             # Encoding doesn't allow sending the content, we expect
             # the filename as a normal text field.
-            expected_content = pic_path.encode()
-        form.find("input", {"name": "pic"})["value"] = pic_path
+            expected_content = os.path.basename(pic_path.encode())
+        tag = form.find("input", {"name": "pic"})
+        tag["value"] = open(pic_path, "rb")
 
     browser = mechanicalsoup.Browser()
     response = browser._request(form)
 
     if enctype not in valid_enctypes_file_submit:
         expected_enctype = default_enctype
     else:
@@ -258,15 +259,15 @@
     resp = browser.get(httpbin + "/nosuchpage")
     assert resp.status_code == 404
 
 
 def test_404(httpbin):
     browser = mechanicalsoup.Browser(raise_on_404=True)
     with pytest.raises(mechanicalsoup.LinkNotFoundError):
-        resp = browser.get(httpbin + "/nosuchpage")
+        browser.get(httpbin + "/nosuchpage")
     resp = browser.get(httpbin.url)
     assert resp.status_code == 200
 
 
 def test_set_cookiejar(httpbin):
     """Set cookies locally and test that they are received remotely."""
     # construct a phony cookiejar and attach it to the session
```

### Comparing `MechanicalSoup-1.2.0/tests/test_form.py` & `MechanicalSoup-1.3.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `MechanicalSoup-1.2.0/tests/test_stateful_browser.py` & `MechanicalSoup-1.3.0/tests/test_stateful_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     resp = browser.open(httpbin + "/nosuchpage")
     assert resp.status_code == 404
 
 
 def test_404(httpbin):
     browser = mechanicalsoup.StatefulBrowser(raise_on_404=True)
     with pytest.raises(mechanicalsoup.LinkNotFoundError):
-        resp = browser.open(httpbin + "/nosuchpage")
+        browser.open(httpbin + "/nosuchpage")
     resp = browser.open(httpbin.url)
     assert resp.status_code == 200
 
 
 def test_user_agent(httpbin):
     browser = mechanicalsoup.StatefulBrowser(user_agent='007')
     resp = browser.open(httpbin + "/user-agent")
@@ -166,14 +166,39 @@
     browser['comment'] = dict(expected_post)['comment']
     initial_state = browser._StatefulBrowser__state
     res = browser.submit_selected(btnName=expected_post[2][0])
     assert res.status_code == 200 and res.text == 'Success!'
     assert initial_state != browser._StatefulBrowser__state
 
 
+@pytest.mark.parametrize("expected_post", [
+    pytest.param(
+        [
+            ('text', 'Setting some text!'),
+            ('comment', 'Selecting an input submit'),
+        ], id='input'),
+    pytest.param(
+        [
+            ('text', '= Heading =\n\nNew page here!\n'),
+            ('comment', 'Selecting a button submit'),
+        ], id='button'),
+])
+def test_submit_no_btn(expected_post):
+    '''Tests that no submit inputs are posted when btnName=False.'''
+    browser, url = setup_mock_browser(expected_post=expected_post)
+    browser.open(url)
+    browser.select_form('#choose-submit-form')
+    browser['text'] = dict(expected_post)['text']
+    browser['comment'] = dict(expected_post)['comment']
+    initial_state = browser._StatefulBrowser__state
+    res = browser.submit_selected(btnName=False)
+    assert res.status_code == 200 and res.text == 'Success!'
+    assert initial_state != browser._StatefulBrowser__state
+
+
 def test_submit_dont_modify_kwargs():
     """Test that submit_selected() doesn't modify the caller's passed-in
     kwargs, for example when adding a Referer header.
     """
     kwargs = {'headers': {'Content-Type': 'text/html'}}
     saved_kwargs = copy.deepcopy(kwargs)
 
@@ -362,40 +387,85 @@
     browser.select_form('#choose-submit-form')
     response = browser.submit_selected()
     assert response.status_code == 200 and response.text == 'Success!'
 
 
 def test_upload_file(httpbin):
     browser = mechanicalsoup.StatefulBrowser()
-    browser.open(httpbin + "/forms/post")
+    url = httpbin + "/post"
+    file_input_form = f"""
+    <form method="post" action="{url}" enctype="multipart/form-data">
+        <input type="file" name="first" />
+    </form>
+    """
 
     # Create two temporary files to upload
     def make_file(content):
         path = tempfile.mkstemp()[1]
-        with open(path, "w") as f:
-            f.write(content)
+        with open(path, "w") as fd:
+            fd.write(content)
         return path
-    path1, path2 = (make_file(content) for content in
-                    ("first file content", "second file content"))
+    path1 = make_file("first file content")
+    path2 = make_file("second file content")
 
-    # The form doesn't have a type=file field, but the target action
-    # does show it => add the fields ourselves, and add enctype too.
+    value1 = open(path1, "rb")
+    value2 = open(path2, "rb")
+
+    browser.open_fake_page(file_input_form)
     browser.select_form()
-    browser._StatefulBrowser__state.form.form[
-      "enctype"] = "multipart/form-data"
-    browser.new_control("file", "first", path1)
-    browser.new_control("file", "second", "")
-    browser["second"] = path2
-    browser.form.print_summary()
+
+    # Test filling an existing input and creating a new input
+    browser["first"] = value1
+    browser.new_control("file", "second", value2)
+
     response = browser.submit_selected()
     files = response.json()["files"]
     assert files["first"] == "first file content"
     assert files["second"] == "second file content"
 
 
+def test_upload_file_with_malicious_default(httpbin):
+    """Check for CVE-2023-34457 by setting the form input value directly to a
+    file that the user does not explicitly consent to upload, as a malicious
+    server might do.
+    """
+    browser = mechanicalsoup.StatefulBrowser()
+    sensitive_path = tempfile.mkstemp()[1]
+    with open(sensitive_path, "w") as fd:
+        fd.write("Some sensitive information")
+    url = httpbin + "/post"
+    malicious_html = f"""
+    <form method="post" action="{url}" enctype="multipart/form-data">
+        <input type="file" name="malicious" value="{sensitive_path}" />
+    </form>
+    """
+    browser.open_fake_page(malicious_html)
+    browser.select_form()
+    response = browser.submit_selected()
+    assert response.json()["files"] == {"malicious": ""}
+
+
+def test_upload_file_raise_on_string_input():
+    """Check for use of the file upload API that was modified to remediate
+    CVE-2023-34457. Users must now open files manually to upload them.
+    """
+    browser = mechanicalsoup.StatefulBrowser()
+    file_input_form = """
+    <form enctype="multipart/form-data">
+        <input type="file" name="upload" />
+    </form>
+    """
+    browser.open_fake_page(file_input_form)
+    browser.select_form()
+    with pytest.raises(ValueError, match="CVE-2023-34457"):
+        browser["upload"] = "/path/to/file"
+    with pytest.raises(ValueError, match="CVE-2023-34457"):
+        browser.new_control("file", "upload2", "/path/to/file")
+
+
 def test_with():
     """Test that __enter__/__exit__ properly create/close the browser."""
     with mechanicalsoup.StatefulBrowser() as browser:
         assert browser.session is not None
     assert browser.session is None
 
 
@@ -569,16 +639,16 @@
     browser = mechanicalsoup.StatefulBrowser()
     browser.open_fake_page('<a href="/get">Link</a>', httpbin.url)
     with pytest.raises(ValueError, match="link parameter cannot be .*"):
         browser.follow_link('foo', bs4_kwargs={'url_regex': 'bar'})
 
 
 def file_get_contents(filename):
-    with open(filename, "rb") as f:
-        return f.read()
+    with open(filename, "rb") as fd:
+        return fd.read()
 
 
 def test_download_link(httpbin):
     """Test downloading the contents of a link to file."""
     browser = mechanicalsoup.StatefulBrowser()
     open_legacy_httpbin(browser, httpbin)
     tmpdir = tempfile.mkdtemp()
@@ -668,16 +738,16 @@
 
 def test_download_link_to_existing_file(httpbin):
     """Test downloading the contents of a link to an existing file."""
     browser = mechanicalsoup.StatefulBrowser()
     open_legacy_httpbin(browser, httpbin)
     tmpdir = tempfile.mkdtemp()
     tmpfile = tmpdir + '/existing.png'
-    with open(tmpfile, "w") as f:
-        f.write("initial content")
+    with open(tmpfile, "w") as fd:
+        fd.write("initial content")
     current_url = browser.url
     current_page = browser.page
     response = browser.download_link('image/png', tmpfile)
 
     # Check that the browser state has not changed
     assert browser.url == current_url
     assert browser.page == current_page
@@ -721,16 +791,16 @@
     browser.download_link(file=tmpfile.name, link_text='Link')
 
     # Check that the browser state has not changed
     assert browser.url == current_url
     assert browser.page == current_page
 
     # Check that the file was downloaded
-    with open(tmpfile.name) as f:
-        json_data = json.load(f)
+    with open(tmpfile.name) as fd:
+        json_data = json.load(fd)
     headers = json_data["headers"]
     assert headers["Referer"] == ref
 
 
 def test_refresh_open():
     url = 'mock://example.com'
     initial_page = BeautifulSoup('<p>Fake empty page</p>', 'lxml')
```

### Comparing `MechanicalSoup-1.2.0/tests/utils.py` & `MechanicalSoup-1.3.0/tests/utils.py`

 * *Files identical despite different names*

