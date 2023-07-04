# Comparing `tmp/alibabacloud_dysmsapi20170525-2.0.8.tar.gz` & `tmp/alibabacloud_dysmsapi20170525-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dysmsapi20170525-2.0.8.tar", last modified: Mon Nov 29 06:08:48 2021, max compression
+gzip compressed data, was "dist/alibabacloud_dysmsapi20170525-2.0.9.tar", last modified: Mon Jan 24 07:38:30 2022, max compression
```

## Comparing `alibabacloud_dysmsapi20170525-2.0.8.tar` & `alibabacloud_dysmsapi20170525-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      350 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525/
--rw-r--r--   0 root         (0) root         (0)       21 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68729 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525/client.py
--rw-r--r--   0 root         (0) root         (0)   121282 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-11-29 06:08:48.000000 alibabacloud_dysmsapi20170525-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2021-11-29 06:08:47.000000 alibabacloud_dysmsapi20170525-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79597 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525/client.py
+-rw-r--r--   0 root         (0) root         (0)   118400 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2022-01-24 07:38:30.000000 alibabacloud_dysmsapi20170525-2.0.9/setup.py
```

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/LICENSE` & `alibabacloud_dysmsapi20170525-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/PKG-INFO` & `alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dysmsapi20170525
-Version: 2.0.8
+Name: alibabacloud-dysmsapi20170525
+Version: 2.0.9
 Summary: Alibaba Cloud Dysmsapi (20170525) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/README-CN.md` & `alibabacloud_dysmsapi20170525-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/README.md` & `alibabacloud_dysmsapi20170525-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525/client.py` & `alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,20 +50,30 @@
     def add_short_url_with_options(
         self,
         request: dysmsapi_20170525_models.AddShortUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.AddShortUrlResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        body = {}
+        if not UtilClient.is_unset(request.effective_days):
+            body['EffectiveDays'] = request.effective_days
+        if not UtilClient.is_unset(request.short_url_name):
+            body['ShortUrlName'] = request.short_url_name
+        if not UtilClient.is_unset(request.source_url):
+            body['SourceUrl'] = request.source_url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AddShortUrl',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -80,20 +90,30 @@
     async def add_short_url_with_options_async(
         self,
         request: dysmsapi_20170525_models.AddShortUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.AddShortUrlResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        body = {}
+        if not UtilClient.is_unset(request.effective_days):
+            body['EffectiveDays'] = request.effective_days
+        if not UtilClient.is_unset(request.short_url_name):
+            body['ShortUrlName'] = request.short_url_name
+        if not UtilClient.is_unset(request.source_url):
+            body['SourceUrl'] = request.source_url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AddShortUrl',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -124,23 +144,32 @@
     def add_sms_sign_with_options(
         self,
         request: dysmsapi_20170525_models.AddSmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.AddSmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
-        query['SignSource'] = request.sign_source
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.sign_source):
+            query['SignSource'] = request.sign_source
+        body = {}
+        if not UtilClient.is_unset(request.sign_file_list):
+            body['SignFileList'] = request.sign_file_list
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AddSmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -157,23 +186,32 @@
     async def add_sms_sign_with_options_async(
         self,
         request: dysmsapi_20170525_models.AddSmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.AddSmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
-        query['SignSource'] = request.sign_source
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.sign_source):
+            query['SignSource'] = request.sign_source
+        body = {}
+        if not UtilClient.is_unset(request.sign_file_list):
+            body['SignFileList'] = request.sign_file_list
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AddSmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -204,68 +242,80 @@
     def add_sms_template_with_options(
         self,
         request: dysmsapi_20170525_models.AddSmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.AddSmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateContent'] = request.template_content
-        query['TemplateName'] = request.template_name
-        query['TemplateType'] = request.template_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_content):
+            query['TemplateContent'] = request.template_content
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        if not UtilClient.is_unset(request.template_type):
+            query['TemplateType'] = request.template_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='AddSmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.AddSmsTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def add_sms_template_with_options_async(
         self,
         request: dysmsapi_20170525_models.AddSmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.AddSmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateContent'] = request.template_content
-        query['TemplateName'] = request.template_name
-        query['TemplateType'] = request.template_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_content):
+            query['TemplateContent'] = request.template_content
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        if not UtilClient.is_unset(request.template_type):
+            query['TemplateType'] = request.template_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='AddSmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.AddSmsTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -279,109 +329,33 @@
     async def add_sms_template_async(
         self,
         request: dysmsapi_20170525_models.AddSmsTemplateRequest,
     ) -> dysmsapi_20170525_models.AddSmsTemplateResponse:
         runtime = util_models.RuntimeOptions()
         return await self.add_sms_template_with_options_async(request, runtime)
 
-    def create_card_sms_template_with_options(
-        self,
-        tmp_req: dysmsapi_20170525_models.CreateCardSmsTemplateRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.CreateCardSmsTemplateResponse:
-        UtilClient.validate_model(tmp_req)
-        request = dysmsapi_20170525_models.CreateCardSmsTemplateShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.template):
-            request.template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.template, 'Template', 'json')
-        query = {}
-        query['Memo'] = request.memo
-        query['Template'] = request.template_shrink
-        query['TemplateName'] = request.template_name
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='CreateCardSmsTemplate',
-            version='2017-05-25',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            dysmsapi_20170525_models.CreateCardSmsTemplateResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_card_sms_template_with_options_async(
-        self,
-        tmp_req: dysmsapi_20170525_models.CreateCardSmsTemplateRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.CreateCardSmsTemplateResponse:
-        UtilClient.validate_model(tmp_req)
-        request = dysmsapi_20170525_models.CreateCardSmsTemplateShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.template):
-            request.template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.template, 'Template', 'json')
-        query = {}
-        query['Memo'] = request.memo
-        query['Template'] = request.template_shrink
-        query['TemplateName'] = request.template_name
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='CreateCardSmsTemplate',
-            version='2017-05-25',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            dysmsapi_20170525_models.CreateCardSmsTemplateResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def create_card_sms_template(
-        self,
-        request: dysmsapi_20170525_models.CreateCardSmsTemplateRequest,
-    ) -> dysmsapi_20170525_models.CreateCardSmsTemplateResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.create_card_sms_template_with_options(request, runtime)
-
-    async def create_card_sms_template_async(
-        self,
-        request: dysmsapi_20170525_models.CreateCardSmsTemplateRequest,
-    ) -> dysmsapi_20170525_models.CreateCardSmsTemplateResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.create_card_sms_template_with_options_async(request, runtime)
-
     def delete_short_url_with_options(
         self,
         request: dysmsapi_20170525_models.DeleteShortUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.DeleteShortUrlResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        body = {}
+        if not UtilClient.is_unset(request.source_url):
+            body['SourceUrl'] = request.source_url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteShortUrl',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -398,20 +372,26 @@
     async def delete_short_url_with_options_async(
         self,
         request: dysmsapi_20170525_models.DeleteShortUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.DeleteShortUrlResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        body = {}
+        if not UtilClient.is_unset(request.source_url):
+            body['SourceUrl'] = request.source_url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteShortUrl',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -442,62 +422,68 @@
     def delete_sms_sign_with_options(
         self,
         request: dysmsapi_20170525_models.DeleteSmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.DeleteSmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteSmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.DeleteSmsSignResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def delete_sms_sign_with_options_async(
         self,
         request: dysmsapi_20170525_models.DeleteSmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.DeleteSmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteSmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.DeleteSmsSignResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -518,62 +504,68 @@
     def delete_sms_template_with_options(
         self,
         request: dysmsapi_20170525_models.DeleteSmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.DeleteSmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteSmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.DeleteSmsTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def delete_sms_template_with_options_async(
         self,
         request: dysmsapi_20170525_models.DeleteSmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.DeleteSmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteSmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.DeleteSmsTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -587,209 +579,99 @@
     async def delete_sms_template_async(
         self,
         request: dysmsapi_20170525_models.DeleteSmsTemplateRequest,
     ) -> dysmsapi_20170525_models.DeleteSmsTemplateResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_sms_template_with_options_async(request, runtime)
 
-    def get_media_resource_id_with_options(
-        self,
-        request: dysmsapi_20170525_models.GetMediaResourceIdRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.GetMediaResourceIdResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        query['ExtendInfo'] = request.extend_info
-        query['FileSize'] = request.file_size
-        query['Memo'] = request.memo
-        query['OssKey'] = request.oss_key
-        query['ResourceType'] = request.resource_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='GetMediaResourceId',
-            version='2017-05-25',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            dysmsapi_20170525_models.GetMediaResourceIdResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def get_media_resource_id_with_options_async(
-        self,
-        request: dysmsapi_20170525_models.GetMediaResourceIdRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.GetMediaResourceIdResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        query['ExtendInfo'] = request.extend_info
-        query['FileSize'] = request.file_size
-        query['Memo'] = request.memo
-        query['OssKey'] = request.oss_key
-        query['ResourceType'] = request.resource_type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='GetMediaResourceId',
-            version='2017-05-25',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            dysmsapi_20170525_models.GetMediaResourceIdResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def get_media_resource_id(
-        self,
-        request: dysmsapi_20170525_models.GetMediaResourceIdRequest,
-    ) -> dysmsapi_20170525_models.GetMediaResourceIdResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.get_media_resource_id_with_options(request, runtime)
-
-    async def get_media_resource_id_async(
-        self,
-        request: dysmsapi_20170525_models.GetMediaResourceIdRequest,
-    ) -> dysmsapi_20170525_models.GetMediaResourceIdResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.get_media_resource_id_with_options_async(request, runtime)
-
-    def get_ossinfo_for_card_template_with_options(
-        self,
-        runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.GetOSSInfoForCardTemplateResponse:
-        req = open_api_models.OpenApiRequest()
-        params = open_api_models.Params(
-            action='GetOSSInfoForCardTemplate',
-            version='2017-05-25',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            dysmsapi_20170525_models.GetOSSInfoForCardTemplateResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def get_ossinfo_for_card_template_with_options_async(
-        self,
-        runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.GetOSSInfoForCardTemplateResponse:
-        req = open_api_models.OpenApiRequest()
-        params = open_api_models.Params(
-            action='GetOSSInfoForCardTemplate',
-            version='2017-05-25',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            dysmsapi_20170525_models.GetOSSInfoForCardTemplateResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def get_ossinfo_for_card_template(self) -> dysmsapi_20170525_models.GetOSSInfoForCardTemplateResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.get_ossinfo_for_card_template_with_options(runtime)
-
-    async def get_ossinfo_for_card_template_async(self) -> dysmsapi_20170525_models.GetOSSInfoForCardTemplateResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.get_ossinfo_for_card_template_with_options_async(runtime)
-
     def list_tag_resources_with_options(
         self,
         request: dysmsapi_20170525_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.ListTagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['NextToken'] = request.next_token
-        query['OwnerId'] = request.owner_id
-        query['PageSize'] = request.page_size
-        query['ProdCode'] = request.prod_code
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['ResourceType'] = request.resource_type
-        query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.prod_code):
+            query['ProdCode'] = request.prod_code
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagResources',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.ListTagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_tag_resources_with_options_async(
         self,
         request: dysmsapi_20170525_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.ListTagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['NextToken'] = request.next_token
-        query['OwnerId'] = request.owner_id
-        query['PageSize'] = request.page_size
-        query['ProdCode'] = request.prod_code
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['ResourceType'] = request.resource_type
-        query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.prod_code):
+            query['ProdCode'] = request.prod_code
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagResources',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.ListTagResourcesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -810,23 +692,32 @@
     def modify_sms_sign_with_options(
         self,
         request: dysmsapi_20170525_models.ModifySmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.ModifySmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
-        query['SignSource'] = request.sign_source
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.sign_source):
+            query['SignSource'] = request.sign_source
+        body = {}
+        if not UtilClient.is_unset(request.sign_file_list):
+            body['SignFileList'] = request.sign_file_list
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ModifySmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -843,23 +734,32 @@
     async def modify_sms_sign_with_options_async(
         self,
         request: dysmsapi_20170525_models.ModifySmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.ModifySmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
-        query['SignSource'] = request.sign_source
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.sign_source):
+            query['SignSource'] = request.sign_source
+        body = {}
+        if not UtilClient.is_unset(request.sign_file_list):
+            body['SignFileList'] = request.sign_file_list
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='ModifySmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -890,70 +790,84 @@
     def modify_sms_template_with_options(
         self,
         request: dysmsapi_20170525_models.ModifySmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.ModifySmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateCode'] = request.template_code
-        query['TemplateContent'] = request.template_content
-        query['TemplateName'] = request.template_name
-        query['TemplateType'] = request.template_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.template_content):
+            query['TemplateContent'] = request.template_content
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        if not UtilClient.is_unset(request.template_type):
+            query['TemplateType'] = request.template_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifySmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.ModifySmsTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def modify_sms_template_with_options_async(
         self,
         request: dysmsapi_20170525_models.ModifySmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.ModifySmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['Remark'] = request.remark
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateCode'] = request.template_code
-        query['TemplateContent'] = request.template_content
-        query['TemplateName'] = request.template_name
-        query['TemplateType'] = request.template_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.remark):
+            query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.template_content):
+            query['TemplateContent'] = request.template_content
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        if not UtilClient.is_unset(request.template_type):
+            query['TemplateType'] = request.template_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifySmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.ModifySmsTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -967,181 +881,229 @@
     async def modify_sms_template_async(
         self,
         request: dysmsapi_20170525_models.ModifySmsTemplateRequest,
     ) -> dysmsapi_20170525_models.ModifySmsTemplateResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_sms_template_with_options_async(request, runtime)
 
-    def query_card_sms_template_with_options(
+    def query_send_details_with_options(
         self,
-        request: dysmsapi_20170525_models.QueryCardSmsTemplateRequest,
+        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.QueryCardSmsTemplateResponse:
+    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.biz_id):
+            query['BizId'] = request.biz_id
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.send_date):
+            query['SendDate'] = request.send_date
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='QueryCardSmsTemplate',
+            action='QuerySendDetails',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.QueryCardSmsTemplateResponse(),
+            dysmsapi_20170525_models.QuerySendDetailsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def query_card_sms_template_with_options_async(
+    async def query_send_details_with_options_async(
         self,
-        request: dysmsapi_20170525_models.QueryCardSmsTemplateRequest,
+        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.QueryCardSmsTemplateResponse:
+    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.biz_id):
+            query['BizId'] = request.biz_id
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.send_date):
+            query['SendDate'] = request.send_date
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='QueryCardSmsTemplate',
+            action='QuerySendDetails',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.QueryCardSmsTemplateResponse(),
+            dysmsapi_20170525_models.QuerySendDetailsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def query_card_sms_template(
+    def query_send_details(
         self,
-        request: dysmsapi_20170525_models.QueryCardSmsTemplateRequest,
-    ) -> dysmsapi_20170525_models.QueryCardSmsTemplateResponse:
+        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
+    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
         runtime = util_models.RuntimeOptions()
-        return self.query_card_sms_template_with_options(request, runtime)
+        return self.query_send_details_with_options(request, runtime)
 
-    async def query_card_sms_template_async(
+    async def query_send_details_async(
         self,
-        request: dysmsapi_20170525_models.QueryCardSmsTemplateRequest,
-    ) -> dysmsapi_20170525_models.QueryCardSmsTemplateResponse:
+        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
+    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.query_card_sms_template_with_options_async(request, runtime)
+        return await self.query_send_details_with_options_async(request, runtime)
 
-    def query_send_details_with_options(
+    def query_send_statistics_with_options(
         self,
-        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
+        request: dysmsapi_20170525_models.QuerySendStatisticsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
+    ) -> dysmsapi_20170525_models.QuerySendStatisticsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['BizId'] = request.biz_id
-        query['CurrentPage'] = request.current_page
-        query['OwnerId'] = request.owner_id
-        query['PageSize'] = request.page_size
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SendDate'] = request.send_date
+        if not UtilClient.is_unset(request.end_date):
+            query['EndDate'] = request.end_date
+        if not UtilClient.is_unset(request.is_globe):
+            query['IsGlobe'] = request.is_globe
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_index):
+            query['PageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.start_date):
+            query['StartDate'] = request.start_date
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='QuerySendDetails',
+            action='QuerySendStatistics',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.QuerySendDetailsResponse(),
+            dysmsapi_20170525_models.QuerySendStatisticsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def query_send_details_with_options_async(
+    async def query_send_statistics_with_options_async(
         self,
-        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
+        request: dysmsapi_20170525_models.QuerySendStatisticsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
+    ) -> dysmsapi_20170525_models.QuerySendStatisticsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['BizId'] = request.biz_id
-        query['CurrentPage'] = request.current_page
-        query['OwnerId'] = request.owner_id
-        query['PageSize'] = request.page_size
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SendDate'] = request.send_date
+        if not UtilClient.is_unset(request.end_date):
+            query['EndDate'] = request.end_date
+        if not UtilClient.is_unset(request.is_globe):
+            query['IsGlobe'] = request.is_globe
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_index):
+            query['PageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.start_date):
+            query['StartDate'] = request.start_date
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='QuerySendDetails',
+            action='QuerySendStatistics',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.QuerySendDetailsResponse(),
+            dysmsapi_20170525_models.QuerySendStatisticsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def query_send_details(
+    def query_send_statistics(
         self,
-        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
-    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
+        request: dysmsapi_20170525_models.QuerySendStatisticsRequest,
+    ) -> dysmsapi_20170525_models.QuerySendStatisticsResponse:
         runtime = util_models.RuntimeOptions()
-        return self.query_send_details_with_options(request, runtime)
+        return self.query_send_statistics_with_options(request, runtime)
 
-    async def query_send_details_async(
+    async def query_send_statistics_async(
         self,
-        request: dysmsapi_20170525_models.QuerySendDetailsRequest,
-    ) -> dysmsapi_20170525_models.QuerySendDetailsResponse:
+        request: dysmsapi_20170525_models.QuerySendStatisticsRequest,
+    ) -> dysmsapi_20170525_models.QuerySendStatisticsResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.query_send_details_with_options_async(request, runtime)
+        return await self.query_send_statistics_with_options_async(request, runtime)
 
     def query_short_url_with_options(
         self,
         request: dysmsapi_20170525_models.QueryShortUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.QueryShortUrlResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        body = {}
+        if not UtilClient.is_unset(request.short_url):
+            body['ShortUrl'] = request.short_url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='QueryShortUrl',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1158,20 +1120,26 @@
     async def query_short_url_with_options_async(
         self,
         request: dysmsapi_20170525_models.QueryShortUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.QueryShortUrlResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        body = {}
+        if not UtilClient.is_unset(request.short_url):
+            body['ShortUrl'] = request.short_url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='QueryShortUrl',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1202,62 +1170,68 @@
     def query_sms_sign_with_options(
         self,
         request: dysmsapi_20170525_models.QuerySmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.QuerySmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QuerySmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.QuerySmsSignResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def query_sms_sign_with_options_async(
         self,
         request: dysmsapi_20170525_models.QuerySmsSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.QuerySmsSignResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QuerySmsSign',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.QuerySmsSignResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1271,69 +1245,161 @@
     async def query_sms_sign_async(
         self,
         request: dysmsapi_20170525_models.QuerySmsSignRequest,
     ) -> dysmsapi_20170525_models.QuerySmsSignResponse:
         runtime = util_models.RuntimeOptions()
         return await self.query_sms_sign_with_options_async(request, runtime)
 
+    def query_sms_sign_list_with_options(
+        self,
+        request: dysmsapi_20170525_models.QuerySmsSignListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dysmsapi_20170525_models.QuerySmsSignListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_index):
+            query['PageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QuerySmsSignList',
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
+            dysmsapi_20170525_models.QuerySmsSignListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def query_sms_sign_list_with_options_async(
+        self,
+        request: dysmsapi_20170525_models.QuerySmsSignListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dysmsapi_20170525_models.QuerySmsSignListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_index):
+            query['PageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QuerySmsSignList',
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
+            dysmsapi_20170525_models.QuerySmsSignListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def query_sms_sign_list(
+        self,
+        request: dysmsapi_20170525_models.QuerySmsSignListRequest,
+    ) -> dysmsapi_20170525_models.QuerySmsSignListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.query_sms_sign_list_with_options(request, runtime)
+
+    async def query_sms_sign_list_async(
+        self,
+        request: dysmsapi_20170525_models.QuerySmsSignListRequest,
+    ) -> dysmsapi_20170525_models.QuerySmsSignListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.query_sms_sign_list_with_options_async(request, runtime)
+
     def query_sms_template_with_options(
         self,
         request: dysmsapi_20170525_models.QuerySmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.QuerySmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QuerySmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.QuerySmsTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def query_sms_template_with_options_async(
         self,
         request: dysmsapi_20170525_models.QuerySmsTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.QuerySmsTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='QuerySmsTemplate',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.QuerySmsTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1347,251 +1413,279 @@
     async def query_sms_template_async(
         self,
         request: dysmsapi_20170525_models.QuerySmsTemplateRequest,
     ) -> dysmsapi_20170525_models.QuerySmsTemplateResponse:
         runtime = util_models.RuntimeOptions()
         return await self.query_sms_template_with_options_async(request, runtime)
 
-    def send_batch_sms_with_options(
+    def query_sms_template_list_with_options(
         self,
-        request: dysmsapi_20170525_models.SendBatchSmsRequest,
+        request: dysmsapi_20170525_models.QuerySmsTemplateListRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
+    ) -> dysmsapi_20170525_models.QuerySmsTemplateListResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumberJson'] = request.phone_number_json
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignNameJson'] = request.sign_name_json
-        query['SmsUpExtendCodeJson'] = request.sms_up_extend_code_json
-        query['TemplateCode'] = request.template_code
-        query['TemplateParamJson'] = request.template_param_json
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_index):
+            query['PageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='SendBatchSms',
+            action='QuerySmsTemplateList',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.SendBatchSmsResponse(),
+            dysmsapi_20170525_models.QuerySmsTemplateListResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def send_batch_sms_with_options_async(
+    async def query_sms_template_list_with_options_async(
         self,
-        request: dysmsapi_20170525_models.SendBatchSmsRequest,
+        request: dysmsapi_20170525_models.QuerySmsTemplateListRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
+    ) -> dysmsapi_20170525_models.QuerySmsTemplateListResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumberJson'] = request.phone_number_json
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignNameJson'] = request.sign_name_json
-        query['SmsUpExtendCodeJson'] = request.sms_up_extend_code_json
-        query['TemplateCode'] = request.template_code
-        query['TemplateParamJson'] = request.template_param_json
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.page_index):
+            query['PageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='SendBatchSms',
+            action='QuerySmsTemplateList',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.SendBatchSmsResponse(),
+            dysmsapi_20170525_models.QuerySmsTemplateListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def send_batch_sms(
+    def query_sms_template_list(
         self,
-        request: dysmsapi_20170525_models.SendBatchSmsRequest,
-    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
+        request: dysmsapi_20170525_models.QuerySmsTemplateListRequest,
+    ) -> dysmsapi_20170525_models.QuerySmsTemplateListResponse:
         runtime = util_models.RuntimeOptions()
-        return self.send_batch_sms_with_options(request, runtime)
+        return self.query_sms_template_list_with_options(request, runtime)
 
-    async def send_batch_sms_async(
+    async def query_sms_template_list_async(
         self,
-        request: dysmsapi_20170525_models.SendBatchSmsRequest,
-    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
+        request: dysmsapi_20170525_models.QuerySmsTemplateListRequest,
+    ) -> dysmsapi_20170525_models.QuerySmsTemplateListResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.send_batch_sms_with_options_async(request, runtime)
+        return await self.query_sms_template_list_with_options_async(request, runtime)
 
-    def send_card_sms_with_options(
+    def send_batch_sms_with_options(
         self,
-        request: dysmsapi_20170525_models.SendCardSmsRequest,
+        request: dysmsapi_20170525_models.SendBatchSmsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.SendCardSmsResponse:
+    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['CardObjects'] = request.card_objects
-        query['CardTemplateCode'] = request.card_template_code
-        query['DigitalTemplateCode'] = request.digital_template_code
-        query['DigitalTemplateParam'] = request.digital_template_param
-        query['FallbackType'] = request.fallback_type
-        query['OutId'] = request.out_id
-        query['SignName'] = request.sign_name
-        query['SmsTemplateCode'] = request.sms_template_code
-        query['SmsTemplateParam'] = request.sms_template_param
-        query['SmsUpExtendCode'] = request.sms_up_extend_code
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number_json):
+            query['PhoneNumberJson'] = request.phone_number_json
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name_json):
+            query['SignNameJson'] = request.sign_name_json
+        if not UtilClient.is_unset(request.sms_up_extend_code_json):
+            query['SmsUpExtendCodeJson'] = request.sms_up_extend_code_json
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.template_param_json):
+            query['TemplateParamJson'] = request.template_param_json
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='SendCardSms',
+            action='SendBatchSms',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.SendCardSmsResponse(),
+            dysmsapi_20170525_models.SendBatchSmsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def send_card_sms_with_options_async(
+    async def send_batch_sms_with_options_async(
         self,
-        request: dysmsapi_20170525_models.SendCardSmsRequest,
+        request: dysmsapi_20170525_models.SendBatchSmsRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dysmsapi_20170525_models.SendCardSmsResponse:
+    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['CardObjects'] = request.card_objects
-        query['CardTemplateCode'] = request.card_template_code
-        query['DigitalTemplateCode'] = request.digital_template_code
-        query['DigitalTemplateParam'] = request.digital_template_param
-        query['FallbackType'] = request.fallback_type
-        query['OutId'] = request.out_id
-        query['SignName'] = request.sign_name
-        query['SmsTemplateCode'] = request.sms_template_code
-        query['SmsTemplateParam'] = request.sms_template_param
-        query['SmsUpExtendCode'] = request.sms_up_extend_code
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number_json):
+            query['PhoneNumberJson'] = request.phone_number_json
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name_json):
+            query['SignNameJson'] = request.sign_name_json
+        if not UtilClient.is_unset(request.sms_up_extend_code_json):
+            query['SmsUpExtendCodeJson'] = request.sms_up_extend_code_json
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.template_param_json):
+            query['TemplateParamJson'] = request.template_param_json
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='SendCardSms',
+            action='SendBatchSms',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dysmsapi_20170525_models.SendCardSmsResponse(),
+            dysmsapi_20170525_models.SendBatchSmsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def send_card_sms(
+    def send_batch_sms(
         self,
-        request: dysmsapi_20170525_models.SendCardSmsRequest,
-    ) -> dysmsapi_20170525_models.SendCardSmsResponse:
+        request: dysmsapi_20170525_models.SendBatchSmsRequest,
+    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
         runtime = util_models.RuntimeOptions()
-        return self.send_card_sms_with_options(request, runtime)
+        return self.send_batch_sms_with_options(request, runtime)
 
-    async def send_card_sms_async(
+    async def send_batch_sms_async(
         self,
-        request: dysmsapi_20170525_models.SendCardSmsRequest,
-    ) -> dysmsapi_20170525_models.SendCardSmsResponse:
+        request: dysmsapi_20170525_models.SendBatchSmsRequest,
+    ) -> dysmsapi_20170525_models.SendBatchSmsResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.send_card_sms_with_options_async(request, runtime)
+        return await self.send_batch_sms_with_options_async(request, runtime)
 
     def send_sms_with_options(
         self,
         request: dysmsapi_20170525_models.SendSmsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.SendSmsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OutId'] = request.out_id
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumbers'] = request.phone_numbers
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
-        query['SmsUpExtendCode'] = request.sms_up_extend_code
-        query['TemplateCode'] = request.template_code
-        query['TemplateParam'] = request.template_param
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_numbers):
+            query['PhoneNumbers'] = request.phone_numbers
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.sms_up_extend_code):
+            query['SmsUpExtendCode'] = request.sms_up_extend_code
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.template_param):
+            query['TemplateParam'] = request.template_param
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SendSms',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.SendSmsResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def send_sms_with_options_async(
         self,
         request: dysmsapi_20170525_models.SendSmsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.SendSmsResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OutId'] = request.out_id
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumbers'] = request.phone_numbers
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['SignName'] = request.sign_name
-        query['SmsUpExtendCode'] = request.sms_up_extend_code
-        query['TemplateCode'] = request.template_code
-        query['TemplateParam'] = request.template_param
+        if not UtilClient.is_unset(request.out_id):
+            query['OutId'] = request.out_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_numbers):
+            query['PhoneNumbers'] = request.phone_numbers
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.sign_name):
+            query['SignName'] = request.sign_name
+        if not UtilClient.is_unset(request.sms_up_extend_code):
+            query['SmsUpExtendCode'] = request.sms_up_extend_code
+        if not UtilClient.is_unset(request.template_code):
+            query['TemplateCode'] = request.template_code
+        if not UtilClient.is_unset(request.template_param):
+            query['TemplateParam'] = request.template_param
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SendSms',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.SendSmsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1612,70 +1706,84 @@
     def tag_resources_with_options(
         self,
         request: dysmsapi_20170525_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.TagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ProdCode'] = request.prod_code
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['ResourceType'] = request.resource_type
-        query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.prod_code):
+            query['ProdCode'] = request.prod_code
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='TagResources',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.TagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def tag_resources_with_options_async(
         self,
         request: dysmsapi_20170525_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.TagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['ProdCode'] = request.prod_code
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['ResourceType'] = request.resource_type
-        query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.prod_code):
+            query['ProdCode'] = request.prod_code
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='TagResources',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.TagResourcesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1696,72 +1804,88 @@
     def untag_resources_with_options(
         self,
         request: dysmsapi_20170525_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.UntagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['All'] = request.all
-        query['OwnerId'] = request.owner_id
-        query['ProdCode'] = request.prod_code
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['ResourceType'] = request.resource_type
-        query['TagKey'] = request.tag_key
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.prod_code):
+            query['ProdCode'] = request.prod_code
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UntagResources',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.UntagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def untag_resources_with_options_async(
         self,
         request: dysmsapi_20170525_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dysmsapi_20170525_models.UntagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['All'] = request.all
-        query['OwnerId'] = request.owner_id
-        query['ProdCode'] = request.prod_code
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['ResourceType'] = request.resource_type
-        query['TagKey'] = request.tag_key
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.prod_code):
+            query['ProdCode'] = request.prod_code
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UntagResources',
             version='2017-05-25',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             dysmsapi_20170525_models.UntagResourcesResponse(),
             await self.call_api_async(params, req, runtime)
         )
```

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525/models.py` & `alibabacloud_dysmsapi20170525-2.0.9/alibabacloud_dysmsapi20170525/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List, Any
+from typing import Dict, List
 
 
 class AddShortUrlRequest(TeaModel):
     def __init__(
         self,
         effective_days: str = None,
         owner_id: int = None,
@@ -511,203 +511,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = AddSmsTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateCardSmsTemplateRequest(TeaModel):
-    def __init__(
-        self,
-        memo: str = None,
-        template: Dict[str, Any] = None,
-        template_name: str = None,
-    ):
-        self.memo = memo
-        self.template = template
-        self.template_name = template_name
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.memo is not None:
-            result['Memo'] = self.memo
-        if self.template is not None:
-            result['Template'] = self.template
-        if self.template_name is not None:
-            result['TemplateName'] = self.template_name
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Memo') is not None:
-            self.memo = m.get('Memo')
-        if m.get('Template') is not None:
-            self.template = m.get('Template')
-        if m.get('TemplateName') is not None:
-            self.template_name = m.get('TemplateName')
-        return self
-
-
-class CreateCardSmsTemplateShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        memo: str = None,
-        template_shrink: str = None,
-        template_name: str = None,
-    ):
-        self.memo = memo
-        self.template_shrink = template_shrink
-        self.template_name = template_name
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.memo is not None:
-            result['Memo'] = self.memo
-        if self.template_shrink is not None:
-            result['Template'] = self.template_shrink
-        if self.template_name is not None:
-            result['TemplateName'] = self.template_name
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Memo') is not None:
-            self.memo = m.get('Memo')
-        if m.get('Template') is not None:
-            self.template_shrink = m.get('Template')
-        if m.get('TemplateName') is not None:
-            self.template_name = m.get('TemplateName')
-        return self
-
-
-class CreateCardSmsTemplateResponseBodyData(TeaModel):
-    def __init__(
-        self,
-        template_code: str = None,
-    ):
-        self.template_code = template_code
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.template_code is not None:
-            result['TemplateCode'] = self.template_code
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('TemplateCode') is not None:
-            self.template_code = m.get('TemplateCode')
-        return self
-
-
-class CreateCardSmsTemplateResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        data: CreateCardSmsTemplateResponseBodyData = None,
-        request_id: str = None,
-        success: bool = None,
-    ):
-        self.code = code
-        self.data = data
-        self.request_id = request_id
-        self.success = success
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = CreateCardSmsTemplateResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class CreateCardSmsTemplateResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        body: CreateCardSmsTemplateResponseBody = None,
-    ):
-        self.headers = headers
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = CreateCardSmsTemplateResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DeleteShortUrlRequest(TeaModel):
     def __init__(
         self,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         source_url: str = None,
@@ -1075,317 +886,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DeleteSmsTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetMediaResourceIdRequest(TeaModel):
-    def __init__(
-        self,
-        extend_info: str = None,
-        file_size: int = None,
-        memo: str = None,
-        oss_key: str = None,
-        resource_type: int = None,
-    ):
-        self.extend_info = extend_info
-        self.file_size = file_size
-        self.memo = memo
-        self.oss_key = oss_key
-        self.resource_type = resource_type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.extend_info is not None:
-            result['ExtendInfo'] = self.extend_info
-        if self.file_size is not None:
-            result['FileSize'] = self.file_size
-        if self.memo is not None:
-            result['Memo'] = self.memo
-        if self.oss_key is not None:
-            result['OssKey'] = self.oss_key
-        if self.resource_type is not None:
-            result['ResourceType'] = self.resource_type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ExtendInfo') is not None:
-            self.extend_info = m.get('ExtendInfo')
-        if m.get('FileSize') is not None:
-            self.file_size = m.get('FileSize')
-        if m.get('Memo') is not None:
-            self.memo = m.get('Memo')
-        if m.get('OssKey') is not None:
-            self.oss_key = m.get('OssKey')
-        if m.get('ResourceType') is not None:
-            self.resource_type = m.get('ResourceType')
-        return self
-
-
-class GetMediaResourceIdResponseBodyData(TeaModel):
-    def __init__(
-        self,
-        resource_id: int = None,
-    ):
-        self.resource_id = resource_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.resource_id is not None:
-            result['ResourceId'] = self.resource_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ResourceId') is not None:
-            self.resource_id = m.get('ResourceId')
-        return self
-
-
-class GetMediaResourceIdResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        data: GetMediaResourceIdResponseBodyData = None,
-        request_id: str = None,
-        success: bool = None,
-    ):
-        self.code = code
-        self.data = data
-        self.request_id = request_id
-        self.success = success
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetMediaResourceIdResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class GetMediaResourceIdResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        body: GetMediaResourceIdResponseBody = None,
-    ):
-        self.headers = headers
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = GetMediaResourceIdResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class GetOSSInfoForCardTemplateResponseBodyData(TeaModel):
-    def __init__(
-        self,
-        access_key_id: str = None,
-        ali_uid: str = None,
-        expire_time: str = None,
-        host: str = None,
-        policy: str = None,
-        signature: str = None,
-    ):
-        self.access_key_id = access_key_id
-        self.ali_uid = ali_uid
-        self.expire_time = expire_time
-        self.host = host
-        self.policy = policy
-        self.signature = signature
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.access_key_id is not None:
-            result['AccessKeyId'] = self.access_key_id
-        if self.ali_uid is not None:
-            result['AliUid'] = self.ali_uid
-        if self.expire_time is not None:
-            result['ExpireTime'] = self.expire_time
-        if self.host is not None:
-            result['Host'] = self.host
-        if self.policy is not None:
-            result['Policy'] = self.policy
-        if self.signature is not None:
-            result['Signature'] = self.signature
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('AccessKeyId') is not None:
-            self.access_key_id = m.get('AccessKeyId')
-        if m.get('AliUid') is not None:
-            self.ali_uid = m.get('AliUid')
-        if m.get('ExpireTime') is not None:
-            self.expire_time = m.get('ExpireTime')
-        if m.get('Host') is not None:
-            self.host = m.get('Host')
-        if m.get('Policy') is not None:
-            self.policy = m.get('Policy')
-        if m.get('Signature') is not None:
-            self.signature = m.get('Signature')
-        return self
-
-
-class GetOSSInfoForCardTemplateResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        data: GetOSSInfoForCardTemplateResponseBodyData = None,
-        request_id: str = None,
-        success: bool = None,
-    ):
-        self.code = code
-        self.data = data
-        self.request_id = request_id
-        self.success = success
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetOSSInfoForCardTemplateResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class GetOSSInfoForCardTemplateResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        body: GetOSSInfoForCardTemplateResponseBody = None,
-    ):
-        self.headers = headers
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = GetOSSInfoForCardTemplateResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -2001,120 +1509,245 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ModifySmsTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryCardSmsTemplateRequest(TeaModel):
+class QuerySendDetailsRequest(TeaModel):
     def __init__(
         self,
+        biz_id: str = None,
+        current_page: int = None,
+        owner_id: int = None,
+        page_size: int = None,
+        phone_number: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+        send_date: str = None,
+    ):
+        self.biz_id = biz_id
+        self.current_page = current_page
+        self.owner_id = owner_id
+        self.page_size = page_size
+        self.phone_number = phone_number
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+        self.send_date = send_date
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_id is not None:
+            result['BizId'] = self.biz_id
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.send_date is not None:
+            result['SendDate'] = self.send_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BizId') is not None:
+            self.biz_id = m.get('BizId')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('SendDate') is not None:
+            self.send_date = m.get('SendDate')
+        return self
+
+
+class QuerySendDetailsResponseBodySmsSendDetailDTOsSmsSendDetailDTO(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        err_code: str = None,
+        out_id: str = None,
+        phone_num: str = None,
+        receive_date: str = None,
+        send_date: str = None,
+        send_status: int = None,
         template_code: str = None,
     ):
+        self.content = content
+        self.err_code = err_code
+        self.out_id = out_id
+        self.phone_num = phone_num
+        self.receive_date = receive_date
+        self.send_date = send_date
+        self.send_status = send_status
         self.template_code = template_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.err_code is not None:
+            result['ErrCode'] = self.err_code
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
+        if self.phone_num is not None:
+            result['PhoneNum'] = self.phone_num
+        if self.receive_date is not None:
+            result['ReceiveDate'] = self.receive_date
+        if self.send_date is not None:
+            result['SendDate'] = self.send_date
+        if self.send_status is not None:
+            result['SendStatus'] = self.send_status
         if self.template_code is not None:
             result['TemplateCode'] = self.template_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('ErrCode') is not None:
+            self.err_code = m.get('ErrCode')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
+        if m.get('PhoneNum') is not None:
+            self.phone_num = m.get('PhoneNum')
+        if m.get('ReceiveDate') is not None:
+            self.receive_date = m.get('ReceiveDate')
+        if m.get('SendDate') is not None:
+            self.send_date = m.get('SendDate')
+        if m.get('SendStatus') is not None:
+            self.send_status = m.get('SendStatus')
         if m.get('TemplateCode') is not None:
             self.template_code = m.get('TemplateCode')
         return self
 
 
-class QueryCardSmsTemplateResponseBodyData(TeaModel):
+class QuerySendDetailsResponseBodySmsSendDetailDTOs(TeaModel):
     def __init__(
         self,
-        templates: List[Dict[str, Any]] = None,
+        sms_send_detail_dto: List[QuerySendDetailsResponseBodySmsSendDetailDTOsSmsSendDetailDTO] = None,
     ):
-        self.templates = templates
+        self.sms_send_detail_dto = sms_send_detail_dto
 
     def validate(self):
-        pass
+        if self.sms_send_detail_dto:
+            for k in self.sms_send_detail_dto:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.templates is not None:
-            result['Templates'] = self.templates
+        result['SmsSendDetailDTO'] = []
+        if self.sms_send_detail_dto is not None:
+            for k in self.sms_send_detail_dto:
+                result['SmsSendDetailDTO'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Templates') is not None:
-            self.templates = m.get('Templates')
+        self.sms_send_detail_dto = []
+        if m.get('SmsSendDetailDTO') is not None:
+            for k in m.get('SmsSendDetailDTO'):
+                temp_model = QuerySendDetailsResponseBodySmsSendDetailDTOsSmsSendDetailDTO()
+                self.sms_send_detail_dto.append(temp_model.from_map(k))
         return self
 
 
-class QueryCardSmsTemplateResponseBody(TeaModel):
+class QuerySendDetailsResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
-        data: QueryCardSmsTemplateResponseBodyData = None,
+        message: str = None,
         request_id: str = None,
-        success: bool = None,
+        sms_send_detail_dtos: QuerySendDetailsResponseBodySmsSendDetailDTOs = None,
+        total_count: str = None,
     ):
         self.code = code
-        self.data = data
+        self.message = message
         self.request_id = request_id
-        self.success = success
+        self.sms_send_detail_dtos = sms_send_detail_dtos
+        self.total_count = total_count
 
     def validate(self):
-        if self.data:
-            self.data.validate()
+        if self.sms_send_detail_dtos:
+            self.sms_send_detail_dtos.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.sms_send_detail_dtos is not None:
+            result['SmsSendDetailDTOs'] = self.sms_send_detail_dtos.to_map()
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = QueryCardSmsTemplateResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('SmsSendDetailDTOs') is not None:
+            temp_model = QuerySendDetailsResponseBodySmsSendDetailDTOs()
+            self.sms_send_detail_dtos = temp_model.from_map(m['SmsSendDetailDTOs'])
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
         return self
 
 
-class QueryCardSmsTemplateResponse(TeaModel):
+class QuerySendDetailsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: QueryCardSmsTemplateResponseBody = None,
+        body: QuerySendDetailsResponseBody = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
@@ -2134,250 +1767,232 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = QueryCardSmsTemplateResponseBody()
+            temp_model = QuerySendDetailsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QuerySendDetailsRequest(TeaModel):
+class QuerySendStatisticsRequest(TeaModel):
     def __init__(
         self,
-        biz_id: str = None,
-        current_page: int = None,
+        end_date: str = None,
+        is_globe: int = None,
         owner_id: int = None,
+        page_index: int = None,
         page_size: int = None,
-        phone_number: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
-        send_date: str = None,
+        start_date: str = None,
     ):
-        self.biz_id = biz_id
-        self.current_page = current_page
+        self.end_date = end_date
+        self.is_globe = is_globe
         self.owner_id = owner_id
+        self.page_index = page_index
         self.page_size = page_size
-        self.phone_number = phone_number
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
-        self.send_date = send_date
+        self.start_date = start_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.biz_id is not None:
-            result['BizId'] = self.biz_id
-        if self.current_page is not None:
-            result['CurrentPage'] = self.current_page
+        if self.end_date is not None:
+            result['EndDate'] = self.end_date
+        if self.is_globe is not None:
+            result['IsGlobe'] = self.is_globe
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.page_index is not None:
+            result['PageIndex'] = self.page_index
         if self.page_size is not None:
             result['PageSize'] = self.page_size
-        if self.phone_number is not None:
-            result['PhoneNumber'] = self.phone_number
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.send_date is not None:
-            result['SendDate'] = self.send_date
+        if self.start_date is not None:
+            result['StartDate'] = self.start_date
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('BizId') is not None:
-            self.biz_id = m.get('BizId')
-        if m.get('CurrentPage') is not None:
-            self.current_page = m.get('CurrentPage')
+        if m.get('EndDate') is not None:
+            self.end_date = m.get('EndDate')
+        if m.get('IsGlobe') is not None:
+            self.is_globe = m.get('IsGlobe')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PageIndex') is not None:
+            self.page_index = m.get('PageIndex')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
-        if m.get('PhoneNumber') is not None:
-            self.phone_number = m.get('PhoneNumber')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('SendDate') is not None:
-            self.send_date = m.get('SendDate')
+        if m.get('StartDate') is not None:
+            self.start_date = m.get('StartDate')
         return self
 
 
-class QuerySendDetailsResponseBodySmsSendDetailDTOsSmsSendDetailDTO(TeaModel):
+class QuerySendStatisticsResponseBodyDataTargetList(TeaModel):
     def __init__(
         self,
-        content: str = None,
-        err_code: str = None,
-        out_id: str = None,
-        phone_num: str = None,
-        receive_date: str = None,
+        no_responded_count: int = None,
+        responded_fail_count: int = None,
+        responded_success_count: int = None,
         send_date: str = None,
-        send_status: int = None,
-        template_code: str = None,
+        total_count: int = None,
     ):
-        self.content = content
-        self.err_code = err_code
-        self.out_id = out_id
-        self.phone_num = phone_num
-        self.receive_date = receive_date
+        self.no_responded_count = no_responded_count
+        self.responded_fail_count = responded_fail_count
+        self.responded_success_count = responded_success_count
         self.send_date = send_date
-        self.send_status = send_status
-        self.template_code = template_code
+        self.total_count = total_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.content is not None:
-            result['Content'] = self.content
-        if self.err_code is not None:
-            result['ErrCode'] = self.err_code
-        if self.out_id is not None:
-            result['OutId'] = self.out_id
-        if self.phone_num is not None:
-            result['PhoneNum'] = self.phone_num
-        if self.receive_date is not None:
-            result['ReceiveDate'] = self.receive_date
+        if self.no_responded_count is not None:
+            result['NoRespondedCount'] = self.no_responded_count
+        if self.responded_fail_count is not None:
+            result['RespondedFailCount'] = self.responded_fail_count
+        if self.responded_success_count is not None:
+            result['RespondedSuccessCount'] = self.responded_success_count
         if self.send_date is not None:
             result['SendDate'] = self.send_date
-        if self.send_status is not None:
-            result['SendStatus'] = self.send_status
-        if self.template_code is not None:
-            result['TemplateCode'] = self.template_code
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Content') is not None:
-            self.content = m.get('Content')
-        if m.get('ErrCode') is not None:
-            self.err_code = m.get('ErrCode')
-        if m.get('OutId') is not None:
-            self.out_id = m.get('OutId')
-        if m.get('PhoneNum') is not None:
-            self.phone_num = m.get('PhoneNum')
-        if m.get('ReceiveDate') is not None:
-            self.receive_date = m.get('ReceiveDate')
+        if m.get('NoRespondedCount') is not None:
+            self.no_responded_count = m.get('NoRespondedCount')
+        if m.get('RespondedFailCount') is not None:
+            self.responded_fail_count = m.get('RespondedFailCount')
+        if m.get('RespondedSuccessCount') is not None:
+            self.responded_success_count = m.get('RespondedSuccessCount')
         if m.get('SendDate') is not None:
             self.send_date = m.get('SendDate')
-        if m.get('SendStatus') is not None:
-            self.send_status = m.get('SendStatus')
-        if m.get('TemplateCode') is not None:
-            self.template_code = m.get('TemplateCode')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
         return self
 
 
-class QuerySendDetailsResponseBodySmsSendDetailDTOs(TeaModel):
+class QuerySendStatisticsResponseBodyData(TeaModel):
     def __init__(
         self,
-        sms_send_detail_dto: List[QuerySendDetailsResponseBodySmsSendDetailDTOsSmsSendDetailDTO] = None,
+        target_list: List[QuerySendStatisticsResponseBodyDataTargetList] = None,
+        total_size: int = None,
     ):
-        self.sms_send_detail_dto = sms_send_detail_dto
+        self.target_list = target_list
+        self.total_size = total_size
 
     def validate(self):
-        if self.sms_send_detail_dto:
-            for k in self.sms_send_detail_dto:
+        if self.target_list:
+            for k in self.target_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['SmsSendDetailDTO'] = []
-        if self.sms_send_detail_dto is not None:
-            for k in self.sms_send_detail_dto:
-                result['SmsSendDetailDTO'].append(k.to_map() if k else None)
+        result['TargetList'] = []
+        if self.target_list is not None:
+            for k in self.target_list:
+                result['TargetList'].append(k.to_map() if k else None)
+        if self.total_size is not None:
+            result['TotalSize'] = self.total_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.sms_send_detail_dto = []
-        if m.get('SmsSendDetailDTO') is not None:
-            for k in m.get('SmsSendDetailDTO'):
-                temp_model = QuerySendDetailsResponseBodySmsSendDetailDTOsSmsSendDetailDTO()
-                self.sms_send_detail_dto.append(temp_model.from_map(k))
+        self.target_list = []
+        if m.get('TargetList') is not None:
+            for k in m.get('TargetList'):
+                temp_model = QuerySendStatisticsResponseBodyDataTargetList()
+                self.target_list.append(temp_model.from_map(k))
+        if m.get('TotalSize') is not None:
+            self.total_size = m.get('TotalSize')
         return self
 
 
-class QuerySendDetailsResponseBody(TeaModel):
+class QuerySendStatisticsResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
+        data: QuerySendStatisticsResponseBodyData = None,
         message: str = None,
         request_id: str = None,
-        sms_send_detail_dtos: QuerySendDetailsResponseBodySmsSendDetailDTOs = None,
-        total_count: str = None,
     ):
         self.code = code
+        self.data = data
         self.message = message
         self.request_id = request_id
-        self.sms_send_detail_dtos = sms_send_detail_dtos
-        self.total_count = total_count
 
     def validate(self):
-        if self.sms_send_detail_dtos:
-            self.sms_send_detail_dtos.validate()
+        if self.data:
+            self.data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.sms_send_detail_dtos is not None:
-            result['SmsSendDetailDTOs'] = self.sms_send_detail_dtos.to_map()
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = QuerySendStatisticsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('SmsSendDetailDTOs') is not None:
-            temp_model = QuerySendDetailsResponseBodySmsSendDetailDTOs()
-            self.sms_send_detail_dtos = temp_model.from_map(m['SmsSendDetailDTOs'])
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
         return self
 
 
-class QuerySendDetailsResponse(TeaModel):
+class QuerySendStatisticsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: QuerySendDetailsResponseBody = None,
+        body: QuerySendStatisticsResponseBody = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
@@ -2397,15 +2012,15 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = QuerySendDetailsResponseBody()
+            temp_model = QuerySendStatisticsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryShortUrlRequest(TeaModel):
     def __init__(
         self,
@@ -2745,14 +2360,253 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = QuerySmsSignResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QuerySmsSignListRequest(TeaModel):
+    def __init__(
+        self,
+        owner_id: int = None,
+        page_index: int = None,
+        page_size: int = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.owner_id = owner_id
+        self.page_index = page_index
+        self.page_size = page_size
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.page_index is not None:
+            result['PageIndex'] = self.page_index
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PageIndex') is not None:
+            self.page_index = m.get('PageIndex')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class QuerySmsSignListResponseBodySmsSignListReason(TeaModel):
+    def __init__(
+        self,
+        reject_date: str = None,
+        reject_info: str = None,
+        reject_sub_info: str = None,
+    ):
+        self.reject_date = reject_date
+        self.reject_info = reject_info
+        self.reject_sub_info = reject_sub_info
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.reject_date is not None:
+            result['RejectDate'] = self.reject_date
+        if self.reject_info is not None:
+            result['RejectInfo'] = self.reject_info
+        if self.reject_sub_info is not None:
+            result['RejectSubInfo'] = self.reject_sub_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RejectDate') is not None:
+            self.reject_date = m.get('RejectDate')
+        if m.get('RejectInfo') is not None:
+            self.reject_info = m.get('RejectInfo')
+        if m.get('RejectSubInfo') is not None:
+            self.reject_sub_info = m.get('RejectSubInfo')
+        return self
+
+
+class QuerySmsSignListResponseBodySmsSignList(TeaModel):
+    def __init__(
+        self,
+        audit_status: str = None,
+        business_type: str = None,
+        create_date: str = None,
+        order_id: str = None,
+        reason: QuerySmsSignListResponseBodySmsSignListReason = None,
+        sign_name: str = None,
+    ):
+        self.audit_status = audit_status
+        self.business_type = business_type
+        self.create_date = create_date
+        self.order_id = order_id
+        self.reason = reason
+        self.sign_name = sign_name
+
+    def validate(self):
+        if self.reason:
+            self.reason.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audit_status is not None:
+            result['AuditStatus'] = self.audit_status
+        if self.business_type is not None:
+            result['BusinessType'] = self.business_type
+        if self.create_date is not None:
+            result['CreateDate'] = self.create_date
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.reason is not None:
+            result['Reason'] = self.reason.to_map()
+        if self.sign_name is not None:
+            result['SignName'] = self.sign_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuditStatus') is not None:
+            self.audit_status = m.get('AuditStatus')
+        if m.get('BusinessType') is not None:
+            self.business_type = m.get('BusinessType')
+        if m.get('CreateDate') is not None:
+            self.create_date = m.get('CreateDate')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Reason') is not None:
+            temp_model = QuerySmsSignListResponseBodySmsSignListReason()
+            self.reason = temp_model.from_map(m['Reason'])
+        if m.get('SignName') is not None:
+            self.sign_name = m.get('SignName')
+        return self
+
+
+class QuerySmsSignListResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        sms_sign_list: List[QuerySmsSignListResponseBodySmsSignList] = None,
+    ):
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.sms_sign_list = sms_sign_list
+
+    def validate(self):
+        if self.sms_sign_list:
+            for k in self.sms_sign_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+        result['SmsSignList'] = []
+        if self.sms_sign_list is not None:
+            for k in self.sms_sign_list:
+                result['SmsSignList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.sms_sign_list = []
+        if m.get('SmsSignList') is not None:
+            for k in m.get('SmsSignList'):
+                temp_model = QuerySmsSignListResponseBodySmsSignList()
+                self.sms_sign_list.append(temp_model.from_map(k))
+        return self
+
+
+class QuerySmsSignListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: QuerySmsSignListResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QuerySmsSignListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QuerySmsTemplateRequest(TeaModel):
     def __init__(
         self,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         template_code: str = None,
@@ -2908,402 +2762,384 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = QuerySmsTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class SendBatchSmsRequest(TeaModel):
+class QuerySmsTemplateListRequest(TeaModel):
     def __init__(
         self,
         owner_id: int = None,
-        phone_number_json: str = None,
+        page_index: int = None,
+        page_size: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
-        sign_name_json: str = None,
-        sms_up_extend_code_json: str = None,
-        template_code: str = None,
-        template_param_json: str = None,
     ):
         self.owner_id = owner_id
-        self.phone_number_json = phone_number_json
+        self.page_index = page_index
+        self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
-        self.sign_name_json = sign_name_json
-        self.sms_up_extend_code_json = sms_up_extend_code_json
-        self.template_code = template_code
-        self.template_param_json = template_param_json
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
-        if self.phone_number_json is not None:
-            result['PhoneNumberJson'] = self.phone_number_json
+        if self.page_index is not None:
+            result['PageIndex'] = self.page_index
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.sign_name_json is not None:
-            result['SignNameJson'] = self.sign_name_json
-        if self.sms_up_extend_code_json is not None:
-            result['SmsUpExtendCodeJson'] = self.sms_up_extend_code_json
-        if self.template_code is not None:
-            result['TemplateCode'] = self.template_code
-        if self.template_param_json is not None:
-            result['TemplateParamJson'] = self.template_param_json
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
-        if m.get('PhoneNumberJson') is not None:
-            self.phone_number_json = m.get('PhoneNumberJson')
+        if m.get('PageIndex') is not None:
+            self.page_index = m.get('PageIndex')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('SignNameJson') is not None:
-            self.sign_name_json = m.get('SignNameJson')
-        if m.get('SmsUpExtendCodeJson') is not None:
-            self.sms_up_extend_code_json = m.get('SmsUpExtendCodeJson')
-        if m.get('TemplateCode') is not None:
-            self.template_code = m.get('TemplateCode')
-        if m.get('TemplateParamJson') is not None:
-            self.template_param_json = m.get('TemplateParamJson')
         return self
 
 
-class SendBatchSmsResponseBody(TeaModel):
+class QuerySmsTemplateListResponseBodySmsTemplateListReason(TeaModel):
     def __init__(
         self,
-        biz_id: str = None,
-        code: str = None,
-        message: str = None,
-        request_id: str = None,
+        reject_date: str = None,
+        reject_info: str = None,
+        reject_sub_info: str = None,
     ):
-        self.biz_id = biz_id
-        self.code = code
-        self.message = message
-        self.request_id = request_id
+        self.reject_date = reject_date
+        self.reject_info = reject_info
+        self.reject_sub_info = reject_sub_info
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.biz_id is not None:
-            result['BizId'] = self.biz_id
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
+        if self.reject_date is not None:
+            result['RejectDate'] = self.reject_date
+        if self.reject_info is not None:
+            result['RejectInfo'] = self.reject_info
+        if self.reject_sub_info is not None:
+            result['RejectSubInfo'] = self.reject_sub_info
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('BizId') is not None:
-            self.biz_id = m.get('BizId')
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
+        if m.get('RejectDate') is not None:
+            self.reject_date = m.get('RejectDate')
+        if m.get('RejectInfo') is not None:
+            self.reject_info = m.get('RejectInfo')
+        if m.get('RejectSubInfo') is not None:
+            self.reject_sub_info = m.get('RejectSubInfo')
         return self
 
 
-class SendBatchSmsResponse(TeaModel):
+class QuerySmsTemplateListResponseBodySmsTemplateList(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        body: SendBatchSmsResponseBody = None,
+        audit_status: str = None,
+        create_date: str = None,
+        order_id: str = None,
+        reason: QuerySmsTemplateListResponseBodySmsTemplateListReason = None,
+        template_code: str = None,
+        template_content: str = None,
+        template_name: str = None,
+        template_type: int = None,
     ):
-        self.headers = headers
-        self.body = body
+        self.audit_status = audit_status
+        self.create_date = create_date
+        self.order_id = order_id
+        self.reason = reason
+        self.template_code = template_code
+        self.template_content = template_content
+        self.template_name = template_name
+        self.template_type = template_type
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        if self.reason:
+            self.reason.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.audit_status is not None:
+            result['AuditStatus'] = self.audit_status
+        if self.create_date is not None:
+            result['CreateDate'] = self.create_date
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.reason is not None:
+            result['Reason'] = self.reason.to_map()
+        if self.template_code is not None:
+            result['TemplateCode'] = self.template_code
+        if self.template_content is not None:
+            result['TemplateContent'] = self.template_content
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        if self.template_type is not None:
+            result['TemplateType'] = self.template_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = SendBatchSmsResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('AuditStatus') is not None:
+            self.audit_status = m.get('AuditStatus')
+        if m.get('CreateDate') is not None:
+            self.create_date = m.get('CreateDate')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Reason') is not None:
+            temp_model = QuerySmsTemplateListResponseBodySmsTemplateListReason()
+            self.reason = temp_model.from_map(m['Reason'])
+        if m.get('TemplateCode') is not None:
+            self.template_code = m.get('TemplateCode')
+        if m.get('TemplateContent') is not None:
+            self.template_content = m.get('TemplateContent')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        if m.get('TemplateType') is not None:
+            self.template_type = m.get('TemplateType')
         return self
 
 
-class SendCardSmsRequestCardObjects(TeaModel):
+class QuerySmsTemplateListResponseBody(TeaModel):
     def __init__(
         self,
-        custom_url: str = None,
-        dync_params: str = None,
-        mobile: str = None,
+        code: str = None,
+        message: str = None,
+        request_id: str = None,
+        sms_template_list: List[QuerySmsTemplateListResponseBodySmsTemplateList] = None,
     ):
-        self.custom_url = custom_url
-        self.dync_params = dync_params
-        self.mobile = mobile
+        self.code = code
+        self.message = message
+        self.request_id = request_id
+        self.sms_template_list = sms_template_list
 
     def validate(self):
-        pass
+        if self.sms_template_list:
+            for k in self.sms_template_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.custom_url is not None:
-            result['customUrl'] = self.custom_url
-        if self.dync_params is not None:
-            result['dyncParams'] = self.dync_params
-        if self.mobile is not None:
-            result['mobile'] = self.mobile
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['SmsTemplateList'] = []
+        if self.sms_template_list is not None:
+            for k in self.sms_template_list:
+                result['SmsTemplateList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('customUrl') is not None:
-            self.custom_url = m.get('customUrl')
-        if m.get('dyncParams') is not None:
-            self.dync_params = m.get('dyncParams')
-        if m.get('mobile') is not None:
-            self.mobile = m.get('mobile')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.sms_template_list = []
+        if m.get('SmsTemplateList') is not None:
+            for k in m.get('SmsTemplateList'):
+                temp_model = QuerySmsTemplateListResponseBodySmsTemplateList()
+                self.sms_template_list.append(temp_model.from_map(k))
         return self
 
 
-class SendCardSmsRequest(TeaModel):
+class QuerySmsTemplateListResponse(TeaModel):
     def __init__(
         self,
-        card_objects: List[SendCardSmsRequestCardObjects] = None,
-        card_template_code: str = None,
-        digital_template_code: str = None,
-        digital_template_param: str = None,
-        fallback_type: str = None,
-        out_id: str = None,
-        sign_name: str = None,
-        sms_template_code: str = None,
-        sms_template_param: str = None,
-        sms_up_extend_code: str = None,
-    ):
-        self.card_objects = card_objects
-        self.card_template_code = card_template_code
-        self.digital_template_code = digital_template_code
-        self.digital_template_param = digital_template_param
-        self.fallback_type = fallback_type
-        self.out_id = out_id
-        self.sign_name = sign_name
-        self.sms_template_code = sms_template_code
-        self.sms_template_param = sms_template_param
-        self.sms_up_extend_code = sms_up_extend_code
+        headers: Dict[str, str] = None,
+        body: QuerySmsTemplateListResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
 
     def validate(self):
-        if self.card_objects:
-            for k in self.card_objects:
-                if k:
-                    k.validate()
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['CardObjects'] = []
-        if self.card_objects is not None:
-            for k in self.card_objects:
-                result['CardObjects'].append(k.to_map() if k else None)
-        if self.card_template_code is not None:
-            result['CardTemplateCode'] = self.card_template_code
-        if self.digital_template_code is not None:
-            result['DigitalTemplateCode'] = self.digital_template_code
-        if self.digital_template_param is not None:
-            result['DigitalTemplateParam'] = self.digital_template_param
-        if self.fallback_type is not None:
-            result['FallbackType'] = self.fallback_type
-        if self.out_id is not None:
-            result['OutId'] = self.out_id
-        if self.sign_name is not None:
-            result['SignName'] = self.sign_name
-        if self.sms_template_code is not None:
-            result['SmsTemplateCode'] = self.sms_template_code
-        if self.sms_template_param is not None:
-            result['SmsTemplateParam'] = self.sms_template_param
-        if self.sms_up_extend_code is not None:
-            result['SmsUpExtendCode'] = self.sms_up_extend_code
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.card_objects = []
-        if m.get('CardObjects') is not None:
-            for k in m.get('CardObjects'):
-                temp_model = SendCardSmsRequestCardObjects()
-                self.card_objects.append(temp_model.from_map(k))
-        if m.get('CardTemplateCode') is not None:
-            self.card_template_code = m.get('CardTemplateCode')
-        if m.get('DigitalTemplateCode') is not None:
-            self.digital_template_code = m.get('DigitalTemplateCode')
-        if m.get('DigitalTemplateParam') is not None:
-            self.digital_template_param = m.get('DigitalTemplateParam')
-        if m.get('FallbackType') is not None:
-            self.fallback_type = m.get('FallbackType')
-        if m.get('OutId') is not None:
-            self.out_id = m.get('OutId')
-        if m.get('SignName') is not None:
-            self.sign_name = m.get('SignName')
-        if m.get('SmsTemplateCode') is not None:
-            self.sms_template_code = m.get('SmsTemplateCode')
-        if m.get('SmsTemplateParam') is not None:
-            self.sms_template_param = m.get('SmsTemplateParam')
-        if m.get('SmsUpExtendCode') is not None:
-            self.sms_up_extend_code = m.get('SmsUpExtendCode')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QuerySmsTemplateListResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class SendCardSmsResponseBodyData(TeaModel):
+class SendBatchSmsRequest(TeaModel):
     def __init__(
         self,
-        biz_card_id: str = None,
-        biz_digital_id: str = None,
-        biz_sms_id: str = None,
-        card_tmp_state: int = None,
-        media_mobiles: str = None,
-        not_media_mobiles: str = None,
+        owner_id: int = None,
+        phone_number_json: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+        sign_name_json: str = None,
+        sms_up_extend_code_json: str = None,
+        template_code: str = None,
+        template_param_json: str = None,
     ):
-        self.biz_card_id = biz_card_id
-        self.biz_digital_id = biz_digital_id
-        self.biz_sms_id = biz_sms_id
-        self.card_tmp_state = card_tmp_state
-        self.media_mobiles = media_mobiles
-        self.not_media_mobiles = not_media_mobiles
+        self.owner_id = owner_id
+        self.phone_number_json = phone_number_json
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+        self.sign_name_json = sign_name_json
+        self.sms_up_extend_code_json = sms_up_extend_code_json
+        self.template_code = template_code
+        self.template_param_json = template_param_json
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.biz_card_id is not None:
-            result['BizCardId'] = self.biz_card_id
-        if self.biz_digital_id is not None:
-            result['BizDigitalId'] = self.biz_digital_id
-        if self.biz_sms_id is not None:
-            result['BizSmsId'] = self.biz_sms_id
-        if self.card_tmp_state is not None:
-            result['CardTmpState'] = self.card_tmp_state
-        if self.media_mobiles is not None:
-            result['MediaMobiles'] = self.media_mobiles
-        if self.not_media_mobiles is not None:
-            result['NotMediaMobiles'] = self.not_media_mobiles
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.phone_number_json is not None:
+            result['PhoneNumberJson'] = self.phone_number_json
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.sign_name_json is not None:
+            result['SignNameJson'] = self.sign_name_json
+        if self.sms_up_extend_code_json is not None:
+            result['SmsUpExtendCodeJson'] = self.sms_up_extend_code_json
+        if self.template_code is not None:
+            result['TemplateCode'] = self.template_code
+        if self.template_param_json is not None:
+            result['TemplateParamJson'] = self.template_param_json
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('BizCardId') is not None:
-            self.biz_card_id = m.get('BizCardId')
-        if m.get('BizDigitalId') is not None:
-            self.biz_digital_id = m.get('BizDigitalId')
-        if m.get('BizSmsId') is not None:
-            self.biz_sms_id = m.get('BizSmsId')
-        if m.get('CardTmpState') is not None:
-            self.card_tmp_state = m.get('CardTmpState')
-        if m.get('MediaMobiles') is not None:
-            self.media_mobiles = m.get('MediaMobiles')
-        if m.get('NotMediaMobiles') is not None:
-            self.not_media_mobiles = m.get('NotMediaMobiles')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PhoneNumberJson') is not None:
+            self.phone_number_json = m.get('PhoneNumberJson')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('SignNameJson') is not None:
+            self.sign_name_json = m.get('SignNameJson')
+        if m.get('SmsUpExtendCodeJson') is not None:
+            self.sms_up_extend_code_json = m.get('SmsUpExtendCodeJson')
+        if m.get('TemplateCode') is not None:
+            self.template_code = m.get('TemplateCode')
+        if m.get('TemplateParamJson') is not None:
+            self.template_param_json = m.get('TemplateParamJson')
         return self
 
 
-class SendCardSmsResponseBody(TeaModel):
+class SendBatchSmsResponseBody(TeaModel):
     def __init__(
         self,
+        biz_id: str = None,
         code: str = None,
-        data: SendCardSmsResponseBodyData = None,
+        message: str = None,
         request_id: str = None,
-        success: bool = None,
     ):
+        self.biz_id = biz_id
         self.code = code
-        self.data = data
+        self.message = message
         self.request_id = request_id
-        self.success = success
 
     def validate(self):
-        if self.data:
-            self.data.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.biz_id is not None:
+            result['BizId'] = self.biz_id
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('BizId') is not None:
+            self.biz_id = m.get('BizId')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = SendCardSmsResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         return self
 
 
-class SendCardSmsResponse(TeaModel):
+class SendBatchSmsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: SendCardSmsResponseBody = None,
+        body: SendBatchSmsResponseBody = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
@@ -3323,15 +3159,15 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = SendCardSmsResponseBody()
+            temp_model = SendBatchSmsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SendSmsRequest(TeaModel):
     def __init__(
         self,
```

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/alibabacloud_dysmsapi20170525.egg-info/PKG-INFO` & `alibabacloud_dysmsapi20170525-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dysmsapi20170525
-Version: 2.0.8
+Name: alibabacloud_dysmsapi20170525
+Version: 2.0.9
 Summary: Alibaba Cloud Dysmsapi (20170525) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dysmsapi20170525-2.0.8/setup.py` & `alibabacloud_dysmsapi20170525-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dysmsapi20170525.
 
-Created on 29/11/2021
+Created on 24/01/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dysmsapi20170525"
 NAME = "alibabacloud_dysmsapi20170525" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dysmsapi (20170525) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.2.10, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.5, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

