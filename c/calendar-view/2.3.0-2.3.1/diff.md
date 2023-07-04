# Comparing `tmp/calendar-view-2.3.0.tar.gz` & `tmp/calendar-view-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar-view-2.3.0.tar", last modified: Thu Jun  8 20:39:24 2023, max compression
+gzip compressed data, was "calendar-view-2.3.1.tar", last modified: Tue Jul  4 17:28:14 2023, max compression
```

## Comparing `calendar-view-2.3.0.tar` & `calendar-view-2.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-08 20:38:59.000000 calendar-view-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 20:38:59.000000 calendar-view-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-08 20:39:24.209219 calendar-view-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-08 20:38:59.000000 calendar-view-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/calendar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/config/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/config/__pycache__/style.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/config/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/config/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/data.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/event.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/time_utils.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/calendar_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/calendar_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/round_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/resources/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   168260 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/fonts/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/fonts/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/resources/fonts/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:39:24.209219 calendar-view-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-08 20:38:59.000000 calendar-view-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-08 20:38:59.000000 calendar-view-2.3.0/tests/test_calendar_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-08 20:38:59.000000 calendar-view-2.3.0/tests/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-07-04 17:27:52.000000 calendar-view-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 17:27:52.000000 calendar-view-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-07-04 17:28:14.984032 calendar-view-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-04 17:27:52.000000 calendar-view-2.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.980032 calendar-view-2.3.1/calendar_view/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.980032 calendar-view-2.3.1/calendar_view/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.980032 calendar-view-2.3.1/calendar_view/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.980032 calendar-view-2.3.1/calendar_view/config/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/config/__pycache__/style.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/config/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/config/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/calendar_view/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/calendar_view/core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/core/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/core/__pycache__/data.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/core/__pycache__/event.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/core/__pycache__/time_utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/calendar_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/calendar_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/round_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/calendar_view/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/calendar_view/resources/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/resources/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/calendar_view/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/resources/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   168260 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/resources/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:27:52.000000 calendar-view-2.3.1/calendar_view/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/calendar_view/resources/fonts/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 17:28:08.000000 calendar-view-2.3.1/calendar_view/resources/fonts/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.980032 calendar-view-2.3.1/calendar_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-07-04 17:28:14.000000 calendar-view-2.3.1/calendar_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 17:28:14.000000 calendar-view-2.3.1/calendar_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:28:14.000000 calendar-view-2.3.1/calendar_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 17:28:14.000000 calendar-view-2.3.1/calendar_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 17:28:14.000000 calendar-view-2.3.1/calendar_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:28:14.984032 calendar-view-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 17:27:52.000000 calendar-view-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:14.984032 calendar-view-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 17:27:52.000000 calendar-view-2.3.1/tests/test_calendar_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-04 17:27:52.000000 calendar-view-2.3.1/tests/test_time_utils.py
```

### Comparing `calendar-view-2.3.0/LICENSE` & `calendar-view-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/PKG-INFO` & `calendar-view-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-view
-Version: 2.3.0
+Version: 2.3.1
 Summary: Library provides a graphical view of the calendar.
 Home-page: https://github.com/sakhnevych/calendar-view
 Author: Oleksandr Sakhnevych, Daniil Limariev
 Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `calendar-view-2.3.0/README.rst` & `calendar-view-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/calendar.py` & `calendar-view-2.3.1/calendar_view/calendar.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/config/__pycache__/style.cpython-311.pyc` & `calendar-view-2.3.1/calendar_view/config/__pycache__/style.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
+moddate:  0x9856a464 (Tue Jul  4 17:27:52 2023 UTC)
 files sz: 1356
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
@@ -42,15 +42,15 @@
                 34 LOAD_NAME                6 (__annotations__)
                 36 LOAD_CONST               4 ('font_path')
                 38 STORE_SUBSCR
    
      7          42 LOAD_CONST               5 ('size')
                 44 LOAD_NAME                7 (int)
                 46 BUILD_TUPLE              2
-                48 LOAD_CONST               6 (<code object image_font, file "/home/runner/work/CalendarView/CalendarView/calendar_view/config/style.py", line 7>)
+                48 LOAD_CONST               6 (<code object image_font, file "/home/runner/work/calendar-view/calendar-view/calendar_view/config/style.py", line 7>)
                 50 MAKE_FUNCTION            4 (annotations)
                 52 STORE_NAME               8 (image_font)
    
     12          54 LOAD_CONST               7 ((255, 255, 255, 255))
                 56 STORE_NAME               9 (image_bg)
    
     14          58 LOAD_CONST               8 (50)
@@ -226,15 +226,15 @@
          consts
             None
             'calendar_view.resources.fonts'
          names      ('resource_filename', 'font_path', 'ImageFont', 'truetype')
          varnames   ('size', 'path')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/config/style.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/config/style.py'
          name       'image_font'
          firstlineno 7
          lnotab 0x02012a01
       (255, 255, 255, 255)
       50
       400
       60
@@ -259,14 +259,14 @@
       40
       70
       None
    names      ('PIL', 'ImageFont', 'pkg_resources', 'resource_filename', 'font_path', 'str', '__annotations__', 'int', 'image_font', 'image_bg', 'hour_height', 'day_width', 'padding_horizontal', 'padding_vertical', 'title_font', 'title_color', 'title_padding_left', 'title_padding_right', 'title_padding_top', 'title_padding_bottom', 'hour_number_font', 'hour_number_color', 'day_of_week_font', 'day_of_week_color', 'line_day_color', 'line_day_width', 'line_hour_color', 'line_hour_width', 'event_border_width', 'event_radius', 'event_border_default', 'event_fill_default', 'event_title_font', 'event_title_color', 'event_notes_font', 'event_notes_color', 'event_padding', 'event_title_margin', 'legend_spacing', 'legend_padding_top', 'legend_padding_bottom', 'legend_padding_left', 'legend_padding_right', 'legend_name_font', 'legend_name_color')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/config/style.py'
+   filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/config/style.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010e010c020e030c050402040104010401040216010401040104
       010401040216010402160104020401040104010402040104010401040216
       010401160104010e010e02040104010401040104011601
```

### Comparing `calendar-view-2.3.0/calendar_view/config/i18n.py` & `calendar-view-2.3.1/calendar_view/config/i18n.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/config/style.py` & `calendar-view-2.3.1/calendar_view/config/style.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/__pycache__/config.cpython-311.pyc` & `calendar-view-2.3.1/calendar_view/core/__pycache__/config.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
+moddate:  0x9856a464 (Tue Jul  4 17:27:52 2023 UTC)
 files sz: 3558
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -55,15 +55,15 @@
      8          70 LOAD_NAME                7 (Literal)
                 72 LOAD_CONST               6 (('top', 'center', 'bottom'))
                 74 BINARY_SUBSCR
                 84 STORE_NAME              12 (VerticalAlign)
    
     11          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object CalendarConfig, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py", line 11>)
+                90 LOAD_CONST               7 (<code object CalendarConfig, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py", line 11>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('CalendarConfig')
                 96 LOAD_NAME               13 (object)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME              14 (CalendarConfig)
                114 LOAD_CONST               1 (None)
@@ -155,45 +155,45 @@
           29          70 LOAD_NAME                6 (bool)
          
           20          72 LOAD_CONST              18 ('title_vertical_align')
          
           30          74 LOAD_NAME                7 (VerticalAlign)
          
           20          76 BUILD_TUPLE             20
-                      78 LOAD_CONST              19 (<code object __init__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py", line 20>)
+                      78 LOAD_CONST              19 (<code object __init__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py", line 20>)
                       80 MAKE_FUNCTION            5 (defaults, annotations)
                       82 STORE_NAME               8 (__init__)
          
-          43          84 LOAD_CONST              20 (<code object _configure_mode, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py", line 43>)
+          43          84 LOAD_CONST              20 (<code object _configure_mode, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py", line 43>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME               9 (_configure_mode)
          
-          60          90 LOAD_CONST              21 (<code object validate, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py", line 60>)
+          60          90 LOAD_CONST              21 (<code object validate, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py", line 60>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              10 (validate)
          
           72          96 LOAD_CONST              22 ('return')
                       98 LOAD_NAME               11 (Tuple)
                      100 LOAD_NAME               12 (date)
                      102 LOAD_NAME               12 (date)
                      104 BUILD_TUPLE              2
                      106 BINARY_SUBSCR
                      116 BUILD_TUPLE              2
-                     118 LOAD_CONST              23 (<code object get_date_range, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py", line 72>)
+                     118 LOAD_CONST              23 (<code object get_date_range, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py", line 72>)
                      120 MAKE_FUNCTION            4 (annotations)
                      122 STORE_NAME              13 (get_date_range)
          
           84         124 LOAD_CONST              22 ('return')
                      126 LOAD_NAME               11 (Tuple)
                      128 LOAD_NAME                5 (int)
                      130 LOAD_NAME                5 (int)
                      132 BUILD_TUPLE              2
                      134 BINARY_SUBSCR
                      144 BUILD_TUPLE              2
-                     146 LOAD_CONST              24 (<code object get_hours_range, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py", line 84>)
+                     146 LOAD_CONST              24 (<code object get_hours_range, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py", line 84>)
                      148 MAKE_FUNCTION            4 (annotations)
                      150 STORE_NAME              14 (get_hours_range)
                      152 LOAD_CONST               4 (None)
                      154 RETURN_VALUE
          consts
             'CalendarConfig'
             "\n    Mode will override some parameters.\n    Available modes:\n    'auto' - modes 'week' + 'day_hours'\n    'week' - show current week\n    'day_hours' - show hours range '8:00 - 22:00'\n    'working_hours' - show hours range '8:00 - 19:00'\n    "
@@ -278,15 +278,15 @@
                            184 RETURN_VALUE
                consts
                   None
                names      ('lang', 'title', 'dates', 'days', 'hours', 'mode', 'show_date', 'show_year', 'legend', 'title_vertical_align', '_configure_mode')
                varnames   ('self', 'lang', 'title', 'dates', 'days', 'hours', 'mode', 'show_date', 'show_year', 'legend', 'title_vertical_align')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
                name       '__init__'
                firstlineno 20
                lnotab 0x020b0e010e010e010e010e010e010e010e010e010e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
@@ -419,15 +419,15 @@
                   '8:00 - 22:00'
                   'working_hours'
                   '8:00 - 19:00'
                names      ('mode', 'replace', 'split', 'append', 'format', 'time_utils', 'current_week_day', 'strftime', 'dates', 'hours')
                varnames   ('self', 'modes')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
                name       '_configure_mode'
                firstlineno 43
                lnotab
                   0x02010e0104015c0108012a012a01080118014c014cfe1a0408010e0108
                   0112ff
             code
                argcount  : 1
@@ -537,15 +537,15 @@
                   "Parameter 'days' can be in interval [1, 14]"
                   "Both parameters 'days' and 'dates' are used. 'days' value will be skipped."
                   "'show_year' is set to True, but date wont be displayed, because 'show_date' is False."
                names      ('StringUtils', 'is_blank', 'lang', 'Exception', 'days', 'get_hours_range', 'get_date_range', 'dates', 'logging', 'warning', 'show_year', 'show_date')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
                name       'validate'
                firstlineno 60
                lnotab 0x020132011e0128011e01280128011c0128011c012cff
             'return'
             code
                argcount  : 1
                nlocals   : 1
@@ -633,15 +633,15 @@
                   "Date range is not defined. Using default range 'Mo - Su'."
                   0
                   6
                names      ('StringUtils', 'is_not_blank', 'dates', 'time_utils', 'parse_date_interval', 'days', 'date', 'today', 'timedelta', 'logging', 'warning', 'current_week_day')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
                name       'get_date_range'
                firstlineno 72
                lnotab 0x0204320132010e017e022801
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 3
@@ -710,32 +710,32 @@
                   0
                   1
                   24
                names      ('StringUtils', 'is_blank', 'hours', 'time_utils', 'parse_time_interval', 'minute', 'hour')
                varnames   ('self', 'start', 'end', 'fixed_end')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
                name       'get_hours_range'
                firstlineno 84
                lnotab 0x020432010402380138010c010402
             ('en', '', None, 7, None, None, True, False, None, 'center')
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'int', 'bool', 'VerticalAlign', '__init__', '_configure_mode', 'validate', 'Tuple', 'date', 'get_date_range', 'get_hours_range')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
          name       'CalendarConfig'
          firstlineno 11
          lnotab
             0x0a01040902010201020102010201020102010201020102f6040102ff02
             0202fe020302fd020402fc020502fb020602fa020702f9020802f8020902
             f7020a02f608170611060c1c0c
       'CalendarConfig'
    names      ('logging', 'datetime', 'date', 'timedelta', 'typing', 'Tuple', 'List', 'Literal', 'calendar_view.core', 'time_utils', 'calendar_view.core.utils', 'StringUtils', 'VerticalAlign', 'object', 'CalendarConfig')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/config.py'
+   filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/config.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010801100114020c010c021003
```

### Comparing `calendar-view-2.3.0/calendar_view/core/__pycache__/data.cpython-311.pyc` & `calendar-view-2.3.1/calendar_view/core/__pycache__/data.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
+moddate:  0x9856a464 (Tue Jul  4 17:27:52 2023 UTC)
 files sz: 1675
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -38,51 +38,51 @@
                 38 IMPORT_NAME              5 (calendar_view.core.event)
                 40 IMPORT_FROM              6 (Event)
                 42 STORE_NAME               6 (Event)
                 44 POP_TOP
    
      8          46 PUSH_NULL
                 48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               5 (<code object InputData, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py", line 8>)
+                50 LOAD_CONST               5 (<code object InputData, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py", line 8>)
                 52 MAKE_FUNCTION            0
                 54 LOAD_CONST               6 ('InputData')
                 56 LOAD_NAME                7 (object)
                 58 PRECALL                  3
                 62 CALL                     3
                 72 STORE_NAME               8 (InputData)
    
     14          74 LOAD_CONST               7 ('config')
                 76 LOAD_NAME                4 (CalendarConfig)
                 78 BUILD_TUPLE              2
-                80 LOAD_CONST               8 (<code object validate_config, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py", line 14>)
+                80 LOAD_CONST               8 (<code object validate_config, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py", line 14>)
                 82 MAKE_FUNCTION            4 (annotations)
                 84 STORE_NAME               9 (validate_config)
    
     18          86 LOAD_CONST               9 ('event')
                 88 LOAD_NAME                6 (Event)
                 90 LOAD_CONST               7 ('config')
                 92 LOAD_NAME                4 (CalendarConfig)
                 94 BUILD_TUPLE              4
-                96 LOAD_CONST              10 (<code object validate_event, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py", line 18>)
+                96 LOAD_CONST              10 (<code object validate_event, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py", line 18>)
                 98 MAKE_FUNCTION            4 (annotations)
                100 STORE_NAME              10 (validate_event)
    
     40         102 LOAD_CONST              11 ('events')
                104 LOAD_NAME               11 (list)
                106 LOAD_CONST               7 ('config')
                108 LOAD_NAME                4 (CalendarConfig)
                110 BUILD_TUPLE              4
-               112 LOAD_CONST              12 (<code object validate_events, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py", line 40>)
+               112 LOAD_CONST              12 (<code object validate_events, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py", line 40>)
                114 MAKE_FUNCTION            4 (annotations)
                116 STORE_NAME              12 (validate_events)
    
     45         118 LOAD_CONST              13 ('data')
                120 LOAD_NAME                8 (InputData)
                122 BUILD_TUPLE              2
-               124 LOAD_CONST              14 (<code object validate_data, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py", line 45>)
+               124 LOAD_CONST              14 (<code object validate_data, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py", line 45>)
                126 MAKE_FUNCTION            4 (annotations)
                128 STORE_NAME              13 (validate_data)
                130 LOAD_CONST               1 (None)
                132 RETURN_VALUE
    consts
       0
       None
@@ -104,15 +104,15 @@
                        8 STORE_NAME               2 (__qualname__)
          
            9          10 LOAD_CONST               1 ('config')
                       12 LOAD_NAME                3 (CalendarConfig)
                       14 LOAD_CONST               2 ('events')
                       16 LOAD_NAME                4 (list)
                       18 BUILD_TUPLE              4
-                      20 LOAD_CONST               3 (<code object __init__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py", line 9>)
+                      20 LOAD_CONST               3 (<code object __init__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py", line 9>)
                       22 MAKE_FUNCTION            4 (annotations)
                       24 STORE_NAME               5 (__init__)
                       26 LOAD_CONST               4 (None)
                       28 RETURN_VALUE
          consts
             'InputData'
             'config'
@@ -138,24 +138,24 @@
                             32 RETURN_VALUE
                consts
                   None
                names      ('config', 'events')
                varnames   ('self', 'config', 'events')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
                name       '__init__'
                firstlineno 9
                lnotab 0x02010e01
             None
          names      ('__name__', '__module__', '__qualname__', 'CalendarConfig', 'list', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
          name       'InputData'
          firstlineno 8
          lnotab 0x0a01
       'InputData'
       'config'
       code
          argcount  : 1
@@ -176,15 +176,15 @@
                       44 RETURN_VALUE
          consts
             None
          names      ('validate',)
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
          name       'validate_config'
          firstlineno 14
          lnotab 0x0201
       'event'
       code
          argcount  : 2
          nlocals   : 6
@@ -391,15 +391,15 @@
             '%H:%M'
             24
             "Event can't be shown, because its end is after time range: {} is before {}"
          names      ('get_date_range', 'time', 'get_hours_range', 'get_start_date', 'logging', 'warning', 'format', 'strftime', 'start_time', 'end_time')
          varnames   ('event', 'config', 'start_date', 'end_date', 'start_time', 'end_hour')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
          name       'validate_event'
          firstlineno 18
          lnotab
             0x02012e015001340144012e014e01280128fd1e0516012e01320128fe1e
             043e012e01320144fe22ff
       'events'
       code
@@ -429,15 +429,15 @@
                       46 RETURN_VALUE
          consts
             None
          names      ('validate_event',)
          varnames   ('events', 'config', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
          name       'validate_events'
          firstlineno 40
          lnotab 0x0201080122ff
       'data'
       code
          argcount  : 1
          nlocals   : 1
@@ -469,19 +469,19 @@
                       96 RETURN_VALUE
          consts
             None
          names      ('validate_config', 'config', 'validate_events', 'events')
          varnames   ('data',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
          name       'validate_data'
          firstlineno 45
          lnotab 0x02012801
    names      ('logging', 'datetime', 'time', 'calendar_view.core.config', 'CalendarConfig', 'calendar_view.core.event', 'Event', 'object', 'InputData', 'validate_config', 'validate_event', 'list', 'validate_events', 'validate_data')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/data.py'
+   filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/data.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010c020c010c031c060c0410161005
```

### Comparing `calendar-view-2.3.0/calendar_view/core/__pycache__/event.cpython-311.pyc` & `calendar-view-2.3.1/calendar_view/core/__pycache__/event.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
+moddate:  0x9856a464 (Tue Jul  4 17:27:52 2023 UTC)
 files sz: 8898
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -40,35 +40,35 @@
      5          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               4 (('*',))
                 46 IMPORT_NAME              7 (calendar_view.core.time_utils)
                 48 IMPORT_STAR
    
      8          50 PUSH_NULL
                 52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               5 (<code object EventStyle, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 8>)
+                54 LOAD_CONST               5 (<code object EventStyle, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 8>)
                 56 MAKE_FUNCTION            0
                 58 LOAD_CONST               6 ('EventStyle')
                 60 LOAD_NAME                8 (object)
                 62 PRECALL                  3
                 66 CALL                     3
                 76 STORE_NAME               9 (EventStyle)
    
     31          78 PUSH_NULL
                 80 LOAD_BUILD_CLASS
-                82 LOAD_CONST               7 (<code object EventStyles, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 31>)
+                82 LOAD_CONST               7 (<code object EventStyles, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 31>)
                 84 MAKE_FUNCTION            0
                 86 LOAD_CONST               8 ('EventStyles')
                 88 LOAD_NAME                8 (object)
                 90 PRECALL                  3
                 94 CALL                     3
                104 STORE_NAME              10 (EventStyles)
    
     41         106 PUSH_NULL
                108 LOAD_BUILD_CLASS
-               110 LOAD_CONST               9 (<code object Event, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 41>)
+               110 LOAD_CONST               9 (<code object Event, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 41>)
                112 MAKE_FUNCTION            0
                114 LOAD_CONST              10 ('Event')
                116 LOAD_NAME                8 (object)
                118 PRECALL                  3
                122 CALL                     3
                132 STORE_NAME              11 (Event)
                134 LOAD_CONST              11 (None)
@@ -114,29 +114,29 @@
                       48 LOAD_NAME                5 (int)
                       50 LOAD_NAME                5 (int)
                       52 BUILD_TUPLE              4
                       54 BINARY_SUBSCR
                       64 LOAD_CONST               5 ('return')
                       66 LOAD_CONST               2 (None)
                       68 BUILD_TUPLE              6
-                      70 LOAD_CONST               6 (<code object __init__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 12>)
+                      70 LOAD_CONST               6 (<code object __init__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 12>)
                       72 MAKE_FUNCTION            5 (defaults, annotations)
                       74 STORE_NAME               6 (__init__)
          
           22          76 LOAD_CONST               5 ('return')
                       78 LOAD_NAME                7 (str)
                       80 BUILD_TUPLE              2
-                      82 LOAD_CONST               7 (<code object __repr__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 22>)
+                      82 LOAD_CONST               7 (<code object __repr__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 22>)
                       84 MAKE_FUNCTION            4 (annotations)
                       86 STORE_NAME               8 (__repr__)
          
           25          88 LOAD_CONST               5 ('return')
                       90 LOAD_NAME                9 (bool)
                       92 BUILD_TUPLE              2
-                      94 LOAD_CONST               8 (<code object __eq__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 25>)
+                      94 LOAD_CONST               8 (<code object __eq__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 25>)
                       96 MAKE_FUNCTION            4 (annotations)
                       98 STORE_NAME              10 (__eq__)
                      100 LOAD_CONST               2 (None)
                      102 RETURN_VALUE
          consts
             'EventStyle'
             '\n    Defined the style of the painted event.\n    '
@@ -178,15 +178,15 @@
                consts
                   '\n        :param event_border: the color of the border as a tuple (r, g, b, a)\n            Example: (120, 180, 120, 240) - green\n        :param event_fill: the color of the background as a tuple (r, g, b, a)\n            Example: (196, 234, 188, 180) - light green\n        '
                   None
                names      ('style', 'event_border_default', 'event_border', 'event_fill_default', 'event_fill')
                varnames   ('self', 'event_border', 'event_fill')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__init__'
                firstlineno 12
                lnotab 0x02072a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
@@ -212,15 +212,15 @@
                   'EventStyle[event_border: '
                   ', event_fill: '
                   ']'
                names      ('event_border', 'event_fill')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__repr__'
                firstlineno 22
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -256,24 +256,24 @@
                 26     >>  106 RETURN_VALUE
                consts
                   None
                names      ('isinstance', 'EventStyle', 'event_border', 'event_fill')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__eq__'
                firstlineno 25
                lnotab 0x02012a011eff02021efe
             (None, None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Tuple', 'int', '__init__', 'str', '__repr__', 'bool', '__eq__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
          name       'EventStyle'
          firstlineno 8
          lnotab 0x0a0104033e0a0c03
       'EventStyle'
       code
          argcount  : 0
          nlocals   : 0
@@ -344,15 +344,15 @@
             (110, 110, 110, 240)
             (200, 200, 200, 190)
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'EventStyle', 'GREEN', 'RED', 'BLUE', 'GRAY')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
          name       'EventStyles'
          firstlineno 31
          lnotab 0x0a0104031a011a011a01
       'EventStyles'
       code
          argcount  : 0
          nlocals   : 0
@@ -433,15 +433,15 @@
           44          98 LOAD_NAME                9 (EventStyle)
          
           42         100 LOAD_CONST               9 ('return')
          
           44         102 LOAD_CONST               1 (None)
          
           42         104 BUILD_TUPLE             16
-                     106 LOAD_CONST              10 (<code object __init__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 42>)
+                     106 LOAD_CONST              10 (<code object __init__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 42>)
                      108 MAKE_FUNCTION            5 (defaults, annotations)
                      110 STORE_NAME              10 (__init__)
          
           76         112 LOAD_NAME               11 (staticmethod)
          
           77         114 LOAD_CONST               4 ('day_of_week')
                      116 LOAD_NAME               12 (Optional)
@@ -470,15 +470,15 @@
           77         186 LOAD_CONST               9 ('return')
          
           79         188 LOAD_NAME               12 (Optional)
                      190 LOAD_NAME                6 (date)
                      192 BINARY_SUBSCR
          
           77         202 BUILD_TUPLE              8
-                     204 LOAD_CONST              11 (<code object __parse_start_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 76>)
+                     204 LOAD_CONST              11 (<code object __parse_start_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 76>)
                      206 MAKE_FUNCTION            4 (annotations)
          
           76         208 PRECALL                  0
                      212 CALL                     0
          
           77         222 STORE_NAME              13 (_Event__parse_start_date)
          
@@ -513,15 +513,15 @@
           87         310 LOAD_CONST               9 ('return')
          
           89         312 LOAD_NAME               12 (Optional)
                      314 LOAD_NAME                6 (date)
                      316 BINARY_SUBSCR
          
           87         326 BUILD_TUPLE              8
-                     328 LOAD_CONST              12 (<code object __parse_end_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 86>)
+                     328 LOAD_CONST              12 (<code object __parse_end_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 86>)
                      330 MAKE_FUNCTION            4 (annotations)
          
           86         332 PRECALL                  0
                      336 CALL                     0
          
           87         346 STORE_NAME              14 (_Event__parse_end_date)
          
@@ -556,15 +556,15 @@
           97         434 LOAD_CONST               9 ('return')
          
           99         436 LOAD_NAME               12 (Optional)
                      438 LOAD_NAME                6 (date)
                      440 BINARY_SUBSCR
          
           97         450 BUILD_TUPLE              8
-                     452 LOAD_CONST              14 (<code object __parse_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 96>)
+                     452 LOAD_CONST              14 (<code object __parse_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 96>)
                      454 MAKE_FUNCTION            4 (annotations)
          
           96         456 PRECALL                  0
                      460 CALL                     0
          
           97         470 STORE_NAME              15 (_Event__parse_date)
          
@@ -578,99 +578,99 @@
                      484 BUILD_TUPLE              3
                      486 BINARY_SUBSCR
                      496 LOAD_CONST               9 ('return')
                      498 LOAD_NAME               12 (Optional)
                      500 LOAD_NAME                8 (time)
                      502 BINARY_SUBSCR
                      512 BUILD_TUPLE              4
-                     514 LOAD_CONST              15 (<code object __parse_time, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 113>)
+                     514 LOAD_CONST              15 (<code object __parse_time, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 113>)
                      516 MAKE_FUNCTION            4 (annotations)
          
          113         518 PRECALL                  0
                      522 CALL                     0
          
          114         532 STORE_NAME              16 (_Event__parse_time)
          
-         122         534 LOAD_CONST              16 (<code object __validate, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 122>)
+         122         534 LOAD_CONST              16 (<code object __validate, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 122>)
                      536 MAKE_FUNCTION            0
                      538 STORE_NAME              17 (_Event__validate)
          
          132         540 LOAD_CONST              17 ('config')
                      542 LOAD_NAME               18 (CalendarConfig)
                      544 LOAD_CONST               9 ('return')
                      546 LOAD_NAME                6 (date)
                      548 BUILD_TUPLE              4
-                     550 LOAD_CONST              18 (<code object get_start_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 132>)
+                     550 LOAD_CONST              18 (<code object get_start_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 132>)
                      552 MAKE_FUNCTION            4 (annotations)
                      554 STORE_NAME              19 (get_start_date)
          
          139         556 LOAD_CONST              17 ('config')
                      558 LOAD_NAME               18 (CalendarConfig)
                      560 LOAD_CONST               9 ('return')
                      562 LOAD_NAME                6 (date)
                      564 BUILD_TUPLE              4
-                     566 LOAD_CONST              19 (<code object get_end_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 139>)
+                     566 LOAD_CONST              19 (<code object get_end_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 139>)
                      568 MAKE_FUNCTION            4 (annotations)
                      570 STORE_NAME              20 (get_end_date)
          
          146         572 LOAD_CONST              17 ('config')
                      574 LOAD_NAME               18 (CalendarConfig)
                      576 LOAD_CONST               9 ('return')
                      578 LOAD_NAME                6 (date)
                      580 BUILD_TUPLE              4
-                     582 LOAD_CONST              20 (<code object __get_date_by_day_of_week, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 146>)
+                     582 LOAD_CONST              20 (<code object __get_date_by_day_of_week, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 146>)
                      584 MAKE_FUNCTION            4 (annotations)
                      586 STORE_NAME              21 (_Event__get_date_by_day_of_week)
          
          164         588 LOAD_CONST              17 ('config')
                      590 LOAD_NAME               18 (CalendarConfig)
                      592 LOAD_CONST               9 ('return')
                      594 LOAD_NAME               22 (float)
                      596 BUILD_TUPLE              4
-                     598 LOAD_CONST              21 (<code object get_duration_seconds, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 164>)
+                     598 LOAD_CONST              21 (<code object get_duration_seconds, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 164>)
                      600 MAKE_FUNCTION            4 (annotations)
                      602 STORE_NAME              23 (get_duration_seconds)
          
          168         604 LOAD_NAME               24 (property)
          
          169         606 LOAD_CONST               9 ('return')
                      608 LOAD_NAME                8 (time)
                      610 BUILD_TUPLE              2
-                     612 LOAD_CONST              22 (<code object start_time, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 168>)
+                     612 LOAD_CONST              22 (<code object start_time, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 168>)
                      614 MAKE_FUNCTION            4 (annotations)
          
          168         616 PRECALL                  0
                      620 CALL                     0
          
          169         630 STORE_NAME              25 (start_time)
          
          172         632 LOAD_NAME               24 (property)
          
          173         634 LOAD_CONST               9 ('return')
                      636 LOAD_NAME                8 (time)
                      638 BUILD_TUPLE              2
-                     640 LOAD_CONST              23 (<code object end_time, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 172>)
+                     640 LOAD_CONST              23 (<code object end_time, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 172>)
                      642 MAKE_FUNCTION            4 (annotations)
          
          172         644 PRECALL                  0
                      648 CALL                     0
          
          173         658 STORE_NAME              26 (end_time)
          
          176         660 LOAD_CONST               9 ('return')
                      662 LOAD_NAME                3 (str)
                      664 BUILD_TUPLE              2
-                     666 LOAD_CONST              24 (<code object __repr__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 176>)
+                     666 LOAD_CONST              24 (<code object __repr__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 176>)
                      668 MAKE_FUNCTION            4 (annotations)
                      670 STORE_NAME              27 (__repr__)
          
          183         672 LOAD_CONST               9 ('return')
                      674 LOAD_NAME               28 (bool)
                      676 BUILD_TUPLE              2
-                     678 LOAD_CONST              25 (<code object __eq__, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py", line 183>)
+                     678 LOAD_CONST              25 (<code object __eq__, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py", line 183>)
                      680 MAKE_FUNCTION            4 (annotations)
                      682 STORE_NAME              29 (__eq__)
                      684 LOAD_CONST               1 (None)
                      686 RETURN_VALUE
          consts
             'Event'
             None
@@ -855,15 +855,15 @@
                   "'start' argument is required"
                   "'end' argument is required"
                   1
                names      ('ValueError', 'format', 'title', 'notes', 'EventStyle', 'style', '_Event__parse_start_date', '_Event__start_date', '_Event__parse_end_date', '_Event__end_date', '_Event__day_of_week', 'Event', '_Event__parse_time', '_Event__start_time', '_Event__end_time', 'cascade_total', 'cascade_index', 'cascade_group', '_Event__validate')
                varnames   ('self', 'title', 'notes', 'day_of_week', 'day', 'start', 'end', 'style')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__init__'
                firstlineno 42
                lnotab
                   0x02032201440104011e0104011e020e010e012e03380138010e0118010e
                   0104010e033e013e020e010e010e02
             code
                argcount  : 3
@@ -919,15 +919,15 @@
                   None
                   "'day_of_week' is defined together with a 'day'."
                   "'day_of_week' is defined together with a 'start' as a datetime."
                names      ('ValueError', 'isinstance', 'datetime', 'Event', '_Event__parse_date')
                varnames   ('day_of_week', 'day', 'start')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__parse_start_date'
                firstlineno 76
                lnotab 0x020408011e0132011e01
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
@@ -981,15 +981,15 @@
                   None
                   "'day_of_week' is defined together with a 'day'."
                   "'day_of_week' is defined together with a 'end' as a datetime."
                names      ('ValueError', 'isinstance', 'datetime', 'Event', '_Event__parse_date')
                varnames   ('day_of_week', 'day', 'end')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__parse_end_date'
                firstlineno 86
                lnotab 0x020408011e0132011e01
             'time_entry'
             code
                argcount  : 3
                nlocals   : 3
@@ -1073,15 +1073,15 @@
                            302 RETURN_VALUE
                consts
                   None
                names      ('isinstance', 'date', 'datetime', 'str', 'parse_date')
                varnames   ('day_of_week', 'day', 'time_entry')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__parse_date'
                firstlineno 96
                lnotab 0x02040401040104012a0104012a0128012a011e012e012801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -1136,15 +1136,15 @@
                            204 RETURN_VALUE
                consts
                   None
                names      ('isinstance', 'datetime', 'time', 'str', 'parse_time')
                varnames   ('time_entry',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__parse_time'
                firstlineno 113
                lnotab 0x02022a0128012a0104012a011eff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -1237,15 +1237,15 @@
                   'Either date of the end event or the day of the week has to be defined.'
                   "Event's start date has to be before end date"
                   "Event's start time has to be before end time"
                names      ('_Event__start_date', '_Event__day_of_week', 'ValueError', '_Event__end_date', '_Event__start_time', '_Event__end_time')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__validate'
                firstlineno 122
                lnotab 0x02011c011e011c011e013c011e0140011eff
             'config'
             code
                argcount  : 2
                nlocals   : 2
@@ -1284,15 +1284,15 @@
                            114 RETURN_VALUE
                consts
                   None
                names      ('_Event__start_date', 'current_week_day', '_Event__day_of_week', '_Event__get_date_by_day_of_week')
                varnames   ('self', 'config')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       'get_start_date'
                firstlineno 132
                lnotab 0x02010e010e0104012801
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -1330,15 +1330,15 @@
                            114 RETURN_VALUE
                consts
                   None
                names      ('_Event__end_date', 'current_week_day', '_Event__day_of_week', '_Event__get_date_by_day_of_week')
                varnames   ('self', 'config')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       'get_end_date'
                firstlineno 139
                lnotab 0x02010e010e0104012801
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 7
@@ -1442,15 +1442,15 @@
                   ']'
                   1
                   ('weeks',)
                names      ('ValueError', 'get_date_range', 'days', 'week_day_for_date', '_Event__day_of_week', 'timedelta')
                varnames   ('self', 'config', 'start_date', 'end_date', 'days_duration', 'result_date')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__get_date_by_day_of_week'
                firstlineno 146
                lnotab 0x020404011e022e0114010c010e0102ff040102ff16032a0120010401
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -1499,15 +1499,15 @@
                            246 RETURN_VALUE
                consts
                   None
                names      ('datetime', 'combine', 'get_end_date', 'end_time', 'get_start_date', 'start_time', 'total_seconds')
                varnames   ('self', 'config', 'duration')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       'get_duration_seconds'
                firstlineno 164
                lnotab 0x0201ce01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1520,15 +1520,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Event__start_time',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       'start_time'
                firstlineno 168
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1541,15 +1541,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_Event__end_time',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       'end_time'
                firstlineno 172
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 23
@@ -1641,15 +1641,15 @@
                   ', cascade_total: '
                   ', cascade_index: '
                   ']'
                names      ('title', 'notes', 'style', '_Event__day_of_week', '_Event__start_date', '_Event__end_date', 'start_time', 'end_time', 'cascade_group', 'cascade_total', 'cascade_index')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__repr__'
                firstlineno 176
                lnotab
                   0x020132010cff04010cff04010cff04020cfe04020cfe04030cfd04030c
                   fd04040cfc
             code
                argcount  : 2
@@ -1769,37 +1769,37 @@
                184     >>  394 RETURN_VALUE
                consts
                   None
                names      ('isinstance', 'Event', 'title', 'notes', 'style', '_Event__day_of_week', '_Event__start_date', '_Event__end_date', 'start_time', 'end_time', 'cascade_group', 'cascade_total', 'cascade_index')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
                name       '__eq__'
                firstlineno 183
                lnotab
                   0x02012a011eff02021efe02031efd02041efc02051efb02061efa02071e
                   f902081ef802091ef7020a1ef6020b1ef5
             (None, None, None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'Union', 'date', 'datetime', 'time', 'EventStyle', '__init__', 'staticmethod', 'Optional', '_Event__parse_start_date', '_Event__parse_end_date', '_Event__parse_date', '_Event__parse_time', '_Event__validate', 'CalendarConfig', 'get_start_date', 'get_end_date', '_Event__get_date_by_day_of_week', 'float', 'get_duration_seconds', 'property', 'start_time', 'end_time', '__repr__', 'bool', '__eq__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
          name       'Event'
          firstlineno 41
          lnotab
             0x0a010201020102fe100114ff020114ff020214fe020202fe020202fe08
             220201120114ff020220fe02020efe06ff0e0102090201120120ff020220
             fe02020efe06ff0e0102090201120120ff020220fe02020efe06ff0e0102
             1002012cff0e010208060a100710071012100402010aff0e01020302010a
             ff0e0102030c07
       'Event'
       None
    names      ('typing', 'Union', 'NoReturn', 'calendar_view.config', 'style', 'calendar_view.core.config', 'CalendarConfig', 'calendar_view.core.time_utils', 'object', 'EventStyle', 'EventStyles', 'Event')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/event.py'
+   filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/event.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020110020c010c0108031c171c0a
```

### Comparing `calendar-view-2.3.0/calendar_view/core/__pycache__/time_utils.cpython-311.pyc` & `calendar-view-2.3.1/calendar_view/core/__pycache__/time_utils.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
+moddate:  0x9856a464 (Tue Jul  4 17:27:52 2023 UTC)
 files sz: 5426
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
@@ -113,110 +113,110 @@
     29         158 LOAD_CONST              14 ('value')
                160 LOAD_NAME               15 (str)
                162 LOAD_CONST              15 ('return')
                164 LOAD_NAME                7 (Optional)
                166 LOAD_NAME                2 (time)
                168 BINARY_SUBSCR
                178 BUILD_TUPLE              4
-               180 LOAD_CONST              16 (<code object parse_time, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 29>)
+               180 LOAD_CONST              16 (<code object parse_time, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 29>)
                182 MAKE_FUNCTION            4 (annotations)
                184 STORE_NAME              16 (parse_time)
    
     49         186 LOAD_CONST              14 ('value')
                188 LOAD_NAME               15 (str)
                190 LOAD_CONST              15 ('return')
                192 LOAD_NAME               17 (bool)
                194 BUILD_TUPLE              4
-               196 LOAD_CONST              17 (<code object is_valid_time, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 49>)
+               196 LOAD_CONST              17 (<code object is_valid_time, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 49>)
                198 MAKE_FUNCTION            4 (annotations)
                200 STORE_NAME              18 (is_valid_time)
    
     56         202 LOAD_CONST              18 ('interval')
                204 LOAD_NAME               15 (str)
                206 LOAD_CONST              15 ('return')
                208 LOAD_NAME                7 (Optional)
                210 LOAD_NAME                6 (Tuple)
                212 LOAD_NAME                2 (time)
                214 LOAD_NAME                2 (time)
                216 BUILD_TUPLE              2
                218 BINARY_SUBSCR
                228 BINARY_SUBSCR
                238 BUILD_TUPLE              4
-               240 LOAD_CONST              19 (<code object parse_time_interval, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 56>)
+               240 LOAD_CONST              19 (<code object parse_time_interval, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 56>)
                242 MAKE_FUNCTION            4 (annotations)
                244 STORE_NAME              19 (parse_time_interval)
    
     76         246 LOAD_CONST              15 ('return')
                248 LOAD_NAME                3 (date)
                250 BUILD_TUPLE              2
-               252 LOAD_CONST              20 (<code object week_day_for_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 76>)
+               252 LOAD_CONST              20 (<code object week_day_for_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 76>)
                254 MAKE_FUNCTION            4 (annotations)
                256 STORE_NAME              20 (week_day_for_date)
    
     81         258 LOAD_CONST              15 ('return')
                260 LOAD_NAME                3 (date)
                262 BUILD_TUPLE              2
-               264 LOAD_CONST              21 (<code object current_week_day, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 81>)
+               264 LOAD_CONST              21 (<code object current_week_day, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 81>)
                266 MAKE_FUNCTION            4 (annotations)
                268 STORE_NAME              21 (current_week_day)
    
     85         270 LOAD_CONST              14 ('value')
                272 LOAD_NAME               15 (str)
                274 LOAD_CONST              15 ('return')
                276 LOAD_NAME                7 (Optional)
                278 LOAD_NAME                3 (date)
                280 BINARY_SUBSCR
                290 BUILD_TUPLE              4
-               292 LOAD_CONST              22 (<code object parse_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 85>)
+               292 LOAD_CONST              22 (<code object parse_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 85>)
                294 MAKE_FUNCTION            4 (annotations)
                296 STORE_NAME              22 (parse_date)
    
    122         298 LOAD_CONST              23 ('parsed')
                300 LOAD_NAME               23 (list)
                302 LOAD_CONST              15 ('return')
                304 LOAD_NAME                3 (date)
                306 BUILD_TUPLE              4
-               308 LOAD_CONST              24 (<code object _parse_date, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 122>)
+               308 LOAD_CONST              24 (<code object _parse_date, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 122>)
                310 MAKE_FUNCTION            4 (annotations)
                312 STORE_NAME              24 (_parse_date)
    
    143         314 LOAD_CONST              25 ('dates')
                316 LOAD_NAME               15 (str)
                318 LOAD_CONST              15 ('return')
                320 LOAD_NAME                7 (Optional)
                322 LOAD_NAME                6 (Tuple)
                324 LOAD_NAME                3 (date)
                326 LOAD_NAME                3 (date)
                328 BUILD_TUPLE              2
                330 BINARY_SUBSCR
                340 BINARY_SUBSCR
                350 BUILD_TUPLE              4
-               352 LOAD_CONST              26 (<code object parse_date_interval, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 143>)
+               352 LOAD_CONST              26 (<code object parse_date_interval, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 143>)
                354 MAKE_FUNCTION            4 (annotations)
                356 STORE_NAME              25 (parse_date_interval)
    
    167         358 LOAD_CONST              27 ('start_date')
                360 LOAD_NAME                3 (date)
                362 LOAD_CONST              28 ('end_date')
                364 LOAD_NAME                3 (date)
                366 BUILD_TUPLE              4
-               368 LOAD_CONST              29 (<code object date_range, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 167>)
+               368 LOAD_CONST              29 (<code object date_range, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 167>)
                370 MAKE_FUNCTION            4 (annotations)
                372 STORE_NAME              26 (date_range)
    
    177         374 LOAD_CONST              30 ('any_time')
                376 LOAD_NAME                1 (datetime)
                378 LOAD_CONST              15 ('return')
                380 LOAD_NAME                6 (Tuple)
                382 LOAD_NAME                3 (date)
                384 LOAD_NAME                3 (date)
                386 BUILD_TUPLE              2
                388 BINARY_SUBSCR
                398 BUILD_TUPLE              4
-               400 LOAD_CONST              31 (<code object get_week_borders, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py", line 177>)
+               400 LOAD_CONST              31 (<code object get_week_borders, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py", line 177>)
                402 MAKE_FUNCTION            4 (annotations)
                404 STORE_NAME              27 (get_week_borders)
                406 LOAD_CONST               1 (None)
                408 RETURN_VALUE
    consts
       0
       None
@@ -382,15 +382,15 @@
             23
             59
             ('hour', 'minute')
          names      ('StringUtils', 'is_blank', 'time_regex', 'search', 'ValueError', 'format', 'int', 'group', 'time')
          varnames   ('value', 'm', 'hour', 'minute_match', 'minute')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'parse_time'
          firstlineno 29
          lnotab 0x02042801040134010401440144012a0126011801040140012202
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -432,15 +432,15 @@
          consts
             None
             False
          names      ('parse_time', 'ValueError')
          varnames   ('value',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'is_valid_time'
          firstlineno 49
          lnotab 0x020102012401120106ff
       'interval'
       code
          argcount  : 1
          nlocals   : 5
@@ -547,15 +547,15 @@
             '-'
             "Wrong interval format: {}. Use: 'hh:mm - hh:mm'"
             'Start time has to be before end time: {} - {}'
          names      ('strip', 'ValueError', 'format', 'split', 'parse_time', 'ZERO_TIME')
          varnames   ('interval', 'start_value', 'end_value', 'start', 'end')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'parse_time_interval'
          firstlineno 56
          lnotab 0x02042801040104010801440230014201420222014602
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
@@ -583,15 +583,15 @@
                       82 RETURN_VALUE
          consts
             None
          names      ('weekday', 'timedelta')
          varnames   ('d', 'weekday', 'days_ahead')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'week_day_for_date'
          firstlineno 76
          lnotab 0x02012e01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -613,15 +613,15 @@
                       66 RETURN_VALUE
          consts
             None
          names      ('week_day_for_date', 'date', 'today')
          varnames   ('weekday',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'current_week_day'
          firstlineno 81
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 8
          stacksize : 5
@@ -810,15 +810,15 @@
             1900
             2100
             'Wrong date range: {}. Can use only dates with year from 1900 to 2100.'
          names      ('weekday_dict', 'get', 'lower', 'current_week_day', 'int', 'ValueError', 'format', 'split', 'len', '_parse_date', 'year')
          varnames   ('value', 'weekday', 'dash', 'dot', 'slash', 'sum', 'parsed', 'result')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'parse_date'
          firstlineno 85
          lnotab
             0x020e580104011e020801080108015e010c0144010c0144023a0138011e
             021e0128011e01
       'parsed'
       code
@@ -1026,15 +1026,15 @@
             ('year', 'month', 'day')
             4
             'Wrong date format: {}.'
          names      ('len', 'date', 'today', 'year', 'int', 'ValueError')
          varnames   ('parsed',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       '_parse_date'
          firstlineno 122
          lnotab 0x0201020226019c033201960332019603320196ff060212011eff
       'dates'
       code
          argcount  : 1
          nlocals   : 6
@@ -1215,15 +1215,15 @@
             ('weeks',)
             'Start date has to be before end date: {} - {}'
             'Maximum allowed range of days is {}. But {} is configured.'
          names      ('strip', 'StringUtils', 'is_blank', 'parse_date', 'split', 'lower', 'weekday_dict', 'timedelta', 'ValueError', 'format', 'days', 'MAX_DAYS_RANGE_ALLOWED')
          varnames   ('dates', 'one_day', 'start_value', 'end_value', 'start', 'end')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'parse_date_interval'
          firstlineno 143
          lnotab
             0x0201280128010402080142010802300142014202c00126020c01460126
             016002
       'start_date'
       'end_date'
@@ -1294,15 +1294,15 @@
             ' is after the '
             1
             None
          names      ('ValueError', 'range', 'int', 'days', 'timedelta')
          varnames   ('start_date', 'end_date', 'n')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'date_range'
          firstlineno 167
          lnotab 0x06040c01280152012aff
       'any_time'
       code
          argcount  : 1
          nlocals   : 2
@@ -1346,22 +1346,22 @@
             '\n    Returns the start end the end of the week.\n    '
             ('days',)
             6
          names      ('timedelta', 'weekday', 'date')
          varnames   ('any_time', 'start')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
          name       'get_week_borders'
          firstlineno 177
          lnotab 0x02044a01
    names      ('re', 'datetime', 'time', 'date', 'timedelta', 'typing', 'Tuple', 'Optional', 'calendar_view.core.utils', 'StringUtils', 'MAX_DAYS_RANGE_ALLOWED', 'ZERO_TIME', 'weekday_dict', 'compile', 'time_regex', 'str', 'parse_time', 'bool', 'is_valid_time', 'parse_time_interval', 'week_day_for_date', 'current_week_day', 'parse_date', 'list', '_parse_date', 'parse_date_interval', 'date_range', 'get_week_borders')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/time_utils.py'
+   filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/time_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801180110020c020401180202010201020102010201020102
       01020102010201020102010201020102f1061120031c1410072c140c050c
       041c2510152c18100a
```

### Comparing `calendar-view-2.3.0/calendar_view/core/__pycache__/utils.cpython-311.pyc` & `calendar-view-2.3.1/calendar_view/core/__pycache__/utils.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,40 +1,42 @@
 magic:    0xa70d0d0a
-moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
-files sz: 1298
+moddate:  0x9856a464 (Tue Jul  4 17:27:52 2023 UTC)
+files sz: 1304
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c006d015a01010002004700640284006403a6020000ab
-      0200000000000000005a0264045300
+      0x9700640064016c006d015a016d025a02010002004700640284006403a6
+      020000ab0200000000000000005a0364045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Union',))
+                 4 LOAD_CONST               1 (('Union', 'List'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Union)
                 10 STORE_NAME               1 (Union)
-                12 POP_TOP
+                12 IMPORT_FROM              2 (List)
+                14 STORE_NAME               2 (List)
+                16 POP_TOP
    
-     4          14 PUSH_NULL
-                16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object StringUtils, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 4>)
-                20 MAKE_FUNCTION            0
-                22 LOAD_CONST               3 ('StringUtils')
-                24 PRECALL                  2
-                28 CALL                     2
-                38 STORE_NAME               2 (StringUtils)
-                40 LOAD_CONST               4 (None)
-                42 RETURN_VALUE
+     4          18 PUSH_NULL
+                20 LOAD_BUILD_CLASS
+                22 LOAD_CONST               2 (<code object StringUtils, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 4>)
+                24 MAKE_FUNCTION            0
+                26 LOAD_CONST               3 ('StringUtils')
+                28 PRECALL                  2
+                32 CALL                     2
+                42 STORE_NAME               3 (StringUtils)
+                44 LOAD_CONST               4 (None)
+                46 RETURN_VALUE
    consts
       0
-      ('Union',)
+      ('Union', 'List')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a0265036401650464026505660464038404a60000
@@ -55,75 +57,75 @@
            5          10 LOAD_NAME                3 (staticmethod)
          
            6          12 LOAD_CONST               1 ('value')
                       14 LOAD_NAME                4 (str)
                       16 LOAD_CONST               2 ('return')
                       18 LOAD_NAME                5 (bool)
                       20 BUILD_TUPLE              4
-                      22 LOAD_CONST               3 (<code object is_blank, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 5>)
+                      22 LOAD_CONST               3 (<code object is_blank, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 5>)
                       24 MAKE_FUNCTION            4 (annotations)
          
            5          26 PRECALL                  0
                       30 CALL                     0
          
            6          40 STORE_NAME               6 (is_blank)
          
            9          42 LOAD_NAME                3 (staticmethod)
          
           10          44 LOAD_CONST               1 ('value')
                       46 LOAD_NAME                4 (str)
                       48 LOAD_CONST               2 ('return')
                       50 LOAD_NAME                5 (bool)
                       52 BUILD_TUPLE              4
-                      54 LOAD_CONST               4 (<code object is_not_blank, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 9>)
+                      54 LOAD_CONST               4 (<code object is_not_blank, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 9>)
                       56 MAKE_FUNCTION            4 (annotations)
          
            9          58 PRECALL                  0
                       62 CALL                     0
          
           10          72 STORE_NAME               7 (is_not_blank)
          
           13          74 LOAD_NAME                3 (staticmethod)
          
           14          76 LOAD_CONST               5 ('input_lines')
-                      78 LOAD_NAME                8 (list)
+                      78 LOAD_NAME                8 (List)
                       80 LOAD_NAME                4 (str)
                       82 BINARY_SUBSCR
                       92 LOAD_CONST               6 ('strip_lines')
                       94 LOAD_NAME                5 (bool)
                       96 LOAD_CONST               2 ('return')
-                      98 LOAD_NAME                8 (list)
+                      98 LOAD_NAME                8 (List)
                      100 LOAD_NAME                4 (str)
                      102 BINARY_SUBSCR
                      112 BUILD_TUPLE              6
-                     114 LOAD_CONST               7 (<code object strip_lines, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 13>)
+                     114 LOAD_CONST               7 (<code object strip_lines, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 13>)
                      116 MAKE_FUNCTION            4 (annotations)
          
           13         118 PRECALL                  0
                      122 CALL                     0
          
           14         132 STORE_NAME               9 (strip_lines)
          
           23         134 LOAD_NAME                3 (staticmethod)
          
           24         136 LOAD_CONST              16 ((False,))
                      138 LOAD_CONST               9 ('text')
                      140 LOAD_NAME               10 (Union)
                      142 LOAD_NAME                4 (str)
-                     144 LOAD_NAME                8 (list)
+                     144 LOAD_NAME                8 (List)
                      146 LOAD_NAME                4 (str)
                      148 BINARY_SUBSCR
                      158 BUILD_TUPLE              2
                      160 BINARY_SUBSCR
                      170 LOAD_CONST              10 ('left_strip_lines')
                      172 LOAD_NAME                5 (bool)
                      174 LOAD_CONST               2 ('return')
                      176 LOAD_NAME               11 (int)
                      178 BUILD_TUPLE              6
-                     180 LOAD_CONST              11 (<code object count_max_text_width, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 23>)
+                     180 LOAD_CONST              11 (<code object count_max_text_width, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 23>)
                      182 MAKE_FUNCTION            5 (defaults, annotations)
          
           23         184 PRECALL                  0
                      188 CALL                     0
          
           24         198 STORE_NAME              12 (count_max_text_width)
          
@@ -134,15 +136,15 @@
                      206 LOAD_CONST              12 ('left_strip')
                      208 LOAD_NAME                5 (bool)
                      210 LOAD_CONST              13 ('right_strip')
                      212 LOAD_NAME                5 (bool)
                      214 LOAD_CONST               2 ('return')
                      216 LOAD_NAME                4 (str)
                      218 BUILD_TUPLE              8
-                     220 LOAD_CONST              14 (<code object strip, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 31>)
+                     220 LOAD_CONST              14 (<code object strip, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 31>)
                      222 MAKE_FUNCTION            4 (annotations)
          
           31         224 PRECALL                  0
                      228 CALL                     0
          
           32         238 STORE_NAME              13 (strip)
                      240 LOAD_CONST              15 (None)
@@ -171,15 +173,15 @@
                             46 RETURN_VALUE
                consts
                   None
                names      ('strip',)
                varnames   ('value',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                name       'is_blank'
                firstlineno 5
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -202,15 +204,15 @@
                             70 RETURN_VALUE
                consts
                   None
                names      ('bool', 'strip')
                varnames   ('value',)
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                name       'is_not_blank'
                firstlineno 9
                lnotab 0x0202
             'input_lines'
             'strip_lines'
             code
                argcount  : 2
@@ -267,15 +269,15 @@
                consts
                   None
                   '\n'
                names      ('split', 'strip', 'append')
                varnames   ('input_lines', 'strip_lines', 'result', 'line', 'row')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                name       'strip_lines'
                firstlineno 13
                lnotab 0x0202040108012e01040128012cfd0204
             False
             'text'
             'left_strip_lines'
             code
@@ -304,15 +306,15 @@
                             30 PRECALL                  2
                             34 CALL                     2
                             44 POP_JUMP_FORWARD_IF_FALSE    46 (to 138)
                
                 26          46 LOAD_GLOBAL              5 (NULL + max)
                             58 LOAD_CLOSURE             1 (left_strip_lines)
                             60 BUILD_TUPLE              1
-                            62 LOAD_CONST               1 (<code object <listcomp>, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 26>)
+                            62 LOAD_CONST               1 (<code object <listcomp>, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 26>)
                             64 MAKE_FUNCTION            8 (closure)
                             66 LOAD_FAST                0 (text)
                             68 LOAD_METHOD              3 (split)
                             90 LOAD_CONST               2 ('\n')
                             92 PRECALL                  1
                             96 CALL                     1
                            106 GET_ITER
@@ -328,15 +330,15 @@
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_JUMP_FORWARD_IF_FALSE    27 (to 234)
                
                 28         180 LOAD_GLOBAL              5 (NULL + max)
                            192 LOAD_CLOSURE             1 (left_strip_lines)
                            194 BUILD_TUPLE              1
-                           196 LOAD_CONST               3 (<code object <listcomp>, file "/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py", line 28>)
+                           196 LOAD_CONST               3 (<code object <listcomp>, file "/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py", line 28>)
                            198 MAKE_FUNCTION            8 (closure)
                            200 LOAD_FAST                0 (text)
                            202 GET_ITER
                            204 PRECALL                  0
                            208 CALL                     0
                            218 PRECALL                  1
                            222 CALL                     1
@@ -387,15 +389,15 @@
                              >>   96 RETURN_VALUE
                      consts
                         True
                      names      ('len', 'StringUtils', 'strip')
                      varnames   ('.0', 'line')
                      freevars   ('left_strip_lines',)
                      cellvars   ()
-                     filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+                     filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                      name       '<listcomp>'
                      firstlineno 26
                      lnotab 0x
                   '\n'
                   code
                      argcount  : 1
                      nlocals   : 2
@@ -422,24 +424,24 @@
                                   66 JUMP_BACKWARD           30 (to 8)
                              >>   68 RETURN_VALUE
                      consts
                      names      ('StringUtils', 'count_max_text_width')
                      varnames   ('.0', 'line')
                      freevars   ('left_strip_lines',)
                      cellvars   ()
-                     filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+                     filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                      name       '<listcomp>'
                      firstlineno 28
                      lnotab 0x
                   'Wrong input type. Required: Union[str, list[str]]. Actual: '
                names      ('isinstance', 'str', 'max', 'split', 'list', 'ValueError', 'type')
                varnames   ('text', 'left_strip_lines')
                freevars   ()
                cellvars   ('left_strip_lines',)
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                name       'count_max_text_width'
                firstlineno 23
                lnotab 0x04022a015c012a013601
             'left_strip'
             'right_strip'
             code
                argcount  : 3
@@ -475,33 +477,33 @@
                             92 RETURN_VALUE
                consts
                   None
                names      ('lstrip', 'rstrip')
                varnames   ('text', 'left_strip', 'right_strip')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+               filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
                name       'strip'
                firstlineno 31
                lnotab 0x02020401280104012801
             None
             (False,)
-         names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'str', 'bool', 'is_blank', 'is_not_blank', 'list', 'strip_lines', 'Union', 'int', 'count_max_text_width', 'strip')
+         names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'str', 'bool', 'is_blank', 'is_not_blank', 'List', 'strip_lines', 'Union', 'int', 'count_max_text_width', 'strip')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+         filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
          name       'StringUtils'
          firstlineno 4
          lnotab
             0x0a0102010eff0e01020302010eff0e01020302012aff0e010209020130
             ff0e010207020116ff0e01
       'StringUtils'
       None
-   names      ('typing', 'Union', 'StringUtils')
+   names      ('typing', 'Union', 'List', 'StringUtils')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/CalendarView/CalendarView/calendar_view/core/utils.py'
+   filename   '/home/runner/work/calendar-view/calendar-view/calendar_view/core/utils.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c03
+   lnotab 0x00ff02011003
```

### Comparing `calendar-view-2.3.0/calendar_view/core/calendar_events.py` & `calendar-view-2.3.1/calendar_view/core/calendar_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from calendar_view.core.utils import StringUtils
 
 
 class MultilineTextMetadata(object):
     """
     The required information to draw the text (title or notes) for the event.
     """
-    def __init__(self, text: Optional[str] = None, size: tuple[int, int] = (0, 0)):
+    def __init__(self, text: Optional[str] = None, size: Tuple[int, int] = (0, 0)):
         self.text: Optional[str] = text
-        self.size: tuple[int, int] = size
+        self.size: Tuple[int, int] = size
         self.visible: bool = text is not None and size[0] > 0 and size[1] > 0
         # self.trimmed: bool = False
 
     def __repr__(self) -> str:
         return f'MultilineTextMetadata[visible: {self.visible}, size: {self.size}, text: {self.text}]'
 
 
@@ -149,21 +149,21 @@
         p2 = (x2, y[1])
         draw_rounded_rectangle(self.event_draw, [p1, p2], style.event_radius, outline=event.style.event_border,
                                fill=event.style.event_fill, width=style.event_border_width)
 
         if self.config.legend:
             return  # The title and notes are printed in the legend. Skip drawing here.
 
-        cell_inner_size: tuple[int, int] = EventDrawHelper.count_cell_inner_size(x, y)
+        cell_inner_size: Tuple[int, int] = EventDrawHelper.count_cell_inner_size(x, y)
         if cell_inner_size[0] == 0 or cell_inner_size[1] == 0:
             return  # not possible to draw nothing inside the event cell
 
         # calculate text block sizes
         title_metadata: MultilineTextMetadata = EventDrawHelper.build_title_metadata(event.title, cell_inner_size)
-        notes_inner_size: tuple[int, int] = (
+        notes_inner_size: Tuple[int, int] = (
             cell_inner_size[0],
             cell_inner_size[1] - (title_metadata.size[1] + style.event_title_margin if title_metadata.visible else 0)
         )
         notes_metadata: MultilineTextMetadata = EventDrawHelper.build_notes_metadata(event.notes, notes_inner_size)
 
         total_height: int = EventDrawHelper.count_final_text_height(title_metadata, notes_metadata)
         y_top_offset: int = y[0] + style.event_padding
@@ -171,15 +171,15 @@
         if title_metadata.visible:
             # calculate the top position of the title multiline text block
             y_text_offset: int = EventDrawHelper.calculate_text_y_position_offset(self.config.title_vertical_align,
                                                                                   box_height=cell_inner_size[1],
                                                                                   text_height=title_metadata.size[1],
                                                                                   total_text_height=total_height)
             # the top-left position of the title block
-            title_pos: tuple[int, int] = (
+            title_pos: Tuple[int, int] = (
                 (p1[0] + p2[0]) / 2 - title_metadata.size[0] / 2,
                 y_top_offset + y_text_offset
             )
             self.event_draw.multiline_text(title_pos, title_metadata.text, align='center',
                                            font=style.event_title_font, fill=style.event_title_color)
             # update offset for notes
             y_top_offset = title_pos[1] + title_metadata.size[1] + style.event_title_margin
@@ -190,15 +190,15 @@
             if not title_metadata.visible:
                 # if the title is not visible, calculate the top-left position of the notes multiline text block
                 y_text_offset = EventDrawHelper.calculate_text_y_position_offset(self.config.title_vertical_align,
                                                                                  box_height=cell_inner_size[1],
                                                                                  text_height=notes_metadata.size[1],
                                                                                  total_text_height=total_height)
             # the top-left position of the notes block
-            notes_pos: tuple[int, int] = (
+            notes_pos: Tuple[int, int] = (
                 p1[0] + style.event_padding,
                 y_top_offset + y_text_offset
             )
             self.event_draw.multiline_text(notes_pos, notes_metadata.text, align='left',
                                            font=style.event_notes_font, fill=style.event_notes_color)
 
     def destroy(self):
@@ -270,15 +270,15 @@
     def __get_event_x(day_number: int):
         x_start = style.padding_horizontal + day_number * style.day_width
         return x_start, x_start + style.day_width
 
 
 class EventDrawHelper:
     @staticmethod
-    def count_cell_inner_size(x: tuple[float, float], y: tuple[float, float]) -> tuple[int, int]:
+    def count_cell_inner_size(x: Tuple[float, float], y: Tuple[float, float]) -> Tuple[int, int]:
         return (
             max(0, int(x[1] - x[0] - 2 * style.line_day_width) - 2 * style.event_padding),
             max(0, int(y[1] - y[0] - 2 * style.line_day_width) - 2 * style.event_padding)
         )
 
     @staticmethod
     def count_final_text_height(title: MultilineTextMetadata, notes: MultilineTextMetadata) -> int:
@@ -289,22 +289,22 @@
         if title.visible:
             height += title.size[1]
         if notes.visible:
             height += notes.size[1]
         return height
 
     @staticmethod
-    def build_title_metadata(title: Optional[str], cell_inner_size: tuple[int, int]) -> MultilineTextMetadata:
+    def build_title_metadata(title: Optional[str], cell_inner_size: Tuple[int, int]) -> MultilineTextMetadata:
         """
         Try to fit the title in the event inner cell. Split the text into the multiple lines if required.
         """
         return EventDrawHelper.__build_text_metadata(title, cell_inner_size, style.event_title_font, True)
 
     @staticmethod
-    def build_notes_metadata(notes: Optional[str], notes_inner_size: tuple[int, int]) -> MultilineTextMetadata:
+    def build_notes_metadata(notes: Optional[str], notes_inner_size: Tuple[int, int]) -> MultilineTextMetadata:
         """
         Try to fit notes in the event inner cell. Split the text into the multiple lines if required.
         """
         return EventDrawHelper.__build_text_metadata(notes, notes_inner_size, style.event_notes_font, False)
 
     @staticmethod
     def calculate_text_y_position_offset(vertical_align: VerticalAlign, box_height: int, text_height: int,
@@ -321,36 +321,36 @@
         if vertical_align == 'center':
             return int(box_height / 2 - text_height / 2)
         if vertical_align == 'bottom':
             return max(0, box_height - total_text_height)
         raise RuntimeError(f'Wrong vertical align value: {vertical_align}')
 
     @staticmethod
-    def __build_text_metadata(text: Optional[str], box_size: tuple[int, int], font: FreeTypeFont, strip_lines: bool) \
+    def __build_text_metadata(text: Optional[str], box_size: Tuple[int, int], font: FreeTypeFont, strip_lines: bool) \
             -> MultilineTextMetadata:
         """
         Try to fit text in the given box. Split the text into the multiple lines if required.
         """
         if not text or len(text.strip()) == 0:
             return MultilineTextMetadata()
         if box_size[0] <= 0 or box_size[1] <= 0:
             return MultilineTextMetadata()
 
         text = text.strip()
-        text_size: tuple[int, int] = font.getsize_multiline(text)
+        text_size: Tuple[int, int] = font.getsize_multiline(text)
         if EventDrawHelper.__fits_the_borders(text_size, box_size):
             return MultilineTextMetadata(text, text_size)
         elif EventDrawHelper.__fits_the_width(text_size, box_size):
             return MultilineTextMetadata(text, text_size)
 
         max_width: int = StringUtils.count_max_text_width(text, strip_lines)
         base_new_text_width: int = int(box_size[0] * max_width / text_size[0])
 
         new_text: str = ''
-        new_text_size: tuple[int, int] = (0, 0)
+        new_text_size: Tuple[int, int] = (0, 0)
         for retry_count in range(0, 12, 2):
             new_test_width: int = base_new_text_width - retry_count
             if new_test_width <= 0:
                 return MultilineTextMetadata(text, text_size)  # no place to fit the text
 
             lines: list[str] = textwrap.wrap(text, width=new_test_width, replace_whitespace=False)
             lines = StringUtils.strip_lines(lines, strip_lines)
@@ -360,13 +360,13 @@
                 return MultilineTextMetadata(new_text, new_text_size)
             elif EventDrawHelper.__fits_the_width(new_text_size, box_size):
                 return MultilineTextMetadata(new_text, new_text_size)
         raise RuntimeError('Not possible to wrap the text to fit the width.')
         # textwrap.shorten(title, width=20, placeholder=' ...')
 
     @staticmethod
-    def __fits_the_borders(size: tuple[int, int], border: tuple[int, int]) -> bool:
+    def __fits_the_borders(size: Tuple[int, int], border: Tuple[int, int]) -> bool:
         return size[0] <= border[0] and size[1] <= border[1]
 
     @staticmethod
-    def __fits_the_width(size: tuple[int, int], border: tuple[int, int]) -> bool:
+    def __fits_the_width(size: Tuple[int, int], border: Tuple[int, int]) -> bool:
         return size[0] <= border[0]
```

### Comparing `calendar-view-2.3.0/calendar_view/core/calendar_grid.py` & `calendar-view-2.3.1/calendar_view/core/calendar_grid.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/config.py` & `calendar-view-2.3.1/calendar_view/core/config.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/data.py` & `calendar-view-2.3.1/calendar_view/core/data.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/event.py` & `calendar-view-2.3.1/calendar_view/core/event.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/round_rectangle.py` & `calendar-view-2.3.1/calendar_view/core/round_rectangle.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/time_utils.py` & `calendar-view-2.3.1/calendar_view/core/time_utils.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/core/utils.py` & `calendar-view-2.3.1/calendar_view/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Union
+from typing import Union, List
 
 
 class StringUtils:
     @staticmethod
     def is_blank(value: str) -> bool:
         return not (value and value.strip())
 
     @staticmethod
     def is_not_blank(value: str) -> bool:
         return bool(value and value.strip())
 
     @staticmethod
-    def strip_lines(input_lines: list[str], strip_lines: bool) -> list[str]:
+    def strip_lines(input_lines: List[str], strip_lines: bool) -> List[str]:
         result: list[str] = []
         for line in input_lines:
             for row in line.split('\n'):
                 if strip_lines:
                     row = row.strip()
                 result.append(row)
         return result
 
     @staticmethod
-    def count_max_text_width(text: Union[str, list[str]], left_strip_lines: bool = False) -> int:
+    def count_max_text_width(text: Union[str, List[str]], left_strip_lines: bool = False) -> int:
         if isinstance(text, str):
             return max([len(StringUtils.strip(line, left_strip_lines, True)) for line in text.split('\n')])
         if isinstance(text, list):
             return max([StringUtils.count_max_text_width(line, left_strip_lines) for line in text])
         raise ValueError(f'Wrong input type. Required: Union[str, list[str]]. Actual: {type(text)}')
 
     @staticmethod
```

### Comparing `calendar-view-2.3.0/calendar_view/resources/fonts/LICENSE.txt` & `calendar-view-2.3.1/calendar_view/resources/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view/resources/fonts/Roboto-Regular.ttf` & `calendar-view-2.3.1/calendar_view/resources/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/calendar_view.egg-info/PKG-INFO` & `calendar-view-2.3.1/calendar_view.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-view
-Version: 2.3.0
+Version: 2.3.1
 Summary: Library provides a graphical view of the calendar.
 Home-page: https://github.com/sakhnevych/calendar-view
 Author: Oleksandr Sakhnevych, Daniil Limariev
 Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `calendar-view-2.3.0/calendar_view.egg-info/SOURCES.txt` & `calendar-view-2.3.1/calendar_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/setup.py` & `calendar-view-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="calendar-view",
-    version="2.3.0",
+    version="2.3.1",
     author="Oleksandr Sakhnevych, Daniil Limariev",
     author_email="o.sakhnevych@gmail.com, danillim02102003@gmail.com",
     description="Library provides a graphical view of the calendar.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/sakhnevych/calendar-view",
     packages=setuptools.find_packages(),
```

### Comparing `calendar-view-2.3.0/tests/test_calendar_config.py` & `calendar-view-2.3.1/tests/test_calendar_config.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.3.0/tests/test_time_utils.py` & `calendar-view-2.3.1/tests/test_time_utils.py`

 * *Files identical despite different names*

