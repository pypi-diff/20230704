# Comparing `tmp/interval-search-0.5.0.tar.gz` & `tmp/interval-search-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval-search-0.5.0.tar", last modified: Tue Jul  4 02:17:24 2023, max compression
+gzip compressed data, was "interval-search-0.5.1.tar", last modified: Tue Jul  4 05:48:30 2023, max compression
```

## Comparing `interval-search-0.5.0.tar` & `interval-search-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:17:24.988744 interval-search-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 02:17:10.000000 interval-search-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-04 02:17:10.000000 interval-search-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 02:17:10.000000 interval-search-0.5.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 02:17:10.000000 interval-search-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 02:17:10.000000 interval-search-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 02:17:24.988744 interval-search-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 02:17:10.000000 interval-search-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:17:24.988744 interval-search-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 02:17:10.000000 interval-search-0.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:17:24.988744 interval-search-0.5.0/interval_search/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/binary_search_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/curried_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/curried_binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/curried_binary_search_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/curried_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 02:17:10.000000 interval-search-0.5.0/interval_search/interval_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:17:24.988744 interval-search-0.5.0/interval_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 02:17:24.000000 interval-search-0.5.0/interval_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 02:17:24.000000 interval-search-0.5.0/interval_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 02:17:24.000000 interval-search-0.5.0/interval_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 02:17:24.000000 interval-search-0.5.0/interval_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 02:17:24.000000 interval-search-0.5.0/interval_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 02:17:24.988744 interval-search-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-04 02:17:10.000000 interval-search-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 02:17:24.988744 interval-search-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_binary_search_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_curried_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_curried_binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_curried_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 02:17:10.000000 interval-search-0.5.0/tests/test_interval_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.800614 interval-search-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 05:48:19.000000 interval-search-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-04 05:48:19.000000 interval-search-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 05:48:19.000000 interval-search-0.5.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 05:48:19.000000 interval-search-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 05:48:19.000000 interval-search-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 05:48:30.800614 interval-search-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 05:48:19.000000 interval-search-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.796615 interval-search-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.796615 interval-search-0.5.1/interval_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/interval_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.796615 interval-search-0.5.1/interval_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 05:48:30.800614 interval-search-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-04 05:48:19.000000 interval-search-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.800614 interval-search-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_curried_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_curried_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_curried_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_interval_search.py
```

### Comparing `interval-search-0.5.0/CONTRIBUTING.rst` & `interval-search-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/LICENSE` & `interval-search-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/PKG-INFO` & `interval-search-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: interval-search
-Version: 0.5.0
+Version: 0.5.1
 Summary: interval-search provides predicate-based binary and doubling search implementations
 Home-page: https://github.com/mmore500/interval-search
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Description: ===============
         interval-search
```

### Comparing `interval-search-0.5.0/README.rst` & `interval-search-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/docs/Makefile` & `interval-search-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/docs/conf.py` & `interval-search-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/docs/installation.rst` & `interval-search-0.5.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/docs/make.bat` & `interval-search-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/interval_search/__init__.py` & `interval-search-0.5.1/interval_search/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for interval_search."""
 
 __author__ = """Matthew Andres Moreno"""
 __email__ = 'm.more500@gmail.com'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 from .binary_search import binary_search
 from .binary_search_iterative import binary_search_iterative
 from .binary_search_recursive import binary_search_recursive
 from .curried_binary_search import curried_binary_search
 from .curried_binary_search_iterative import curried_binary_search_iterative
 from .curried_binary_search_recursive import curried_binary_search_recursive
```

### Comparing `interval-search-0.5.0/interval_search/binary_search_iterative.py` & `interval-search-0.5.1/interval_search/binary_search_iterative.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/interval_search/binary_search_recursive.py` & `interval-search-0.5.1/interval_search/binary_search_recursive.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/interval_search/curried_binary_search_iterative.py` & `interval-search-0.5.1/interval_search/curried_binary_search_iterative.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         # Check if the range is invalid.
         if lower_bound > upper_bound:
             return None
 
         # Loop until lower_bound is greater than upper_bound
         while lower_bound <= upper_bound:
             # Find the midpoint
-            midpoint = (lower_bound + upper_bound) // 2
+            midpoint = (lower_bound + upper_bound) >> 1  # equiv // 2
 
             # If predicate is satisfied by midpoint, search the left half.
             if predicate(midpoint):
                 upper_bound = midpoint - 1
             # Otherwise, search the right half.
             else:
                 lower_bound = midpoint + 1
```

### Comparing `interval-search-0.5.0/interval_search/curried_binary_search_recursive.py` & `interval-search-0.5.1/interval_search/curried_binary_search_recursive.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             return None
         if lower_bound == upper_bound:
             if predicate(lower_bound):
                 return lower_bound
             else:
                 return None
 
-        midpoint = (lower_bound + upper_bound) // 2
+        midpoint = (lower_bound + upper_bound) >> 1  # equiv // 2
 
         if predicate(midpoint):
             return binary_search_recursive(lower_bound, midpoint)
         else:
             return binary_search_recursive(midpoint + 1, upper_bound)
 
     return binary_search_recursive
```

### Comparing `interval-search-0.5.0/interval_search/curried_doubling_search.py` & `interval-search-0.5.1/interval_search/curried_doubling_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,16 @@
             The lowest integer value that satisfies the search criteria.
         """
 
         assert lower_bound >= 0, lower_bound
 
         bound = 1
         while not predicate(lower_bound + bound):
-            bound *= 2
+            bound <<= 1  # equiv *= 2
 
-        prev_bound = bound // 2
+        prev_bound = bound >> 1  # equiv // 2
         prev_guess = lower_bound + prev_bound
         return binary_search_iterative(
             predicate, prev_guess, lower_bound + bound
         )
 
     return doubling_search
```

### Comparing `interval-search-0.5.0/interval_search/doubling_search.py` & `interval-search-0.5.1/interval_search/doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/interval_search/interval_search.py` & `interval-search-0.5.1/interval_search/interval_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/interval_search.egg-info/PKG-INFO` & `interval-search-0.5.1/interval_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: interval-search
-Version: 0.5.0
+Version: 0.5.1
 Summary: interval-search provides predicate-based binary and doubling search implementations
 Home-page: https://github.com/mmore500/interval-search
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Description: ===============
         interval-search
```

### Comparing `interval-search-0.5.0/interval_search.egg-info/SOURCES.txt` & `interval-search-0.5.1/interval_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/setup.py` & `interval-search-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords='interval-search',
     name='interval-search',
     packages=find_packages(include=['interval_search', 'interval_search.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mmore500/interval-search',
-    version='0.5.0',
+    version='0.5.1',
     zip_safe=False,
 )
```

### Comparing `interval-search-0.5.0/tests/test_binary_search.py` & `interval-search-0.5.1/tests/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_binary_search_iterative.py` & `interval-search-0.5.1/tests/test_binary_search_iterative.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_binary_search_recursive.py` & `interval-search-0.5.1/tests/test_binary_search_recursive.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_curried_binary_search.py` & `interval-search-0.5.1/tests/test_curried_binary_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_curried_binary_search_iterative.py` & `interval-search-0.5.1/tests/test_curried_binary_search_iterative.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_curried_doubling_search.py` & `interval-search-0.5.1/tests/test_curried_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_doubling_search.py` & `interval-search-0.5.1/tests/test_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.0/tests/test_interval_search.py` & `interval-search-0.5.1/tests/test_interval_search.py`

 * *Files identical despite different names*

