# Comparing `tmp/alibabacloud_btripopen20220520-1.1.6.tar.gz` & `tmp/alibabacloud_btripopen20220520-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.6.tar", last modified: Mon Jun 26 02:21:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.7.tar", last modified: Tue Jul  4 01:58:44 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520-1.1.6.tar` & `alibabacloud_btripopen20220520-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/
--rw-r--r--   0 root         (0) root         (0)     3580 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   525626 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  1984483 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-06-26 02:21:41.000000 alibabacloud_btripopen20220520-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   525626 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  1984800 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/setup.py
```

### Comparing `alibabacloud_btripopen20220520-1.1.6/ChangeLog.md` & `alibabacloud_btripopen20220520-1.1.7/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-26 Version: 1.1.6
+- Update.
+
 2023-06-16 Version: 1.1.5
 - Update.
 
 2023-06-15 Version: 1.1.4
 - Update.
 
 2023-06-12 Version: 1.1.3
```

### Comparing `alibabacloud_btripopen20220520-1.1.6/LICENSE` & `alibabacloud_btripopen20220520-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.6/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520
-Version: 1.1.6
+Version: 1.1.7
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.6/README-CN.md` & `alibabacloud_btripopen20220520-1.1.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.6/README.md` & `alibabacloud_btripopen20220520-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -44566,22 +44566,24 @@
         return self
 
 
 class QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions(TeaModel):
     def __init__(
         self,
         bill_settlement_id: int = None,
+        capital_direction: str = None,
         fee_type: str = None,
         remark: str = None,
         remind_tag_list: List[str] = None,
         settlement_amount: str = None,
         settlement_time: str = None,
         voucher_type: int = None,
     ):
         self.bill_settlement_id = bill_settlement_id
+        self.capital_direction = capital_direction
         self.fee_type = fee_type
         self.remark = remark
         self.remind_tag_list = remind_tag_list
         self.settlement_amount = settlement_amount
         self.settlement_time = settlement_time
         self.voucher_type = voucher_type
 
@@ -44592,14 +44594,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.bill_settlement_id is not None:
             result['bill_settlement_id'] = self.bill_settlement_id
+        if self.capital_direction is not None:
+            result['capital_direction'] = self.capital_direction
         if self.fee_type is not None:
             result['fee_type'] = self.fee_type
         if self.remark is not None:
             result['remark'] = self.remark
         if self.remind_tag_list is not None:
             result['remind_tag_list'] = self.remind_tag_list
         if self.settlement_amount is not None:
@@ -44610,14 +44614,16 @@
             result['voucher_type'] = self.voucher_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('bill_settlement_id') is not None:
             self.bill_settlement_id = m.get('bill_settlement_id')
+        if m.get('capital_direction') is not None:
+            self.capital_direction = m.get('capital_direction')
         if m.get('fee_type') is not None:
             self.fee_type = m.get('fee_type')
         if m.get('remark') is not None:
             self.remark = m.get('remark')
         if m.get('remind_tag_list') is not None:
             self.remind_tag_list = m.get('remind_tag_list')
         if m.get('settlement_amount') is not None:
```

### Comparing `alibabacloud_btripopen20220520-1.1.6/alibabacloud_btripopen20220520.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520
-Version: 1.1.6
+Version: 1.1.7
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.6/setup.py` & `alibabacloud_btripopen20220520-1.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520.
 
-Created on 26/06/2023
+Created on 04/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

