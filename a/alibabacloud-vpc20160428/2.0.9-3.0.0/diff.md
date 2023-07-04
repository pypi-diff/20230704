# Comparing `tmp/alibabacloud_vpc20160428-2.0.9.tar.gz` & `tmp/alibabacloud_vpc20160428-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_vpc20160428-2.0.9.tar", last modified: Thu Sep  1 08:09:30 2022, max compression
+gzip compressed data, was "dist/alibabacloud_vpc20160428-3.0.0.tar", last modified: Tue Jul  4 03:27:07 2023, max compression
```

## Comparing `alibabacloud_vpc20160428-2.0.9.tar` & `alibabacloud_vpc20160428-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/
--rw-r--r--   0 root         (0) root         (0)      635 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1557912 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/client.py
--rw-r--r--   0 root         (0) root         (0)  2424267 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2628 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     7208 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2196316 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428/client.py
+-rw-r--r--   0 root         (0) root         (0)  3437323 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-04 03:27:07.000000 alibabacloud_vpc20160428-3.0.0/setup.py
```

### Comparing `alibabacloud_vpc20160428-2.0.9/LICENSE` & `alibabacloud_vpc20160428-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.9/PKG-INFO` & `alibabacloud_vpc20160428-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_vpc20160428
-Version: 2.0.9
+Version: 3.0.0
 Summary: Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpc20160428-2.0.9/README-CN.md` & `alibabacloud_vpc20160428-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.9/README.md` & `alibabacloud_vpc20160428-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/PKG-INFO` & `alibabacloud_vpc20160428-3.0.0/alibabacloud_vpc20160428.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-vpc20160428
-Version: 2.0.9
+Version: 3.0.0
 Summary: Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpc20160428-2.0.9/setup.py` & `alibabacloud_vpc20160428-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_vpc20160428.
 
-Created on 01/09/2022
+Created on 04/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_vpc20160428"
 NAME = "alibabacloud_vpc20160428" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

