# Comparing `tmp/antchain_bot-1.8.90.tar.gz` & `tmp/antchain_bot-1.8.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.8.90.tar", last modified: Mon Jul  3 03:13:27 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.8.94.tar", last modified: Tue Jul  4 06:40:46 2023, max compression
```

## Comparing `antchain_bot-1.8.90.tar` & `antchain_bot-1.8.94.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   444092 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)  1184117 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   444092 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1185996 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 06:40:46.000000 antchain_bot-1.8.94/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-07-04 06:40:45.000000 antchain_bot-1.8.94/setup.py
```

### Comparing `antchain_bot-1.8.90/LICENSE` & `antchain_bot-1.8.94/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.90/PKG-INFO` & `antchain_bot-1.8.94/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_bot
-Version: 1.8.90
+Version: 1.8.94
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.90/README-CN.md` & `antchain_bot-1.8.94/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.90/README.md` & `antchain_bot-1.8.94/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.90/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.8.94/antchain_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-bot
-Version: 1.8.90
+Version: 1.8.94
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.90/antchain_sdk_bot/client.py` & `antchain_bot-1.8.94/antchain_sdk_bot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.90',
+                    'sdk_version': '1.8.94',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.90',
+                    'sdk_version': '1.8.94',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_bot-1.8.90/antchain_sdk_bot/models.py` & `antchain_bot-1.8.94/antchain_sdk_bot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1399,28 +1399,58 @@
 class JtData(TeaModel):
     def __init__(
         self,
         trustiot_id: int = None,
         trustiot_entity_id: int = None,
         processed_content: str = None,
         delta_mileage: int = None,
+        biz_type: str = None,
+        alarm_sub_type: int = None,
     ):
         # 数据的可信平台唯一ID
         self.trustiot_id = trustiot_id
         # IoT可信平台设备唯一ID
         self.trustiot_entity_id = trustiot_entity_id
         # 上报原文解析处理之后的数据
         self.processed_content = processed_content
         # 和上一次上报数据里程对比，新增的里程数
         self.delta_mileage = delta_mileage
+        # 正常位置信息：LOCATION
+        # 告警信息：ALARM_BASIC、 ALARM_ADAS、 ALARM_DSM、 ALARM_ACCELEROMETER
+        self.biz_type = biz_type
+        # 告警子类型
+        # //ADAS
+        # 10001: 前向碰撞报警
+        # 10002: 车辆偏离报警
+        # 10003: 车距过近报警
+        # 10004: 行人碰撞报警
+        # 10005: 频繁变道报警
+        # 10006: 道路标识超限报警
+        # 10007: 障碍物报警 //10008~10015 保留
+        # 10016: 道路标志识别事件
+        # 10017: 主动抓拍事件 //10018~10031 保留
+        # //DSM
+        # 10101: 疲劳驾驶报警
+        # 10102: 接打电话报警
+        # 10103: 抽烟报警报警
+        # 10104: 分神驾驶报警
+        # 10105: 驾驶员异常报警 //10106~10115 保留
+        # 10116: 自动抓拍事件
+        # 10117: 驾驶员变更事件 //10118~10031 保留
+        # //加速度
+        # 11701: 急加速
+        # 11702: 急减速
+        # 11703: 急转弯
+        self.alarm_sub_type = alarm_sub_type
 
     def validate(self):
         self.validate_required(self.trustiot_id, 'trustiot_id')
         self.validate_required(self.trustiot_entity_id, 'trustiot_entity_id')
         self.validate_required(self.processed_content, 'processed_content')
+        self.validate_required(self.biz_type, 'biz_type')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1428,26 +1458,34 @@
             result['trustiot_id'] = self.trustiot_id
         if self.trustiot_entity_id is not None:
             result['trustiot_entity_id'] = self.trustiot_entity_id
         if self.processed_content is not None:
             result['processed_content'] = self.processed_content
         if self.delta_mileage is not None:
             result['delta_mileage'] = self.delta_mileage
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        if self.alarm_sub_type is not None:
+            result['alarm_sub_type'] = self.alarm_sub_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('trustiot_id') is not None:
             self.trustiot_id = m.get('trustiot_id')
         if m.get('trustiot_entity_id') is not None:
             self.trustiot_entity_id = m.get('trustiot_entity_id')
         if m.get('processed_content') is not None:
             self.processed_content = m.get('processed_content')
         if m.get('delta_mileage') is not None:
             self.delta_mileage = m.get('delta_mileage')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        if m.get('alarm_sub_type') is not None:
+            self.alarm_sub_type = m.get('alarm_sub_type')
         return self
 
 
 class RentContractInfo(TeaModel):
     def __init__(
         self,
         contract_id: str = None,
@@ -30853,14 +30891,15 @@
         scene: str = None,
         trustiot_device_id_list: List[int] = None,
         start_time: int = None,
         end_time: int = None,
         alarm_types: List[str] = None,
         page_index: int = None,
         page_size: int = None,
+        alarm_sub_types: List[int] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 查询类型，支持LOCATION, TRACE,  ALARM三类
         self.query_type = query_type
         # 查询模式，支持抽样SAMPLE和分页PAGE两类，query_type不是LOCATION时必填
@@ -30875,14 +30914,16 @@
         self.end_time = end_time
         # 查询ALARM的类型，默认查全部类型，包括ALARM_BASIC,ALARM_ADAS ,ALARM_DSM,ALARM_ACCELEROMETER四类
         self.alarm_types = alarm_types
         # 页码
         self.page_index = page_index
         # 单页数量
         self.page_size = page_size
+        # 告警子类型
+        self.alarm_sub_types = alarm_sub_types
 
     def validate(self):
         self.validate_required(self.query_type, 'query_type')
         self.validate_required(self.scene, 'scene')
 
     def to_map(self):
         _map = super().to_map()
@@ -30908,14 +30949,16 @@
             result['end_time'] = self.end_time
         if self.alarm_types is not None:
             result['alarm_types'] = self.alarm_types
         if self.page_index is not None:
             result['page_index'] = self.page_index
         if self.page_size is not None:
             result['page_size'] = self.page_size
+        if self.alarm_sub_types is not None:
+            result['alarm_sub_types'] = self.alarm_sub_types
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -30934,14 +30977,16 @@
             self.end_time = m.get('end_time')
         if m.get('alarm_types') is not None:
             self.alarm_types = m.get('alarm_types')
         if m.get('page_index') is not None:
             self.page_index = m.get('page_index')
         if m.get('page_size') is not None:
             self.page_size = m.get('page_size')
+        if m.get('alarm_sub_types') is not None:
+            self.alarm_sub_types = m.get('alarm_sub_types')
         return self
 
 
 class QueryCollectorJtfluxResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_bot-1.8.90/setup.py` & `antchain_bot-1.8.94/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 03/07/2023
+Created on 04/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
```

