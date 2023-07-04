# Comparing `tmp/mykit-5.1.0.tar.gz` & `tmp/mykit-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-eyp075i2/mykit-5.1.0.tar", last modified: Mon Jul  3 10:57:44 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-shk2fh36/mykit-5.2.0.tar", last modified: Tue Jul  4 06:15:37 2023, max compression
```

## Comparing `mykit-5.1.0.tar` & `mykit-5.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 10:57:23.000000 mykit-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-03 10:57:44.000000 mykit-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-03 10:57:23.000000 mykit-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/app/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/architecture/eventdriven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/rec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/rec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:23.000000 mykit-5.1.0/mykit/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:57:44.000000 mykit-5.1.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-03 10:57:23.000000 mykit-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 10:57:44.000000 mykit-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 10:57:23.000000 mykit-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-04 06:15:17.000000 mykit-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-04 06:15:37.000000 mykit-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 06:15:17.000000 mykit-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/rec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/rec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:17.000000 mykit-5.2.0/mykit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 06:15:37.000000 mykit-5.2.0/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 06:15:17.000000 mykit-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 06:15:37.000000 mykit-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 06:15:17.000000 mykit-5.2.0/setup.py
```

### Comparing `mykit-5.1.0/LICENSE` & `mykit-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/PKG-INFO` & `mykit-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 5.1.0
+Version: 5.2.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-5.1.0/README.md` & `mykit-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/__init__.py` & `mykit-5.2.0/mykit/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/__main__.py` & `mykit-5.2.0/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/__init__.py` & `mykit-5.2.0/mykit/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tkinter as _tk
 from typing import (
     Any as _Any,
     Callable as _Callable,
+    Dict as _Dict,
     List as _List,
 )
 
 from mykit.app.button import Button as _Button
 from mykit.app.label import Label as _Label
 from mykit.app.slider import _Slider
 
@@ -120,16 +121,16 @@
         self._background_processes[every].append(do)
 
     def setup(self, funcs: _List[_Callable[[], None]]):
         self._setup = funcs
 
     def teardown(self, funcs: _List[_Callable[[], None]]):
         self._teardown = funcs
-    
-    def use(self, component: _Callable[..., None], /, dependencies: dict[str, _Any]) -> None:
+
+    def use(self, component: _Callable[..., None], /, dependencies: _Dict[str, _Any]) -> None:
         component(**dependencies)
 
     def run(self):
 
         ## <internal>
 
         self.listen(to='left-mouse-press', do=_Button._press_listener)
```

### Comparing `mykit-5.1.0/mykit/app/architecture/eventdriven.py` & `mykit-5.2.0/mykit/app/architecture/eventdriven.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/arrow.py` & `mykit-5.2.0/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/button.py` & `mykit-5.2.0/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/complex/biplot.py` & `mykit-5.2.0/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/complex/plot.py` & `mykit-5.2.0/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/label.py` & `mykit-5.2.0/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/app/slider.py` & `mykit-5.2.0/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/color.py` & `mykit-5.2.0/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-5.2.0/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/ffmpeg.py` & `mykit-5.2.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/keycrate/__init__.py` & `mykit-5.2.0/mykit/kit/keycrate/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re as _re
 import os as _os
 from typing import (
     Any as _Any,
     Dict as _Dict,
     List as _List,
     NoReturn as _NoReturn,
-    Optional as _Optional
+    Tuple as _Tuple,
+    Union as _Union
 )
 
 from mykit.kit.path import open_file as _open_file
 from mykit.kit.utils import is_valid_var_name as _is_valid_var_name
 
 
 class KeyCrate:
@@ -20,16 +21,16 @@
 
     def __init__(
         self,
         file_pth: str,
         /,
         key_is_var: bool = False,
         eval_value: bool = False,
-        only_keys: _Optional[_List[str]] = None,
-        need_keys: _Optional[_List[str]] = None
+        only_keys: _Union[_List[str], _Tuple[str, ...], None] = None,
+        need_keys: _Union[_List[str], _Tuple[str, ...], None] = None
     ) -> None:
         """
         Storing key-value pairs (key: value) in the .txt file `file_pth`.
         Access the value using either the class-like way (`kc.key`)
         or the dictionary-like way (`kc['key']`).
 
         ---
@@ -62,20 +63,29 @@
         if not file_pth.endswith('.txt'):
             raise ValueError(f'KeyCrate file {repr(file_pth)} should be a .txt file.')
 
         ## keycrate file must exist
         if not _os.path.isfile(file_pth):
             raise FileNotFoundError(f'KeyCrate file {repr(file_pth)} is not found.')
 
+
         ## added the prefix "_kc__" to prevent conflicts with the keys
+
         self._kc__file_pth = file_pth
         self._kc__key_is_var = key_is_var
         self._kc__eval_value = eval_value
+
         self._kc__only_keys = only_keys
+        if type(only_keys) is tuple:
+            self._kc__only_keys = list(only_keys)
+
         self._kc__need_keys = need_keys
+        if type(need_keys) is tuple:
+            self._kc__need_keys = list(need_keys)
+
 
         ## init
         self.parse()
 
     def __getattr__(self, __name: str, __default: _Any = None, /) -> _NoReturn:
         """This method is called when attribute `__name` is not found"""
         raise AttributeError(f'KeyCrate file {repr(self._kc__file_pth)} does not have key {repr(__name)}.')
```

### Comparing `mykit-5.1.0/mykit/kit/math.py` & `mykit-5.2.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/neuralnet/dense.py` & `mykit-5.2.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/neuralnet/genetic.py` & `mykit-5.2.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/noise.py` & `mykit-5.2.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/path.py` & `mykit-5.2.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/time.py` & `mykit-5.2.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit/kit/utils.py` & `mykit-5.2.0/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/mykit.egg-info/PKG-INFO` & `mykit-5.2.0/mykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 5.1.0
+Version: 5.2.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-5.1.0/mykit.egg-info/SOURCES.txt` & `mykit-5.2.0/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-5.1.0/pyproject.toml` & `mykit-5.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "5.1.0"
+version = "5.2.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

