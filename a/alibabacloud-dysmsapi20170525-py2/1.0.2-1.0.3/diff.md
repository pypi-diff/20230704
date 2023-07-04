# Comparing `tmp/alibabacloud_dysmsapi20170525_py2-1.0.2.tar.gz` & `tmp/alibabacloud_dysmsapi20170525_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dysmsapi20170525_py2-1.0.2.tar", last modified: Tue Nov 29 07:24:28 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dysmsapi20170525_py2-1.0.3.tar", last modified: Tue Jul  4 11:31:32 2023, max compression
```

## Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2.tar` & `alibabacloud_dysmsapi20170525_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      144 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50703 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525/client.py
--rw-r--r--   0 root         (0) root         (0)   193383 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2022-11-29 07:24:28.000000 alibabacloud_dysmsapi20170525_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:31:32.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-04 11:31:32.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:31:32.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58017 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525/client.py
+-rw-r--r--   0 root         (0) root         (0)   219970 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:31:32.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 11:31:32.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-07-04 11:31:31.000000 alibabacloud_dysmsapi20170525_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/LICENSE` & `alibabacloud_dysmsapi20170525_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/PKG-INFO` & `alibabacloud_dysmsapi20170525_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dysmsapi20170525_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Dysmsapi (20170525) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/README-CN.md` & `alibabacloud_dysmsapi20170525_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/README.md` & `alibabacloud_dysmsapi20170525_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525/client.py` & `alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,19 @@
     *\
     """
     def __init__(self, config):
         super(Client, self).__init__(config)
         self._endpoint_rule = 'central'
         self._endpoint_map = {
             'ap-southeast-1': 'dysmsapi.ap-southeast-1.aliyuncs.com',
-            'ap-southeast-5': 'dysmsapi-xman.ap-southeast-5.aliyuncs.com',
+            'ap-southeast-5': 'dysmsapi.ap-southeast-5.aliyuncs.com',
             'cn-beijing': 'dysmsapi-proxy.cn-beijing.aliyuncs.com',
-            'cn-hongkong': 'dysmsapi-xman.cn-hongkong.aliyuncs.com'
+            'cn-hongkong': 'dysmsapi-xman.cn-hongkong.aliyuncs.com',
+            'eu-central-1': 'dysmsapi.eu-central-1.aliyuncs.com',
+            'us-east-1': 'dysmsapi.us-east-1.aliyuncs.com'
         }
         self.check_config(config)
         self._endpoint = self.get_endpoint('dysmsapi', self._region_id, self._endpoint_rule, self._network, self._suffix, self._endpoint_map, self._endpoint)
 
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
@@ -186,14 +188,50 @@
             self.call_api(params, req, runtime)
         )
 
     def check_mobiles_card_support(self, request):
         runtime = util_models.RuntimeOptions()
         return self.check_mobiles_card_support_with_options(request, runtime)
 
+    def conversion_data_intl_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.conversion_rate):
+            query['ConversionRate'] = request.conversion_rate
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.report_time):
+            query['ReportTime'] = request.report_time
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ConversionDataIntl',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dysmsapi_20170525_models.ConversionDataIntlResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def conversion_data_intl(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.conversion_data_intl_with_options(request, runtime)
+
     def create_card_sms_template_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = dysmsapi_20170525_models.CreateCardSmsTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.template):
             request.template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.template, 'Template', 'json')
         query = {}
@@ -224,14 +262,54 @@
             self.call_api(params, req, runtime)
         )
 
     def create_card_sms_template(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_card_sms_template_with_options(request, runtime)
 
+    def create_smart_short_url_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.expiration):
+            query['Expiration'] = request.expiration
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_numbers):
+            query['PhoneNumbers'] = request.phone_numbers
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.source_name):
+            query['SourceName'] = request.source_name
+        if not UtilClient.is_unset(request.source_url):
+            query['SourceUrl'] = request.source_url
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateSmartShortUrl',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dysmsapi_20170525_models.CreateSmartShortUrlResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_smart_short_url(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_smart_short_url_with_options(request, runtime)
+
     def delete_short_url_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
@@ -656,14 +734,66 @@
             self.call_api(params, req, runtime)
         )
 
     def query_mobiles_card_support(self, request):
         runtime = util_models.RuntimeOptions()
         return self.query_mobiles_card_support_with_options(request, runtime)
 
+    def query_page_smart_short_url_log_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.click_state):
+            query['ClickState'] = request.click_state
+        if not UtilClient.is_unset(request.create_date_end):
+            query['CreateDateEnd'] = request.create_date_end
+        if not UtilClient.is_unset(request.create_date_start):
+            query['CreateDateStart'] = request.create_date_start
+        if not UtilClient.is_unset(request.end_id):
+            query['EndId'] = request.end_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_no):
+            query['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.short_name):
+            query['ShortName'] = request.short_name
+        if not UtilClient.is_unset(request.short_url):
+            query['ShortUrl'] = request.short_url
+        if not UtilClient.is_unset(request.start_id):
+            query['StartId'] = request.start_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryPageSmartShortUrlLog',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dysmsapi_20170525_models.QueryPageSmartShortUrlLogResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def query_page_smart_short_url_log(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.query_page_smart_short_url_log_with_options(request, runtime)
+
     def query_send_details_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
@@ -1112,14 +1242,52 @@
             self.call_api(params, req, runtime)
         )
 
     def send_sms(self, request):
         runtime = util_models.RuntimeOptions()
         return self.send_sms_with_options(request, runtime)
 
+    def sms_conversion_intl_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.conversion_time):
+            query['ConversionTime'] = request.conversion_time
+        if not UtilClient.is_unset(request.delivered):
+            query['Delivered'] = request.delivered
+        if not UtilClient.is_unset(request.message_id):
+            query['MessageId'] = request.message_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SmsConversionIntl',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dysmsapi_20170525_models.SmsConversionIntlResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def sms_conversion_intl(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.sms_conversion_intl_with_options(request, runtime)
+
     def tag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.prod_code):
             query['ProdCode'] = request.prod_code
```

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525/models.py` & `alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -641,14 +641,132 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CheckMobilesCardSupportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ConversionDataIntlRequest(TeaModel):
+    def __init__(self, conversion_rate=None, owner_id=None, report_time=None, resource_owner_account=None,
+                 resource_owner_id=None):
+        self.conversion_rate = conversion_rate  # type: str
+        self.owner_id = owner_id  # type: long
+        self.report_time = report_time  # type: long
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ConversionDataIntlRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conversion_rate is not None:
+            result['ConversionRate'] = self.conversion_rate
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.report_time is not None:
+            result['ReportTime'] = self.report_time
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ConversionRate') is not None:
+            self.conversion_rate = m.get('ConversionRate')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ReportTime') is not None:
+            self.report_time = m.get('ReportTime')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class ConversionDataIntlResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, request_id=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ConversionDataIntlResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ConversionDataIntlResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ConversionDataIntlResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ConversionDataIntlResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ConversionDataIntlResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateCardSmsTemplateRequest(TeaModel):
     def __init__(self, factorys=None, memo=None, template=None, template_name=None):
         self.factorys = factorys  # type: str
         self.memo = memo  # type: str
         self.template = template  # type: dict[str, any]
         self.template_name = template_name  # type: str
 
@@ -823,14 +941,199 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateCardSmsTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateSmartShortUrlRequest(TeaModel):
+    def __init__(self, expiration=None, owner_id=None, phone_numbers=None, resource_owner_account=None,
+                 resource_owner_id=None, source_name=None, source_url=None):
+        self.expiration = expiration  # type: long
+        self.owner_id = owner_id  # type: long
+        self.phone_numbers = phone_numbers  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+        self.source_name = source_name  # type: str
+        self.source_url = source_url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateSmartShortUrlRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.expiration is not None:
+            result['Expiration'] = self.expiration
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.phone_numbers is not None:
+            result['PhoneNumbers'] = self.phone_numbers
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.source_name is not None:
+            result['SourceName'] = self.source_name
+        if self.source_url is not None:
+            result['SourceUrl'] = self.source_url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Expiration') is not None:
+            self.expiration = m.get('Expiration')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PhoneNumbers') is not None:
+            self.phone_numbers = m.get('PhoneNumbers')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('SourceName') is not None:
+            self.source_name = m.get('SourceName')
+        if m.get('SourceUrl') is not None:
+            self.source_url = m.get('SourceUrl')
+        return self
+
+
+class CreateSmartShortUrlResponseBodyModel(TeaModel):
+    def __init__(self, domain=None, expiration=None, phone_number=None, short_name=None, short_url=None):
+        self.domain = domain  # type: str
+        self.expiration = expiration  # type: long
+        self.phone_number = phone_number  # type: str
+        self.short_name = short_name  # type: str
+        self.short_url = short_url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateSmartShortUrlResponseBodyModel, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.domain is not None:
+            result['Domain'] = self.domain
+        if self.expiration is not None:
+            result['Expiration'] = self.expiration
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.short_name is not None:
+            result['ShortName'] = self.short_name
+        if self.short_url is not None:
+            result['ShortUrl'] = self.short_url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Domain') is not None:
+            self.domain = m.get('Domain')
+        if m.get('Expiration') is not None:
+            self.expiration = m.get('Expiration')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('ShortName') is not None:
+            self.short_name = m.get('ShortName')
+        if m.get('ShortUrl') is not None:
+            self.short_url = m.get('ShortUrl')
+        return self
+
+
+class CreateSmartShortUrlResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, model=None, request_id=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.model = model  # type: list[CreateSmartShortUrlResponseBodyModel]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.model:
+            for k in self.model:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(CreateSmartShortUrlResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        result['Model'] = []
+        if self.model is not None:
+            for k in self.model:
+                result['Model'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        self.model = []
+        if m.get('Model') is not None:
+            for k in m.get('Model'):
+                temp_model = CreateSmartShortUrlResponseBodyModel()
+                self.model.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateSmartShortUrlResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateSmartShortUrlResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateSmartShortUrlResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateSmartShortUrlResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteShortUrlRequest(TeaModel):
     def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, source_url=None):
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.source_url = source_url  # type: str
 
@@ -2689,14 +2992,287 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryMobilesCardSupportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryPageSmartShortUrlLogRequest(TeaModel):
+    def __init__(self, click_state=None, create_date_end=None, create_date_start=None, end_id=None, owner_id=None,
+                 page_no=None, page_size=None, phone_number=None, resource_owner_account=None, resource_owner_id=None,
+                 short_name=None, short_url=None, start_id=None):
+        self.click_state = click_state  # type: long
+        self.create_date_end = create_date_end  # type: long
+        self.create_date_start = create_date_start  # type: long
+        self.end_id = end_id  # type: long
+        self.owner_id = owner_id  # type: long
+        self.page_no = page_no  # type: long
+        self.page_size = page_size  # type: long
+        self.phone_number = phone_number  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+        self.short_name = short_name  # type: str
+        self.short_url = short_url  # type: str
+        self.start_id = start_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryPageSmartShortUrlLogRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.click_state is not None:
+            result['ClickState'] = self.click_state
+        if self.create_date_end is not None:
+            result['CreateDateEnd'] = self.create_date_end
+        if self.create_date_start is not None:
+            result['CreateDateStart'] = self.create_date_start
+        if self.end_id is not None:
+            result['EndId'] = self.end_id
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.short_name is not None:
+            result['ShortName'] = self.short_name
+        if self.short_url is not None:
+            result['ShortUrl'] = self.short_url
+        if self.start_id is not None:
+            result['StartId'] = self.start_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClickState') is not None:
+            self.click_state = m.get('ClickState')
+        if m.get('CreateDateEnd') is not None:
+            self.create_date_end = m.get('CreateDateEnd')
+        if m.get('CreateDateStart') is not None:
+            self.create_date_start = m.get('CreateDateStart')
+        if m.get('EndId') is not None:
+            self.end_id = m.get('EndId')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('ShortName') is not None:
+            self.short_name = m.get('ShortName')
+        if m.get('ShortUrl') is not None:
+            self.short_url = m.get('ShortUrl')
+        if m.get('StartId') is not None:
+            self.start_id = m.get('StartId')
+        return self
+
+
+class QueryPageSmartShortUrlLogResponseBodyModelList(TeaModel):
+    def __init__(self, click_state=None, click_time=None, create_time=None, phone_number=None, short_name=None,
+                 short_url=None):
+        self.click_state = click_state  # type: long
+        self.click_time = click_time  # type: long
+        self.create_time = create_time  # type: long
+        self.phone_number = phone_number  # type: str
+        self.short_name = short_name  # type: str
+        self.short_url = short_url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryPageSmartShortUrlLogResponseBodyModelList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.click_state is not None:
+            result['ClickState'] = self.click_state
+        if self.click_time is not None:
+            result['ClickTime'] = self.click_time
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.short_name is not None:
+            result['ShortName'] = self.short_name
+        if self.short_url is not None:
+            result['ShortUrl'] = self.short_url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClickState') is not None:
+            self.click_state = m.get('ClickState')
+        if m.get('ClickTime') is not None:
+            self.click_time = m.get('ClickTime')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('ShortName') is not None:
+            self.short_name = m.get('ShortName')
+        if m.get('ShortUrl') is not None:
+            self.short_url = m.get('ShortUrl')
+        return self
+
+
+class QueryPageSmartShortUrlLogResponseBodyModel(TeaModel):
+    def __init__(self, list=None, page_no=None, page_size=None, total_count=None, total_page=None):
+        self.list = list  # type: list[QueryPageSmartShortUrlLogResponseBodyModelList]
+        self.page_no = page_no  # type: long
+        self.page_size = page_size  # type: long
+        self.total_count = total_count  # type: long
+        self.total_page = total_page  # type: long
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(QueryPageSmartShortUrlLogResponseBodyModel, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        if self.total_page is not None:
+            result['TotalPage'] = self.total_page
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = QueryPageSmartShortUrlLogResponseBodyModelList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        if m.get('TotalPage') is not None:
+            self.total_page = m.get('TotalPage')
+        return self
+
+
+class QueryPageSmartShortUrlLogResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, model=None, request_id=None, success=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.model = model  # type: QueryPageSmartShortUrlLogResponseBodyModel
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.model:
+            self.model.validate()
+
+    def to_map(self):
+        _map = super(QueryPageSmartShortUrlLogResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.model is not None:
+            result['Model'] = self.model.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Model') is not None:
+            temp_model = QueryPageSmartShortUrlLogResponseBodyModel()
+            self.model = temp_model.from_map(m['Model'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QueryPageSmartShortUrlLogResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: QueryPageSmartShortUrlLogResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(QueryPageSmartShortUrlLogResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryPageSmartShortUrlLogResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QuerySendDetailsRequest(TeaModel):
     def __init__(self, biz_id=None, current_page=None, owner_id=None, page_size=None, phone_number=None,
                  resource_owner_account=None, resource_owner_id=None, send_date=None):
         self.biz_id = biz_id  # type: str
         self.current_page = current_page  # type: long
         self.owner_id = owner_id  # type: long
         self.page_size = page_size  # type: long
@@ -4856,14 +5432,137 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SendSmsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SmsConversionIntlRequest(TeaModel):
+    def __init__(self, conversion_time=None, delivered=None, message_id=None, owner_id=None,
+                 resource_owner_account=None, resource_owner_id=None):
+        self.conversion_time = conversion_time  # type: long
+        self.delivered = delivered  # type: bool
+        self.message_id = message_id  # type: str
+        self.owner_id = owner_id  # type: long
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SmsConversionIntlRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conversion_time is not None:
+            result['ConversionTime'] = self.conversion_time
+        if self.delivered is not None:
+            result['Delivered'] = self.delivered
+        if self.message_id is not None:
+            result['MessageId'] = self.message_id
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ConversionTime') is not None:
+            self.conversion_time = m.get('ConversionTime')
+        if m.get('Delivered') is not None:
+            self.delivered = m.get('Delivered')
+        if m.get('MessageId') is not None:
+            self.message_id = m.get('MessageId')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class SmsConversionIntlResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, request_id=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SmsConversionIntlResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SmsConversionIntlResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SmsConversionIntlResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SmsConversionIntlResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SmsConversionIntlResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class TagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
         self.key = key  # type: str
         self.value = value  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/alibabacloud_dysmsapi20170525_py2.egg-info/PKG-INFO` & `alibabacloud_dysmsapi20170525_py2-1.0.3/alibabacloud_dysmsapi20170525_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dysmsapi20170525-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Dysmsapi (20170525) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dysmsapi20170525_py2-1.0.2/setup.py` & `alibabacloud_dysmsapi20170525_py2-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dysmsapi20170525_py2.
 
-Created on 29/11/2022
+Created on 04/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dysmsapi20170525"
 NAME = "alibabacloud_dysmsapi20170525_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dysmsapi (20170525) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

