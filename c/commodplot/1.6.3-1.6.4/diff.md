# Comparing `tmp/commodplot-1.6.3.tar.gz` & `tmp/commodplot-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commodplot-1.6.3.tar", last modified: Tue Jun  6 12:03:01 2023, max compression
+gzip compressed data, was "commodplot-1.6.4.tar", last modified: Tue Jul  4 14:53:51 2023, max compression
```

## Comparing `commodplot-1.6.3.tar` & `commodplot-1.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.383042 commodplot-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 12:03:01.383042 commodplot-1.6.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.379042 commodplot-1.6.3/commodplot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplottable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplottrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplottransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplotutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/jinjautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.383042 commodplot-1.6.3/commodplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 12:03:01.383042 commodplot-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-06 12:02:50.000000 commodplot-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.383042 commodplot-1.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplottable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplottrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplotutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_jinjautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:51.467579 commodplot-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-04 14:53:51.467579 commodplot-1.6.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:51.463579 commodplot-1.6.4/commodplot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16487 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/commodplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/commodplottable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/commodplottrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/commodplottransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/commodplotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/jinjautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-04 14:53:37.000000 commodplot-1.6.4/commodplot/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:51.467579 commodplot-1.6.4/commodplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-04 14:53:51.000000 commodplot-1.6.4/commodplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 14:53:51.000000 commodplot-1.6.4/commodplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:53:51.000000 commodplot-1.6.4/commodplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-04 14:53:51.000000 commodplot-1.6.4/commodplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 14:53:51.000000 commodplot-1.6.4/commodplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-04 14:53:51.467579 commodplot-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-04 14:53:37.000000 commodplot-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:51.467579 commodplot-1.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/test_commodplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/test_commodplottable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/test_commodplottrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/test_commodplotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/test_jinjautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 14:53:37.000000 commodplot-1.6.4/test/test_messaging.py
```

### Comparing `commodplot-1.6.3/commodplot/commodplot.py` & `commodplot-1.6.4/commodplot/commodplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,17 +415,18 @@
     fig.update_layout(title=title)
     return fig
 
 
 def stacked_area_chart(df, **kwargs):
     fig = go.Figure()
     group = kwargs.get("stackgroup", "stackgroup")
+    showlegend = kwargs.get("showlegend", None)
 
     for col in df.columns:
-        fig.add_trace(go.Scatter(x=df.index, y=df[col], name=col, stackgroup=group))
+        fig.add_trace(go.Scatter(x=df.index, y=df[col], name=col, stackgroup=group, showlegend=showlegend))
 
     fig.update_layout(title=kwargs.get("title", ""))
     return fig
 
 
 def bar_chart(df, **kwargs):
     fig = go.Figure()
```

### Comparing `commodplot-1.6.3/commodplot/commodplottable.py` & `commodplot-1.6.4/commodplot/commodplottable.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/commodplot/commodplottrace.py` & `commodplot-1.6.4/commodplot/commodplottrace.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/commodplot/commodplottransform.py` & `commodplot-1.6.4/commodplot/commodplottransform.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/commodplot/commodplotutil.py` & `commodplot-1.6.4/commodplot/commodplotutil.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/commodplot/jinjautils.py` & `commodplot-1.6.4/commodplot/jinjautils.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/commodplot/messaging.py` & `commodplot-1.6.4/commodplot/messaging.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/commodplot.egg-info/SOURCES.txt` & `commodplot-1.6.4/commodplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/setup.py` & `commodplot-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="commodplot",
-    version="1.6.3",
+    version="1.6.4",
     author="aeorxc",
     author_email="author@example.com",
     description="common commodity plotting including seasonal charts using plotly",
     url="https://github.com/aeorxc/commodplot",
     project_urls={
         "Source": "https://github.com/aeorxc/commodplot",
     },
```

### Comparing `commodplot-1.6.3/test/test_commodplot.py` & `commodplot-1.6.4/test/test_commodplot.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/test/test_commodplottable.py` & `commodplot-1.6.4/test/test_commodplottable.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/test/test_commodplottrace.py` & `commodplot-1.6.4/test/test_commodplottrace.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/test/test_commodplotutil.py` & `commodplot-1.6.4/test/test_commodplotutil.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/test/test_jinjautils.py` & `commodplot-1.6.4/test/test_jinjautils.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.3/test/test_messaging.py` & `commodplot-1.6.4/test/test_messaging.py`

 * *Files identical despite different names*

