# Comparing `tmp/alibabacloud_aiccs20230516-1.0.0.tar.gz` & `tmp/alibabacloud_aiccs20230516-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiccs20230516-1.0.0.tar", last modified: Tue Jul  4 06:55:32 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiccs20230516-1.0.1.tar", last modified: Tue Jul  4 13:12:45 2023, max compression
```

## Comparing `alibabacloud_aiccs20230516-1.0.0.tar` & `alibabacloud_aiccs20230516-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92832 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516/client.py
--rw-r--r--   0 root         (0) root         (0)   205402 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 06:55:32.000000 alibabacloud_aiccs20230516-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-07-04 06:55:31.000000 alibabacloud_aiccs20230516-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93024 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/client.py
+-rw-r--r--   0 root         (0) root         (0)   205832 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/setup.py
```

### Comparing `alibabacloud_aiccs20230516-1.0.0/LICENSE` & `alibabacloud_aiccs20230516-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516-1.0.0/PKG-INFO` & `alibabacloud_aiccs20230516-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiccs20230516
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516-1.0.0/README-CN.md` & `alibabacloud_aiccs20230516-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516-1.0.0/README.md` & `alibabacloud_aiccs20230516-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516/client.py` & `alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,14 +812,16 @@
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
@@ -854,14 +856,16 @@
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

### Comparing `alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516/models.py` & `alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2354,21 +2354,23 @@
 
 
 class ImportNumberRequest(TeaModel):
     def __init__(
         self,
         customers: List[ImportNumberRequestCustomers] = None,
         fail_return: int = None,
+        out_id: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         task_id: int = None,
     ):
         self.customers = customers
         self.fail_return = fail_return
+        self.out_id = out_id
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.task_id = task_id
 
     def validate(self):
         if self.customers:
@@ -2384,14 +2386,16 @@
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
@@ -2403,14 +2407,16 @@
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
@@ -2419,21 +2425,23 @@
 
 
 class ImportNumberShrinkRequest(TeaModel):
     def __init__(
         self,
         customers_shrink: str = None,
         fail_return: int = None,
+        out_id: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         task_id: int = None,
     ):
         self.customers_shrink = customers_shrink
         self.fail_return = fail_return
+        self.out_id = out_id
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.task_id = task_id
 
     def validate(self):
         pass
@@ -2444,14 +2452,16 @@
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
@@ -2460,14 +2470,16 @@
 
     def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_aiccs20230516-1.0.0/alibabacloud_aiccs20230516.egg-info/PKG-INFO` & `alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiccs20230516
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516-1.0.0/setup.py` & `alibabacloud_aiccs20230516-1.0.1/setup.py`

 * *Files identical despite different names*

