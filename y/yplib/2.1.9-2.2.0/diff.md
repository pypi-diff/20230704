# Comparing `tmp/yplib-2.1.9.tar.gz` & `tmp/yplib-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.1.9.tar", last modified: Tue Jul  4 00:53:38 2023, max compression
+gzip compressed data, was "dist\yplib-2.2.0.tar", last modified: Tue Jul  4 07:39:38 2023, max compression
```

## Comparing `yplib-2.1.9.tar` & `yplib-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:38.116354 yplib-2.1.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.1.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-04 00:53:38.116006 yplib-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 00:53:38.116654 yplib-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-04 00:53:23.000000 yplib-2.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:38.112901 yplib-2.1.9/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.1.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.1.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.1.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.1.9/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.1.9/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.1.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.1.9/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.1.9/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.1.9/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.1.9/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.1.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:53:38.115120 yplib-2.1.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-04 00:53:38.000000 yplib-2.1.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-04 00:53:38.000000 yplib-2.1.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:53:38.000000 yplib-2.1.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 00:53:38.000000 yplib-2.1.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 07:39:38.393331 yplib-2.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-04 07:39:38.393331 yplib-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 07:39:38.393865 yplib-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-04 07:39:15.000000 yplib-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:39:38.389294 yplib-2.2.0/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.2.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    12428 2023-07-04 00:52:40.000000 yplib-2.2.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.2.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.2.0/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.2.0/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.2.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    27090 2023-07-04 07:38:56.000000 yplib-2.2.0/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.2.0/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.2.0/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.2.0/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.2.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:39:38.392332 yplib-2.2.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-04 07:39:38.000000 yplib-2.2.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-04 07:39:38.000000 yplib-2.2.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:39:38.000000 yplib-2.2.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 07:39:38.000000 yplib-2.2.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.1.9/LICENSE` & `yplib-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/setup.py` & `yplib-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.1.9",
+  version="2.2.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.1.9/yplib/__init__.py` & `yplib-2.2.0/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/chart.py` & `yplib-2.2.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/chart_html.py` & `yplib-2.2.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/db.py` & `yplib-2.2.0/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/file.py` & `yplib-2.2.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/http_util.py` & `yplib-2.2.0/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/index.py` & `yplib-2.2.0/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,14 +517,26 @@
         else:
             data_list.append(line)
     if sep_all is not None:
         data_list = ''.join(data_list).split(str(sep_all))
     return data_list
 
 
+# 读取文件中的数据,返回一个 str
+def to_str_from_file(file_name='a.txt'):
+    return to_list_data(file_name=file_name,
+                        r_str=True)
+
+
+# 读取文件中的数据,返回一个 json
+def to_json_from_file(file_name='a.txt'):
+    return to_list_data(file_name=file_name,
+                        r_json=True)
+
+
 # 在 to_list 方法上再嵌套一层,
 # r_str : 返回的数据是否是一个 字符串, ''.join(list)
 # r_json : 返回的数据是否是一个 json 类型的数据
 def to_list_data(file_name='a.txt',
                  sep=None,
                  sep_all=None,
                  start_index=None,
```

### Comparing `yplib-2.1.9/yplib/mail.py` & `yplib-2.2.0/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/mail_html.py` & `yplib-2.2.0/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.9/yplib/markdown.py` & `yplib-2.2.0/yplib/markdown.py`

 * *Files identical despite different names*

