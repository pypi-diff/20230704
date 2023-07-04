# Comparing `tmp/alibabacloud_vpc20160428_py2-1.0.1.tar.gz` & `tmp/alibabacloud_vpc20160428_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_vpc20160428_py2-1.0.1.tar", last modified: Tue Jan 31 06:21:16 2023, max compression
+gzip compressed data, was "dist/alibabacloud_vpc20160428_py2-2.0.0.tar", last modified: Tue Jul  4 03:26:28 2023, max compression
```

## Comparing `alibabacloud_vpc20160428_py2-1.0.1.tar` & `alibabacloud_vpc20160428_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      197 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428/__init__.py
--rw-r--r--   0 root         (0) root         (0)   724803 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428/client.py
--rw-r--r--   0 root         (0) root         (0)  2629820 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2921 2023-01-31 06:21:16.000000 alibabacloud_vpc20160428_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:26:28.000000 alibabacloud_vpc20160428_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-04 03:26:28.000000 alibabacloud_vpc20160428_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:26:28.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   987888 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428/client.py
+-rw-r--r--   0 root         (0) root         (0)  3468933 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:26:28.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 03:26:28.000000 alibabacloud_vpc20160428_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-07-04 03:26:27.000000 alibabacloud_vpc20160428_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_vpc20160428_py2-1.0.1/LICENSE` & `alibabacloud_vpc20160428_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428_py2-1.0.1/PKG-INFO` & `alibabacloud_vpc20160428_py2-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_vpc20160428_py2
-Version: 1.0.1
+Version: 2.0.0
 Summary: Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpc20160428_py2-1.0.1/README-CN.md` & `alibabacloud_vpc20160428_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428_py2-1.0.1/README.md` & `alibabacloud_vpc20160428_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428_py2-1.0.1/alibabacloud_vpc20160428_py2.egg-info/PKG-INFO` & `alibabacloud_vpc20160428_py2-2.0.0/alibabacloud_vpc20160428_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-vpc20160428-py2
-Version: 1.0.1
+Version: 2.0.0
 Summary: Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpc20160428_py2-1.0.1/setup.py` & `alibabacloud_vpc20160428_py2-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_vpc20160428_py2.
 
-Created on 31/01/2023
+Created on 04/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_vpc20160428"
 NAME = "alibabacloud_vpc20160428_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

