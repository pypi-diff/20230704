# Comparing `tmp/alibabacloud_aiccs20230516_py2-1.0.0.tar.gz` & `tmp/alibabacloud_aiccs20230516_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiccs20230516_py2-1.0.0.tar", last modified: Tue Jul  4 06:55:15 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiccs20230516_py2-1.0.1.tar", last modified: Tue Jul  4 13:12:38 2023, max compression
```

## Comparing `alibabacloud_aiccs20230516_py2-1.0.0.tar` & `alibabacloud_aiccs20230516_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41616 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516/client.py
--rw-r--r--   0 root         (0) root         (0)   206007 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-07-04 06:55:15.000000 alibabacloud_aiccs20230516_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41712 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/client.py
+-rw-r--r--   0 root         (0) root         (0)   206433 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/LICENSE` & `alibabacloud_aiccs20230516_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/PKG-INFO` & `alibabacloud_aiccs20230516_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiccs20230516_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/README-CN.md` & `alibabacloud_aiccs20230516_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/README.md` & `alibabacloud_aiccs20230516_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516/client.py` & `alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,14 +375,16 @@
         if not UtilClient.is_unset(tmp_req.customers):
             request.customers_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.customers, 'Customers', 'json')
         query = {}
         if not UtilClient.is_unset(request.customers_shrink):
             query['Customers'] = request.customers_shrink
         if not UtilClient.is_unset(request.fail_return):
             query['FailReturn'] = request.fail_return
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.task_id):
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516/models.py` & `alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2070,18 +2070,19 @@
             self.properties = m.get('Properties')
         if m.get('Tag') is not None:
             self.tag = m.get('Tag')
         return self
 
 
 class ImportNumberRequest(TeaModel):
-    def __init__(self, customers=None, fail_return=None, owner_id=None, resource_owner_account=None,
+    def __init__(self, customers=None, fail_return=None, out_id=None, owner_id=None, resource_owner_account=None,
                  resource_owner_id=None, task_id=None):
         self.customers = customers  # type: list[ImportNumberRequestCustomers]
         self.fail_return = fail_return  # type: long
+        self.out_id = out_id  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.task_id = task_id  # type: long
 
     def validate(self):
         if self.customers:
@@ -2097,14 +2098,16 @@
         result = dict()
         result['Customers'] = []
         if self.customers is not None:
             for k in self.customers:
                 result['Customers'].append(k.to_map() if k else None)
         if self.fail_return is not None:
             result['FailReturn'] = self.fail_return
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
         if self.task_id is not None:
@@ -2116,30 +2119,33 @@
         self.customers = []
         if m.get('Customers') is not None:
             for k in m.get('Customers'):
                 temp_model = ImportNumberRequestCustomers()
                 self.customers.append(temp_model.from_map(k))
         if m.get('FailReturn') is not None:
             self.fail_return = m.get('FailReturn')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         if m.get('TaskId') is not None:
             self.task_id = m.get('TaskId')
         return self
 
 
 class ImportNumberShrinkRequest(TeaModel):
-    def __init__(self, customers_shrink=None, fail_return=None, owner_id=None, resource_owner_account=None,
-                 resource_owner_id=None, task_id=None):
+    def __init__(self, customers_shrink=None, fail_return=None, out_id=None, owner_id=None,
+                 resource_owner_account=None, resource_owner_id=None, task_id=None):
         self.customers_shrink = customers_shrink  # type: str
         self.fail_return = fail_return  # type: long
+        self.out_id = out_id  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.task_id = task_id  # type: long
 
     def validate(self):
         pass
@@ -2150,14 +2156,16 @@
             return _map
 
         result = dict()
         if self.customers_shrink is not None:
             result['Customers'] = self.customers_shrink
         if self.fail_return is not None:
             result['FailReturn'] = self.fail_return
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
         if self.task_id is not None:
@@ -2166,14 +2174,16 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Customers') is not None:
             self.customers_shrink = m.get('Customers')
         if m.get('FailReturn') is not None:
             self.fail_return = m.get('FailReturn')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         if m.get('TaskId') is not None:
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO` & `alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiccs20230516-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.0/setup.py` & `alibabacloud_aiccs20230516_py2-1.0.1/setup.py`

 * *Files identical despite different names*

