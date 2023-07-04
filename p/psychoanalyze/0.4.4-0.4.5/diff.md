# Comparing `tmp/psychoanalyze-0.4.4.tar.gz` & `tmp/psychoanalyze-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.4.4.tar", max compression
+gzip compressed data, was "psychoanalyze-0.4.5.tar", max compression
```

## Comparing `psychoanalyze-0.4.4.tar` & `psychoanalyze-0.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-06-18 00:25:21.788348 psychoanalyze-0.4.4/LICENSE
--rw-r--r--   0        0        0     1188 2023-06-18 00:25:21.788348 psychoanalyze-0.4.4/README.md
--rw-r--r--   0        0        0     1307 2023-06-18 00:27:30.330049 psychoanalyze-0.4.4/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      150 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/__main__.py
--rw-r--r--   0        0        0      358 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/app.py
--rw-r--r--   0        0        0     6216 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/blocks.py
--rw-r--r--   0        0        0       90 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/dashboard/__init__.py
--rw-r--r--   0        0        0        0 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/dashboard/__main__.py
--rw-r--r--   0        0        0      219 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/dashboard/app.py
--rw-r--r--   0        0        0     5239 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/dashboard/callbacks.py
--rw-r--r--   0        0        0     6932 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/dashboard/layout.py
--rw-r--r--   0        0        0     2133 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/data.py
--rw-r--r--   0        0        0      148 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/gescheider.py
--rw-r--r--   0        0        0     5602 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/plot.py
--rw-r--r--   0        0        0     5024 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/points.py
--rw-r--r--   0        0        0     1784 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/schemas.py
--rw-r--r--   0        0        0     2289 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/sessions.py
--rw-r--r--   0        0        0     2380 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/simulate.py
--rw-r--r--   0        0        0       95 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/stimulus.py
--rw-r--r--   0        0        0      565 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/strength_duration.py
--rw-r--r--   0        0        0      642 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/subjects.py
--rw-r--r--   0        0        0        0 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/transformations.py
--rw-r--r--   0        0        0     3367 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/trials.py
--rw-r--r--   0        0        0     1692 2023-06-18 00:25:21.860349 psychoanalyze-0.4.4/psychoanalyze/weber.py
--rw-r--r--   0        0        0     1499 2023-06-18 00:27:30.330049 psychoanalyze-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 psychoanalyze-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 05:02:55.657209 psychoanalyze-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1188 2023-07-04 05:02:55.657209 psychoanalyze-0.4.5/README.md
+-rw-r--r--   0        0        0     1307 2023-07-04 05:05:01.171348 psychoanalyze-0.4.5/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      150 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/__main__.py
+-rw-r--r--   0        0        0      358 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/app.py
+-rw-r--r--   0        0        0     6216 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/blocks.py
+-rw-r--r--   0        0        0       90 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/dashboard/__main__.py
+-rw-r--r--   0        0        0      219 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0     5239 2023-07-04 05:05:01.143347 psychoanalyze-0.4.5/psychoanalyze/dashboard/callbacks.py
+-rw-r--r--   0        0        0     6932 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     2133 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/data.py
+-rw-r--r--   0        0        0      148 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/gescheider.py
+-rw-r--r--   0        0        0     5602 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     5024 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/points.py
+-rw-r--r--   0        0        0     1784 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/schemas.py
+-rw-r--r--   0        0        0     2289 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/sessions.py
+-rw-r--r--   0        0        0     2380 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/simulate.py
+-rw-r--r--   0        0        0       95 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/stimulus.py
+-rw-r--r--   0        0        0      565 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/strength_duration.py
+-rw-r--r--   0        0        0      642 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/subjects.py
+-rw-r--r--   0        0        0        0 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/transformations.py
+-rw-r--r--   0        0        0     3367 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/trials.py
+-rw-r--r--   0        0        0     1692 2023-07-04 05:05:01.147347 psychoanalyze-0.4.5/psychoanalyze/weber.py
+-rw-r--r--   0        0        0     1499 2023-07-04 05:05:01.171348 psychoanalyze-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 psychoanalyze-0.4.5/PKG-INFO
```

### Comparing `psychoanalyze-0.4.4/LICENSE` & `psychoanalyze-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/README.md` & `psychoanalyze-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/__init__.py` & `psychoanalyze-0.4.5/psychoanalyze/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     stimulus,
     simulate,
 )
 from psychoanalyze.dashboard import layout
 
 pd.options.plotting.backend = "plotly"
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 __all__ = [
     "schemas",
     "plot",
     "data",
     "trial",
     "blocks",
```

### Comparing `psychoanalyze-0.4.4/psychoanalyze/blocks.py` & `psychoanalyze-0.4.5/psychoanalyze/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/dashboard/callbacks.py` & `psychoanalyze-0.4.5/psychoanalyze/dashboard/callbacks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/dashboard/layout.py` & `psychoanalyze-0.4.5/psychoanalyze/dashboard/layout.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/data.py` & `psychoanalyze-0.4.5/psychoanalyze/data.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/plot.py` & `psychoanalyze-0.4.5/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/points.py` & `psychoanalyze-0.4.5/psychoanalyze/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/schemas.py` & `psychoanalyze-0.4.5/psychoanalyze/schemas.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/sessions.py` & `psychoanalyze-0.4.5/psychoanalyze/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/simulate.py` & `psychoanalyze-0.4.5/psychoanalyze/simulate.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/strength_duration.py` & `psychoanalyze-0.4.5/psychoanalyze/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/subjects.py` & `psychoanalyze-0.4.5/psychoanalyze/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/trials.py` & `psychoanalyze-0.4.5/psychoanalyze/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/psychoanalyze/weber.py` & `psychoanalyze-0.4.5/psychoanalyze/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.4/pyproject.toml` & `psychoanalyze-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.4.4"
+version = "0.4.5"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
```

### Comparing `psychoanalyze-0.4.4/PKG-INFO` & `psychoanalyze-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

