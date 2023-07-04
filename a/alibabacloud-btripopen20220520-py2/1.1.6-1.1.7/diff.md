# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.1.6.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.6.tar", last modified: Mon Jun 26 02:21:11 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.7.tar", last modified: Tue Jul  4 01:58:58 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.1.6.tar` & `alibabacloud_btripopen20220520_py2-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/
--rw-r--r--   0 root         (0) root         (0)     3454 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223404 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  2006565 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 02:21:11.000000 alibabacloud_btripopen20220520_py2-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-26 02:21:10.000000 alibabacloud_btripopen20220520_py2-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)     3491 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223404 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2006880 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-04 01:58:58.000000 alibabacloud_btripopen20220520_py2-1.1.7/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/ChangeLog.md` & `alibabacloud_btripopen20220520_py2-1.1.7/ChangeLog.md`

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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.1.6
+Version: 1.1.7
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/README.md` & `alibabacloud_btripopen20220520_py2-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -39103,17 +39103,18 @@
             self.reimb_order_no = m.get('reimb_order_no')
         if m.get('sub_corp_id') is not None:
             self.sub_corp_id = m.get('sub_corp_id')
         return self
 
 
 class QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions(TeaModel):
-    def __init__(self, bill_settlement_id=None, fee_type=None, remark=None, remind_tag_list=None,
-                 settlement_amount=None, settlement_time=None, voucher_type=None):
+    def __init__(self, bill_settlement_id=None, capital_direction=None, fee_type=None, remark=None,
+                 remind_tag_list=None, settlement_amount=None, settlement_time=None, voucher_type=None):
         self.bill_settlement_id = bill_settlement_id  # type: long
+        self.capital_direction = capital_direction  # type: str
         self.fee_type = fee_type  # type: str
         self.remark = remark  # type: str
         self.remind_tag_list = remind_tag_list  # type: list[str]
         self.settlement_amount = settlement_amount  # type: str
         self.settlement_time = settlement_time  # type: str
         self.voucher_type = voucher_type  # type: int
 
@@ -39124,14 +39125,16 @@
         _map = super(QueryReimbursementOrderResponseBodyModuleExpensesExpenseCompositions, self).to_map()
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
@@ -39142,14 +39145,16 @@
             result['voucher_type'] = self.voucher_type
         return result
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.7/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.1.6
+Version: 1.1.7
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.6/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 26/06/2023
+Created on 04/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
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

