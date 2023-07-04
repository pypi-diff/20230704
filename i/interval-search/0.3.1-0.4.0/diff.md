# Comparing `tmp/interval-search-0.3.1.tar.gz` & `tmp/interval-search-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval-search-0.3.1.tar", last modified: Tue Feb 21 13:30:32 2023, max compression
+gzip compressed data, was "interval-search-0.4.0.tar", last modified: Tue Jul  4 01:51:15 2023, max compression
```

## Comparing `interval-search-0.3.1.tar` & `interval-search-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 13:30:32.278959 interval-search-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-21 13:30:20.000000 interval-search-0.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-02-21 13:30:20.000000 interval-search-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-21 13:30:20.000000 interval-search-0.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-21 13:30:20.000000 interval-search-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-21 13:30:20.000000 interval-search-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-02-21 13:30:32.278959 interval-search-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-21 13:30:20.000000 interval-search-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 13:30:32.274959 interval-search-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-21 13:30:20.000000 interval-search-0.3.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 13:30:32.274959 interval-search-0.3.1/interval_search/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-21 13:30:20.000000 interval-search-0.3.1/interval_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-21 13:30:20.000000 interval-search-0.3.1/interval_search/binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-02-21 13:30:20.000000 interval-search-0.3.1/interval_search/curried_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-02-21 13:30:20.000000 interval-search-0.3.1/interval_search/curried_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-21 13:30:20.000000 interval-search-0.3.1/interval_search/doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-21 13:30:20.000000 interval-search-0.3.1/interval_search/interval_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 13:30:32.278959 interval-search-0.3.1/interval_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-02-21 13:30:32.000000 interval-search-0.3.1/interval_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-21 13:30:32.000000 interval-search-0.3.1/interval_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 13:30:32.000000 interval-search-0.3.1/interval_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 13:30:32.000000 interval-search-0.3.1/interval_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-21 13:30:32.000000 interval-search-0.3.1/interval_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-21 13:30:32.282959 interval-search-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-21 13:30:20.000000 interval-search-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 13:30:32.278959 interval-search-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-21 13:30:20.000000 interval-search-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-21 13:30:20.000000 interval-search-0.3.1/tests/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-21 13:30:20.000000 interval-search-0.3.1/tests/test_curried_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-21 13:30:20.000000 interval-search-0.3.1/tests/test_curried_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-21 13:30:20.000000 interval-search-0.3.1/tests/test_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-02-21 13:30:20.000000 interval-search-0.3.1/tests/test_interval_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:51:15.698355 interval-search-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 01:50:55.000000 interval-search-0.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-04 01:50:55.000000 interval-search-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 01:50:55.000000 interval-search-0.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 01:50:55.000000 interval-search-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 01:50:55.000000 interval-search-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 01:51:15.698355 interval-search-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 01:50:55.000000 interval-search-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:51:15.694354 interval-search-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 01:50:55.000000 interval-search-0.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:51:15.698355 interval-search-0.4.0/interval_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/curried_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/curried_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/curried_binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/curried_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 01:50:55.000000 interval-search-0.4.0/interval_search/interval_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:51:15.698355 interval-search-0.4.0/interval_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 01:51:15.000000 interval-search-0.4.0/interval_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 01:51:15.000000 interval-search-0.4.0/interval_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:51:15.000000 interval-search-0.4.0/interval_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:51:15.000000 interval-search-0.4.0/interval_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 01:51:15.000000 interval-search-0.4.0/interval_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 01:51:15.698355 interval-search-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-04 01:50:55.000000 interval-search-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:51:15.698355 interval-search-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_curried_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_curried_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_curried_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 01:50:55.000000 interval-search-0.4.0/tests/test_interval_search.py
```

### Comparing `interval-search-0.3.1/CONTRIBUTING.rst` & `interval-search-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/LICENSE` & `interval-search-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/PKG-INFO` & `interval-search-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: interval-search
-Version: 0.3.1
+Version: 0.4.0
 Summary: interval-search provides predicate-based binary and doubling search implementations
 Home-page: https://github.com/mmore500/interval-search
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Description: ===============
         interval-search
```

### Comparing `interval-search-0.3.1/README.rst` & `interval-search-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/docs/Makefile` & `interval-search-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/docs/conf.py` & `interval-search-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/docs/installation.rst` & `interval-search-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/docs/make.bat` & `interval-search-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/interval_search/binary_search.py` & `interval-search-0.4.0/interval_search/binary_search_iterative.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 
-from .curried_binary_search import curried_binary_search
+from .curried_binary_search_iterative import curried_binary_search_iterative
 
-def binary_search(
+
+def binary_search_iterative(
     predicate: typing.Callable[[int], bool],
     lower_bound: int,
     upper_bound: int,
 ) -> typing.Optional[int]:
     """Find the positive integer threshold below which a search criteria is
     never satisfied and above which it is always satisfied.
 
@@ -23,8 +24,8 @@
     -------
     guess
         The lowest integer value that satisfies the search criteria, and None
         if upper_bound does not satisfy the search criteria or search range is
         empty (i.e., lower_bound > upper_bound).
     """
 
-    return curried_binary_search(predicate)(lower_bound, upper_bound)
+    return curried_binary_search_iterative(predicate)(lower_bound, upper_bound)
```

### Comparing `interval-search-0.3.1/interval_search/curried_binary_search.py` & `interval-search-0.4.0/interval_search/curried_binary_search_recursive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 
-def curried_binary_search(
+def curried_binary_search_recursive(
     predicate: typing.Callable[[int], bool],
     decorate_with: typing.Callable[
         [typing.Callable], typing.Callable
     ] = lambda x: x,
 ) -> typing.Callable[[int, int], typing.Optional[int]]:
     """Find the positive integer threshold below which a search criteria is
     never satisfied and above which it is always satisfied.
@@ -30,15 +30,15 @@
         that satisfies the search criteria.
 
         If no value satisfies the search criteria, the curried search function
         will return None.
     """
 
     @decorate_with
-    def binary_search(
+    def binary_search_recursive(
         lower_bound: int,
         upper_bound: int,
     ) -> typing.Optional[int]:
         """Find the positive integer threshold below which a search criteria is
         never satisfied and above which it is always satisfied.
 
         Parameters
@@ -63,12 +63,12 @@
                 return lower_bound
             else:
                 return None
 
         midpoint = (lower_bound + upper_bound) // 2
 
         if predicate(midpoint):
-            return binary_search(lower_bound, midpoint)
+            return binary_search_recursive(lower_bound, midpoint)
         else:
-            return binary_search(midpoint + 1, upper_bound)
+            return binary_search_recursive(midpoint + 1, upper_bound)
 
-    return binary_search
+    return binary_search_recursive
```

### Comparing `interval-search-0.3.1/interval_search/curried_doubling_search.py` & `interval-search-0.4.0/interval_search/curried_doubling_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 
-from .binary_search import binary_search
+from .binary_search_iterative import binary_search_iterative
 
 
 def curried_doubling_search(
     predicate: typing.Callable[[int], bool],
     decorate_with: typing.Callable[
         [typing.Callable], typing.Callable
     ] = lambda x: x,
@@ -53,10 +53,12 @@
 
         bound = 1
         while not predicate(lower_bound + bound):
             bound *= 2
 
         prev_bound = bound // 2
         prev_guess = lower_bound + prev_bound
-        return binary_search(predicate, prev_guess, lower_bound + bound)
+        return binary_search_iterative(
+            predicate, prev_guess, lower_bound + bound
+        )
 
     return doubling_search
```

### Comparing `interval-search-0.3.1/interval_search/doubling_search.py` & `interval-search-0.4.0/interval_search/doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/interval_search/interval_search.py` & `interval-search-0.4.0/interval_search/interval_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 
-from .binary_search import binary_search
+from .binary_search_iterative import binary_search_iterative
 from .doubling_search import doubling_search
 
 
 def interval_search(
     predicate: typing.Callable[[int], bool],
     lower_bound: int=0,
     upper_bound: typing.Optional[int]=None,
@@ -31,12 +31,12 @@
         if upper_bound does not satisfy the search criteria or search range is
         empty (i.e., lower_bound > upper_bound).
     """
 
     return doubling_search(
         predicate,
         lower_bound,
-    ) if upper_bound is None else binary_search(
+    ) if upper_bound is None else binary_search_iterative(
         predicate,
         lower_bound,
         upper_bound,
     )
```

### Comparing `interval-search-0.3.1/interval_search.egg-info/PKG-INFO` & `interval-search-0.4.0/interval_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: interval-search
-Version: 0.3.1
+Version: 0.4.0
 Summary: interval-search provides predicate-based binary and doubling search implementations
 Home-page: https://github.com/mmore500/interval-search
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Description: ===============
         interval-search
```

### Comparing `interval-search-0.3.1/interval_search.egg-info/SOURCES.txt` & `interval-search-0.4.0/interval_search.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,22 +14,29 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 interval_search/__init__.py
 interval_search/binary_search.py
+interval_search/binary_search_iterative.py
+interval_search/binary_search_recursive.py
 interval_search/curried_binary_search.py
+interval_search/curried_binary_search_iterative.py
+interval_search/curried_binary_search_recursive.py
 interval_search/curried_doubling_search.py
 interval_search/doubling_search.py
 interval_search/interval_search.py
 interval_search.egg-info/PKG-INFO
 interval_search.egg-info/SOURCES.txt
 interval_search.egg-info/dependency_links.txt
 interval_search.egg-info/not-zip-safe
 interval_search.egg-info/top_level.txt
 tests/__init__.py
 tests/test_binary_search.py
+tests/test_binary_search_iterative.py
+tests/test_binary_search_recursive.py
 tests/test_curried_binary_search.py
+tests/test_curried_binary_search_iterative.py
 tests/test_curried_doubling_search.py
 tests/test_doubling_search.py
 tests/test_interval_search.py
```

### Comparing `interval-search-0.3.1/setup.py` & `interval-search-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords='interval-search',
     name='interval-search',
     packages=find_packages(include=['interval_search', 'interval_search.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mmore500/interval-search',
-    version='0.3.1',
+    version='0.4.0',
     zip_safe=False,
 )
```

### Comparing `interval-search-0.3.1/tests/test_binary_search.py` & `interval-search-0.4.0/tests/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/tests/test_curried_binary_search.py` & `interval-search-0.4.0/tests/test_curried_binary_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/tests/test_curried_doubling_search.py` & `interval-search-0.4.0/tests/test_curried_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/tests/test_doubling_search.py` & `interval-search-0.4.0/tests/test_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.3.1/tests/test_interval_search.py` & `interval-search-0.4.0/tests/test_interval_search.py`

 * *Files identical despite different names*

