# Comparing `tmp/survey-4.4.0.tar.gz` & `tmp/survey-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.4.0.tar", last modified: Sun Jun 11 09:46:59 2023, max compression
+gzip compressed data, was "survey-4.5.0.tar", last modified: Tue Jul  4 17:38:00 2023, max compression
```

## Comparing `survey-4.4.0.tar` & `survey-4.5.0.tar`

### file list

```diff
@@ -1,46 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.835433 survey-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-11 09:46:50.000000 survey-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-11 09:46:59.835433 survey-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-11 09:46:50.000000 survey-4.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:46:59.835433 survey-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-11 09:46:50.000000 survey-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.831433 survey-4.4.0/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-11 09:46:50.000000 survey-4.4.0/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.835433 survey-4.4.0/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30590 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    59339 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.831433 survey-4.4.0/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.243526 survey-4.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.231525 survey-4.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.231525 survey-4.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-04 17:37:48.000000 survey-4.5.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-04 17:37:48.000000 survey-4.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 17:37:48.000000 survey-4.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 17:37:48.000000 survey-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-04 17:38:00.243526 survey-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 17:37:48.000000 survey-4.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.235525 survey-4.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-04 17:37:48.000000 survey-4.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.231525 survey-4.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.239526 survey-4.5.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/graphics.lineprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/graphics.spinprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/printers.done-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/printers.fail-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/printers.info-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.basket-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.basket-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.conceal-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.datetime-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.datetime-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.form-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.input-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.input-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.inquire-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.numeric-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.numeric-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.select-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/routines.select-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/showcase-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-04 17:37:48.000000 survey-4.5.0/docs/_static/images/showcase-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-04 17:37:48.000000 survey-4.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 17:37:48.000000 survey-4.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 17:37:48.000000 survey-4.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 17:37:48.000000 survey-4.5.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:38:00.243526 survey-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-04 17:37:48.000000 survey-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.239526 survey-4.5.0/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-04 17:37:48.000000 survey-4.5.0/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.243526 survey-4.5.0/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58115 2023-07-04 17:37:48.000000 survey-4.5.0/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:38:00.243526 survey-4.5.0/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-04 17:38:00.000000 survey-4.5.0/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-04 17:38:00.000000 survey-4.5.0/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:38:00.000000 survey-4.5.0/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 17:38:00.000000 survey-4.5.0/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 17:38:00.000000 survey-4.5.0/survey.egg-info/top_level.txt
```

### Comparing `survey-4.4.0/LICENSE` & `survey-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/PKG-INFO` & `survey-4.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.4.0
+Version: 4.5.0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
 
 ✨ A simple library for creating beautiful interactive prompts.
 
 .. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
```

### Comparing `survey-4.4.0/README.rst` & `survey-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/__init__.py` & `survey-4.5.0/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_colors.py` & `survey-4.5.0/survey/_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 def _color_bit8_info_get(layer, part):
 
     args = _color_bit8_info[layer]
 
     return _get(*args, part)
 
 
-def standard(part: str, /, layer: str = _color_default_layer) -> str:
+def standard(part: str, layer: str = _color_default_layer) -> str:
 
     """
     Get a standard ansi color by value (`8 bit docs <https://en.wikipedia.org/wiki/ANSI_escape_code#8-bit>`_).
 
     :param part:
         The color in ``[0, 255]`` range.
     :param layer:
@@ -203,15 +203,15 @@
 def _color_bit24_get(layer, part_r, part_g, part_b):
 
     args = _color_bit24_info[layer]
 
     return _get(*args, part_r, part_g, part_b)
 
 
-def full(part_r: int, part_g: int, part_b: int, /, layer: str = _color_default_layer) -> str:
+def full(part_r: int, part_g: int, part_b: int, layer: str = _color_default_layer) -> str:
 
     """
     Get a full rgb ansi color by the respective values (`224 bit docs <https://en.wikipedia.org/wiki/ANSI_escape_code#24-bit>`_).
 
     :param part_r:
         The red component.
     :param part_g:
```

### Comparing `survey-4.4.0/survey/_controls.py` & `survey-4.5.0/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/__init__.py` & `survey-4.5.0/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_ansi.py` & `survey-4.5.0/survey/_core/_ansi.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         if bits == _BITS_ESCAPE:
             return _parse_escape(get)
         return Control(rune)
 
     return Text(rune)
 
 
-_type_parse_return: typing.TypeAlias = Text | Escape | Control | Sequence
+_type_parse_return = typing.Union[Text, Escape, Control, Sequence]
 
 
 def parse(get: typing.Callable[[], str]) -> _type_parse_return:
 
     """
     Parse an incoming series of characters into their ANSI representation.
```

### Comparing `survey-4.4.0/survey/_core/_console.py` & `survey-4.5.0/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_cursor.py` & `survey-4.5.0/survey/_core/_cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,60 +98,60 @@
 
         self._io.send(value)
 
     def _up(self, size):
 
         self._send('A', size)
 
-    def up(self, size: int | None = None):
+    def up(self, size: typing.Union[int, None] = None):
 
         """
         Move up. No effect if at the edge of the screen.
 
         :param size:
             The amount of lines to move by. System default  is usually :code:`1`.
         """
 
         self._up(size)
 
     def _down(self, size):
 
         self._send('B', size)
 
-    def down(self, size: int | None = None):
+    def down(self, size: typing.Union[int, None] = None):
 
         """
         Move down. No effect if at the edge of the screen.
 
         :param size:
             The amount of lines to move by. System default  is usually :code:`1`.
         """
 
         self._down(size)
 
     def _left(self, size):
 
         self._send('D', size)
 
-    def left(self, size: int | None = None):
+    def left(self, size: typing.Union[int, None] = None):
 
         """
         Move left. No effect if at the edge of the screen.
 
         :param size:
             The amount of lines to move by. System default  is usually :code:`1`.
         """
 
         self._left(size)
 
     def _right(self, size):
 
         self._send('C', size)
 
-    def right(self, size: int | None = None):
+    def right(self, size: typing.Union[int, None] = None):
 
         """
         Move right. No effect if at the edge of the screen.
 
         :param size:
             The amount of lines to move by. System default  is usually :code:`1`.
         """
@@ -173,45 +173,45 @@
 
         self._goto(x)
 
     def _last(self, size):
 
         self._send('F', size)
 
-    def last(self, size: int | None = None):
+    def last(self, size: typing.Union[int, None] = None):
 
         """
         Move up at line start.
 
         :param size:
             The amount of lines to move by. System default  is usually :code:`1`.
         """
 
         self._last(size)
 
     def _next(self, size):
 
         self._send('E', size)
 
-    def next(self, size: int | None = None):
+    def next(self, size: typing.Union[int, None] = None):
 
         """
         Move down at line start.
 
         :param size:
             The amount of lines to move by. System default  is usually :code:`1`.
         """
 
         self._next(size)
 
     def _move(self, y, x):
 
         self._send('f', y, x)
 
-    def move(self, y: int | None = None, x: int | None = None):
+    def move(self, y: typing.Union[int, None] = None, x: typing.Union[int, None] = None):
 
         """
         Move absolutely on screen.
 
         :param y:
             The absolute vertical coordinate to move to. System default  is usually :code:`1`.
         :param x:
@@ -310,15 +310,15 @@
                 continue
             break
 
         point = tuple(map(int, code.args))
 
         return point
 
-    def locate(self) -> tuple[int, int]:
+    def locate(self) -> typing.Tuple[int, int]:
 
         """
         Get the current absolute vertical and horizontal coordinates.
 
         :returns:
             ``(vertical, horizontal)``
         """
@@ -338,15 +338,15 @@
 
         point = self._locate()
 
         self._load()
 
         return point
 
-    def measure(self) -> tuple[int, int]:
+    def measure(self) -> typing.Tuple[int, int]:
 
         """
         Get the maximum possible vertical and horizontal coordinates.
 
         :returns:
             ``(vertical, horizontal)``
         """
```

### Comparing `survey-4.4.0/survey/_core/_handle.py` & `survey-4.5.0/survey/_core/_handle.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Terminate(Exception):
 
     """
     Signals the invokation loop to stop.
     """
 
 
-_type_Handle_start_invoke: typing.TypeAlias = typing.Callable[[str, _ansi._type_parse_return], None]
+_type_Handle_start_invoke = typing.Callable[[str, _ansi._type_parse_return], None]
 
     
 class Handle:
 
     """
     Encapsulates the invokation loop logic.
     """
```

### Comparing `survey-4.4.0/survey/_core/_helpers.py` & `survey-4.5.0/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_io.py` & `survey-4.5.0/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_io_os.py` & `survey-4.5.0/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_io_os_nt.py` & `survey-4.5.0/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_io_os_posix.py` & `survey-4.5.0/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_core/_render.py` & `survey-4.5.0/survey/_core/_render.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         _get_line_wrap_y(5, 33) # 7
     """
 
     return math.floor(size / limit) + 1
 
 
 def _get_line_wrap_y_sum(limit: int, 
-                         sizes: list[int]):
+                         sizes: typing.List[int]):
 
     """
     Get the amount of y-space needed to render a list of lines in a given x-space.
 
     :param limit:
         The x-space limit.
     :param size:
@@ -56,15 +56,15 @@
 
     get = functools.partial(_get_line_wrap_y, limit)
 
     return sum(map(get, sizes))
 
 
 def _get_point_wrap(limit: int, 
-                    sizes: list[int], 
+                    sizes: typing.List[int], 
                     cur_y: int, 
                     cur_x: int):
 
     """
     Get the (y, x) in a list of lines after accounting for a given x-space.
     """
 
@@ -85,16 +85,16 @@
 
     def __init__(self, y, x):
 
         self.y = y
         self.x = x
     
 
-_type_Render_draw_lines: typing.TypeAlias = list[list[str]]
-_type_Render_draw_point: typing.TypeAlias = list[int, int] | None
+_type_Render_draw_lines = typing.List[typing.List[str]]
+_type_Render_draw_point = typing.Union[typing.List[int], None]
 
 
 class Render:
 
     """
     Assists with printing text in a predictible way.
 
@@ -225,15 +225,14 @@
         if not point is None:
             # "memory" from loop above
             self._move(sizes, memory.y, memory.x, max_x, point)
 
     def draw(self, 
              lines: _type_Render_draw_lines,
              point: _type_Render_draw_point = None,
-             /,
              *,
              clean: bool = True,
              learn: bool = True):
 
         """
         Draw lines and place the cursor among them.
 
@@ -247,15 +246,17 @@
             Whether to keep track of the initial cursor position.
         """
 
         self._draw(learn, clean, lines, point)
 
     def _back(self):
 
-        if (memory := self._memory) is None:
+        memory = self._memory
+
+        if memory is None:
             return
         
         self._cursor.move(memory.y, memory.x)
 
         self._memory = None
 
     def back(self):
```

### Comparing `survey-4.4.0/survey/_core/_screen.py` & `survey-4.5.0/survey/_core/_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import _cursor
 from . import _render
 
 
 __all__ = ('Screen',)
 
 
-_type_Screen_draw_sketch: typing.TypeAlias = typing.Callable[[], tuple[_render._type_Render_draw_lines, _render._type_Render_draw_point]]
+_type_Screen_draw_sketch = typing.Callable[[], typing.Tuple[_render._type_Render_draw_lines, _render._type_Render_draw_point]]
 
 
 class Screen:
 
     """
     Encapsulates the visualization logic.
```

### Comparing `survey-4.4.0/survey/_core/_source.py` & `survey-4.5.0/survey/_core/_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 class _EmptyRead(Exception):
 
     __slots__ = ()
 
 
-_type_Source_init_callback: typing.TypeAlias = typing.Callable[[Event, _ansi._type_parse_return], None]
+_type_Source_init_callback = typing.Callable[[Event, _ansi._type_parse_return], None]
 
 
 class Source:
 
     """
     Translates incoming ANSI sequences to events and calls back with relevant information.
```

### Comparing `survey-4.4.0/survey/_funnels.py` & `survey-4.5.0/survey/_funnels.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     sizes = get()
 
     for (function, size) in zip(functions, sizes):
         function(size, lines, point)
 
 
 @_call_direct
-def text_max_dynamic(get: typing.Callable[[], tuple[int, int]]):
+def text_max_dynamic(get: typing.Callable[[], typing.Tuple[int, int]]):
     
     """
     A combination of :func:`.text_max_horizontal` and :func:`.text_max_vertical`.
     
     :param get:
         Should return an iterable with each function's size on their axis index.
     """
@@ -532,16 +532,16 @@
         args = [*tile]
         if aware:
             args.insert(0, spot)
         function(*args)
 
 
 @_call_direct
-def mesh_delegate(function: typing.Callable[[list[list[str]], list[int, int]], None], 
-                  check   : typing.Callable[[tuple[int, int], list[list[list[str]]], list[int, int]], bool] = None, 
+def mesh_delegate(function: typing.Callable[[typing.List[typing.List[str]], typing.List[int]], None], 
+                  check   : typing.Callable[[typing.Tuple[int, int], typing.List[typing.List[typing.List[str]]], typing.List[int]], bool] = None, 
                   aware   : bool = False):
     
     """
     Call a function on each tile of the mesh.
 
     :param function:
         The function called.
@@ -620,16 +620,16 @@
         color = colors[current]
         _text_paint(color, *tile)
     
     _mesh_focal(function, tiles, point)
 
 
 @_call_direct
-def mesh_light(focus_color: str | None = None,
-               evade_color: str | None = None):
+def mesh_light(focus_color: typing.Union[str, None] = None,
+               evade_color: typing.Union[str, None] = None):
     
     """
     Paint the mesh's tiles depending on whether they are pointed.
 
     :param focus_color:
         The color used for the pointed tile.
     :param evade_color:
@@ -757,15 +757,15 @@
             tiles[spot] = (lines, [0, 0])
 
 
 @_call_direct
 def mesh_min(axis: int, 
              size: int, 
              just: JustType = JustType.start, 
-             fill: typing.Callable[[tuple[int, int]], list[list[str]]] = lambda spot: [[]]):
+             fill: typing.Callable[[typing.Tuple[int, int]], typing.List[typing.List[str]]] = lambda spot: [[]]):
     
     """
     Ensure there is most of a certain amount of tiles along an certain axis, aligned accordingly by ``fill``\ing with new tiles.
 
     :param axis:
         The axis considered for the operation.
     :param size:
@@ -929,15 +929,15 @@
         yield get('top_right')
     else:
         yield ' '
 
 
 def _mesh_grid(runes, runes_color, tiles, point, **mesh_grid_fill_kwargs):
 
-    @functools.cache
+    @functools.lru_cache()
     def get_rune(name):
         rune = runes[name]
         if not runes_color is None:
             rune =_helpers.paint_rune(runes_color, rune)
         return rune
 
     spots = set(tiles)
@@ -980,15 +980,15 @@
                 old_line.append(new_line[0])
         else:
             continue
         del tiles[spot]
         
 
 @_call_direct
-def mesh_grid(runes: dict[str, str] = {
+def mesh_grid(runes: typing.Dict[str, str] = {
                 'horizontal': '─',
                 'vertical': '│',
                 'cross': '┼',
                 'cross_top': '┬',
                 'cross_bottom': '┴',
                 'cross_left': '├',
                 'cross_right': '┤',
@@ -1061,16 +1061,16 @@
         spot[axis] = cur_a
         spot = tuple(spot)
         tiles[spot] = tile
 
 
 @_call_direct
 def mesh_head(axis: int, 
-              get : typing.Callable[[int], list[list[str]]], 
-              just: JustType | None = None,
+              get : typing.Callable[[int], typing.List[typing.List[str]]], 
+              just: typing.Union[JustType, None] = None,
               skip: int = 0, 
               min : int = 0):
     
     """
     Add headers to the mesh.
     
     :param axis:
```

### Comparing `survey-4.4.0/survey/_graphics.py` & `survey-4.5.0/survey/_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     _top_point = (0, 0)
     _cur_count = 0
 
     def __init__(self, 
                  inline   : bool = False, 
                  throttle : float = 0.1,
-                 epilogue : str | typing.Callable[[], str] | None = None):
+                 epilogue : typing.Union[str, typing.Callable[[], str], None] = None):
 
         self._inline = inline
 
         self._throttle = throttle
         self._time_last = 0
 
         self._epilogue = epilogue
@@ -72,15 +72,16 @@
     @property
     def _final(self):
 
         return self._cur_point == self._top_point
 
     def _sketch(self, close):
 
-        if close and not (value := self._epilogue) is None:
+        value = self._epilogue
+        if close and not value is None:
             if callable(value):
                 value = value()
         else:
             value = self._get()
 
         lines = _helpers.split_lines(value)
         point = None
@@ -275,15 +276,15 @@
 
     .. image:: /_static/images/graphics.spinprogress-1.gif
     """
 
     @_theme.add('graphics.SpinProgress')
     def __init__(self, 
                  *args,
-                 phases: list[str] = ('.', 'o', 'O', '@', '*'),
+                 phases: typing.List[str] = ('.', 'o', 'O', '@', '*'),
                  prefix: str       = ' ',
                  suffix: str       = '',
                  **kwargs):
 
         self._prefix = prefix
         self._suffix = suffix
 
@@ -358,15 +359,15 @@
     """
 
     @_theme.add('graphics.LineProgress')
     def __init__(self, 
                  total                 : int, 
                  *args,
                  width                 : int       = 50,
-                 phases                : list[str] = ('-',), 
+                 phases                : typing.List[str] = ('-',), 
                  empty                 : str       = ' ',
                  prefix_wall           : str       = '[', 
                  suffix_wall           : str       = ']',
                  prefix                : str       = '',
                  suffix                : str       = '',
                  percentage_zfill_value: str       = '0',
                  percentage_zfill_color: str       = _colors.basic('black'),
@@ -411,26 +412,30 @@
 
         super()._set(step)
 
     def _get(self):
 
         size_limit = self._cursor.measure()[1]
         size_limit -= self._cursor.locate()[1]
-        
-        if not (size_given := self._width) is None:
+
+        size_given = self._width
+
+        if not size_given is None:
             size_limit = min(size_given, size_limit)
 
         size_ratio = min(self._total, self._cycle_actual) / self._total
 
         percentage = ''
-        if not (percentage_template := self._percentage_template) is None:
+        percentage_template = self._percentage_template
+        if not percentage is None:
             percentage_value = str(math.ceil(size_ratio * 100))
             percentage_zfill_count = self._percentage_zfill_count - len(percentage_value)
             percentage_zfill_value = self._percentage_zfill_value * percentage_zfill_count
-            if not (percentage_zfill_color := self._percentage_zfill_color) is None:
+            percentage_zfill_color = self._percentage_zfill_color
+            if not percentage_zfill_color is None:
                 percentage_zfill_value = _helpers.paint_text(percentage_zfill_color, percentage_zfill_value)
             percentage_value = percentage_zfill_value + percentage_value
             percentage = percentage_template.format(value = percentage_value)
             percentage = percentage + ' '
 
         full_size_limit = size_limit
         full_size_ratio = size_ratio
@@ -442,27 +447,29 @@
         half_size_precise = half_size_limit * half_size_ratio
         half_size = math.floor(half_size_precise)
         half_index = half_size % half_size_limit
 
         add_size = full_size_limit - full_size
 
         throughput = ''
-        if not (throughput_template := self._throughput_template) is None:
+        throughput_template = self._throughput_template
+        if not throughput_template is None:
             try:
                 throughput_times, throughput_steps = zip(*self._throughput_deque)
                 throughput_period = max(throughput_times) - min(throughput_times)
                 throughput_amount = sum(throughput_steps)
                 throughput_ratio = throughput_amount / throughput_period
             except (ValueError, ZeroDivisionError):
                 throughput_value = ''
             else:
                 throughput_value = str(math.ceil(throughput_ratio * 100))
             throughput_zfill_count = self._throughput_zfill_count - len(throughput_value)
             throughput_zfill_value = self._throughput_zfill_value * throughput_zfill_count
-            if not (throughput_zfill_color := self._throughput_zfill_color) is None:
+            throughput_zfill_color = self._throughput_zfill_color
+            if not throughput_zfill_color is None:
                 throughput_zfill_value = _helpers.paint_text(throughput_zfill_color, throughput_zfill_value)
             throughput_value = throughput_zfill_value + throughput_value
             throughput = throughput_template.format(value = throughput_value)
             throughput = ' ' + throughput
 
         line = (
               self._prefix
```

### Comparing `survey-4.4.0/survey/_handle.py` & `survey-4.5.0/survey/_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     """
     Can be raised during a callback with :attr:`EventType.enter` to prevent invokation.
     """
 
     __slots__ = ()
 
 
-_type_Handle_init_unsafe  : typing.TypeAlias = bool
-_type_Handle_init_callback: typing.TypeAlias = typing.Callable[[tuple[EventType, _core.Event], _core._type_ansi_parse_return], None]
+_type_Handle_init_unsafe   = bool
+_type_Handle_init_callback = typing.Callable[[typing.Tuple[EventType, _core.Event], _core._type_ansi_parse_return], None]
 
-_type_Handle_add_control  : typing.TypeAlias = _controls.Control
+_type_Handle_add_control   = _controls.Control
 
-_type_Handle_invoke_event : typing.TypeAlias = _core.Event
+_type_Handle_invoke_event  = _core.Event
 
 
 class Handle:
 
     """
     Used for holding and calling "control" functions that determine action for each :class:`._core.Event`.
```

### Comparing `survey-4.4.0/survey/_helpers.py` & `survey-4.5.0/survey/_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,16 +79,15 @@
         if not radius in map(abs, (i, j)):
             continue
         yield (origin[0] + i, origin[1] + j)
 
 
 def get_point_distance_to_point(origin, target):
 
-    return math.dist(origin, target)
-
+    return math.sqrt(sum((px - qx) ** 2.0 for px, qx in zip(origin, target)))
 
 def get_point_distance_to_line(slope, intercept, target):
 
     return abs(-slope * target[1] + target[0] - intercept) / math.hypot(slope, 1)
 
 
 def get_point_direction_to_point(origin, target):
@@ -399,48 +398,52 @@
     point = [default] * dimensions
     
     point[axis] = index
 
     return point
 
 
-@functools.cache
+@functools.lru_cache()
 def get_function_parameters(function):
 
     if isinstance(function, type):
         functions = function.__mro__
     else:
         functions = ()
 
     signatures = reversed(tuple(map(inspect.signature, functions)))
 
     ignore_kinds = {inspect.Parameter.VAR_POSITIONAL, inspect.Parameter.VAR_KEYWORD}
 
-    parameters = functools.reduce(operator.or_, (signature.parameters for signature in signatures))
+    parameters = {}
+    for signature in signatures:
+        parameters.update(signature.parameters)
 
     parameters = {name: parameter for (name, parameter) in parameters.items() if not parameter.kind in ignore_kinds}
 
     return parameters
 
 
-@functools.cache
+@functools.lru_cache()
 def get_function_args_names(function):
 
     parameters = get_function_parameters(function)
 
     return tuple(parameters)
 
 
 def get_function_args_default(function, name):
 
     parameters = get_function_parameters(function)
 
     parameter = parameters[name]
 
-    if (default := parameter.default) is inspect.Parameter.empty:
+    default = parameter.default
+
+    if default is inspect.Parameter.empty:
         raise ValueError(f'parameter "{name}" of {function} has no default')
 
     return default
 
 
 def get_function_arg_safe(function, name, store, pop = False):
```

### Comparing `survey-4.4.0/survey/_mutates.py` & `survey-4.5.0/survey/_mutates.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         """
         Restore the current state to the one provided.
         """
 
         return self._set_state(state)
     
 
-_type_cursor_point: typing.TypeAlias = list[int]
+_type_cursor_point = typing.List[int]
     
 
 class Cursor(Mutate):
 
     """
     A mutate for a point representing a position in space.
 
@@ -98,29 +98,29 @@
     
     def _move(self, instructions):
 
         for (axis, coordinate) in instructions:
             self._point[axis] = coordinate
 
     def move(self, 
-             instructions: list[tuple[int, int]]) -> None:
+             instructions: typing.List[typing.Tuple[int, int]]) -> None:
 
         """
         Move according to the instructions given. 
         
         Each instruction should be of ``(index, new_coordinate)`` form.
         """
 
         self._move(instructions)
 
 
-_type_Text_init_rune : typing.TypeAlias = str
-_type_Text_init_line : typing.TypeAlias = list[_type_Text_init_rune]
-_type_Text_init_lines: typing.TypeAlias = list[_type_Text_init_line]
-_type_Text_init_point: typing.TypeAlias = _type_cursor_point
+_type_Text_init_rune  = str
+_type_Text_init_line  = typing.List[_type_Text_init_rune]
+_type_Text_init_lines = typing.List[_type_Text_init_line]
+_type_Text_init_point = _type_cursor_point
 
 
 class Text(Mutate):
 
     """
     A mutate for a block of text and a cursor among it.
 
@@ -188,15 +188,15 @@
         cur_lines = self._lines
         
         cur_line = cur_lines[cur_y]
 
         cur_line[cur_x:cur_x] = runes
 
     def insert(self, 
-               runes: list[str]):
+               runes: typing.List[str]):
 
         """
         Insert text at the current cursor position and move it accordingly.
 
         :param runes:
             The runes to insert.
         """
@@ -338,23 +338,23 @@
         """
         Insert a new line under the cursor, cutting the current one as necessary.
         """
 
         self._newline()
 
 
-_type_Mesh_init_clean : typing.TypeAlias = None | int
-_type_Mesh_init_spot  : typing.TypeAlias =        tuple[int, int]
-_type_Mesh_init_tile  : typing.TypeAlias =        typing.Any
-_type_Mesh_init_tiles : typing.TypeAlias =        dict[_type_Mesh_init_spot, _type_Mesh_init_tile]
-_type_Mesh_init_point : typing.TypeAlias =        _type_cursor_point
-_type_Mesh_init_score : typing.TypeAlias = None | typing.Callable[[_type_Text_init_lines, _type_Mesh_init_tile], int | None]
-_type_Mesh_init_scout : typing.TypeAlias = None | typing.Callable[[_type_Mesh_init_spot], bool]
-_type_Mesh_init_rigid : typing.TypeAlias =        bool
-_type_Mesh_init_create: typing.TypeAlias = None | typing.Callable[[_type_Mesh_init_spot], _type_Mesh_init_tile | None]
+_type_Mesh_init_clean  = typing.Union[None, int]
+_type_Mesh_init_spot   = typing.Tuple[int, int]
+_type_Mesh_init_tile   = typing.Any
+_type_Mesh_init_tiles  = typing.Dict[_type_Mesh_init_spot, _type_Mesh_init_tile]
+_type_Mesh_init_point  = _type_cursor_point
+_type_Mesh_init_score  = typing.Union[None, typing.Callable[[_type_Text_init_lines, _type_Mesh_init_tile], typing.Union[int, None]]]
+_type_Mesh_init_scout  = typing.Union[None, typing.Callable[[_type_Mesh_init_spot], bool]]
+_type_Mesh_init_rigid  = bool
+_type_Mesh_init_create = typing.Union[None, typing.Callable[[_type_Mesh_init_spot], typing.Union[_type_Mesh_init_tile, None]]]
 
 
 class Mesh(Mutate):
 
     """
     A mutate for a collection of tiles.
 
@@ -457,15 +457,15 @@
         
         Tile creation is only possible when this is empty.
         """
 
         return self._search_line
     
     @property
-    def vision(self) -> dict[_type_Mesh_init_spot, _type_Mesh_init_spot]:
+    def vision(self) -> typing.Dict[_type_Mesh_init_spot, _type_Mesh_init_spot]:
 
         """
         A mapping of currently visible spots to the real ones they correspond to.
         """
 
         return self._vision
 
@@ -580,15 +580,15 @@
         if not tile is None:
             self._tiles[spot] = tile
             self._vision[spot] = spot
 
         return tile
     
     def insert(self, 
-               spot: _type_Mesh_init_spot) -> _type_Mesh_init_tile | None:
+               spot: _type_Mesh_init_spot) -> typing.Union[_type_Mesh_init_tile, None]:
         
         """
         Attempt to insert a tile.
 
         :param spot:
             The spot to insert the tile at.
 
@@ -611,15 +611,15 @@
             del self._vision[spot]
         except KeyError:
             pass
 
         return tile
 
     def delete(self,
-               spot: _type_Mesh_init_spot) -> _type_Mesh_init_tile | None:
+               spot: _type_Mesh_init_spot) -> typing.Union[_type_Mesh_init_tile, None]:
 
         """
         Attempt to delete a tile
         
         :param spot:
             The spot to delete the tile from.
         
@@ -746,15 +746,15 @@
         self._search_mutate.move_x(size)
 
     def _search_insert(self, runes):
 
         self._search_execute(self._search_insert_act, runes)
 
     def search_insert(self, 
-                      runes: list[str]):
+                      runes: typing.List[str]):
 
         """
         Insert text to the search line, and filter or displace tiles accordingly.
 
         :param runes:
             The runes to insert.
         """
```

### Comparing `survey-4.4.0/survey/_printers.py` & `survey-4.5.0/survey/_printers.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from . import _colors
 from . import _theme
 
 
 __all__ = ('text', 'info', 'done', 'fail')
 
 
-_type_text_sep: typing.TypeAlias = str
-_type_text_end: typing.TypeAlias = str
-_type_text_re : typing.TypeAlias = bool
+_type_text_sep = str
+_type_text_end = str
+_type_text_re  = bool
 
 
 def _text(*values, 
           sep: _type_text_sep = ' ', 
           end: _type_text_end = _constants.linesep, 
           re : _type_text_re  = False):
 
@@ -53,16 +53,16 @@
 
     if not mark_color is None:
         mark = _helpers.paint_text(mark_color, mark)
 
     _text(mark, *values, **kwargs)
 
 
-_type_info_mark      : typing.TypeAlias = str
-_type_info_mark_color: typing.TypeAlias = str
+_type_info_mark       = str
+_type_info_mark_color = str
 
 
 @_theme.add('printers.info')
 def _info(*values,
           mark      : _type_info_mark       = '!', 
           mark_color: _type_info_mark_color = _colors.basic('cyan'),
           **kwargs):
@@ -86,16 +86,16 @@
 
     _annotate(mark_color, mark, values, **kwargs)
 
 
 info = _info
 
 
-_type_done_mark      : typing.TypeAlias = str
-_type_done_mark_color: typing.TypeAlias = str
+_type_done_mark       = str
+_type_done_mark_color = str
 
 
 @_theme.add('printers.done')
 def _done(*values,
           mark      : _type_done_mark       = '!' if os.name == 'nt' else '✔', 
           mark_color: _type_done_mark_color = _colors.basic('green'),
           **kwargs):
@@ -119,16 +119,16 @@
 
     _annotate(mark_color, mark, values, **kwargs)
 
 
 done = _done
 
 
-_type_fail_mark      : typing.TypeAlias = str
-_type_fail_mark_color: typing.TypeAlias = str
+_type_fail_mark       = str
+_type_fail_mark_color = str
 
 
 @_theme.add('printers.fail')
 def _fail(*values,
           mark      : _type_fail_mark       = '!' if os.name == 'nt' else '✘', 
           mark_color: _type_fail_mark_color = _colors.basic('red'),
           **kwargs):
```

### Comparing `survey-4.4.0/survey/_routines.py` & `survey-4.5.0/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_searches.py` & `survey-4.5.0/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_stage.py` & `survey-4.5.0/survey/_stage.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,23 +30,23 @@
             point[0] += 1
         else:
             lines.append([''])
     
     return funnel
 
 
-_type_get_multi_maybe: typing.TypeAlias = bool
-_type_get_multi_force: typing.TypeAlias = bool
-_type_get_site       : typing.TypeAlias = str
-_type_get_info_get   : typing.TypeAlias = _visuals._type_Text_init_get
-_type_get_hint_get   : typing.TypeAlias = _visuals._type_Text_init_get
-_type_get_body_get   : typing.TypeAlias = _visuals._type_Text_init_get
-_type_get_info_color : typing.TypeAlias = str
-_type_get_hint_color : typing.TypeAlias = str
-_type_get_warn_color : typing.TypeAlias = str
+_type_get_multi_maybe = bool
+_type_get_multi_force = bool
+_type_get_site        = str
+_type_get_info_get    = _visuals._type_Text_init_get
+_type_get_hint_get    = _visuals._type_Text_init_get
+_type_get_body_get    = _visuals._type_Text_init_get
+_type_get_info_color  = str
+_type_get_hint_color  = str
+_type_get_warn_color  = str
 
 
 def _get(multi_maybe: _type_get_multi_maybe,
          multi_force: _type_get_multi_force, 
          site       : _type_get_site,
          info_get   : _type_get_info_get,
          hint_get   : _type_get_hint_get,
```

### Comparing `survey-4.4.0/survey/_theme.py` & `survey-4.5.0/survey/_theme.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,12 +67,12 @@
         def wrapper(*args, **kwargs):
             theme = _get()
             try:
                 defaults = theme[name]
             except KeyError:
                 pass
             else:
-                kwargs = defaults | kwargs
+                kwargs = {**defaults, **kwargs}
             return function(*args, **kwargs)
         return wrapper
 
     return decorator
```

### Comparing `survey-4.4.0/survey/_utils.py` & `survey-4.5.0/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.4.0/survey/_visuals.py` & `survey-4.5.0/survey/_visuals.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 from . import _core
 
 
 __all__ = ('Visual', 'Text', 'Mesh', 'Line')
 
 
-_type_Visual_init_get         : typing.TypeAlias = typing.Callable[[bool, bool], tuple[typing.Any]]
-_type_Visual_init_funnel_enter: typing.TypeAlias = typing.Callable[[typing.Any], None] | None
-_type_Visual_init_funnel_leave: typing.TypeAlias = typing.Callable[[_core._type_Render_draw_lines, _core._type_Render_draw_point], None] | None
-
-_type_Visual_get_enter        : typing.TypeAlias = bool
-_type_Visual_get_leave        : typing.TypeAlias = bool
-_type_Visual_get_return       : typing.TypeAlias = tuple[_core._type_Render_draw_lines, _core._type_Render_draw_point] | None
+_type_Visual_init_get          = typing.Callable[[bool, bool], typing.Tuple[typing.Any]]
+_type_Visual_init_funnel_enter = typing.Union[typing.Callable[[typing.Any], None], None]
+_type_Visual_init_funnel_leave = typing.Union[typing.Callable[[_core._type_Render_draw_lines, _core._type_Render_draw_point], None], None]
+
+_type_Visual_get_enter         = bool
+_type_Visual_get_leave         = bool
+_type_Visual_get_return        = typing.Union[typing.Tuple[_core._type_Render_draw_lines, _core._type_Render_draw_point] , None]
 
 
 class Visual(abc.ABC):
 
     """
     Base class for transformers of data into lines and point for rendering.
 
@@ -84,20 +84,20 @@
 
         if leave and not self._funnel_leave is None:
             self._funnel_leave(lines, point)
 
         return (lines, point)
 
 
-_type_Text_link_lines       : typing.TypeAlias = list[list[str]]
-_type_Text_link_point       : typing.TypeAlias = list[int, int]
+_type_Text_link_lines        = typing.List[typing.List[str]]
+_type_Text_link_point        = typing.List[int]
 
-_type_Text_init_get         : typing.TypeAlias = typing.Callable[[bool, bool], tuple[_type_Text_link_lines, _type_Text_link_point]]
-_type_Text_init_funnel_enter: typing.TypeAlias = typing.Callable[[_type_Text_link_lines, _type_Text_link_point], None] | None
-_type_Text_init_funnel_leave: typing.TypeAlias = _type_Visual_init_funnel_leave
+_type_Text_init_get          = typing.Callable[[bool, bool], typing.Tuple[_type_Text_link_lines, _type_Text_link_point]]
+_type_Text_init_funnel_enter = typing.Union[typing.Callable[[_type_Text_link_lines, _type_Text_link_point], None], None]
+_type_Text_init_funnel_leave = _type_Visual_init_funnel_leave
 
 
 class Text(Visual):
 
     """
     Transforms lines and point into... lines and cursor point.
 
@@ -134,20 +134,20 @@
         return cls(get, *args, **kwargs)
 
     def _format(self, lines, point):
 
         return (lines, point)
     
 
-_type_Mesh_link_tiles       : typing.TypeAlias = dict[tuple[int, int], tuple[_type_Text_link_lines, _type_Text_link_point]]
-_type_Mesh_link_point       : typing.TypeAlias = list[int, int]
+_type_Mesh_link_tiles        = typing.Dict[typing.Tuple[int, int], typing.Tuple[_type_Text_link_lines, _type_Text_link_point]]
+_type_Mesh_link_point        = typing.List[int]
 
-_type_Mesh_init_get         : typing.TypeAlias = typing.Callable[[bool, bool], tuple[_type_Mesh_link_tiles, _type_Mesh_link_point]]
-_type_Mesh_init_funnel_enter: typing.TypeAlias = typing.Callable[[_type_Mesh_link_tiles, _type_Mesh_link_point], None] | None
-_type_Mesh_init_funnel_leave: typing.TypeAlias = _type_Visual_init_funnel_leave
+_type_Mesh_init_get          = typing.Callable[[bool, bool], typing.Tuple[_type_Mesh_link_tiles, _type_Mesh_link_point]]
+_type_Mesh_init_funnel_enter = typing.Union[typing.Callable[[_type_Mesh_link_tiles, _type_Mesh_link_point], None], None]
+_type_Mesh_init_funnel_leave = _type_Visual_init_funnel_leave
 
 
 class Mesh(Visual):
 
     """
     Transforms mesh tiles and point into lines and cursor point.
 
@@ -238,20 +238,20 @@
         fin_y = len(done_lines) - fin_y
 
         done_point = [fin_y, fin_x]
 
         return (done_lines, done_point)
 
 
-_type_Line_link_tiles       : typing.TypeAlias = dict[tuple[int, int], tuple[_type_Text_link_lines, _type_Mesh_link_point]]
-_type_Line_link_point       : typing.TypeAlias = list[int]
+_type_Line_link_tiles        = typing.Dict[typing.Tuple[int, int], typing.Tuple[_type_Text_link_lines, _type_Mesh_link_point]]
+_type_Line_link_point        = typing.List[int]
 
-_type_Line_init_get         : typing.TypeAlias = typing.Callable[[bool, bool], tuple[_type_Line_link_tiles, _type_Line_link_point]]
-_type_Line_init_funnel_enter: typing.TypeAlias = typing.Callable[[_type_Line_link_tiles, _type_Line_link_point], None] | None
-_type_Line_init_funnel_leave: typing.TypeAlias = _type_Visual_init_funnel_leave
+_type_Line_init_get          = typing.Callable[[bool, bool], typing.Tuple[_type_Line_link_tiles, _type_Line_link_point]]
+_type_Line_init_funnel_enter = typing.Union[typing.Callable[[_type_Line_link_tiles, _type_Line_link_point], None], None]
+_type_Line_init_funnel_leave = _type_Visual_init_funnel_leave
 
 
 class Line(Visual):
 
     """
     Transforms a list of tiles and point into lines and cursor point.
```

### Comparing `survey-4.4.0/survey/_widgets.py` & `survey-4.5.0/survey/_widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,23 +46,23 @@
     """
     Raised when the users pressed the ``Esc`` button.
     """
 
     __slots__ = ()
 
 
-_type_Widget_init_mutate   : typing.TypeAlias = _mutates.Mutate
-_type_Widget_init_visual   : typing.TypeAlias = _visuals.Visual
-_type_Widget_init_callback : typing.TypeAlias = _handle._type_Handle_init_callback
-_type_Widget_init_delegate : typing.TypeAlias = typing.Callable[[_core.Event], bool]
-_type_Widget_init_validate : typing.TypeAlias = typing.Callable[[typing.Any], None]
-_type_Widget_init_escapable: typing.TypeAlias = bool
+_type_Widget_init_mutate    = _mutates.Mutate
+_type_Widget_init_visual    = _visuals.Visual
+_type_Widget_init_callback  = _handle._type_Handle_init_callback
+_type_Widget_init_delegate  = typing.Callable[[_core.Event], bool]
+_type_Widget_init_validate  = typing.Callable[[typing.Any], None]
+_type_Widget_init_escapable = bool
 
-_type_Widget_invoke_event: typing.TypeAlias = _core.Event
-_type_Widget_invoke_info : typing.TypeAlias = _core._type_ansi_parse_return
+_type_Widget_invoke_event = _core.Event
+_type_Widget_invoke_info  = _core._type_ansi_parse_return
 
 
 class Widget:
 
     """
     A team of mutate, handle and visual working together.
 
@@ -129,25 +129,30 @@
     
     def resolve(self):
 
         """
         Get the resolved value.
         """
 
-        if (result := self._result_c) is self._mark_result_c:
+        result = self._result_c
+        if result is self._mark_result_c:
             result = self._resolve()
 
         return result
     
     def _invoke_validate(self):
 
-        if (validate := self._validate) is None:
+        validate = self._validate
+
+        if validate is None:
             return
 
-        if (result := self._result_c) is self._mark_result_c:
+        result = self._result_c
+
+        if result is self._mark_result_c:
             result = self._result_c = self._resolve()
 
         validate(result)
         
         self._result_c = self._mark_result_c
 
     def _invoke(self, event, *args, **kwargs):
@@ -208,46 +213,46 @@
         point_y = len(lines) - 1
         point_x = len(lines[point_y])
         point = [point_y, point_x]
         value = (lines, point)
     return value
 
 
-_type_start_get_actor_contextual_parse  : typing.TypeAlias = bool
-_type_start_get_actor_contextual_context: typing.TypeAlias = contextvars.ContextVar
+_type_start_get_actor_contextual_parse   = bool
+_type_start_get_actor_contextual_context = contextvars.ContextVar
 
 
 def _start_get_actor_contextual(parse  : _type_start_get_actor_contextual_parse,
                                 context: _type_start_get_actor_contextual_context):
 
     def wrapper(*args, **kwargs):
         value = context.get()
         return _start_variant_parse(parse, value)
     
     return wrapper
 
 
-_type_start_start_get_actor_static_parse: typing.TypeAlias = _type_start_get_actor_contextual_parse
-_type_start_start_get_actor_static_value: typing.TypeAlias = str | list[list[str]]
+_type_start_start_get_actor_static_parse = _type_start_get_actor_contextual_parse
+_type_start_start_get_actor_static_value = typing.Union[str, typing.List[typing.List[str]]]
 
 
 def _start_get_actor_static(parse: _type_start_start_get_actor_static_parse, 
                             value: _type_start_start_get_actor_static_value):
 
     context = contextvars.ContextVar('state')
 
     context.set(value)
 
     wrapper = _start_get_actor_contextual(parse, context)
 
     return wrapper
 
 
-_type_start_start_get_actor_dynamic_parse: typing.TypeAlias = _type_start_get_actor_contextual_parse
-_type_start_start_get_actor_dynamic_fetch: typing.TypeAlias = typing.Callable[[typing.Any], tuple[_visuals._type_Text_link_lines, _visuals._type_Text_link_point]]
+_type_start_start_get_actor_dynamic_parse = _type_start_get_actor_contextual_parse
+_type_start_start_get_actor_dynamic_fetch = typing.Callable[[typing.Any], typing.Tuple[_visuals._type_Text_link_lines, _visuals._type_Text_link_point]]
 
 
 def _start_get_actor_dynamic(parse: _type_start_start_get_actor_dynamic_parse, 
                              fetch: _type_start_start_get_actor_dynamic_fetch):
 
     context = contextvars.ContextVar('state')
 
@@ -255,16 +260,16 @@
         context.set(fetch(*args, **kwargs))
     
     wrapper = _start_get_actor_contextual(parse, context)
 
     return wrapper, updater
 
 
-_type_start_get_actor_dichotomic_parse: typing.TypeAlias = _type_start_get_actor_contextual_parse
-_type_start_get_actor_dichotomic_value: typing.TypeAlias = _type_start_start_get_actor_static_value | _type_start_start_get_actor_dynamic_fetch
+_type_start_get_actor_dichotomic_parse = _type_start_get_actor_contextual_parse
+_type_start_get_actor_dichotomic_value = typing.Union[_type_start_start_get_actor_static_value, _type_start_start_get_actor_dynamic_fetch]
 
 
 def _start_get_actor_dichotomic(parse: _type_start_get_actor_dichotomic_parse, 
                                 value: _type_start_get_actor_dichotomic_value):
 
     if callable(value):
         wrapper, updater = _start_get_actor_dynamic(parse, value)
@@ -273,26 +278,26 @@
         updater = _helpers.noop
 
     return wrapper, updater
 
 
 _start_warn_reset_lines = [[]]
 
-_type_start_multi_pre  =        _stage._type_get_multi_maybe
-_type_start_multi_aft  =        bool
-_type_start_widget     =        Widget
-_type_start_show       = None | str
-_type_start_mark       = None | str
-_type_start_mark_color =        str
-_type_start_info       =        _type_start_get_actor_dichotomic_value
-_type_start_info_parse =        _type_start_get_actor_dichotomic_parse
-_type_start_hint       =        _type_start_get_actor_dichotomic_value
-_type_start_hint_parse =        _type_start_get_actor_dichotomic_parse
-_type_start_site       =        _stage._type_get_site
-_type_start_reply      = None | typing.Callable[[Widget, typing.Any], str]
+_type_start_multi_pre  = _stage._type_get_multi_maybe
+_type_start_multi_aft  = bool
+_type_start_widget     = Widget
+_type_start_show       = typing.Union[None, str]
+_type_start_mark       = typing.Union[None, str]
+_type_start_mark_color = str
+_type_start_info       = _type_start_get_actor_dichotomic_value
+_type_start_info_parse = _type_start_get_actor_dichotomic_parse
+_type_start_hint       = _type_start_get_actor_dichotomic_value
+_type_start_hint_parse = _type_start_get_actor_dichotomic_parse
+_type_start_site       = _stage._type_get_site
+_type_start_reply      = typing.Union[None, typing.Callable[[Widget, typing.Any], str]]
 
 
 def _start(multi_pre : _type_start_multi_pre, 
            multi_aft : _type_start_multi_aft,
            widget    : _type_start_widget, 
            show      : _type_start_show       = None,
            mark      : _type_start_mark       = '? ',
@@ -370,16 +375,17 @@
                 _stage.warn(_start_warn_reset_lines)
                 update(widget, *args, **kwargs)
         except _mutates.Error:
             _system.io.ring()
             raise _core.SkipDraw()
         except Abort as error:
             widget.mutate.set_state(memory)
-            if not (text := error.text) is None:
-                lines = _helpers.split_lines(text)
+            message = error.text
+            if not message is None:
+                lines = _helpers.split_lines(message)
                 _stage.warn(lines)
             _system.io.ring()
 
     update(widget, None, None) # emulate
 
     try:
         _system.console.start(sketch, invoke)
@@ -400,23 +406,23 @@
 
     return result
 
 
 start = _start
 
 
-_type_BaseText_init_lines       : typing.TypeAlias = _mutates._type_Text_init_lines 
-_type_BaseText_init_point       : typing.TypeAlias = _mutates._type_Text_init_point
-_type_BaseText_init_multi       : typing.TypeAlias = bool
-_type_BaseText_init_callback    : typing.TypeAlias = _type_Widget_init_callback
-_type_BaseText_init_delegate    : typing.TypeAlias = _type_Widget_init_delegate
-_type_BaseText_init_validate    : typing.TypeAlias = _type_Widget_init_validate
-_type_BaseText_init_escapable   : typing.TypeAlias = _type_Widget_init_escapable
-_type_BaseText_init_funnel_enter: typing.TypeAlias = _visuals._type_Text_init_funnel_enter
-_type_BaseText_init_funnel_leave: typing.TypeAlias = _visuals._type_Text_init_funnel_leave
+_type_BaseText_init_lines        = _mutates._type_Text_init_lines 
+_type_BaseText_init_point        = _mutates._type_Text_init_point
+_type_BaseText_init_multi        = bool
+_type_BaseText_init_callback     = _type_Widget_init_callback
+_type_BaseText_init_delegate     = _type_Widget_init_delegate
+_type_BaseText_init_validate     = _type_Widget_init_validate
+_type_BaseText_init_escapable    = _type_Widget_init_escapable
+_type_BaseText_init_funnel_enter = _visuals._type_Text_init_funnel_enter
+_type_BaseText_init_funnel_leave = _visuals._type_Text_init_funnel_leave
 
 
 _BaseText_controls = (
     _controls.text_insert,
     _controls.text_move_left,
     _controls.text_move_right,
     _controls.text_move_up,
@@ -486,16 +492,16 @@
             callback = callback,
             delegate = delegate,
             validate = validate,
             escapable = escapable
         )
 
 
-_type_Input_init_value: typing.TypeAlias = str
-_type_Input_init_index: typing.TypeAlias = int
+_type_Input_init_value = str
+_type_Input_init_index = int
 
 
 class Input(BaseText):
 
     """
     A text editor.
 
@@ -540,18 +546,18 @@
     def _resolve(self):
 
         value = _helpers.join_lines(self._mutate.lines)
 
         return value
     
 
-_type_Numeric_init_value                : typing.TypeAlias = int
-_type_Numeric_init_decimal              : typing.TypeAlias = bool
-_type_Numeric_init_zfill                : typing.TypeAlias = int
-_type_Numeric_init_invalid_value_message: typing.TypeAlias = str
+_type_Numeric_init_value                 = int
+_type_Numeric_init_decimal               = bool
+_type_Numeric_init_zfill                 = int
+_type_Numeric_init_invalid_value_message = str
 
 
 class Numeric(Input):
 
     """
     A text editor that only allows submission with numeric values.
 
@@ -642,16 +648,16 @@
             result = f'{result}0'
 
         result = self._transform(self._transform_abort_message, result)
 
         return result
 
 
-_type_Conceal_init_rune : typing.TypeAlias =        str
-_type_Conceal_init_color: typing.TypeAlias = None | int 
+_type_Conceal_init_rune  = str
+_type_Conceal_init_color = typing.Union[None, int]
 
 
 class Conceal(Input):
 
     """
     A text editor that replaces all characters with a rune.
 
@@ -685,18 +691,18 @@
             funnel_leave_entry = _funnels.text_paint(color)
             funnel_leave_group.append(funnel_leave_entry)
         funnel_leave = _helpers.chain_functions(*funnel_leave_group, funnel_leave)
 
         super().__init__(*args, funnel_leave = funnel_leave, **kwargs)
 
 
-_type_AutoSubmit_init_evaluate : typing.TypeAlias =        typing.Callable[[str], None]
-_type_AutoSubmit_init_validate : typing.TypeAlias =        typing.Callable[[str], bool]
-_type_AutoSubmit_init_default  : typing.TypeAlias =        typing.Any
-_type_AutoSubmit_init_transform: typing.TypeAlias = None | typing.Callable[[str], str]
+_type_AutoSubmit_init_evaluate  = typing.Callable[[str], None]
+_type_AutoSubmit_init_validate  = typing.Callable[[str], bool]
+_type_AutoSubmit_init_default   = typing.Any
+_type_AutoSubmit_init_transform = typing.Union[None, typing.Callable[[str], str]]
 
 
 class AutoSubmit(Input):
 
     """
     A text editor that automatically submits a upon valid insertion.
 
@@ -770,16 +776,16 @@
             *args, 
             validate = None,
             callback = callback,
             **kwargs
         )
             
 
-_type_Inquire_init_options : typing.TypeAlias = dict[str: typing.Any]
-_type_Inquire_init_tranform: typing.TypeAlias = _type_AutoSubmit_init_transform
+_type_Inquire_init_options  = typing.Dict[str, typing.Any]
+_type_Inquire_init_tranform = _type_AutoSubmit_init_transform
     
 
 class Inquire(AutoSubmit):
 
     """
     A text editor that submits upon insertion of an option.
 
@@ -858,28 +864,28 @@
 def _get_mesh_spot(*args, **kwargs):
 
     point = _get_mesh_point(*args, **kwargs)
 
     return tuple(point)
 
 
-_type_BaseMesh_init_search      : typing.TypeAlias = _mutates._type_Mesh_init_score
-_type_BaseMesh_init_create      : typing.TypeAlias = _mutates._type_Mesh_init_create
-_type_BaseMesh_init_tiles       : typing.TypeAlias = _mutates._type_Mesh_init_tiles
-_type_BaseMesh_init_point       : typing.TypeAlias = _mutates._type_Mesh_init_point
-_type_BaseMesh_init_clean       : typing.TypeAlias = _mutates._type_Mesh_init_clean
-_type_BaseMesh_init_scout       : typing.TypeAlias = _mutates._type_Mesh_init_scout
-_type_BaseMesh_init_rigid       : typing.TypeAlias = _mutates._type_Mesh_init_rigid
-_type_BaseMesh_init_focus       : typing.TypeAlias = bool | typing.Callable[[_core.Event], bool] 
-_type_BaseMesh_init_callback    : typing.TypeAlias = _type_Widget_init_callback
-_type_BaseMesh_init_delegate    : typing.TypeAlias = _type_Widget_init_delegate
-_type_BaseMesh_init_validate    : typing.TypeAlias = _type_Widget_init_validate
-_type_BaseMesh_init_escapable   : typing.TypeAlias = _type_Widget_init_escapable
-_type_BaseMesh_init_funnel_enter: typing.TypeAlias = _visuals._type_Mesh_init_funnel_enter
-_type_BaseMesh_init_funnel_leave: typing.TypeAlias = _visuals._type_Mesh_init_funnel_leave
+_type_BaseMesh_init_search       = _mutates._type_Mesh_init_score
+_type_BaseMesh_init_create       = _mutates._type_Mesh_init_create
+_type_BaseMesh_init_tiles        = _mutates._type_Mesh_init_tiles
+_type_BaseMesh_init_point        = _mutates._type_Mesh_init_point
+_type_BaseMesh_init_clean        = _mutates._type_Mesh_init_clean
+_type_BaseMesh_init_scout        = _mutates._type_Mesh_init_scout
+_type_BaseMesh_init_rigid        = _mutates._type_Mesh_init_rigid
+_type_BaseMesh_init_focus        = typing.Union[bool, typing.Callable[[_core.Event], bool] ]
+_type_BaseMesh_init_callback     = _type_Widget_init_callback
+_type_BaseMesh_init_delegate     = _type_Widget_init_delegate
+_type_BaseMesh_init_validate     = _type_Widget_init_validate
+_type_BaseMesh_init_escapable    = _type_Widget_init_escapable
+_type_BaseMesh_init_funnel_enter = _visuals._type_Mesh_init_funnel_enter
+_type_BaseMesh_init_funnel_leave = _visuals._type_Mesh_init_funnel_leave
 
 
 _BaseMesh_controls = (
     _controls.mesh_move_left,
     _controls.mesh_move_right,
     _controls.mesh_move_up,
     _controls.mesh_move_down,
@@ -1022,24 +1028,24 @@
             self._invoke_focus(event, *args, **kwargs)
         elif switcher and event is _core.Event.indent:
             self._handle_focus()
         else:
             self._invoke_blear(event, *args, **kwargs)
 
 
-_type_BaseList_init_tiles      : typing.TypeAlias =        list[Widget] | _type_BaseMesh_init_tiles
-_type_BaseList_init_axis       : typing.TypeAlias =        int
-_type_BaseList_init_index      : typing.TypeAlias =        int
-_type_BaseList_init_label      : typing.TypeAlias = None | typing.Callable[[int], str]
-_type_BaseList_init_view_max   : typing.TypeAlias = None | int
-_type_BaseList_init_focus_color: typing.TypeAlias = None | str
-_type_BaseList_init_focus_mark : typing.TypeAlias = None | str
-_type_BaseList_init_evade_color: typing.TypeAlias = None | str
-_type_BaseList_init_evade_mark : typing.TypeAlias = None | str
-_type_BaseList_init_fill       : typing.TypeAlias = bool
+_type_BaseList_init_tiles       = typing.Union[typing.List[Widget], _type_BaseMesh_init_tiles]
+_type_BaseList_init_axis        = int
+_type_BaseList_init_index       = int
+_type_BaseList_init_label       = typing.Union[None, typing.Callable[[int], str]]
+_type_BaseList_init_view_max    = typing.Union[None, int]
+_type_BaseList_init_focus_color = typing.Union[None, str]
+_type_BaseList_init_focus_mark  = typing.Union[None, str]
+_type_BaseList_init_evade_color = typing.Union[None, str]
+_type_BaseList_init_evade_mark  = typing.Union[None, str]
+_type_BaseList_init_fill        = bool
 
 
 _BaseList_controls = (
     _controls.mesh_move_up_reverse,
     _controls.mesh_move_down_reverse,
 )
 
@@ -1169,17 +1175,17 @@
     def _resolve(self):
 
         index = self._mutate.cur_spot[self._axis]
 
         return index
 
 
-_type_Select_init_options: typing.TypeAlias =        list[str]
-_type_Select_init_create : typing.TypeAlias = None | typing.Callable[[_mutates._type_Mesh_init_spot], str]
-_type_Select_init_Option : typing.TypeAlias =        Input
+_type_Select_init_options = typing.List[str]
+_type_Select_init_create  = typing.Union[None, typing.Callable[[_mutates._type_Mesh_init_spot], str]]
+_type_Select_init_Option  = Input
 
 
 class Select(BaseList):
 
     """
     A single-option selector.
 
@@ -1237,20 +1243,20 @@
             tiles = tiles, 
             create = create,
             focus = _focus_nil,
             **kwargs
         )
 
 
-_type_Basket_init_options      : typing.TypeAlias = list[str]
-_type_Basket_init_active       : typing.TypeAlias = list[int]
-_type_Basket_init_positive_mark: typing.TypeAlias = str
-_type_Basket_init_negative_mark: typing.TypeAlias = str
-_type_Basket_init_Option       : typing.TypeAlias = Input
-_type_Basket_init_Stamp        : typing.TypeAlias = Select
+_type_Basket_init_options       = typing.List[str]
+_type_Basket_init_active        = typing.List[int]
+_type_Basket_init_positive_mark = str
+_type_Basket_init_negative_mark = str
+_type_Basket_init_Option        = Input
+_type_Basket_init_Stamp         = Select
 
 
 _Basket_focus_events = {
     _core.Event.arrow_left, _core.Event.arrow_right
 }
 
 _Basket_focus = lambda event: event in _Basket_focus_events
@@ -1391,19 +1397,19 @@
                 continue
             index = spot[self._axis]
             indexes.add(index)
         
         return indexes
 
 
-_type_Count_init_value  : typing.TypeAlias =        int | float
-_type_Count_init_rate   : typing.TypeAlias =        int | float
-_type_Count_init_convert: typing.TypeAlias = None | typing.Callable[[_type_Count_init_value], _type_Count_init_value]
-_type_Count_init_decimal: typing.TypeAlias = None | bool
-_type_Count_init_Numeric: typing.TypeAlias =        Numeric
+_type_Count_init_value   = typing.Union[int, float]
+_type_Count_init_rate    = typing.Union[int, float]
+_type_Count_init_convert = typing.Union[None, typing.Callable[[_type_Count_init_value], _type_Count_init_value]]
+_type_Count_init_decimal = typing.Union[None, bool]
+_type_Count_init_Numeric = Numeric
     
 
 _Count_focus_events = {
     _core.Event.insert, _core.Event.delete_left
 }
 
 _Count_focus = lambda event: event in _Count_focus_events
@@ -1458,15 +1464,16 @@
         
         self._decimal = decimal
         
         offset = value
         
         def create(spot):
             value = offset - sum(spot) * rate
-            if (decimal := self._decimal) is None:
+            decimal = self._decimal
+            if decimal is None:
                 decimal = True
             if not convert is None:
                 value = convert(value) 
             tile = Numeric(
                 value = value, 
                 decimal = decimal
             )
@@ -1482,16 +1489,17 @@
             focus_mark = None,
             **kwargs
         )
 
     def _resolve(self):
 
         value_any = self._mutate.cur_tile.resolve()
+        value_int = int(value_any)
 
-        if self._decimal is None and (value_int := int(value_any)) == value_any:
+        if self._decimal is None and value_int == value_any:
             value_any = value_int
 
         return value_any
     
 
 _DateTime_focus_events = {
     _core.Event.arrow_up, _core.Event.arrow_down,
@@ -1559,20 +1567,20 @@
     'day'   : 2,
     'hour'  : 2,
     'minute': 2,
     'second': 2
 }
 
 
-_type_DateTime_init_value       : typing.TypeAlias = datetime.datetime
-_type_DateTime_init_Chron       : typing.TypeAlias = Count
-_type_DateTime_init_attrs       : typing.TypeAlias = list[str]
-_type_DateTime_init_date_delimit: typing.TypeAlias = str
-_type_DateTime_init_time_delimit: typing.TypeAlias = str
-_type_DateTime_init_part_delimit: typing.TypeAlias = str
+_type_DateTime_init_value        = datetime.datetime
+_type_DateTime_init_Chron        = Count
+_type_DateTime_init_attrs        = typing.List[str]
+_type_DateTime_init_date_delimit = str
+_type_DateTime_init_time_delimit = str
+_type_DateTime_init_part_delimit = str
 
 
 class DateTime(BaseList):
 
     """
     A datetime picker.
```

### Comparing `survey-4.4.0/survey.egg-info/PKG-INFO` & `survey-4.5.0/survey.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.4.0
+Version: 4.5.0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
 
 ✨ A simple library for creating beautiful interactive prompts.
 
 .. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
```

