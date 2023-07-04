# Comparing `tmp/yplib-2.1.5.tar.gz` & `tmp/yplib-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.1.5.tar", last modified: Tue Jul  4 00:29:41 2023, max compression
+gzip compressed data, was "dist\yplib-2.1.6.tar", last modified: Tue Jul  4 00:32:48 2023, max compression
```

## Comparing `yplib-2.1.5.tar` & `yplib-2.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:29:41.970272 yplib-2.1.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.1.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-04 00:29:41.969771 yplib-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 00:29:41.970385 yplib-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-04 00:29:23.000000 yplib-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:29:41.965339 yplib-2.1.5/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.1.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    12522 2023-07-04 00:28:17.000000 yplib-2.1.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.1.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.1.5/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.1.5/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.1.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.1.5/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.1.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.1.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.1.5/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.1.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:29:41.968708 yplib-2.1.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-04 00:29:41.000000 yplib-2.1.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-04 00:29:41.000000 yplib-2.1.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:29:41.000000 yplib-2.1.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 00:29:41.000000 yplib-2.1.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 00:32:48.495911 yplib-2.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-04 00:32:48.495775 yplib-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 00:32:48.495911 yplib-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-04 00:32:05.000000 yplib-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:32:48.492809 yplib-2.1.6/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.1.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12590 2023-07-04 00:31:58.000000 yplib-2.1.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.1.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.1.6/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.1.6/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.1.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.1.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.1.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.1.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.1.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.1.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-04 00:32:48.495144 yplib-2.1.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-04 00:32:48.000000 yplib-2.1.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-04 00:32:48.000000 yplib-2.1.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 00:32:48.000000 yplib-2.1.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 00:32:48.000000 yplib-2.1.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.1.5/LICENSE` & `yplib-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/setup.py` & `yplib-2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.1.5",
+  version="2.1.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.1.5/yplib/__init__.py` & `yplib-2.1.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/chart.py` & `yplib-2.1.6/yplib/chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
         y_o = {}
         y_one = y_list[y_index]
         if isinstance(y_one, list) or isinstance(y_one, set):
             y_o['data'] = y_one
         else:
             y_o['name'] = y_one['name'] if 'name' in y_one else str(y_index) + '_' + random_letter(3)
             y_o['smooth'] = 1 if 'smooth' in y_one and y_one['smooth'] else 0
+            y_o['data'] = y_one['data'] if 'data' in y_one else []
         # 只有一条线,就不显示 name 了
         if len(y_list) == 1 and 'name' in y_o:
             del y_o['name']
         y_o['type'] = 'line'
         y_o['stack'] = 'Total'
         series.append(y_o)
```

### Comparing `yplib-2.1.5/yplib/chart_html.py` & `yplib-2.1.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/db.py` & `yplib-2.1.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/file.py` & `yplib-2.1.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/http_util.py` & `yplib-2.1.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/index.py` & `yplib-2.1.6/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/mail.py` & `yplib-2.1.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/mail_html.py` & `yplib-2.1.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.5/yplib/markdown.py` & `yplib-2.1.6/yplib/markdown.py`

 * *Files identical despite different names*

