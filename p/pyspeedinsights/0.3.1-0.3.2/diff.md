# Comparing `tmp/pyspeedinsights-0.3.1.tar.gz` & `tmp/pyspeedinsights-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeedinsights-0.3.1.tar", last modified: Sun Feb 26 02:35:34 2023, max compression
+gzip compressed data, was "pyspeedinsights-0.3.2.tar", last modified: Tue Jul  4 14:43:57 2023, max compression
```

## Comparing `pyspeedinsights-0.3.1.tar` & `pyspeedinsights-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.322233 pyspeedinsights-0.3.1/
--rw-r--r--   0 will       (501) staff       (20)     1080 2022-05-27 03:33:19.000000 pyspeedinsights-0.3.1/LICENSE
--rw-r--r--   0 will       (501) staff       (20)    14017 2023-02-26 02:35:34.322385 pyspeedinsights-0.3.1/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)    12820 2023-02-26 01:59:32.000000 pyspeedinsights-0.3.1/README.md
--rw-r--r--   0 will       (501) staff       (20)      651 2023-02-26 02:20:45.000000 pyspeedinsights-0.3.1/pyproject.toml
--rw-r--r--   0 will       (501) staff       (20)     1613 2023-02-26 02:35:34.323254 pyspeedinsights-0.3.1/setup.cfg
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.311103 pyspeedinsights-0.3.1/src/
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.314999 pyspeedinsights-0.3.1/src/pyspeedinsights/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 03:33:19.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/__init__.py
--rw-r--r--   0 will       (501) staff       (20)      142 2022-06-07 16:31:02.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/__main__.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.318843 pyspeedinsights-0.3.1/src/pyspeedinsights/api/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 04:37:52.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/api/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     1613 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/api/keys.py
--rw-r--r--   0 will       (501) staff       (20)     3990 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/api/request.py
--rw-r--r--   0 will       (501) staff       (20)     4700 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/api/response.py
--rw-r--r--   0 will       (501) staff       (20)     3411 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/app.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.320159 pyspeedinsights-0.3.1/src/pyspeedinsights/cli/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/cli/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     2778 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/cli/choices.py
--rw-r--r--   0 will       (501) staff       (20)     4598 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/cli/commands.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.321086 pyspeedinsights-0.3.1/src/pyspeedinsights/core/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 20:34:15.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/core/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     8497 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/core/excel.py
--rw-r--r--   0 will       (501) staff       (20)     4543 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/core/sitemap.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.321979 pyspeedinsights-0.3.1/src/pyspeedinsights/utils/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/utils/__init__.py
--rw-r--r--   0 will       (501) staff       (20)      509 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/utils/generic.py
--rw-r--r--   0 will       (501) staff       (20)     1178 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.1/src/pyspeedinsights/utils/urls.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-02-26 02:35:34.317215 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/
--rw-r--r--   0 will       (501) staff       (20)    14017 2023-02-26 02:35:34.000000 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)      855 2023-02-26 02:35:34.000000 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/SOURCES.txt
--rw-r--r--   0 will       (501) staff       (20)        1 2023-02-26 02:35:34.000000 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/dependency_links.txt
--rw-r--r--   0 will       (501) staff       (20)       49 2023-02-26 02:35:34.000000 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/entry_points.txt
--rw-r--r--   0 will       (501) staff       (20)      143 2023-02-26 02:35:34.000000 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/requires.txt
--rw-r--r--   0 will       (501) staff       (20)       16 2023-02-26 02:35:34.000000 pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/top_level.txt
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.118915 pyspeedinsights-0.3.2/
+-rw-r--r--   0 will       (501) staff       (20)     1080 2022-05-27 03:33:19.000000 pyspeedinsights-0.3.2/LICENSE
+-rw-r--r--   0 will       (501) staff       (20)    14017 2023-07-04 14:43:57.119461 pyspeedinsights-0.3.2/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)    12820 2023-02-26 01:59:32.000000 pyspeedinsights-0.3.2/README.md
+-rw-r--r--   0 will       (501) staff       (20)      651 2023-02-26 02:20:45.000000 pyspeedinsights-0.3.2/pyproject.toml
+-rw-r--r--   0 will       (501) staff       (20)     1613 2023-07-04 14:43:57.121339 pyspeedinsights-0.3.2/setup.cfg
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.105097 pyspeedinsights-0.3.2/src/
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.108155 pyspeedinsights-0.3.2/src/pyspeedinsights/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 03:33:19.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)      142 2022-06-07 16:31:02.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/__main__.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.112614 pyspeedinsights-0.3.2/src/pyspeedinsights/api/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 04:37:52.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     1613 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/keys.py
+-rw-r--r--   0 will       (501) staff       (20)     3990 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/request.py
+-rw-r--r--   0 will       (501) staff       (20)     4871 2023-07-04 14:36:46.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/response.py
+-rw-r--r--   0 will       (501) staff       (20)     3411 2023-02-26 04:24:39.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/app.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.114204 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     2778 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/choices.py
+-rw-r--r--   0 will       (501) staff       (20)     4598 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/commands.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.115661 pyspeedinsights-0.3.2/src/pyspeedinsights/core/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 20:34:15.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/core/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     8497 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/core/excel.py
+-rw-r--r--   0 will       (501) staff       (20)     4543 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/core/sitemap.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.118045 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)      509 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/generic.py
+-rw-r--r--   0 will       (501) staff       (20)     1304 2023-07-03 22:00:41.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/urls.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.110589 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/
+-rw-r--r--   0 will       (501) staff       (20)    14017 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      855 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/SOURCES.txt
+-rw-r--r--   0 will       (501) staff       (20)        1 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/dependency_links.txt
+-rw-r--r--   0 will       (501) staff       (20)       49 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/entry_points.txt
+-rw-r--r--   0 will       (501) staff       (20)      143 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/requires.txt
+-rw-r--r--   0 will       (501) staff       (20)       16 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/top_level.txt
```

### Comparing `pyspeedinsights-0.3.1/LICENSE` & `pyspeedinsights-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/PKG-INFO` & `pyspeedinsights-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspeedinsights
-Version: 0.3.1
+Version: 0.3.2
 Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 Home-page: https://github.com/wjh18/pyspeedinsights
 Author: Will J. Holmes
 Author-email: will@wjholmes.com
 Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
 Project-URL: Source, https://github.com/wjh18/pyspeedinsights
 Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
```

### Comparing `pyspeedinsights-0.3.1/README.md` & `pyspeedinsights-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/pyproject.toml` & `pyspeedinsights-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/setup.cfg` & `pyspeedinsights-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyspeedinsights
-version = 0.3.1
+version = 0.3.2
 author = Will J. Holmes
 author_email = will@wjholmes.com
 description = Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = google, google-apis, psi-api, page-speed-insights, page-speed-insights-api, pagespeedinsightsapi, python, cli
 url = https://github.com/wjh18/pyspeedinsights
```

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/api/keys.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/api/keys.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/api/request.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/api/request.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/api/response.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/api/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,10 +122,13 @@
 
     Converts the timestamp to a Python datetime object.
 
     Returns:
         A str in format year-month-day_hour.minute.second.
     """
     timestamp = json_resp["analysisUTCTimestamp"]
-    dt_object = datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S.%fZ")
+    ts_no_fractions = timestamp.split(".")[0]  # Remove fraction
+    if ts_no_fractions[-1] != "Z":
+        ts_no_fractions += "Z"  # Add Z back after fraction removal
+    dt_object = datetime.strptime(ts_no_fractions, "%Y-%m-%dT%H:%M:%SZ")
     date = dt_object.strftime("%Y-%m-%d_%H.%M.%S")
     return date
```

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/app.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/app.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/cli/choices.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/cli/choices.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/cli/commands.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/core/excel.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/core/excel.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/core/sitemap.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/core/sitemap.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights/utils/urls.py` & `pyspeedinsights-0.3.2/src/pyspeedinsights/utils/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,18 @@
     err = "Invalid URL. Please enter a valid fully-qualified URL."
     replacements = {}
     u = urlsplit(url)
 
     if not u.scheme:
         replacements["scheme"] = "https"
     if not u.netloc:
-        if ("." not in u.path) or ("." and "/" in u.path):
+        p_sep, dot = u.path.find("/"), u.path.find(".")
+        path_before_host = p_sep < dot and p_sep > 0
+        no_host = "." not in u.path
+        if path_before_host or no_host:
             raise SystemExit(err)
         else:
             replacements["netloc"] = u.path
             replacements["path"] = ""
 
     replacements["fragment"] = ""
     replacements["query"] = ""
```

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/PKG-INFO` & `pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspeedinsights
-Version: 0.3.1
+Version: 0.3.2
 Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 Home-page: https://github.com/wjh18/pyspeedinsights
 Author: Will J. Holmes
 Author-email: will@wjholmes.com
 Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
 Project-URL: Source, https://github.com/wjh18/pyspeedinsights
 Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
```

### Comparing `pyspeedinsights-0.3.1/src/pyspeedinsights.egg-info/SOURCES.txt` & `pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

