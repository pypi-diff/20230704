# Comparing `tmp/alibabacloud_ocr20191230-2.0.9.tar.gz` & `tmp/alibabacloud_ocr20191230-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ocr20191230-2.0.9.tar", last modified: Wed May 25 07:25:25 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ocr20191230-3.0.0.tar", last modified: Tue Jul  4 02:19:00 2023, max compression
```

## Comparing `alibabacloud_ocr20191230-2.0.9.tar` & `alibabacloud_ocr20191230-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/
--rw-r--r--   0 root         (0) root         (0)      712 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230/__init__.py
--rw-r--r--   0 root         (0) root         (0)   328220 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230/client.py
--rw-r--r--   0 root         (0) root         (0)   640193 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      350 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2844 2022-05-25 07:25:25.000000 alibabacloud_ocr20191230-2.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195452 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230/client.py
+-rw-r--r--   0 root         (0) root         (0)   195224 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 02:19:00.000000 alibabacloud_ocr20191230-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-04 02:18:59.000000 alibabacloud_ocr20191230-3.0.0/setup.py
```

### Comparing `alibabacloud_ocr20191230-2.0.9/ChangeLog.md` & `alibabacloud_ocr20191230-3.0.0/ChangeLog.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+2023-02-15 Version: 2.0.16
+- Update RecognizeVideoCharacter.
+
+2023-01-13 Version: 2.0.15
+- Update sdk.
+
+2023-01-11 Version: 2.0.14
+- Update sdk.
+
+2022-11-10 Version: 2.0.13
+- Release RecognizeVATInvoice.
+
+2022-10-17 Version: 2.0.12
+- Release RecognizeVATInvoice.
+
+2022-10-14 Version: 2.0.11
+- Release RecognizeVATInvoice.
+
+2022-06-21 Version: 2.0.10
+- Release RecognizeTurkeyIdentityCard RecognizeMalaysiaIdentityCard RecognizeRussiaIdentityCard RecognizeIndonesiaIdentityCard RecognizeUkraineIdentityCard RecognizeVietnamIdentityCard.
+
+2022-05-25 Version: 2.0.9
+- Release RecognizeTurkeyIdentityCard RecognizeMalaysiaIdentityCard RecognizeRussiaIdentityCard RecognizeIndonesiaIdentityCard RecognizeIndonesiaIdentityCard.
+
 2022-05-05 Version: 2.0.8
 - Release RecognizeUkraineIdentityCard.
 
 2022-03-09 Version: 2.0.7
 - Release RecognizeVideoCastCrewList.
 
 2022-03-03 Version: 2.0.6
```

### Comparing `alibabacloud_ocr20191230-2.0.9/LICENSE` & `alibabacloud_ocr20191230-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr20191230-2.0.9/PKG-INFO` & `alibabacloud_ocr20191230-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ocr20191230
-Version: 2.0.9
+Version: 3.0.0
 Summary: Alibaba Cloud OCR (20191230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr20191230-2.0.9/README-CN.md` & `alibabacloud_ocr20191230-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr20191230-2.0.9/README.md` & `alibabacloud_ocr20191230-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230/client.py` & `alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
 from alibabacloud_ocr20191230 import models as ocr_20191230_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
-from alibabacloud_tea_rpc import models as rpc_models
 from alibabacloud_openplatform20191219.client import Client as OpenPlatformClient
 from alibabacloud_openplatform20191219 import models as open_platform_models
 from alibabacloud_oss_sdk import models as oss_models
 from alibabacloud_tea_fileform import models as file_form_models
 from alibabacloud_oss_util import models as ossutil_models
 from alibabacloud_oss_sdk.client import Client as OSSClient
+from alibabacloud_darabonba_number.client import Client as NumberClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
     def __init__(
@@ -44,226 +44,14 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def detect_card_screenshot_with_options(
-        self,
-        request: ocr_20191230_models.DetectCardScreenshotRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.DetectCardScreenshotResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='DetectCardScreenshot',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.DetectCardScreenshotResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def detect_card_screenshot_with_options_async(
-        self,
-        request: ocr_20191230_models.DetectCardScreenshotRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.DetectCardScreenshotResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='DetectCardScreenshot',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.DetectCardScreenshotResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def detect_card_screenshot(
-        self,
-        request: ocr_20191230_models.DetectCardScreenshotRequest,
-    ) -> ocr_20191230_models.DetectCardScreenshotResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.detect_card_screenshot_with_options(request, runtime)
-
-    async def detect_card_screenshot_async(
-        self,
-        request: ocr_20191230_models.DetectCardScreenshotRequest,
-    ) -> ocr_20191230_models.DetectCardScreenshotResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.detect_card_screenshot_with_options_async(request, runtime)
-
-    def detect_card_screenshot_advance(
-        self,
-        request: ocr_20191230_models.DetectCardScreenshotAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.DetectCardScreenshotResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        detect_card_screenshot_req = ocr_20191230_models.DetectCardScreenshotRequest()
-        OpenApiUtilClient.convert(request, detect_card_screenshot_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            detect_card_screenshot_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        detect_card_screenshot_resp = self.detect_card_screenshot_with_options(detect_card_screenshot_req, runtime)
-        return detect_card_screenshot_resp
-
-    async def detect_card_screenshot_advance_async(
-        self,
-        request: ocr_20191230_models.DetectCardScreenshotAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.DetectCardScreenshotResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        detect_card_screenshot_req = ocr_20191230_models.DetectCardScreenshotRequest()
-        OpenApiUtilClient.convert(request, detect_card_screenshot_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            detect_card_screenshot_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        detect_card_screenshot_resp = await self.detect_card_screenshot_with_options_async(detect_card_screenshot_req, runtime)
-        return detect_card_screenshot_resp
-
     def get_async_job_result_with_options(
         self,
         request: ocr_20191230_models.GetAsyncJobResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.GetAsyncJobResultResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -326,226 +114,14 @@
     async def get_async_job_result_async(
         self,
         request: ocr_20191230_models.GetAsyncJobResultRequest,
     ) -> ocr_20191230_models.GetAsyncJobResultResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_async_job_result_with_options_async(request, runtime)
 
-    def recognize_account_page_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeAccountPageRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeAccountPageResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeAccountPage',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeAccountPageResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_account_page_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeAccountPageRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeAccountPageResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeAccountPage',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeAccountPageResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_account_page(
-        self,
-        request: ocr_20191230_models.RecognizeAccountPageRequest,
-    ) -> ocr_20191230_models.RecognizeAccountPageResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_account_page_with_options(request, runtime)
-
-    async def recognize_account_page_async(
-        self,
-        request: ocr_20191230_models.RecognizeAccountPageRequest,
-    ) -> ocr_20191230_models.RecognizeAccountPageResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_account_page_with_options_async(request, runtime)
-
-    def recognize_account_page_advance(
-        self,
-        request: ocr_20191230_models.RecognizeAccountPageAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeAccountPageResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_account_page_req = ocr_20191230_models.RecognizeAccountPageRequest()
-        OpenApiUtilClient.convert(request, recognize_account_page_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_account_page_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_account_page_resp = self.recognize_account_page_with_options(recognize_account_page_req, runtime)
-        return recognize_account_page_resp
-
-    async def recognize_account_page_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeAccountPageAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeAccountPageResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_account_page_req = ocr_20191230_models.RecognizeAccountPageRequest()
-        OpenApiUtilClient.convert(request, recognize_account_page_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_account_page_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_account_page_resp = await self.recognize_account_page_with_options_async(recognize_account_page_req, runtime)
-        return recognize_account_page_resp
-
     def recognize_bank_card_with_options(
         self,
         request: ocr_20191230_models.RecognizeBankCardRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeBankCardResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -623,15 +199,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -654,36 +230,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_bank_card_req = ocr_20191230_models.RecognizeBankCardRequest()
         OpenApiUtilClient.convert(request, recognize_bank_card_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_bank_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_bank_card_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_bank_card_resp = self.recognize_bank_card_with_options(recognize_bank_card_req, runtime)
         return recognize_bank_card_resp
 
     async def recognize_bank_card_advance_async(
         self,
         request: ocr_20191230_models.RecognizeBankCardAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -694,15 +270,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -725,36 +301,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_bank_card_req = ocr_20191230_models.RecognizeBankCardRequest()
         OpenApiUtilClient.convert(request, recognize_bank_card_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_bank_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_bank_card_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_bank_card_resp = await self.recognize_bank_card_with_options_async(recognize_bank_card_req, runtime)
         return recognize_bank_card_resp
 
     def recognize_business_card_with_options(
         self,
         request: ocr_20191230_models.RecognizeBusinessCardRequest,
         runtime: util_models.RuntimeOptions,
@@ -835,15 +411,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -866,36 +442,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_business_card_req = ocr_20191230_models.RecognizeBusinessCardRequest()
         OpenApiUtilClient.convert(request, recognize_business_card_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_business_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_business_card_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_business_card_resp = self.recognize_business_card_with_options(recognize_business_card_req, runtime)
         return recognize_business_card_resp
 
     async def recognize_business_card_advance_async(
         self,
         request: ocr_20191230_models.RecognizeBusinessCardAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -906,15 +482,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -937,36 +513,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_business_card_req = ocr_20191230_models.RecognizeBusinessCardRequest()
         OpenApiUtilClient.convert(request, recognize_business_card_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_business_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_business_card_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_business_card_resp = await self.recognize_business_card_with_options_async(recognize_business_card_req, runtime)
         return recognize_business_card_resp
 
     def recognize_business_license_with_options(
         self,
         request: ocr_20191230_models.RecognizeBusinessLicenseRequest,
         runtime: util_models.RuntimeOptions,
@@ -1047,15 +623,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1078,36 +654,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_business_license_req = ocr_20191230_models.RecognizeBusinessLicenseRequest()
         OpenApiUtilClient.convert(request, recognize_business_license_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_business_license_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_business_license_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_business_license_resp = self.recognize_business_license_with_options(recognize_business_license_req, runtime)
         return recognize_business_license_resp
 
     async def recognize_business_license_advance_async(
         self,
         request: ocr_20191230_models.RecognizeBusinessLicenseAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -1118,15 +694,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1149,36 +725,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_business_license_req = ocr_20191230_models.RecognizeBusinessLicenseRequest()
         OpenApiUtilClient.convert(request, recognize_business_license_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_business_license_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_business_license_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_business_license_resp = await self.recognize_business_license_with_options_async(recognize_business_license_req, runtime)
         return recognize_business_license_resp
 
     def recognize_character_with_options(
         self,
         request: ocr_20191230_models.RecognizeCharacterRequest,
         runtime: util_models.RuntimeOptions,
@@ -1267,15 +843,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1298,36 +874,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_character_req = ocr_20191230_models.RecognizeCharacterRequest()
         OpenApiUtilClient.convert(request, recognize_character_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_character_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_character_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_character_resp = self.recognize_character_with_options(recognize_character_req, runtime)
         return recognize_character_resp
 
     async def recognize_character_advance_async(
         self,
         request: ocr_20191230_models.RecognizeCharacterAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -1338,15 +914,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1369,251 +945,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_character_req = ocr_20191230_models.RecognizeCharacterRequest()
         OpenApiUtilClient.convert(request, recognize_character_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_character_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_character_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_character_resp = await self.recognize_character_with_options_async(recognize_character_req, runtime)
         return recognize_character_resp
 
-    def recognize_chinapassport_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeChinapassportRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeChinapassportResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeChinapassport',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeChinapassportResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_chinapassport_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeChinapassportRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeChinapassportResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeChinapassport',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeChinapassportResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_chinapassport(
-        self,
-        request: ocr_20191230_models.RecognizeChinapassportRequest,
-    ) -> ocr_20191230_models.RecognizeChinapassportResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_chinapassport_with_options(request, runtime)
-
-    async def recognize_chinapassport_async(
-        self,
-        request: ocr_20191230_models.RecognizeChinapassportRequest,
-    ) -> ocr_20191230_models.RecognizeChinapassportResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_chinapassport_with_options_async(request, runtime)
-
-    def recognize_chinapassport_advance(
-        self,
-        request: ocr_20191230_models.RecognizeChinapassportAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeChinapassportResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_chinapassport_req = ocr_20191230_models.RecognizeChinapassportRequest()
-        OpenApiUtilClient.convert(request, recognize_chinapassport_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_chinapassport_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_chinapassport_resp = self.recognize_chinapassport_with_options(recognize_chinapassport_req, runtime)
-        return recognize_chinapassport_resp
-
-    async def recognize_chinapassport_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeChinapassportAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeChinapassportResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_chinapassport_req = ocr_20191230_models.RecognizeChinapassportRequest()
-        OpenApiUtilClient.convert(request, recognize_chinapassport_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_chinapassport_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_chinapassport_resp = await self.recognize_chinapassport_with_options_async(recognize_chinapassport_req, runtime)
-        return recognize_chinapassport_resp
-
     def recognize_driver_license_with_options(
         self,
         request: ocr_20191230_models.RecognizeDriverLicenseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeDriverLicenseResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1695,15 +1059,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1726,36 +1090,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_driver_license_req = ocr_20191230_models.RecognizeDriverLicenseRequest()
         OpenApiUtilClient.convert(request, recognize_driver_license_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_driver_license_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_driver_license_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_driver_license_resp = self.recognize_driver_license_with_options(recognize_driver_license_req, runtime)
         return recognize_driver_license_resp
 
     async def recognize_driver_license_advance_async(
         self,
         request: ocr_20191230_models.RecognizeDriverLicenseAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -1766,15 +1130,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1797,36 +1161,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_driver_license_req = ocr_20191230_models.RecognizeDriverLicenseRequest()
         OpenApiUtilClient.convert(request, recognize_driver_license_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_driver_license_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_driver_license_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_driver_license_resp = await self.recognize_driver_license_with_options_async(recognize_driver_license_req, runtime)
         return recognize_driver_license_resp
 
     def recognize_driving_license_with_options(
         self,
         request: ocr_20191230_models.RecognizeDrivingLicenseRequest,
         runtime: util_models.RuntimeOptions,
@@ -1911,15 +1275,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -1942,36 +1306,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_driving_license_req = ocr_20191230_models.RecognizeDrivingLicenseRequest()
         OpenApiUtilClient.convert(request, recognize_driving_license_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_driving_license_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_driving_license_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_driving_license_resp = self.recognize_driving_license_with_options(recognize_driving_license_req, runtime)
         return recognize_driving_license_resp
 
     async def recognize_driving_license_advance_async(
         self,
         request: ocr_20191230_models.RecognizeDrivingLicenseAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -1982,15 +1346,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -2013,36 +1377,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_driving_license_req = ocr_20191230_models.RecognizeDrivingLicenseRequest()
         OpenApiUtilClient.convert(request, recognize_driving_license_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_driving_license_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_driving_license_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_driving_license_resp = await self.recognize_driving_license_with_options_async(recognize_driving_license_req, runtime)
         return recognize_driving_license_resp
 
     def recognize_identity_card_with_options(
         self,
         request: ocr_20191230_models.RecognizeIdentityCardRequest,
         runtime: util_models.RuntimeOptions,
@@ -2127,15 +1491,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -2158,36 +1522,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_identity_card_req = ocr_20191230_models.RecognizeIdentityCardRequest()
         OpenApiUtilClient.convert(request, recognize_identity_card_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_identity_card_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_identity_card_resp = self.recognize_identity_card_with_options(recognize_identity_card_req, runtime)
         return recognize_identity_card_resp
 
     async def recognize_identity_card_advance_async(
         self,
         request: ocr_20191230_models.RecognizeIdentityCardAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -2198,15 +1562,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -2229,251 +1593,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_identity_card_req = ocr_20191230_models.RecognizeIdentityCardRequest()
         OpenApiUtilClient.convert(request, recognize_identity_card_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_identity_card_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_identity_card_resp = await self.recognize_identity_card_with_options_async(recognize_identity_card_req, runtime)
         return recognize_identity_card_resp
 
-    def recognize_indonesia_identity_card_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeIndonesiaIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeIndonesiaIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_indonesia_identity_card_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeIndonesiaIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeIndonesiaIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_indonesia_identity_card(
-        self,
-        request: ocr_20191230_models.RecognizeIndonesiaIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_indonesia_identity_card_with_options(request, runtime)
-
-    async def recognize_indonesia_identity_card_async(
-        self,
-        request: ocr_20191230_models.RecognizeIndonesiaIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_indonesia_identity_card_with_options_async(request, runtime)
-
-    def recognize_indonesia_identity_card_advance(
-        self,
-        request: ocr_20191230_models.RecognizeIndonesiaIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_indonesia_identity_card_req = ocr_20191230_models.RecognizeIndonesiaIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_indonesia_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_indonesia_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_indonesia_identity_card_resp = self.recognize_indonesia_identity_card_with_options(recognize_indonesia_identity_card_req, runtime)
-        return recognize_indonesia_identity_card_resp
-
-    async def recognize_indonesia_identity_card_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeIndonesiaIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeIndonesiaIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_indonesia_identity_card_req = ocr_20191230_models.RecognizeIndonesiaIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_indonesia_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_indonesia_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_indonesia_identity_card_resp = await self.recognize_indonesia_identity_card_with_options_async(recognize_indonesia_identity_card_req, runtime)
-        return recognize_indonesia_identity_card_resp
-
     def recognize_license_plate_with_options(
         self,
         request: ocr_20191230_models.RecognizeLicensePlateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeLicensePlateResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -2551,15 +1703,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -2582,36 +1734,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_license_plate_req = ocr_20191230_models.RecognizeLicensePlateRequest()
         OpenApiUtilClient.convert(request, recognize_license_plate_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_license_plate_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_license_plate_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_license_plate_resp = self.recognize_license_plate_with_options(recognize_license_plate_req, runtime)
         return recognize_license_plate_resp
 
     async def recognize_license_plate_advance_async(
         self,
         request: ocr_20191230_models.RecognizeLicensePlateAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -2622,15 +1774,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -2653,463 +1805,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_license_plate_req = ocr_20191230_models.RecognizeLicensePlateRequest()
         OpenApiUtilClient.convert(request, recognize_license_plate_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_license_plate_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_license_plate_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_license_plate_resp = await self.recognize_license_plate_with_options_async(recognize_license_plate_req, runtime)
         return recognize_license_plate_resp
 
-    def recognize_malaysia_identity_card_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeMalaysiaIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeMalaysiaIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_malaysia_identity_card_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeMalaysiaIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeMalaysiaIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_malaysia_identity_card(
-        self,
-        request: ocr_20191230_models.RecognizeMalaysiaIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_malaysia_identity_card_with_options(request, runtime)
-
-    async def recognize_malaysia_identity_card_async(
-        self,
-        request: ocr_20191230_models.RecognizeMalaysiaIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_malaysia_identity_card_with_options_async(request, runtime)
-
-    def recognize_malaysia_identity_card_advance(
-        self,
-        request: ocr_20191230_models.RecognizeMalaysiaIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_malaysia_identity_card_req = ocr_20191230_models.RecognizeMalaysiaIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_malaysia_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_malaysia_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_malaysia_identity_card_resp = self.recognize_malaysia_identity_card_with_options(recognize_malaysia_identity_card_req, runtime)
-        return recognize_malaysia_identity_card_resp
-
-    async def recognize_malaysia_identity_card_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeMalaysiaIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeMalaysiaIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_malaysia_identity_card_req = ocr_20191230_models.RecognizeMalaysiaIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_malaysia_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_malaysia_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_malaysia_identity_card_resp = await self.recognize_malaysia_identity_card_with_options_async(recognize_malaysia_identity_card_req, runtime)
-        return recognize_malaysia_identity_card_resp
-
-    def recognize_passport_mrzwith_options(
-        self,
-        request: ocr_20191230_models.RecognizePassportMRZRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePassportMRZResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizePassportMRZ',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizePassportMRZResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_passport_mrzwith_options_async(
-        self,
-        request: ocr_20191230_models.RecognizePassportMRZRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePassportMRZResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizePassportMRZ',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizePassportMRZResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_passport_mrz(
-        self,
-        request: ocr_20191230_models.RecognizePassportMRZRequest,
-    ) -> ocr_20191230_models.RecognizePassportMRZResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_passport_mrzwith_options(request, runtime)
-
-    async def recognize_passport_mrz_async(
-        self,
-        request: ocr_20191230_models.RecognizePassportMRZRequest,
-    ) -> ocr_20191230_models.RecognizePassportMRZResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_passport_mrzwith_options_async(request, runtime)
-
-    def recognize_passport_mrzadvance(
-        self,
-        request: ocr_20191230_models.RecognizePassportMRZAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePassportMRZResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_passport_mrzreq = ocr_20191230_models.RecognizePassportMRZRequest()
-        OpenApiUtilClient.convert(request, recognize_passport_mrzreq)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_passport_mrzreq.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_passport_mrzresp = self.recognize_passport_mrzwith_options(recognize_passport_mrzreq, runtime)
-        return recognize_passport_mrzresp
-
-    async def recognize_passport_mrzadvance_async(
-        self,
-        request: ocr_20191230_models.RecognizePassportMRZAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePassportMRZResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_passport_mrzreq = ocr_20191230_models.RecognizePassportMRZRequest()
-        OpenApiUtilClient.convert(request, recognize_passport_mrzreq)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_passport_mrzreq.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_passport_mrzresp = await self.recognize_passport_mrzwith_options_async(recognize_passport_mrzreq, runtime)
-        return recognize_passport_mrzresp
-
     def recognize_pdf_with_options(
         self,
         request: ocr_20191230_models.RecognizePdfRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizePdfResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -3187,15 +1915,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -3218,36 +1946,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_pdf_req = ocr_20191230_models.RecognizePdfRequest()
         OpenApiUtilClient.convert(request, recognize_pdf_req)
         if not UtilClient.is_unset(request.file_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.file_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_pdf_req.file_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_pdf_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_pdf_resp = self.recognize_pdf_with_options(recognize_pdf_req, runtime)
         return recognize_pdf_resp
 
     async def recognize_pdf_advance_async(
         self,
         request: ocr_20191230_models.RecognizePdfAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -3258,15 +1986,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -3289,125 +2017,125 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_pdf_req = ocr_20191230_models.RecognizePdfRequest()
         OpenApiUtilClient.convert(request, recognize_pdf_req)
         if not UtilClient.is_unset(request.file_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.file_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_pdf_req.file_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_pdf_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_pdf_resp = await self.recognize_pdf_with_options_async(recognize_pdf_req, runtime)
         return recognize_pdf_resp
 
-    def recognize_poi_name_with_options(
+    def recognize_qr_code_with_options(
         self,
-        request: ocr_20191230_models.RecognizePoiNameRequest,
+        request: ocr_20191230_models.RecognizeQrCodeRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePoiNameResponse:
+    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
+        if not UtilClient.is_unset(request.tasks):
+            body['Tasks'] = request.tasks
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='RecognizePoiName',
+            action='RecognizeQrCode',
             version='2019-12-30',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            ocr_20191230_models.RecognizePoiNameResponse(),
+            ocr_20191230_models.RecognizeQrCodeResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def recognize_poi_name_with_options_async(
+    async def recognize_qr_code_with_options_async(
         self,
-        request: ocr_20191230_models.RecognizePoiNameRequest,
+        request: ocr_20191230_models.RecognizeQrCodeRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePoiNameResponse:
+    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
+        if not UtilClient.is_unset(request.tasks):
+            body['Tasks'] = request.tasks
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='RecognizePoiName',
+            action='RecognizeQrCode',
             version='2019-12-30',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            ocr_20191230_models.RecognizePoiNameResponse(),
+            ocr_20191230_models.RecognizeQrCodeResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def recognize_poi_name(
+    def recognize_qr_code(
         self,
-        request: ocr_20191230_models.RecognizePoiNameRequest,
-    ) -> ocr_20191230_models.RecognizePoiNameResponse:
+        request: ocr_20191230_models.RecognizeQrCodeRequest,
+    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
         runtime = util_models.RuntimeOptions()
-        return self.recognize_poi_name_with_options(request, runtime)
+        return self.recognize_qr_code_with_options(request, runtime)
 
-    async def recognize_poi_name_async(
+    async def recognize_qr_code_async(
         self,
-        request: ocr_20191230_models.RecognizePoiNameRequest,
-    ) -> ocr_20191230_models.RecognizePoiNameResponse:
+        request: ocr_20191230_models.RecognizeQrCodeRequest,
+    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.recognize_poi_name_with_options_async(request, runtime)
+        return await self.recognize_qr_code_with_options_async(request, runtime)
 
-    def recognize_poi_name_advance(
+    def recognize_qr_code_advance(
         self,
-        request: ocr_20191230_models.RecognizePoiNameAdvanceRequest,
+        request: ocr_20191230_models.RecognizeQrCodeAdvanceRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePoiNameResponse:
+    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
         # Step 0: init client
         access_key_id = self._credential.get_access_key_id()
         access_key_secret = self._credential.get_access_key_secret()
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -3426,59 +2154,64 @@
         )
         oss_client = None
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_poi_name_req = ocr_20191230_models.RecognizePoiNameRequest()
-        OpenApiUtilClient.convert(request, recognize_poi_name_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_poi_name_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_poi_name_resp = self.recognize_poi_name_with_options(recognize_poi_name_req, runtime)
-        return recognize_poi_name_resp
+        recognize_qr_code_req = ocr_20191230_models.RecognizeQrCodeRequest()
+        OpenApiUtilClient.convert(request, recognize_qr_code_req)
+        if not UtilClient.is_unset(request.tasks):
+            i_0 = 0
+            for item_0 in request.tasks:
+                if not UtilClient.is_unset(item_0.image_urlobject):
+                    auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
+                    oss_config.access_key_id = auth_response.body.access_key_id
+                    oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
+                    oss_client = OSSClient(oss_config)
+                    file_obj = file_form_models.FileField(
+                        filename=auth_response.body.object_key,
+                        content=item_0.image_urlobject,
+                        content_type=''
+                    )
+                    oss_header = oss_models.PostObjectRequestHeader(
+                        access_key_id=auth_response.body.access_key_id,
+                        policy=auth_response.body.encoded_policy,
+                        signature=auth_response.body.signature,
+                        key=auth_response.body.object_key,
+                        file=file_obj,
+                        success_action_status='201'
+                    )
+                    upload_request = oss_models.PostObjectRequest(
+                        bucket_name=auth_response.body.bucket,
+                        header=oss_header
+                    )
+                    oss_client.post_object(upload_request, oss_runtime)
+                    tmp = recognize_qr_code_req.tasks[i_0]
+                    tmp.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
+                    i_0 = NumberClient.ltoi(NumberClient.add(NumberClient.itol(i_0), NumberClient.itol(1)))
+        recognize_qr_code_resp = self.recognize_qr_code_with_options(recognize_qr_code_req, runtime)
+        return recognize_qr_code_resp
 
-    async def recognize_poi_name_advance_async(
+    async def recognize_qr_code_advance_async(
         self,
-        request: ocr_20191230_models.RecognizePoiNameAdvanceRequest,
+        request: ocr_20191230_models.RecognizeQrCodeAdvanceRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizePoiNameResponse:
+    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
         # Step 0: init client
         access_key_id = await self._credential.get_access_key_id_async()
         access_key_secret = await self._credential.get_access_key_secret_async()
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -3497,112 +2230,47 @@
         )
         oss_client = None
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_poi_name_req = ocr_20191230_models.RecognizePoiNameRequest()
-        OpenApiUtilClient.convert(request, recognize_poi_name_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_poi_name_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_poi_name_resp = await self.recognize_poi_name_with_options_async(recognize_poi_name_req, runtime)
-        return recognize_poi_name_resp
-
-    def recognize_qr_code_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeQrCodeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
-        UtilClient.validate_model(request)
-        body = {}
+        recognize_qr_code_req = ocr_20191230_models.RecognizeQrCodeRequest()
+        OpenApiUtilClient.convert(request, recognize_qr_code_req)
         if not UtilClient.is_unset(request.tasks):
-            body['Tasks'] = request.tasks
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeQrCode',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeQrCodeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_qr_code_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeQrCodeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.tasks):
-            body['Tasks'] = request.tasks
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeQrCode',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeQrCodeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_qr_code(
-        self,
-        request: ocr_20191230_models.RecognizeQrCodeRequest,
-    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_qr_code_with_options(request, runtime)
-
-    async def recognize_qr_code_async(
-        self,
-        request: ocr_20191230_models.RecognizeQrCodeRequest,
-    ) -> ocr_20191230_models.RecognizeQrCodeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_qr_code_with_options_async(request, runtime)
+            i_0 = 0
+            for item_0 in request.tasks:
+                if not UtilClient.is_unset(item_0.image_urlobject):
+                    auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
+                    oss_config.access_key_id = auth_response.body.access_key_id
+                    oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
+                    oss_client = OSSClient(oss_config)
+                    file_obj = file_form_models.FileField(
+                        filename=auth_response.body.object_key,
+                        content=item_0.image_urlobject,
+                        content_type=''
+                    )
+                    oss_header = oss_models.PostObjectRequestHeader(
+                        access_key_id=auth_response.body.access_key_id,
+                        policy=auth_response.body.encoded_policy,
+                        signature=auth_response.body.signature,
+                        key=auth_response.body.object_key,
+                        file=file_obj,
+                        success_action_status='201'
+                    )
+                    upload_request = oss_models.PostObjectRequest(
+                        bucket_name=auth_response.body.bucket,
+                        header=oss_header
+                    )
+                    await oss_client.post_object_async(upload_request, oss_runtime)
+                    tmp = recognize_qr_code_req.tasks[i_0]
+                    tmp.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
+                    i_0 = NumberClient.ltoi(NumberClient.add(NumberClient.itol(i_0), NumberClient.itol(1)))
+        recognize_qr_code_resp = await self.recognize_qr_code_with_options_async(recognize_qr_code_req, runtime)
+        return recognize_qr_code_resp
 
     def recognize_quota_invoice_with_options(
         self,
         request: ocr_20191230_models.RecognizeQuotaInvoiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeQuotaInvoiceResponse:
         UtilClient.validate_model(request)
@@ -3681,15 +2349,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -3712,36 +2380,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_quota_invoice_req = ocr_20191230_models.RecognizeQuotaInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_quota_invoice_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_quota_invoice_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_quota_invoice_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_quota_invoice_resp = self.recognize_quota_invoice_with_options(recognize_quota_invoice_req, runtime)
         return recognize_quota_invoice_resp
 
     async def recognize_quota_invoice_advance_async(
         self,
         request: ocr_20191230_models.RecognizeQuotaInvoiceAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -3752,15 +2420,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -3783,251 +2451,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_quota_invoice_req = ocr_20191230_models.RecognizeQuotaInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_quota_invoice_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_quota_invoice_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_quota_invoice_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_quota_invoice_resp = await self.recognize_quota_invoice_with_options_async(recognize_quota_invoice_req, runtime)
         return recognize_quota_invoice_resp
 
-    def recognize_russia_identity_card_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeRussiaIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeRussiaIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeRussiaIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeRussiaIdentityCardResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_russia_identity_card_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeRussiaIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeRussiaIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeRussiaIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeRussiaIdentityCardResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_russia_identity_card(
-        self,
-        request: ocr_20191230_models.RecognizeRussiaIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeRussiaIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_russia_identity_card_with_options(request, runtime)
-
-    async def recognize_russia_identity_card_async(
-        self,
-        request: ocr_20191230_models.RecognizeRussiaIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeRussiaIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_russia_identity_card_with_options_async(request, runtime)
-
-    def recognize_russia_identity_card_advance(
-        self,
-        request: ocr_20191230_models.RecognizeRussiaIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeRussiaIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_russia_identity_card_req = ocr_20191230_models.RecognizeRussiaIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_russia_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_russia_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_russia_identity_card_resp = self.recognize_russia_identity_card_with_options(recognize_russia_identity_card_req, runtime)
-        return recognize_russia_identity_card_resp
-
-    async def recognize_russia_identity_card_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeRussiaIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeRussiaIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_russia_identity_card_req = ocr_20191230_models.RecognizeRussiaIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_russia_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_russia_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_russia_identity_card_resp = await self.recognize_russia_identity_card_with_options_async(recognize_russia_identity_card_req, runtime)
-        return recognize_russia_identity_card_resp
-
     def recognize_stamp_with_options(
         self,
         request: ocr_20191230_models.RecognizeStampRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeStampResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -4105,15 +2561,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -4136,36 +2592,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_stamp_req = ocr_20191230_models.RecognizeStampRequest()
         OpenApiUtilClient.convert(request, recognize_stamp_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_stamp_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_stamp_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_stamp_resp = self.recognize_stamp_with_options(recognize_stamp_req, runtime)
         return recognize_stamp_resp
 
     async def recognize_stamp_advance_async(
         self,
         request: ocr_20191230_models.RecognizeStampAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -4176,15 +2632,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -4207,36 +2663,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_stamp_req = ocr_20191230_models.RecognizeStampRequest()
         OpenApiUtilClient.convert(request, recognize_stamp_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_stamp_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_stamp_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_stamp_resp = await self.recognize_stamp_with_options_async(recognize_stamp_req, runtime)
         return recognize_stamp_resp
 
     def recognize_table_with_options(
         self,
         request: ocr_20191230_models.RecognizeTableRequest,
         runtime: util_models.RuntimeOptions,
@@ -4337,15 +2793,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -4368,36 +2824,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_table_req = ocr_20191230_models.RecognizeTableRequest()
         OpenApiUtilClient.convert(request, recognize_table_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_table_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_table_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_table_resp = self.recognize_table_with_options(recognize_table_req, runtime)
         return recognize_table_resp
 
     async def recognize_table_advance_async(
         self,
         request: ocr_20191230_models.RecognizeTableAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -4408,15 +2864,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -4439,251 +2895,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_table_req = ocr_20191230_models.RecognizeTableRequest()
         OpenApiUtilClient.convert(request, recognize_table_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_table_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_table_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_table_resp = await self.recognize_table_with_options_async(recognize_table_req, runtime)
         return recognize_table_resp
 
-    def recognize_takeout_order_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeTakeoutOrderRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTakeoutOrderResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeTakeoutOrder',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeTakeoutOrderResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_takeout_order_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeTakeoutOrderRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTakeoutOrderResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeTakeoutOrder',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeTakeoutOrderResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_takeout_order(
-        self,
-        request: ocr_20191230_models.RecognizeTakeoutOrderRequest,
-    ) -> ocr_20191230_models.RecognizeTakeoutOrderResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_takeout_order_with_options(request, runtime)
-
-    async def recognize_takeout_order_async(
-        self,
-        request: ocr_20191230_models.RecognizeTakeoutOrderRequest,
-    ) -> ocr_20191230_models.RecognizeTakeoutOrderResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_takeout_order_with_options_async(request, runtime)
-
-    def recognize_takeout_order_advance(
-        self,
-        request: ocr_20191230_models.RecognizeTakeoutOrderAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTakeoutOrderResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_takeout_order_req = ocr_20191230_models.RecognizeTakeoutOrderRequest()
-        OpenApiUtilClient.convert(request, recognize_takeout_order_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_takeout_order_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_takeout_order_resp = self.recognize_takeout_order_with_options(recognize_takeout_order_req, runtime)
-        return recognize_takeout_order_resp
-
-    async def recognize_takeout_order_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeTakeoutOrderAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTakeoutOrderResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_takeout_order_req = ocr_20191230_models.RecognizeTakeoutOrderRequest()
-        OpenApiUtilClient.convert(request, recognize_takeout_order_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_takeout_order_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_takeout_order_resp = await self.recognize_takeout_order_with_options_async(recognize_takeout_order_req, runtime)
-        return recognize_takeout_order_resp
-
     def recognize_taxi_invoice_with_options(
         self,
         request: ocr_20191230_models.RecognizeTaxiInvoiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeTaxiInvoiceResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -4761,15 +3005,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -4792,36 +3036,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_taxi_invoice_req = ocr_20191230_models.RecognizeTaxiInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_taxi_invoice_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_taxi_invoice_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_taxi_invoice_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_taxi_invoice_resp = self.recognize_taxi_invoice_with_options(recognize_taxi_invoice_req, runtime)
         return recognize_taxi_invoice_resp
 
     async def recognize_taxi_invoice_advance_async(
         self,
         request: ocr_20191230_models.RecognizeTaxiInvoiceAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -4832,15 +3076,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -4863,36 +3107,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_taxi_invoice_req = ocr_20191230_models.RecognizeTaxiInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_taxi_invoice_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_taxi_invoice_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_taxi_invoice_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_taxi_invoice_resp = await self.recognize_taxi_invoice_with_options_async(recognize_taxi_invoice_req, runtime)
         return recognize_taxi_invoice_resp
 
     def recognize_ticket_invoice_with_options(
         self,
         request: ocr_20191230_models.RecognizeTicketInvoiceRequest,
         runtime: util_models.RuntimeOptions,
@@ -4973,15 +3217,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -5004,36 +3248,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_ticket_invoice_req = ocr_20191230_models.RecognizeTicketInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_ticket_invoice_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_ticket_invoice_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_ticket_invoice_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_ticket_invoice_resp = self.recognize_ticket_invoice_with_options(recognize_ticket_invoice_req, runtime)
         return recognize_ticket_invoice_resp
 
     async def recognize_ticket_invoice_advance_async(
         self,
         request: ocr_20191230_models.RecognizeTicketInvoiceAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -5044,15 +3288,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -5075,36 +3319,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_ticket_invoice_req = ocr_20191230_models.RecognizeTicketInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_ticket_invoice_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_ticket_invoice_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_ticket_invoice_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_ticket_invoice_resp = await self.recognize_ticket_invoice_with_options_async(recognize_ticket_invoice_req, runtime)
         return recognize_ticket_invoice_resp
 
     def recognize_train_ticket_with_options(
         self,
         request: ocr_20191230_models.RecognizeTrainTicketRequest,
         runtime: util_models.RuntimeOptions,
@@ -5185,15 +3429,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -5216,36 +3460,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_train_ticket_req = ocr_20191230_models.RecognizeTrainTicketRequest()
         OpenApiUtilClient.convert(request, recognize_train_ticket_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_train_ticket_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_train_ticket_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_train_ticket_resp = self.recognize_train_ticket_with_options(recognize_train_ticket_req, runtime)
         return recognize_train_ticket_resp
 
     async def recognize_train_ticket_advance_async(
         self,
         request: ocr_20191230_models.RecognizeTrainTicketAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -5256,15 +3500,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -5287,463 +3531,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_train_ticket_req = ocr_20191230_models.RecognizeTrainTicketRequest()
         OpenApiUtilClient.convert(request, recognize_train_ticket_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_train_ticket_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_train_ticket_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_train_ticket_resp = await self.recognize_train_ticket_with_options_async(recognize_train_ticket_req, runtime)
         return recognize_train_ticket_resp
 
-    def recognize_turkey_identity_card_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeTurkeyIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTurkeyIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeTurkeyIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeTurkeyIdentityCardResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_turkey_identity_card_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeTurkeyIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTurkeyIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeTurkeyIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeTurkeyIdentityCardResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_turkey_identity_card(
-        self,
-        request: ocr_20191230_models.RecognizeTurkeyIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeTurkeyIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_turkey_identity_card_with_options(request, runtime)
-
-    async def recognize_turkey_identity_card_async(
-        self,
-        request: ocr_20191230_models.RecognizeTurkeyIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeTurkeyIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_turkey_identity_card_with_options_async(request, runtime)
-
-    def recognize_turkey_identity_card_advance(
-        self,
-        request: ocr_20191230_models.RecognizeTurkeyIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTurkeyIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_turkey_identity_card_req = ocr_20191230_models.RecognizeTurkeyIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_turkey_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_turkey_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_turkey_identity_card_resp = self.recognize_turkey_identity_card_with_options(recognize_turkey_identity_card_req, runtime)
-        return recognize_turkey_identity_card_resp
-
-    async def recognize_turkey_identity_card_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeTurkeyIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeTurkeyIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_turkey_identity_card_req = ocr_20191230_models.RecognizeTurkeyIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_turkey_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_turkey_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_turkey_identity_card_resp = await self.recognize_turkey_identity_card_with_options_async(recognize_turkey_identity_card_req, runtime)
-        return recognize_turkey_identity_card_resp
-
-    def recognize_ukraine_identity_card_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeUkraineIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeUkraineIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeUkraineIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeUkraineIdentityCardResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_ukraine_identity_card_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeUkraineIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeUkraineIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeUkraineIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeUkraineIdentityCardResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_ukraine_identity_card(
-        self,
-        request: ocr_20191230_models.RecognizeUkraineIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeUkraineIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_ukraine_identity_card_with_options(request, runtime)
-
-    async def recognize_ukraine_identity_card_async(
-        self,
-        request: ocr_20191230_models.RecognizeUkraineIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeUkraineIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_ukraine_identity_card_with_options_async(request, runtime)
-
-    def recognize_ukraine_identity_card_advance(
-        self,
-        request: ocr_20191230_models.RecognizeUkraineIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeUkraineIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_ukraine_identity_card_req = ocr_20191230_models.RecognizeUkraineIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_ukraine_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_ukraine_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_ukraine_identity_card_resp = self.recognize_ukraine_identity_card_with_options(recognize_ukraine_identity_card_req, runtime)
-        return recognize_ukraine_identity_card_resp
-
-    async def recognize_ukraine_identity_card_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeUkraineIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeUkraineIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_ukraine_identity_card_req = ocr_20191230_models.RecognizeUkraineIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_ukraine_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_ukraine_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_ukraine_identity_card_resp = await self.recognize_ukraine_identity_card_with_options_async(recognize_ukraine_identity_card_req, runtime)
-        return recognize_ukraine_identity_card_resp
-
     def recognize_vatinvoice_with_options(
         self,
         request: ocr_20191230_models.RecognizeVATInvoiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeVATInvoiceResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -5825,15 +3645,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -5856,36 +3676,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_vatinvoice_req = ocr_20191230_models.RecognizeVATInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_vatinvoice_req)
         if not UtilClient.is_unset(request.file_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.file_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_vatinvoice_req.file_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_vatinvoice_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_vatinvoice_resp = self.recognize_vatinvoice_with_options(recognize_vatinvoice_req, runtime)
         return recognize_vatinvoice_resp
 
     async def recognize_vatinvoice_advance_async(
         self,
         request: ocr_20191230_models.RecognizeVATInvoiceAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -5896,15 +3716,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -5927,36 +3747,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_vatinvoice_req = ocr_20191230_models.RecognizeVATInvoiceRequest()
         OpenApiUtilClient.convert(request, recognize_vatinvoice_req)
         if not UtilClient.is_unset(request.file_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.file_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_vatinvoice_req.file_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_vatinvoice_req.file_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_vatinvoice_resp = await self.recognize_vatinvoice_with_options_async(recognize_vatinvoice_req, runtime)
         return recognize_vatinvoice_resp
 
     def recognize_vincode_with_options(
         self,
         request: ocr_20191230_models.RecognizeVINCodeRequest,
         runtime: util_models.RuntimeOptions,
@@ -6037,15 +3857,15 @@
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -6068,36 +3888,36 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_vincode_req = ocr_20191230_models.RecognizeVINCodeRequest()
         OpenApiUtilClient.convert(request, recognize_vincode_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            recognize_vincode_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_vincode_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_vincode_resp = self.recognize_vincode_with_options(recognize_vincode_req, runtime)
         return recognize_vincode_resp
 
     async def recognize_vincode_advance_async(
         self,
         request: ocr_20191230_models.RecognizeVINCodeAdvanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -6108,15 +3928,15 @@
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -6139,479 +3959,39 @@
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         recognize_vincode_req = ocr_20191230_models.RecognizeVINCodeRequest()
         OpenApiUtilClient.convert(request, recognize_vincode_req)
         if not UtilClient.is_unset(request.image_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
+                filename=auth_response.body.object_key,
                 content=request.image_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_vincode_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
+            recognize_vincode_req.image_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
         recognize_vincode_resp = await self.recognize_vincode_with_options_async(recognize_vincode_req, runtime)
         return recognize_vincode_resp
 
-    def recognize_verificationcode_with_options(
-        self,
-        request: ocr_20191230_models.RecognizeVerificationcodeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVerificationcodeResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeVerificationcode',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeVerificationcodeResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_verificationcode_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeVerificationcodeRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVerificationcodeResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageURL'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeVerificationcode',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeVerificationcodeResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_verificationcode(
-        self,
-        request: ocr_20191230_models.RecognizeVerificationcodeRequest,
-    ) -> ocr_20191230_models.RecognizeVerificationcodeResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_verificationcode_with_options(request, runtime)
-
-    async def recognize_verificationcode_async(
-        self,
-        request: ocr_20191230_models.RecognizeVerificationcodeRequest,
-    ) -> ocr_20191230_models.RecognizeVerificationcodeResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_verificationcode_with_options_async(request, runtime)
-
-    def recognize_verificationcode_advance(
-        self,
-        request: ocr_20191230_models.RecognizeVerificationcodeAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVerificationcodeResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_verificationcode_req = ocr_20191230_models.RecognizeVerificationcodeRequest()
-        OpenApiUtilClient.convert(request, recognize_verificationcode_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_verificationcode_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_verificationcode_resp = self.recognize_verificationcode_with_options(recognize_verificationcode_req, runtime)
-        return recognize_verificationcode_resp
-
-    async def recognize_verificationcode_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeVerificationcodeAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVerificationcodeResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_verificationcode_req = ocr_20191230_models.RecognizeVerificationcodeRequest()
-        OpenApiUtilClient.convert(request, recognize_verificationcode_req)
-        if not UtilClient.is_unset(request.image_urlobject):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_urlobject,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_verificationcode_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_verificationcode_resp = await self.recognize_verificationcode_with_options_async(recognize_verificationcode_req, runtime)
-        return recognize_verificationcode_resp
-
-    def recognize_video_cast_crew_list_with_options(
-        self,
-        tmp_req: ocr_20191230_models.RecognizeVideoCastCrewListRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVideoCastCrewListResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ocr_20191230_models.RecognizeVideoCastCrewListShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.params):
-            request.params_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.params, 'Params', 'json')
-        body = {}
-        if not UtilClient.is_unset(request.params_shrink):
-            body['Params'] = request.params_shrink
-        if not UtilClient.is_unset(request.register_url):
-            body['RegisterUrl'] = request.register_url
-        if not UtilClient.is_unset(request.video_url):
-            body['VideoUrl'] = request.video_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeVideoCastCrewList',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeVideoCastCrewListResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_video_cast_crew_list_with_options_async(
-        self,
-        tmp_req: ocr_20191230_models.RecognizeVideoCastCrewListRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVideoCastCrewListResponse:
-        UtilClient.validate_model(tmp_req)
-        request = ocr_20191230_models.RecognizeVideoCastCrewListShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.params):
-            request.params_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.params, 'Params', 'json')
-        body = {}
-        if not UtilClient.is_unset(request.params_shrink):
-            body['Params'] = request.params_shrink
-        if not UtilClient.is_unset(request.register_url):
-            body['RegisterUrl'] = request.register_url
-        if not UtilClient.is_unset(request.video_url):
-            body['VideoUrl'] = request.video_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeVideoCastCrewList',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeVideoCastCrewListResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_video_cast_crew_list(
-        self,
-        request: ocr_20191230_models.RecognizeVideoCastCrewListRequest,
-    ) -> ocr_20191230_models.RecognizeVideoCastCrewListResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_video_cast_crew_list_with_options(request, runtime)
-
-    async def recognize_video_cast_crew_list_async(
-        self,
-        request: ocr_20191230_models.RecognizeVideoCastCrewListRequest,
-    ) -> ocr_20191230_models.RecognizeVideoCastCrewListResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_video_cast_crew_list_with_options_async(request, runtime)
-
-    def recognize_video_cast_crew_list_advance(
-        self,
-        request: ocr_20191230_models.RecognizeVideoCastCrewListAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVideoCastCrewListResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_video_cast_crew_list_req = ocr_20191230_models.RecognizeVideoCastCrewListRequest()
-        OpenApiUtilClient.convert(request, recognize_video_cast_crew_list_req)
-        if not UtilClient.is_unset(request.video_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.video_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_video_cast_crew_list_req.video_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_video_cast_crew_list_resp = self.recognize_video_cast_crew_list_with_options(recognize_video_cast_crew_list_req, runtime)
-        return recognize_video_cast_crew_list_resp
-
-    async def recognize_video_cast_crew_list_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeVideoCastCrewListAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVideoCastCrewListResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_video_cast_crew_list_req = ocr_20191230_models.RecognizeVideoCastCrewListRequest()
-        OpenApiUtilClient.convert(request, recognize_video_cast_crew_list_req)
-        if not UtilClient.is_unset(request.video_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.video_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_video_cast_crew_list_req.video_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_video_cast_crew_list_resp = await self.recognize_video_cast_crew_list_with_options_async(recognize_video_cast_crew_list_req, runtime)
-        return recognize_video_cast_crew_list_resp
-
     def recognize_video_character_with_options(
         self,
         request: ocr_20191230_models.RecognizeVideoCharacterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_20191230_models.RecognizeVideoCharacterResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -6674,320 +4054,30 @@
     async def recognize_video_character_async(
         self,
         request: ocr_20191230_models.RecognizeVideoCharacterRequest,
     ) -> ocr_20191230_models.RecognizeVideoCharacterResponse:
         runtime = util_models.RuntimeOptions()
         return await self.recognize_video_character_with_options_async(request, runtime)
 
-    def recognize_vietnam_identity_card_with_options(
+    def recognize_video_character_advance(
         self,
-        request: ocr_20191230_models.RecognizeVietnamIdentityCardRequest,
+        request: ocr_20191230_models.RecognizeVideoCharacterAdvanceRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVietnamIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeVietnamIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeVietnamIdentityCardResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def recognize_vietnam_identity_card_with_options_async(
-        self,
-        request: ocr_20191230_models.RecognizeVietnamIdentityCardRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVietnamIdentityCardResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.image_url):
-            body['ImageUrl'] = request.image_url
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='RecognizeVietnamIdentityCard',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.RecognizeVietnamIdentityCardResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def recognize_vietnam_identity_card(
-        self,
-        request: ocr_20191230_models.RecognizeVietnamIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeVietnamIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.recognize_vietnam_identity_card_with_options(request, runtime)
-
-    async def recognize_vietnam_identity_card_async(
-        self,
-        request: ocr_20191230_models.RecognizeVietnamIdentityCardRequest,
-    ) -> ocr_20191230_models.RecognizeVietnamIdentityCardResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.recognize_vietnam_identity_card_with_options_async(request, runtime)
-
-    def recognize_vietnam_identity_card_advance(
-        self,
-        request: ocr_20191230_models.RecognizeVietnamIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVietnamIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = self._credential.get_access_key_id()
-        access_key_secret = self._credential.get_access_key_secret()
-        security_token = self._credential.get_security_token()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_vietnam_identity_card_req = ocr_20191230_models.RecognizeVietnamIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_vietnam_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            oss_client.post_object(upload_request, oss_runtime)
-            recognize_vietnam_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_vietnam_identity_card_resp = self.recognize_vietnam_identity_card_with_options(recognize_vietnam_identity_card_req, runtime)
-        return recognize_vietnam_identity_card_resp
-
-    async def recognize_vietnam_identity_card_advance_async(
-        self,
-        request: ocr_20191230_models.RecognizeVietnamIdentityCardAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.RecognizeVietnamIdentityCardResponse:
-        # Step 0: init client
-        access_key_id = await self._credential.get_access_key_id_async()
-        access_key_secret = await self._credential.get_access_key_secret_async()
-        security_token = await self._credential.get_security_token_async()
-        credential_type = self._credential.get_type()
-        open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
-            open_platform_endpoint = 'openplatform.aliyuncs.com'
-        if UtilClient.is_unset(credential_type):
-            credential_type = 'access_key'
-        auth_config = rpc_models.Config(
-            access_key_id=access_key_id,
-            access_key_secret=access_key_secret,
-            security_token=security_token,
-            type=credential_type,
-            endpoint=open_platform_endpoint,
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        auth_client = OpenPlatformClient(auth_config)
-        auth_request = open_platform_models.AuthorizeFileUploadRequest(
-            product='ocr',
-            region_id=self._region_id
-        )
-        auth_response = open_platform_models.AuthorizeFileUploadResponse()
-        oss_config = oss_models.Config(
-            access_key_secret=access_key_secret,
-            type='access_key',
-            protocol=self._protocol,
-            region_id=self._region_id
-        )
-        oss_client = None
-        file_obj = file_form_models.FileField()
-        oss_header = oss_models.PostObjectRequestHeader()
-        upload_request = oss_models.PostObjectRequest()
-        oss_runtime = ossutil_models.RuntimeOptions()
-        OpenApiUtilClient.convert(runtime, oss_runtime)
-        recognize_vietnam_identity_card_req = ocr_20191230_models.RecognizeVietnamIdentityCardRequest()
-        OpenApiUtilClient.convert(request, recognize_vietnam_identity_card_req)
-        if not UtilClient.is_unset(request.image_url_object):
-            auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
-            oss_client = OSSClient(oss_config)
-            file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.image_url_object,
-                content_type=''
-            )
-            oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
-                file=file_obj,
-                success_action_status='201'
-            )
-            upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
-                header=oss_header
-            )
-            await oss_client.post_object_async(upload_request, oss_runtime)
-            recognize_vietnam_identity_card_req.image_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        recognize_vietnam_identity_card_resp = await self.recognize_vietnam_identity_card_with_options_async(recognize_vietnam_identity_card_req, runtime)
-        return recognize_vietnam_identity_card_resp
-
-    def trim_document_with_options(
-        self,
-        request: ocr_20191230_models.TrimDocumentRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.TrimDocumentResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.file_type):
-            body['FileType'] = request.file_type
-        if not UtilClient.is_unset(request.file_url):
-            body['FileURL'] = request.file_url
-        if not UtilClient.is_unset(request.output_type):
-            body['OutputType'] = request.output_type
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='TrimDocument',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.TrimDocumentResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def trim_document_with_options_async(
-        self,
-        request: ocr_20191230_models.TrimDocumentRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.TrimDocumentResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.file_type):
-            body['FileType'] = request.file_type
-        if not UtilClient.is_unset(request.file_url):
-            body['FileURL'] = request.file_url
-        if not UtilClient.is_unset(request.output_type):
-            body['OutputType'] = request.output_type
-        req = open_api_models.OpenApiRequest(
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='TrimDocument',
-            version='2019-12-30',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            ocr_20191230_models.TrimDocumentResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def trim_document(
-        self,
-        request: ocr_20191230_models.TrimDocumentRequest,
-    ) -> ocr_20191230_models.TrimDocumentResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.trim_document_with_options(request, runtime)
-
-    async def trim_document_async(
-        self,
-        request: ocr_20191230_models.TrimDocumentRequest,
-    ) -> ocr_20191230_models.TrimDocumentResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.trim_document_with_options_async(request, runtime)
-
-    def trim_document_advance(
-        self,
-        request: ocr_20191230_models.TrimDocumentAdvanceRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.TrimDocumentResponse:
+    ) -> ocr_20191230_models.RecognizeVideoCharacterResponse:
         # Step 0: init client
         access_key_id = self._credential.get_access_key_id()
         access_key_secret = self._credential.get_access_key_secret()
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -7006,59 +4096,59 @@
         )
         oss_client = None
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
-        trim_document_req = ocr_20191230_models.TrimDocumentRequest()
-        OpenApiUtilClient.convert(request, trim_document_req)
-        if not UtilClient.is_unset(request.file_urlobject):
+        recognize_video_character_req = ocr_20191230_models.RecognizeVideoCharacterRequest()
+        OpenApiUtilClient.convert(request, recognize_video_character_req)
+        if not UtilClient.is_unset(request.video_urlobject):
             auth_response = auth_client.authorize_file_upload_with_options(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.file_urlobject,
+                filename=auth_response.body.object_key,
+                content=request.video_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             oss_client.post_object(upload_request, oss_runtime)
-            trim_document_req.file_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        trim_document_resp = self.trim_document_with_options(trim_document_req, runtime)
-        return trim_document_resp
+            recognize_video_character_req.video_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
+        recognize_video_character_resp = self.recognize_video_character_with_options(recognize_video_character_req, runtime)
+        return recognize_video_character_resp
 
-    async def trim_document_advance_async(
+    async def recognize_video_character_advance_async(
         self,
-        request: ocr_20191230_models.TrimDocumentAdvanceRequest,
+        request: ocr_20191230_models.RecognizeVideoCharacterAdvanceRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> ocr_20191230_models.TrimDocumentResponse:
+    ) -> ocr_20191230_models.RecognizeVideoCharacterResponse:
         # Step 0: init client
         access_key_id = await self._credential.get_access_key_id_async()
         access_key_secret = await self._credential.get_access_key_secret_async()
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
         if UtilClient.is_unset(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
-        auth_config = rpc_models.Config(
+        auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
             type=credential_type,
             endpoint=open_platform_endpoint,
             protocol=self._protocol,
             region_id=self._region_id
@@ -7077,35 +4167,35 @@
         )
         oss_client = None
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
-        trim_document_req = ocr_20191230_models.TrimDocumentRequest()
-        OpenApiUtilClient.convert(request, trim_document_req)
-        if not UtilClient.is_unset(request.file_urlobject):
+        recognize_video_character_req = ocr_20191230_models.RecognizeVideoCharacterRequest()
+        OpenApiUtilClient.convert(request, recognize_video_character_req)
+        if not UtilClient.is_unset(request.video_urlobject):
             auth_response = await auth_client.authorize_file_upload_with_options_async(auth_request, runtime)
-            oss_config.access_key_id = auth_response.access_key_id
-            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.endpoint, auth_response.use_accelerate, self._endpoint_type)
+            oss_config.access_key_id = auth_response.body.access_key_id
+            oss_config.endpoint = OpenApiUtilClient.get_endpoint(auth_response.body.endpoint, auth_response.body.use_accelerate, self._endpoint_type)
             oss_client = OSSClient(oss_config)
             file_obj = file_form_models.FileField(
-                filename=auth_response.object_key,
-                content=request.file_urlobject,
+                filename=auth_response.body.object_key,
+                content=request.video_urlobject,
                 content_type=''
             )
             oss_header = oss_models.PostObjectRequestHeader(
-                access_key_id=auth_response.access_key_id,
-                policy=auth_response.encoded_policy,
-                signature=auth_response.signature,
-                key=auth_response.object_key,
+                access_key_id=auth_response.body.access_key_id,
+                policy=auth_response.body.encoded_policy,
+                signature=auth_response.body.signature,
+                key=auth_response.body.object_key,
                 file=file_obj,
                 success_action_status='201'
             )
             upload_request = oss_models.PostObjectRequest(
-                bucket_name=auth_response.bucket,
+                bucket_name=auth_response.body.bucket,
                 header=oss_header
             )
             await oss_client.post_object_async(upload_request, oss_runtime)
-            trim_document_req.file_url = f'http://{auth_response.bucket}.{auth_response.endpoint}/{auth_response.object_key}'
-        trim_document_resp = await self.trim_document_with_options_async(trim_document_req, runtime)
-        return trim_document_resp
+            recognize_video_character_req.video_url = f'http://{auth_response.body.bucket}.{auth_response.body.endpoint}/{auth_response.body.object_key}'
+        recognize_video_character_resp = await self.recognize_video_character_with_options_async(recognize_video_character_req, runtime)
+        return recognize_video_character_resp
```

### Comparing `alibabacloud_ocr20191230-2.0.9/alibabacloud_ocr20191230.egg-info/PKG-INFO` & `alibabacloud_ocr20191230-3.0.0/alibabacloud_ocr20191230.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ocr20191230
-Version: 2.0.9
+Version: 3.0.0
 Summary: Alibaba Cloud OCR (20191230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr20191230-2.0.9/setup.py` & `alibabacloud_ocr20191230-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ocr20191230.
 
-Created on 25/05/2022
+Created on 04/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ocr20191230"
 NAME = "alibabacloud_ocr20191230" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OCR (20191230) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
-    "alibabacloud_tea_rpc>=0.1.0, <1.0.0",
-    "alibabacloud_openplatform20191219>=1.1.1, <2.0.0",
+    "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_darabonba_number>=0.0.4, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

