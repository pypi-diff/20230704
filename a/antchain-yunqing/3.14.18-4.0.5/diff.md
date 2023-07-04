# Comparing `tmp/antchain_yunqing-3.14.18.tar.gz` & `tmp/antchain_yunqing-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_yunqing-3.14.18.tar", last modified: Tue Aug 23 03:06:29 2022, max compression
+gzip compressed data, was "dist/antchain_yunqing-4.0.5.tar", last modified: Tue Jul  4 09:50:02 2023, max compression
```

## Comparing `antchain_yunqing-3.14.18.tar` & `antchain_yunqing-4.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/
--rw-r--r--   0 root         (0) root         (0)      600 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2188 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1002 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_sdk_yunqing/
--rw-r--r--   0 root         (0) root         (0)       23 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/antchain_sdk_yunqing/__init__.py
--rw-r--r--   0 root         (0) root         (0)   157892 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/antchain_sdk_yunqing/client.py
--rw-r--r--   0 root         (0) root         (0)   432506 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/antchain_sdk_yunqing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_yunqing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2188 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_yunqing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_yunqing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_yunqing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_yunqing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/antchain_yunqing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-23 03:06:29.000000 antchain_yunqing-3.14.18/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2508 2022-08-23 03:06:28.000000 antchain_yunqing-3.14.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   197878 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/client.py
+-rw-r--r--   0 root         (0) root         (0)   566684 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/antchain_sdk_yunqing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/antchain_yunqing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 09:50:02.000000 antchain_yunqing-4.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-04 09:50:01.000000 antchain_yunqing-4.0.5/setup.py
```

### Comparing `antchain_yunqing-3.14.18/LICENSE` & `antchain_yunqing-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-3.14.18/PKG-INFO` & `antchain_yunqing-4.0.5/antchain_yunqing.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_yunqing
-Version: 3.14.18
+Name: antchain-yunqing
+Version: 4.0.5
 Summary: Ant Chain YUNQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_yunqing-3.14.18/README-CN.md` & `antchain_yunqing-4.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-3.14.18/README.md` & `antchain_yunqing-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_yunqing-3.14.18/antchain_sdk_yunqing/client.py` & `antchain_yunqing-4.0.5/antchain_sdk_yunqing/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,22 +131,22 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '3.14.18',
+                    'sdk_version': '4.0.5',
                     '_prod_code': 'YUNQING',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
-                    'host': UtilClient.default_string(self._endpoint, 'prodapigw-sofastack.cloud.alipay.com'),
+                    'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
                 tmp = UtilClient.anyify_map_value(RPCUtilClient.query(request))
                 _request.body = UtilClient.to_form_string(tmp)
                 _request.headers['content-type'] = 'application/x-www-form-urlencoded'
                 signed_param = TeaCore.merge(_request.query,
                     RPCUtilClient.query(request))
@@ -198,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,22 +235,22 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '3.14.18',
+                    'sdk_version': '4.0.5',
                     '_prod_code': 'YUNQING',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
-                    'host': UtilClient.default_string(self._endpoint, 'prodapigw-sofastack.cloud.alipay.com'),
+                    'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
                 tmp = UtilClient.anyify_map_value(RPCUtilClient.query(request))
                 _request.body = UtilClient.to_form_string(tmp)
                 _request.headers['content-type'] = 'application/x-www-form-urlencoded'
                 signed_param = TeaCore.merge(_request.query,
                     RPCUtilClient.query(request))
@@ -3247,14 +3247,1030 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             yunqing_models.PagequeryRollbackSnapshotversionResponse(),
             await self.do_request_async('1.0', 'yunyou.yunqing.rollback.snapshotversion.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def enable_prod_autotest(
+        self,
+        request: yunqing_models.EnableProdAutotestRequest,
+    ) -> yunqing_models.EnableProdAutotestResponse:
+        """
+        Description: 产品是否可创建测试单
+        Summary: 产品是否可创建测试单
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.enable_prod_autotest_ex(request, headers, runtime)
+
+    async def enable_prod_autotest_async(
+        self,
+        request: yunqing_models.EnableProdAutotestRequest,
+    ) -> yunqing_models.EnableProdAutotestResponse:
+        """
+        Description: 产品是否可创建测试单
+        Summary: 产品是否可创建测试单
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.enable_prod_autotest_ex_async(request, headers, runtime)
+
+    def enable_prod_autotest_ex(
+        self,
+        request: yunqing_models.EnableProdAutotestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.EnableProdAutotestResponse:
+        """
+        Description: 产品是否可创建测试单
+        Summary: 产品是否可创建测试单
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.EnableProdAutotestResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.prod.autotest.enable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def enable_prod_autotest_ex_async(
+        self,
+        request: yunqing_models.EnableProdAutotestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.EnableProdAutotestResponse:
+        """
+        Description: 产品是否可创建测试单
+        Summary: 产品是否可创建测试单
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.EnableProdAutotestResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.prod.autotest.enable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_system_parameter(
+        self,
+        request: yunqing_models.QuerySystemParameterRequest,
+    ) -> yunqing_models.QuerySystemParameterResponse:
+        """
+        Description: 系统参数查询
+        Summary: 系统参数查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_system_parameter_ex(request, headers, runtime)
+
+    async def query_system_parameter_async(
+        self,
+        request: yunqing_models.QuerySystemParameterRequest,
+    ) -> yunqing_models.QuerySystemParameterResponse:
+        """
+        Description: 系统参数查询
+        Summary: 系统参数查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_system_parameter_ex_async(request, headers, runtime)
+
+    def query_system_parameter_ex(
+        self,
+        request: yunqing_models.QuerySystemParameterRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QuerySystemParameterResponse:
+        """
+        Description: 系统参数查询
+        Summary: 系统参数查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QuerySystemParameterResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.system.parameter.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_system_parameter_ex_async(
+        self,
+        request: yunqing_models.QuerySystemParameterRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QuerySystemParameterResponse:
+        """
+        Description: 系统参数查询
+        Summary: 系统参数查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QuerySystemParameterResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.system.parameter.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_opsplan_nodetree(
+        self,
+        request: yunqing_models.QueryOpsplanNodetreeRequest,
+    ) -> yunqing_models.QueryOpsplanNodetreeResponse:
+        """
+        Description: 查询发布单详情
+        发布单详情的任务树是嵌套结构，OP目前不支持定义此类型的结构体
+        故本接口返回了json string，调用方需要自己构造
+        Summary: 查询发布单详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_opsplan_nodetree_ex(request, headers, runtime)
+
+    async def query_opsplan_nodetree_async(
+        self,
+        request: yunqing_models.QueryOpsplanNodetreeRequest,
+    ) -> yunqing_models.QueryOpsplanNodetreeResponse:
+        """
+        Description: 查询发布单详情
+        发布单详情的任务树是嵌套结构，OP目前不支持定义此类型的结构体
+        故本接口返回了json string，调用方需要自己构造
+        Summary: 查询发布单详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_opsplan_nodetree_ex_async(request, headers, runtime)
+
+    def query_opsplan_nodetree_ex(
+        self,
+        request: yunqing_models.QueryOpsplanNodetreeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QueryOpsplanNodetreeResponse:
+        """
+        Description: 查询发布单详情
+        发布单详情的任务树是嵌套结构，OP目前不支持定义此类型的结构体
+        故本接口返回了json string，调用方需要自己构造
+        Summary: 查询发布单详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QueryOpsplanNodetreeResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.opsplan.nodetree.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_opsplan_nodetree_ex_async(
+        self,
+        request: yunqing_models.QueryOpsplanNodetreeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QueryOpsplanNodetreeResponse:
+        """
+        Description: 查询发布单详情
+        发布单详情的任务树是嵌套结构，OP目前不支持定义此类型的结构体
+        故本接口返回了json string，调用方需要自己构造
+        Summary: 查询发布单详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QueryOpsplanNodetreeResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.opsplan.nodetree.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_aap_sites(
+        self,
+        request: yunqing_models.ListAapSitesRequest,
+    ) -> yunqing_models.ListAapSitesResponse:
+        """
+        Description: 站点信息list
+        Summary: 站点信息list
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_aap_sites_ex(request, headers, runtime)
+
+    async def list_aap_sites_async(
+        self,
+        request: yunqing_models.ListAapSitesRequest,
+    ) -> yunqing_models.ListAapSitesResponse:
+        """
+        Description: 站点信息list
+        Summary: 站点信息list
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_aap_sites_ex_async(request, headers, runtime)
+
+    def list_aap_sites_ex(
+        self,
+        request: yunqing_models.ListAapSitesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.ListAapSitesResponse:
+        """
+        Description: 站点信息list
+        Summary: 站点信息list
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.ListAapSitesResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.sites.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_aap_sites_ex_async(
+        self,
+        request: yunqing_models.ListAapSitesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.ListAapSitesResponse:
+        """
+        Description: 站点信息list
+        Summary: 站点信息list
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.ListAapSitesResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.sites.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def import_aap_meta(
+        self,
+        request: yunqing_models.ImportAapMetaRequest,
+    ) -> yunqing_models.ImportAapMetaResponse:
+        """
+        Description: AAP 元数据导入，包含：产品、应用、拓扑信息 。https://yuque.antfin-inc.com/tpaas/ednkxs/izdpx9s4at32mwbi?singleDoc# 《AAP：用户自定义产品接入》
+        Summary: AAP 元数据导入
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.import_aap_meta_ex(request, headers, runtime)
+
+    async def import_aap_meta_async(
+        self,
+        request: yunqing_models.ImportAapMetaRequest,
+    ) -> yunqing_models.ImportAapMetaResponse:
+        """
+        Description: AAP 元数据导入，包含：产品、应用、拓扑信息 。https://yuque.antfin-inc.com/tpaas/ednkxs/izdpx9s4at32mwbi?singleDoc# 《AAP：用户自定义产品接入》
+        Summary: AAP 元数据导入
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.import_aap_meta_ex_async(request, headers, runtime)
+
+    def import_aap_meta_ex(
+        self,
+        request: yunqing_models.ImportAapMetaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.ImportAapMetaResponse:
+        """
+        Description: AAP 元数据导入，包含：产品、应用、拓扑信息 。https://yuque.antfin-inc.com/tpaas/ednkxs/izdpx9s4at32mwbi?singleDoc# 《AAP：用户自定义产品接入》
+        Summary: AAP 元数据导入
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.ImportAapMetaResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.meta.import', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def import_aap_meta_ex_async(
+        self,
+        request: yunqing_models.ImportAapMetaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.ImportAapMetaResponse:
+        """
+        Description: AAP 元数据导入，包含：产品、应用、拓扑信息 。https://yuque.antfin-inc.com/tpaas/ednkxs/izdpx9s4at32mwbi?singleDoc# 《AAP：用户自定义产品接入》
+        Summary: AAP 元数据导入
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.ImportAapMetaResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.meta.import', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def init_aap_productinstance(
+        self,
+        request: yunqing_models.InitAapProductinstanceRequest,
+    ) -> yunqing_models.InitAapProductinstanceResponse:
+        """
+        Description: AAP 产品实例初始化
+        Summary: AAP 产品实例初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.init_aap_productinstance_ex(request, headers, runtime)
+
+    async def init_aap_productinstance_async(
+        self,
+        request: yunqing_models.InitAapProductinstanceRequest,
+    ) -> yunqing_models.InitAapProductinstanceResponse:
+        """
+        Description: AAP 产品实例初始化
+        Summary: AAP 产品实例初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.init_aap_productinstance_ex_async(request, headers, runtime)
+
+    def init_aap_productinstance_ex(
+        self,
+        request: yunqing_models.InitAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.InitAapProductinstanceResponse:
+        """
+        Description: AAP 产品实例初始化
+        Summary: AAP 产品实例初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.InitAapProductinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.productinstance.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def init_aap_productinstance_ex_async(
+        self,
+        request: yunqing_models.InitAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.InitAapProductinstanceResponse:
+        """
+        Description: AAP 产品实例初始化
+        Summary: AAP 产品实例初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.InitAapProductinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.productinstance.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def init_aap_release(
+        self,
+        request: yunqing_models.InitAapReleaseRequest,
+    ) -> yunqing_models.InitAapReleaseResponse:
+        """
+        Description: 产品实例发布初始化
+        Summary: 产品实例发布初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.init_aap_release_ex(request, headers, runtime)
+
+    async def init_aap_release_async(
+        self,
+        request: yunqing_models.InitAapReleaseRequest,
+    ) -> yunqing_models.InitAapReleaseResponse:
+        """
+        Description: 产品实例发布初始化
+        Summary: 产品实例发布初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.init_aap_release_ex_async(request, headers, runtime)
+
+    def init_aap_release_ex(
+        self,
+        request: yunqing_models.InitAapReleaseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.InitAapReleaseResponse:
+        """
+        Description: 产品实例发布初始化
+        Summary: 产品实例发布初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.InitAapReleaseResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.release.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def init_aap_release_ex_async(
+        self,
+        request: yunqing_models.InitAapReleaseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.InitAapReleaseResponse:
+        """
+        Description: 产品实例发布初始化
+        Summary: 产品实例发布初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.InitAapReleaseResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.release.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def deploy_aap_productinstance(
+        self,
+        request: yunqing_models.DeployAapProductinstanceRequest,
+    ) -> yunqing_models.DeployAapProductinstanceResponse:
+        """
+        Description: 产品实例部署
+        Summary: 产品实例部署
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.deploy_aap_productinstance_ex(request, headers, runtime)
+
+    async def deploy_aap_productinstance_async(
+        self,
+        request: yunqing_models.DeployAapProductinstanceRequest,
+    ) -> yunqing_models.DeployAapProductinstanceResponse:
+        """
+        Description: 产品实例部署
+        Summary: 产品实例部署
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.deploy_aap_productinstance_ex_async(request, headers, runtime)
+
+    def deploy_aap_productinstance_ex(
+        self,
+        request: yunqing_models.DeployAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.DeployAapProductinstanceResponse:
+        """
+        Description: 产品实例部署
+        Summary: 产品实例部署
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.DeployAapProductinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.productinstance.deploy', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def deploy_aap_productinstance_ex_async(
+        self,
+        request: yunqing_models.DeployAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.DeployAapProductinstanceResponse:
+        """
+        Description: 产品实例部署
+        Summary: 产品实例部署
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.DeployAapProductinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.productinstance.deploy', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_aap_release(
+        self,
+        request: yunqing_models.GetAapReleaseRequest,
+    ) -> yunqing_models.GetAapReleaseResponse:
+        """
+        Description: 发布单状态查询
+        Summary: 发布单
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_aap_release_ex(request, headers, runtime)
+
+    async def get_aap_release_async(
+        self,
+        request: yunqing_models.GetAapReleaseRequest,
+    ) -> yunqing_models.GetAapReleaseResponse:
+        """
+        Description: 发布单状态查询
+        Summary: 发布单
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_aap_release_ex_async(request, headers, runtime)
+
+    def get_aap_release_ex(
+        self,
+        request: yunqing_models.GetAapReleaseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.GetAapReleaseResponse:
+        """
+        Description: 发布单状态查询
+        Summary: 发布单
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.GetAapReleaseResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.release.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_aap_release_ex_async(
+        self,
+        request: yunqing_models.GetAapReleaseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.GetAapReleaseResponse:
+        """
+        Description: 发布单状态查询
+        Summary: 发布单
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.GetAapReleaseResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.release.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_aap_applicationinstance(
+        self,
+        request: yunqing_models.UpdateAapApplicationinstanceRequest,
+    ) -> yunqing_models.UpdateAapApplicationinstanceResponse:
+        """
+        Description: 应用实例更新，比如：规格、镜像、参数等
+        Summary: 应用实例更新
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_aap_applicationinstance_ex(request, headers, runtime)
+
+    async def update_aap_applicationinstance_async(
+        self,
+        request: yunqing_models.UpdateAapApplicationinstanceRequest,
+    ) -> yunqing_models.UpdateAapApplicationinstanceResponse:
+        """
+        Description: 应用实例更新，比如：规格、镜像、参数等
+        Summary: 应用实例更新
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_aap_applicationinstance_ex_async(request, headers, runtime)
+
+    def update_aap_applicationinstance_ex(
+        self,
+        request: yunqing_models.UpdateAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.UpdateAapApplicationinstanceResponse:
+        """
+        Description: 应用实例更新，比如：规格、镜像、参数等
+        Summary: 应用实例更新
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.UpdateAapApplicationinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.applicationinstance.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_aap_applicationinstance_ex_async(
+        self,
+        request: yunqing_models.UpdateAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.UpdateAapApplicationinstanceResponse:
+        """
+        Description: 应用实例更新，比如：规格、镜像、参数等
+        Summary: 应用实例更新
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.UpdateAapApplicationinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.applicationinstance.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_aap_applicationinstance(
+        self,
+        request: yunqing_models.QueryAapApplicationinstanceRequest,
+    ) -> yunqing_models.QueryAapApplicationinstanceResponse:
+        """
+        Description: 应用实例查询
+        Summary: 应用实例查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_aap_applicationinstance_ex(request, headers, runtime)
+
+    async def query_aap_applicationinstance_async(
+        self,
+        request: yunqing_models.QueryAapApplicationinstanceRequest,
+    ) -> yunqing_models.QueryAapApplicationinstanceResponse:
+        """
+        Description: 应用实例查询
+        Summary: 应用实例查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_aap_applicationinstance_ex_async(request, headers, runtime)
+
+    def query_aap_applicationinstance_ex(
+        self,
+        request: yunqing_models.QueryAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QueryAapApplicationinstanceResponse:
+        """
+        Description: 应用实例查询
+        Summary: 应用实例查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QueryAapApplicationinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.applicationinstance.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_aap_applicationinstance_ex_async(
+        self,
+        request: yunqing_models.QueryAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QueryAapApplicationinstanceResponse:
+        """
+        Description: 应用实例查询
+        Summary: 应用实例查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QueryAapApplicationinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.applicationinstance.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def set_aap_applicationinstance(
+        self,
+        request: yunqing_models.SetAapApplicationinstanceRequest,
+    ) -> yunqing_models.SetAapApplicationinstanceResponse:
+        """
+        Description: 应用规格配置修改
+        Summary: 应用规格配置修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.set_aap_applicationinstance_ex(request, headers, runtime)
+
+    async def set_aap_applicationinstance_async(
+        self,
+        request: yunqing_models.SetAapApplicationinstanceRequest,
+    ) -> yunqing_models.SetAapApplicationinstanceResponse:
+        """
+        Description: 应用规格配置修改
+        Summary: 应用规格配置修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.set_aap_applicationinstance_ex_async(request, headers, runtime)
+
+    def set_aap_applicationinstance_ex(
+        self,
+        request: yunqing_models.SetAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.SetAapApplicationinstanceResponse:
+        """
+        Description: 应用规格配置修改
+        Summary: 应用规格配置修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.SetAapApplicationinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.applicationinstance.set', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def set_aap_applicationinstance_ex_async(
+        self,
+        request: yunqing_models.SetAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.SetAapApplicationinstanceResponse:
+        """
+        Description: 应用规格配置修改
+        Summary: 应用规格配置修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.SetAapApplicationinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.applicationinstance.set', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def set_aap_images(
+        self,
+        request: yunqing_models.SetAapImagesRequest,
+    ) -> yunqing_models.SetAapImagesResponse:
+        """
+        Description: 应用镜像修改
+        Summary: 应用镜像修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.set_aap_images_ex(request, headers, runtime)
+
+    async def set_aap_images_async(
+        self,
+        request: yunqing_models.SetAapImagesRequest,
+    ) -> yunqing_models.SetAapImagesResponse:
+        """
+        Description: 应用镜像修改
+        Summary: 应用镜像修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.set_aap_images_ex_async(request, headers, runtime)
+
+    def set_aap_images_ex(
+        self,
+        request: yunqing_models.SetAapImagesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.SetAapImagesResponse:
+        """
+        Description: 应用镜像修改
+        Summary: 应用镜像修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.SetAapImagesResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.images.set', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def set_aap_images_ex_async(
+        self,
+        request: yunqing_models.SetAapImagesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.SetAapImagesResponse:
+        """
+        Description: 应用镜像修改
+        Summary: 应用镜像修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.SetAapImagesResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.images.set', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_aap_productinstance(
+        self,
+        request: yunqing_models.QueryAapProductinstanceRequest,
+    ) -> yunqing_models.QueryAapProductinstanceResponse:
+        """
+        Description: 产品实例查询
+        Summary: 产品实例查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_aap_productinstance_ex(request, headers, runtime)
+
+    async def query_aap_productinstance_async(
+        self,
+        request: yunqing_models.QueryAapProductinstanceRequest,
+    ) -> yunqing_models.QueryAapProductinstanceResponse:
+        """
+        Description: 产品实例查询
+        Summary: 产品实例查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_aap_productinstance_ex_async(request, headers, runtime)
+
+    def query_aap_productinstance_ex(
+        self,
+        request: yunqing_models.QueryAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QueryAapProductinstanceResponse:
+        """
+        Description: 产品实例查询
+        Summary: 产品实例查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QueryAapProductinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.productinstance.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_aap_productinstance_ex_async(
+        self,
+        request: yunqing_models.QueryAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.QueryAapProductinstanceResponse:
+        """
+        Description: 产品实例查询
+        Summary: 产品实例查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.QueryAapProductinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.productinstance.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def detail_aap_applicationinstance(
+        self,
+        request: yunqing_models.DetailAapApplicationinstanceRequest,
+    ) -> yunqing_models.DetailAapApplicationinstanceResponse:
+        """
+        Description: 应用实例详情查询
+        Summary: 应用实例详情查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_aap_applicationinstance_ex(request, headers, runtime)
+
+    async def detail_aap_applicationinstance_async(
+        self,
+        request: yunqing_models.DetailAapApplicationinstanceRequest,
+    ) -> yunqing_models.DetailAapApplicationinstanceResponse:
+        """
+        Description: 应用实例详情查询
+        Summary: 应用实例详情查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_aap_applicationinstance_ex_async(request, headers, runtime)
+
+    def detail_aap_applicationinstance_ex(
+        self,
+        request: yunqing_models.DetailAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.DetailAapApplicationinstanceResponse:
+        """
+        Description: 应用实例详情查询
+        Summary: 应用实例详情查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.DetailAapApplicationinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.applicationinstance.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_aap_applicationinstance_ex_async(
+        self,
+        request: yunqing_models.DetailAapApplicationinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.DetailAapApplicationinstanceResponse:
+        """
+        Description: 应用实例详情查询
+        Summary: 应用实例详情查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.DetailAapApplicationinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.applicationinstance.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def set_aap_parameters(
+        self,
+        request: yunqing_models.SetAapParametersRequest,
+    ) -> yunqing_models.SetAapParametersResponse:
+        """
+        Description: 应用参数更新
+        Summary: 应用参数更新
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.set_aap_parameters_ex(request, headers, runtime)
+
+    async def set_aap_parameters_async(
+        self,
+        request: yunqing_models.SetAapParametersRequest,
+    ) -> yunqing_models.SetAapParametersResponse:
+        """
+        Description: 应用参数更新
+        Summary: 应用参数更新
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.set_aap_parameters_ex_async(request, headers, runtime)
+
+    def set_aap_parameters_ex(
+        self,
+        request: yunqing_models.SetAapParametersRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.SetAapParametersResponse:
+        """
+        Description: 应用参数更新
+        Summary: 应用参数更新
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.SetAapParametersResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.parameters.set', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def set_aap_parameters_ex_async(
+        self,
+        request: yunqing_models.SetAapParametersRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.SetAapParametersResponse:
+        """
+        Description: 应用参数更新
+        Summary: 应用参数更新
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.SetAapParametersResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.parameters.set', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def delete_aap_productinstance(
+        self,
+        request: yunqing_models.DeleteAapProductinstanceRequest,
+    ) -> yunqing_models.DeleteAapProductinstanceResponse:
+        """
+        Description: 产品实例卸载
+        Summary: 产品实例卸载
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.delete_aap_productinstance_ex(request, headers, runtime)
+
+    async def delete_aap_productinstance_async(
+        self,
+        request: yunqing_models.DeleteAapProductinstanceRequest,
+    ) -> yunqing_models.DeleteAapProductinstanceResponse:
+        """
+        Description: 产品实例卸载
+        Summary: 产品实例卸载
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.delete_aap_productinstance_ex_async(request, headers, runtime)
+
+    def delete_aap_productinstance_ex(
+        self,
+        request: yunqing_models.DeleteAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.DeleteAapProductinstanceResponse:
+        """
+        Description: 产品实例卸载
+        Summary: 产品实例卸载
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.DeleteAapProductinstanceResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.aap.productinstance.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def delete_aap_productinstance_ex_async(
+        self,
+        request: yunqing_models.DeleteAapProductinstanceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.DeleteAapProductinstanceResponse:
+        """
+        Description: 产品实例卸载
+        Summary: 产品实例卸载
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.DeleteAapProductinstanceResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.aap.productinstance.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_env(
+        self,
+        request: yunqing_models.CreateEnvRequest,
+    ) -> yunqing_models.CreateEnvResponse:
+        """
+        Description: 初始化云游local环境
+        Summary: 初始化云游local环境
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_env_ex(request, headers, runtime)
+
+    async def create_env_async(
+        self,
+        request: yunqing_models.CreateEnvRequest,
+    ) -> yunqing_models.CreateEnvResponse:
+        """
+        Description: 初始化云游local环境
+        Summary: 初始化云游local环境
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_env_ex_async(request, headers, runtime)
+
+    def create_env_ex(
+        self,
+        request: yunqing_models.CreateEnvRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.CreateEnvResponse:
+        """
+        Description: 初始化云游local环境
+        Summary: 初始化云游local环境
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.CreateEnvResponse(),
+            self.do_request('1.0', 'yunyou.yunqing.env.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_env_ex_async(
+        self,
+        request: yunqing_models.CreateEnvRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yunqing_models.CreateEnvResponse:
+        """
+        Description: 初始化云游local环境
+        Summary: 初始化云游local环境
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yunqing_models.CreateEnvResponse(),
+            await self.do_request_async('1.0', 'yunyou.yunqing.env.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def all_envs(
         self,
         request: yunqing_models.AllEnvsRequest,
     ) -> yunqing_models.AllEnvsResponse:
         """
         Description: 云游纳管的所有环境基本信息查询
         Summary: 云游纳管的所有环境基本信息查询
```

### Comparing `antchain_yunqing-3.14.18/antchain_sdk_yunqing/models.py` & `antchain_yunqing-4.0.5/antchain_sdk_yunqing/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -2038,14 +2038,72 @@
         if m.get('utc_create') is not None:
             self.utc_create = m.get('utc_create')
         if m.get('utc_modified') is not None:
             self.utc_modified = m.get('utc_modified')
         return self
 
 
+class SystemParameterInfo(TeaModel):
+    def __init__(
+        self,
+        type: str = None,
+        value: str = None,
+        env_id: str = None,
+        description: str = None,
+        id: str = None,
+    ):
+        # 参数名
+        self.type = type
+        # 参数值
+        self.value = value
+        # 环境Id
+        self.env_id = env_id
+        # 参数描述
+        self.description = description
+        # 记录id
+        self.id = id
+
+    def validate(self):
+        self.validate_required(self.type, 'type')
+        self.validate_required(self.value, 'value')
+        self.validate_required(self.env_id, 'env_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.type is not None:
+            result['type'] = self.type
+        if self.value is not None:
+            result['value'] = self.value
+        if self.env_id is not None:
+            result['env_id'] = self.env_id
+        if self.description is not None:
+            result['description'] = self.description
+        if self.id is not None:
+            result['id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        if m.get('env_id') is not None:
+            self.env_id = m.get('env_id')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        return self
+
+
 class Application(TeaModel):
     def __init__(
         self,
         application_name: str = None,
         product_code: str = None,
     ):
         # 应用英文名
@@ -2673,14 +2731,18 @@
         app_type: str = None,
         app_display_name: str = None,
         app_level: str = None,
         tenant_id: str = None,
         product_app: str = None,
         owner: Owner = None,
         admin: Admin = None,
+        expect_replica: int = None,
+        image: str = None,
+        cpu: int = None,
+        memory: int = None,
     ):
         # 应用英文名。
         self.app_name = app_name
         # 应用版本
         self.app_version = app_version
         # 单元ID
         self.cell_id = cell_id
@@ -2706,14 +2768,22 @@
         self.tenant_id = tenant_id
         # 产品码--应用名
         self.product_app = product_app
         # 产品Owner
         self.owner = owner
         # 应用SRE信息
         self.admin = admin
+        # 副本数
+        self.expect_replica = expect_replica
+        # 镜像
+        self.image = image
+        # 2G
+        self.cpu = cpu
+        # 内存资源
+        self.memory = memory
 
     def validate(self):
         if self.owner:
             self.owner.validate()
         if self.admin:
             self.admin.validate()
 
@@ -2751,14 +2821,22 @@
             result['tenant_id'] = self.tenant_id
         if self.product_app is not None:
             result['product_app'] = self.product_app
         if self.owner is not None:
             result['owner'] = self.owner.to_map()
         if self.admin is not None:
             result['admin'] = self.admin.to_map()
+        if self.expect_replica is not None:
+            result['expect_replica'] = self.expect_replica
+        if self.image is not None:
+            result['image'] = self.image
+        if self.cpu is not None:
+            result['cpu'] = self.cpu
+        if self.memory is not None:
+            result['memory'] = self.memory
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('app_name') is not None:
             self.app_name = m.get('app_name')
         if m.get('app_version') is not None:
@@ -2789,14 +2867,22 @@
             self.product_app = m.get('product_app')
         if m.get('owner') is not None:
             temp_model = Owner()
             self.owner = temp_model.from_map(m['owner'])
         if m.get('admin') is not None:
             temp_model = Admin()
             self.admin = temp_model.from_map(m['admin'])
+        if m.get('expect_replica') is not None:
+            self.expect_replica = m.get('expect_replica')
+        if m.get('image') is not None:
+            self.image = m.get('image')
+        if m.get('cpu') is not None:
+            self.cpu = m.get('cpu')
+        if m.get('memory') is not None:
+            self.memory = m.get('memory')
         return self
 
 
 class DeploymentUnitSnapshotOP(TeaModel):
     def __init__(
         self,
         env_id: str = None,
@@ -3084,14 +3170,76 @@
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
+class AutoTestAvailableProdOption(TeaModel):
+    def __init__(
+        self,
+        is_runnable: bool = None,
+        message: str = None,
+        deployment_unit_identity: str = None,
+        identity: str = None,
+        prod_code: str = None,
+    ):
+        # 是否可执行测试用例
+        self.is_runnable = is_runnable
+        # 不能执行自动化测试用例的原因
+        # 
+        self.message = message
+        # 部署单元唯一标识（元数据）
+        # 
+        self.deployment_unit_identity = deployment_unit_identity
+        # 部署单元实例唯一标识
+        self.identity = identity
+        # 产品码
+        self.prod_code = prod_code
+
+    def validate(self):
+        self.validate_required(self.is_runnable, 'is_runnable')
+        self.validate_required(self.message, 'message')
+        self.validate_required(self.deployment_unit_identity, 'deployment_unit_identity')
+        self.validate_required(self.identity, 'identity')
+        self.validate_required(self.prod_code, 'prod_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.is_runnable is not None:
+            result['is_runnable'] = self.is_runnable
+        if self.message is not None:
+            result['message'] = self.message
+        if self.deployment_unit_identity is not None:
+            result['deployment_unit_identity'] = self.deployment_unit_identity
+        if self.identity is not None:
+            result['identity'] = self.identity
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('is_runnable') is not None:
+            self.is_runnable = m.get('is_runnable')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('deployment_unit_identity') is not None:
+            self.deployment_unit_identity = m.get('deployment_unit_identity')
+        if m.get('identity') is not None:
+            self.identity = m.get('identity')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        return self
+
+
 class System(TeaModel):
     def __init__(
         self,
         commit_id: str = None,
         envs: List[Env] = None,
         open_apis: List[OpenAPI] = None,
         version: str = None,
@@ -3389,14 +3537,882 @@
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('resource_pool_id') is not None:
             self.resource_pool_id = m.get('resource_pool_id')
         return self
 
 
+class HTTP(TeaModel):
+    def __init__(
+        self,
+        path: str = None,
+        scheme: str = None,
+        port: int = None,
+    ):
+        # 检查path
+        self.path = path
+        # http schema
+        self.scheme = scheme
+        # port
+        self.port = port
+
+    def validate(self):
+        self.validate_required(self.path, 'path')
+        self.validate_required(self.scheme, 'scheme')
+        self.validate_required(self.port, 'port')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.path is not None:
+            result['path'] = self.path
+        if self.scheme is not None:
+            result['scheme'] = self.scheme
+        if self.port is not None:
+            result['port'] = self.port
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('path') is not None:
+            self.path = m.get('path')
+        if m.get('scheme') is not None:
+            self.scheme = m.get('scheme')
+        if m.get('port') is not None:
+            self.port = m.get('port')
+        return self
+
+
+class HostPathVolumeSource(TeaModel):
+    def __init__(
+        self,
+        path: str = None,
+        type: str = None,
+    ):
+        # 宿主机挂载的路径
+        self.path = path
+        # 挂载的类型：  FILE("File"),
+        # DIRECTORY("Directory");
+        self.type = type
+
+    def validate(self):
+        self.validate_required(self.path, 'path')
+        self.validate_required(self.type, 'type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.path is not None:
+            result['path'] = self.path
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('path') is not None:
+            self.path = m.get('path')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class PersistentVolumeSource(TeaModel):
+    def __init__(
+        self,
+        access_modes: List[str] = None,
+    ):
+        # READWRITEONCE("ReadWriteOnce"),
+        # READONLYMANY("ReadOnlyMany"),
+        # READWRITEMANY("ReadWriteMany");
+        self.access_modes = access_modes
+
+    def validate(self):
+        self.validate_required(self.access_modes, 'access_modes')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_modes is not None:
+            result['access_modes'] = self.access_modes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('access_modes') is not None:
+            self.access_modes = m.get('access_modes')
+        return self
+
+
+class Exec(TeaModel):
+    def __init__(
+        self,
+        args: List[str] = None,
+        cmd: str = None,
+    ):
+        # args
+        self.args = args
+        # cmd
+        self.cmd = cmd
+
+    def validate(self):
+        self.validate_required(self.args, 'args')
+        self.validate_required(self.cmd, 'cmd')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.args is not None:
+            result['args'] = self.args
+        if self.cmd is not None:
+            result['cmd'] = self.cmd
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('args') is not None:
+            self.args = m.get('args')
+        if m.get('cmd') is not None:
+            self.cmd = m.get('cmd')
+        return self
+
+
+class TCP(TeaModel):
+    def __init__(
+        self,
+        port: int = None,
+    ):
+        # tcp port
+        self.port = port
+
+    def validate(self):
+        self.validate_required(self.port, 'port')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.port is not None:
+            result['port'] = self.port
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('port') is not None:
+            self.port = m.get('port')
+        return self
+
+
+class MountOptions(TeaModel):
+    def __init__(
+        self,
+        mount_path: str = None,
+        read_only: str = None,
+        mount_propagation: str = None,
+    ):
+        # 容器内挂载路径
+        self.mount_path = mount_path
+        # 是否只读，默认false
+        self.read_only = read_only
+        # 挂载传递策略：    NONE("None"),
+        # HOSTTOCONTAINER("HostToContainer"),
+        # BIDIRECTIONAL("Bidirectional");
+        # 
+        self.mount_propagation = mount_propagation
+
+    def validate(self):
+        self.validate_required(self.mount_path, 'mount_path')
+        self.validate_required(self.read_only, 'read_only')
+        self.validate_required(self.mount_propagation, 'mount_propagation')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mount_path is not None:
+            result['mount_path'] = self.mount_path
+        if self.read_only is not None:
+            result['read_only'] = self.read_only
+        if self.mount_propagation is not None:
+            result['mount_propagation'] = self.mount_propagation
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('mount_path') is not None:
+            self.mount_path = m.get('mount_path')
+        if m.get('read_only') is not None:
+            self.read_only = m.get('read_only')
+        if m.get('mount_propagation') is not None:
+            self.mount_propagation = m.get('mount_propagation')
+        return self
+
+
+class ProbeConfig(TeaModel):
+    def __init__(
+        self,
+        timeout: str = None,
+        exec: Exec = None,
+        http: HTTP = None,
+        tcp: TCP = None,
+    ):
+        # 超时时间，单位s
+        self.timeout = timeout
+        # exec
+        self.exec = exec
+        # http
+        self.http = http
+        # tcp
+        self.tcp = tcp
+
+    def validate(self):
+        self.validate_required(self.timeout, 'timeout')
+        if self.exec:
+            self.exec.validate()
+        if self.http:
+            self.http.validate()
+        if self.tcp:
+            self.tcp.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.timeout is not None:
+            result['timeout'] = self.timeout
+        if self.exec is not None:
+            result['exec'] = self.exec.to_map()
+        if self.http is not None:
+            result['http'] = self.http.to_map()
+        if self.tcp is not None:
+            result['tcp'] = self.tcp.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('timeout') is not None:
+            self.timeout = m.get('timeout')
+        if m.get('exec') is not None:
+            temp_model = Exec()
+            self.exec = temp_model.from_map(m['exec'])
+        if m.get('http') is not None:
+            temp_model = HTTP()
+            self.http = temp_model.from_map(m['http'])
+        if m.get('tcp') is not None:
+            temp_model = TCP()
+            self.tcp = temp_model.from_map(m['tcp'])
+        return self
+
+
+class GrayRelease(TeaModel):
+    def __init__(
+        self,
+        updated_replicas: int = None,
+        release_strategy: str = None,
+    ):
+        # 需要更新到的副本数，比如：应用A有10个副本，本次更新updated_replicas=5，则会更新前5个
+        self.updated_replicas = updated_replicas
+        # 发布策略：TWO_GROUP("TWO_GROUP", "分两组"),
+        # ALL_ONE("ALL_ONE", "共分一组"),
+        # EACH_ONE("EACH_ONE", "每台一组"),
+        # SYSTEM_RECOMMENDATION("SYSTEM_RECOMMENDATION", "系统推荐"),
+        # CUSTOMIZE("CUSTOMIZE", "自定义分组")
+        self.release_strategy = release_strategy
+
+    def validate(self):
+        self.validate_required(self.release_strategy, 'release_strategy')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.updated_replicas is not None:
+            result['updated_replicas'] = self.updated_replicas
+        if self.release_strategy is not None:
+            result['release_strategy'] = self.release_strategy
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('updated_replicas') is not None:
+            self.updated_replicas = m.get('updated_replicas')
+        if m.get('release_strategy') is not None:
+            self.release_strategy = m.get('release_strategy')
+        return self
+
+
+class VolumeSource(TeaModel):
+    def __init__(
+        self,
+        host_path: HostPathVolumeSource = None,
+        persistent_volume: PersistentVolumeSource = None,
+    ):
+        # 宿主机模式配置
+        self.host_path = host_path
+        # 和Host二选一
+        self.persistent_volume = persistent_volume
+
+    def validate(self):
+        if self.host_path:
+            self.host_path.validate()
+        if self.persistent_volume:
+            self.persistent_volume.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_path is not None:
+            result['host_path'] = self.host_path.to_map()
+        if self.persistent_volume is not None:
+            result['persistent_volume'] = self.persistent_volume.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('host_path') is not None:
+            temp_model = HostPathVolumeSource()
+            self.host_path = temp_model.from_map(m['host_path'])
+        if m.get('persistent_volume') is not None:
+            temp_model = PersistentVolumeSource()
+            self.persistent_volume = temp_model.from_map(m['persistent_volume'])
+        return self
+
+
+class SQLMigration(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        upgrade: str = None,
+        downgrade: str = None,
+    ):
+        # 变更名称
+        self.key = key
+        # 产品升级变更sql
+        self.upgrade = upgrade
+        # 回滚变更sql
+        self.downgrade = downgrade
+
+    def validate(self):
+        self.validate_required(self.key, 'key')
+        self.validate_required(self.upgrade, 'upgrade')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['key'] = self.key
+        if self.upgrade is not None:
+            result['upgrade'] = self.upgrade
+        if self.downgrade is not None:
+            result['downgrade'] = self.downgrade
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('upgrade') is not None:
+            self.upgrade = m.get('upgrade')
+        if m.get('downgrade') is not None:
+            self.downgrade = m.get('downgrade')
+        return self
+
+
+class AffinityConfig(TeaModel):
+    def __init__(
+        self,
+        preferred: List[str] = None,
+        required: List[str] = None,
+    ):
+        # 尽量满足的应用列表
+        self.preferred = preferred
+        # 必须满足的应用列表
+        self.required = required
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
+        if self.preferred is not None:
+            result['preferred'] = self.preferred
+        if self.required is not None:
+            result['required'] = self.required
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('preferred') is not None:
+            self.preferred = m.get('preferred')
+        if m.get('required') is not None:
+            self.required = m.get('required')
+        return self
+
+
+class VolumeSpec(TeaModel):
+    def __init__(
+        self,
+        volume_name: str = None,
+        capacity: str = None,
+    ):
+        # 数据卷名称
+        self.volume_name = volume_name
+        # 数据卷容量，单位为G
+        self.capacity = capacity
+
+    def validate(self):
+        self.validate_required(self.volume_name, 'volume_name')
+        self.validate_required(self.capacity, 'capacity')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.volume_name is not None:
+            result['volume_name'] = self.volume_name
+        if self.capacity is not None:
+            result['capacity'] = self.capacity
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('volume_name') is not None:
+            self.volume_name = m.get('volume_name')
+        if m.get('capacity') is not None:
+            self.capacity = m.get('capacity')
+        return self
+
+
+class ParameterTemplate(TeaModel):
+    def __init__(
+        self,
+        template: str = None,
+        target: str = None,
+    ):
+        # template模板值
+        self.template = template
+        # target 模版对象
+        self.target = target
+
+    def validate(self):
+        self.validate_required(self.template, 'template')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.template is not None:
+            result['template'] = self.template
+        if self.target is not None:
+            result['target'] = self.target
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('template') is not None:
+            self.template = m.get('template')
+        if m.get('target') is not None:
+            self.target = m.get('target')
+        return self
+
+
+class ProductInstanceMeta(TeaModel):
+    def __init__(
+        self,
+        namespace: str = None,
+        prod_code: str = None,
+        name: str = None,
+    ):
+        # 命名空间
+        self.namespace = namespace
+        # 产品Code
+        self.prod_code = prod_code
+        # 实例名称，同一个ns下不可重复
+        self.name = name
+
+    def validate(self):
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.name, 'name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.name is not None:
+            result['name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        return self
+
+
+class Parameter(TeaModel):
+    def __init__(
+        self,
+        default: str = None,
+        key: str = None,
+        description: str = None,
+        kind: str = None,
+        required: bool = None,
+        parameters: List[ParameterTemplate] = None,
+        type: str = None,
+    ):
+        # 参数默认值
+        self.default = default
+        # 参数key
+        self.key = key
+        # 参数描述
+        self.description = description
+        # 参数类型        MANUAL("manual"),
+        # CONSTANT("constant"),
+        # EXPRESSION("expression");
+        self.kind = kind
+        # 是否必须
+        self.required = required
+        # 参数模版
+        self.parameters = parameters
+        # STRING("string"),
+        # SECRET("secret"),
+        # INT("int"),
+        # FLOAT("float"),
+        # ANY("any");
+        self.type = type
+
+    def validate(self):
+        self.validate_required(self.default, 'default')
+        self.validate_required(self.key, 'key')
+        self.validate_required(self.description, 'description')
+        self.validate_required(self.kind, 'kind')
+        self.validate_required(self.required, 'required')
+        self.validate_required(self.parameters, 'parameters')
+        if self.parameters:
+            for k in self.parameters:
+                if k:
+                    k.validate()
+        self.validate_required(self.type, 'type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.default is not None:
+            result['default'] = self.default
+        if self.key is not None:
+            result['key'] = self.key
+        if self.description is not None:
+            result['description'] = self.description
+        if self.kind is not None:
+            result['kind'] = self.kind
+        if self.required is not None:
+            result['required'] = self.required
+        result['parameters'] = []
+        if self.parameters is not None:
+            for k in self.parameters:
+                result['parameters'].append(k.to_map() if k else None)
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('default') is not None:
+            self.default = m.get('default')
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('kind') is not None:
+            self.kind = m.get('kind')
+        if m.get('required') is not None:
+            self.required = m.get('required')
+        self.parameters = []
+        if m.get('parameters') is not None:
+            for k in m.get('parameters'):
+                temp_model = ParameterTemplate()
+                self.parameters.append(temp_model.from_map(k))
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class PersistentVolumeConfig(TeaModel):
+    def __init__(
+        self,
+        volume_name: str = None,
+        access_modes: List[str] = None,
+        storage_class: str = None,
+        use_empty_dir: bool = None,
+    ):
+        # 挂载名称
+        self.volume_name = volume_name
+        # 挂载的获取名称，默认：ReadWriteOnce。READWRITEONCE("ReadWriteOnce"),
+        # READONLYMANY("ReadOnlyMany"),
+        # READWRITEMANY("ReadWriteMany");
+        self.access_modes = access_modes
+        # 存储类
+        self.storage_class = storage_class
+        # 是否使用匿名卷，，默认false
+        self.use_empty_dir = use_empty_dir
+
+    def validate(self):
+        self.validate_required(self.volume_name, 'volume_name')
+        self.validate_required(self.use_empty_dir, 'use_empty_dir')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.volume_name is not None:
+            result['volume_name'] = self.volume_name
+        if self.access_modes is not None:
+            result['access_modes'] = self.access_modes
+        if self.storage_class is not None:
+            result['storage_class'] = self.storage_class
+        if self.use_empty_dir is not None:
+            result['use_empty_dir'] = self.use_empty_dir
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('volume_name') is not None:
+            self.volume_name = m.get('volume_name')
+        if m.get('access_modes') is not None:
+            self.access_modes = m.get('access_modes')
+        if m.get('storage_class') is not None:
+            self.storage_class = m.get('storage_class')
+        if m.get('use_empty_dir') is not None:
+            self.use_empty_dir = m.get('use_empty_dir')
+        return self
+
+
+class Volume(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        volume_source: VolumeSource = None,
+        mount_options: MountOptions = None,
+    ):
+        # 数据卷名称
+        self.name = name
+        # 可挂载的配置
+        self.volume_source = volume_source
+        # 数据卷配置
+        self.mount_options = mount_options
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.volume_source, 'volume_source')
+        if self.volume_source:
+            self.volume_source.validate()
+        self.validate_required(self.mount_options, 'mount_options')
+        if self.mount_options:
+            self.mount_options.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.volume_source is not None:
+            result['volume_source'] = self.volume_source.to_map()
+        if self.mount_options is not None:
+            result['mount_options'] = self.mount_options.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('volume_source') is not None:
+            temp_model = VolumeSource()
+            self.volume_source = temp_model.from_map(m['volume_source'])
+        if m.get('mount_options') is not None:
+            temp_model = MountOptions()
+            self.mount_options = temp_model.from_map(m['mount_options'])
+        return self
+
+
+class TopologyConstraints(TeaModel):
+    def __init__(
+        self,
+        affinity: AffinityConfig = None,
+        anti_affinity: AffinityConfig = None,
+        sidecars: List[str] = None,
+    ):
+        # 亲和性配置
+        self.affinity = affinity
+        # 反亲和性配置
+        self.anti_affinity = anti_affinity
+        # sidecar应用列表
+        self.sidecars = sidecars
+
+    def validate(self):
+        if self.affinity:
+            self.affinity.validate()
+        if self.anti_affinity:
+            self.anti_affinity.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.affinity is not None:
+            result['affinity'] = self.affinity.to_map()
+        if self.anti_affinity is not None:
+            result['anti_affinity'] = self.anti_affinity.to_map()
+        if self.sidecars is not None:
+            result['sidecars'] = self.sidecars
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('affinity') is not None:
+            temp_model = AffinityConfig()
+            self.affinity = temp_model.from_map(m['affinity'])
+        if m.get('anti_affinity') is not None:
+            temp_model = AffinityConfig()
+            self.anti_affinity = temp_model.from_map(m['anti_affinity'])
+        if m.get('sidecars') is not None:
+            self.sidecars = m.get('sidecars')
+        return self
+
+
+class ResourceSpec(TeaModel):
+    def __init__(
+        self,
+        cpu: str = None,
+        gpu: str = None,
+        memory: str = None,
+        name: str = None,
+        replicas: int = None,
+        volumes: List[VolumeSpec] = None,
+    ):
+        # cpu规格
+        self.cpu = cpu
+        # gpu规格
+        self.gpu = gpu
+        # memory
+        self.memory = memory
+        # 规格名称
+        self.name = name
+        # 应用副本数
+        self.replicas = replicas
+        # 数据卷规格
+        self.volumes = volumes
+
+    def validate(self):
+        self.validate_required(self.cpu, 'cpu')
+        self.validate_required(self.memory, 'memory')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.replicas, 'replicas')
+        self.validate_required(self.volumes, 'volumes')
+        if self.volumes:
+            for k in self.volumes:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cpu is not None:
+            result['cpu'] = self.cpu
+        if self.gpu is not None:
+            result['gpu'] = self.gpu
+        if self.memory is not None:
+            result['memory'] = self.memory
+        if self.name is not None:
+            result['name'] = self.name
+        if self.replicas is not None:
+            result['replicas'] = self.replicas
+        result['volumes'] = []
+        if self.volumes is not None:
+            for k in self.volumes:
+                result['volumes'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cpu') is not None:
+            self.cpu = m.get('cpu')
+        if m.get('gpu') is not None:
+            self.gpu = m.get('gpu')
+        if m.get('memory') is not None:
+            self.memory = m.get('memory')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('replicas') is not None:
+            self.replicas = m.get('replicas')
+        self.volumes = []
+        if m.get('volumes') is not None:
+            for k in m.get('volumes'):
+                temp_model = VolumeSpec()
+                self.volumes.append(temp_model.from_map(k))
+        return self
+
+
 class CloudStackConfig(TeaModel):
     def __init__(
         self,
         access_key: str = None,
         encrypted_access_key_secret: str = None,
         region: str = None,
         zone: str = None,
@@ -3449,14 +4465,437 @@
         if m.get('zone') is not None:
             self.zone = m.get('zone')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class Lifecycle(TeaModel):
+    def __init__(
+        self,
+        liveness: ProbeConfig = None,
+        readiness: ProbeConfig = None,
+        pre_stop: ProbeConfig = None,
+        post_start: ProbeConfig = None,
+        start_up: ProbeConfig = None,
+        entrypoint: ProbeConfig = None,
+    ):
+        # 存活探针
+        self.liveness = liveness
+        # readiness
+        self.readiness = readiness
+        # preStop
+        self.pre_stop = pre_stop
+        # postStart
+        self.post_start = post_start
+        # startUp
+        self.start_up = start_up
+        # entrypoint
+        self.entrypoint = entrypoint
+
+    def validate(self):
+        if self.liveness:
+            self.liveness.validate()
+        if self.readiness:
+            self.readiness.validate()
+        if self.pre_stop:
+            self.pre_stop.validate()
+        if self.post_start:
+            self.post_start.validate()
+        if self.start_up:
+            self.start_up.validate()
+        if self.entrypoint:
+            self.entrypoint.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.liveness is not None:
+            result['liveness'] = self.liveness.to_map()
+        if self.readiness is not None:
+            result['readiness'] = self.readiness.to_map()
+        if self.pre_stop is not None:
+            result['pre_stop'] = self.pre_stop.to_map()
+        if self.post_start is not None:
+            result['post_start'] = self.post_start.to_map()
+        if self.start_up is not None:
+            result['start_up'] = self.start_up.to_map()
+        if self.entrypoint is not None:
+            result['entrypoint'] = self.entrypoint.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('liveness') is not None:
+            temp_model = ProbeConfig()
+            self.liveness = temp_model.from_map(m['liveness'])
+        if m.get('readiness') is not None:
+            temp_model = ProbeConfig()
+            self.readiness = temp_model.from_map(m['readiness'])
+        if m.get('pre_stop') is not None:
+            temp_model = ProbeConfig()
+            self.pre_stop = temp_model.from_map(m['pre_stop'])
+        if m.get('post_start') is not None:
+            temp_model = ProbeConfig()
+            self.post_start = temp_model.from_map(m['post_start'])
+        if m.get('start_up') is not None:
+            temp_model = ProbeConfig()
+            self.start_up = temp_model.from_map(m['start_up'])
+        if m.get('entrypoint') is not None:
+            temp_model = ProbeConfig()
+            self.entrypoint = temp_model.from_map(m['entrypoint'])
+        return self
+
+
+class AppEnv(TeaModel):
+    def __init__(
+        self,
+        render_value: str = None,
+        value: str = None,
+        key: str = None,
+    ):
+        # 应用部署时用于渲染的值，渲染为value
+        self.render_value = render_value
+        # 参数的值，部署的时候会被render_value的渲染结果覆盖
+        self.value = value
+        # 参数的key
+        self.key = key
+
+    def validate(self):
+        self.validate_required(self.render_value, 'render_value')
+        self.validate_required(self.value, 'value')
+        self.validate_required(self.key, 'key')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.render_value is not None:
+            result['render_value'] = self.render_value
+        if self.value is not None:
+            result['value'] = self.value
+        if self.key is not None:
+            result['key'] = self.key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('render_value') is not None:
+            self.render_value = m.get('render_value')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        return self
+
+
+class DatabaseSchema(TeaModel):
+    def __init__(
+        self,
+        dialect: str = None,
+        name: str = None,
+        topo_code: str = None,
+        sql_migrations: List[SQLMigration] = None,
+    ):
+        # 数据库方言
+        self.dialect = dialect
+        # 数据库schema名称
+        self.name = name
+        # 拓扑名称
+        self.topo_code = topo_code
+        # schema数据库变更
+        self.sql_migrations = sql_migrations
+
+    def validate(self):
+        self.validate_required(self.dialect, 'dialect')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.topo_code, 'topo_code')
+        self.validate_required(self.sql_migrations, 'sql_migrations')
+        if self.sql_migrations:
+            for k in self.sql_migrations:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dialect is not None:
+            result['dialect'] = self.dialect
+        if self.name is not None:
+            result['name'] = self.name
+        if self.topo_code is not None:
+            result['topo_code'] = self.topo_code
+        result['sql_migrations'] = []
+        if self.sql_migrations is not None:
+            for k in self.sql_migrations:
+                result['sql_migrations'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dialect') is not None:
+            self.dialect = m.get('dialect')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('topo_code') is not None:
+            self.topo_code = m.get('topo_code')
+        self.sql_migrations = []
+        if m.get('sql_migrations') is not None:
+            for k in m.get('sql_migrations'):
+                temp_model = SQLMigration()
+                self.sql_migrations.append(temp_model.from_map(k))
+        return self
+
+
+class ApplicationImage(TeaModel):
+    def __init__(
+        self,
+        arch: str = None,
+        image: str = None,
+    ):
+        # 架构:amd64，arm64
+        self.arch = arch
+        # 镜像名称
+        self.image = image
+
+    def validate(self):
+        self.validate_required(self.arch, 'arch')
+        self.validate_required(self.image, 'image')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.arch is not None:
+            result['arch'] = self.arch
+        if self.image is not None:
+            result['image'] = self.image
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('arch') is not None:
+            self.arch = m.get('arch')
+        if m.get('image') is not None:
+            self.image = m.get('image')
+        return self
+
+
+class ApplicationServiceSpec(TeaModel):
+    def __init__(
+        self,
+        domain: List[str] = None,
+        name: str = None,
+        port: int = None,
+        protocol: str = None,
+    ):
+        # 服务域名
+        self.domain = domain
+        # 服务名称
+        self.name = name
+        # 服务端口
+        self.port = port
+        # 服务协议，http，tcp
+        self.protocol = protocol
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.port, 'port')
+        self.validate_required(self.protocol, 'protocol')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.domain is not None:
+            result['domain'] = self.domain
+        if self.name is not None:
+            result['name'] = self.name
+        if self.port is not None:
+            result['port'] = self.port
+        if self.protocol is not None:
+            result['protocol'] = self.protocol
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('domain') is not None:
+            self.domain = m.get('domain')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('port') is not None:
+            self.port = m.get('port')
+        if m.get('protocol') is not None:
+            self.protocol = m.get('protocol')
+        return self
+
+
+class AppDeployInitOption(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        release_order: int = None,
+        group_strategy: str = None,
+        need_confirm: bool = None,
+    ):
+        # 应用name
+        self.name = name
+        # 产品内应用的依赖关系，决定应用的执行顺序
+        self.release_order = release_order
+        # 分组策略：
+        # TWO_GROUP("TWO_GROUP", "分两组"),
+        # ALL_ONE("ALL_ONE", "共分一组"),
+        # EACH_ONE("EACH_ONE", "每台一组"),
+        # SYSTEM_RECOMMENDATION("SYSTEM_RECOMMENDATION", "系统推荐")
+        self.group_strategy = group_strategy
+        # 分组是否需要手动确认，默认false
+        self.need_confirm = need_confirm
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.release_order, 'release_order')
+        self.validate_required(self.group_strategy, 'group_strategy')
+        self.validate_required(self.need_confirm, 'need_confirm')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.release_order is not None:
+            result['release_order'] = self.release_order
+        if self.group_strategy is not None:
+            result['group_strategy'] = self.group_strategy
+        if self.need_confirm is not None:
+            result['need_confirm'] = self.need_confirm
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('release_order') is not None:
+            self.release_order = m.get('release_order')
+        if m.get('group_strategy') is not None:
+            self.group_strategy = m.get('group_strategy')
+        if m.get('need_confirm') is not None:
+            self.need_confirm = m.get('need_confirm')
+        return self
+
+
+class OpsSpec(TeaModel):
+    def __init__(
+        self,
+        offline_pod: List[str] = None,
+        gray_release: GrayRelease = None,
+    ):
+        # 需要下线的pod列表
+        self.offline_pod = offline_pod
+        # 发布灰度策略
+        self.gray_release = gray_release
+
+    def validate(self):
+        if self.gray_release:
+            self.gray_release.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.offline_pod is not None:
+            result['offline_pod'] = self.offline_pod
+        if self.gray_release is not None:
+            result['gray_release'] = self.gray_release.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('offline_pod') is not None:
+            self.offline_pod = m.get('offline_pod')
+        if m.get('gray_release') is not None:
+            temp_model = GrayRelease()
+            self.gray_release = temp_model.from_map(m['gray_release'])
+        return self
+
+
+class ProductMeta(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        name: str = None,
+        labels: List[str] = None,
+        version: str = None,
+        group: str = None,
+    ):
+        # 产品code
+        self.code = code
+        # 产品名称
+        self.name = name
+        # 产品标签
+        self.labels = labels
+        # 产品版本
+        self.version = version
+        # 所属产品集
+        self.group = group
+
+    def validate(self):
+        self.validate_required(self.code, 'code')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.version, 'version')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['code'] = self.code
+        if self.name is not None:
+            result['name'] = self.name
+        if self.labels is not None:
+            result['labels'] = self.labels
+        if self.version is not None:
+            result['version'] = self.version
+        if self.group is not None:
+            result['group'] = self.group
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('labels') is not None:
+            self.labels = m.get('labels')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('group') is not None:
+            self.group = m.get('group')
+        return self
+
+
 class EnvInfo(TeaModel):
     def __init__(
         self,
         name: str = None,
         display_name: str = None,
         tenant_id: str = None,
         type: str = None,
@@ -3631,66 +5070,14 @@
             self.keystone_pool_name = m.get('keystone_pool_name')
         if m.get('cloud_stack_config') is not None:
             temp_model = CloudStackConfig()
             self.cloud_stack_config = temp_model.from_map(m['cloud_stack_config'])
         return self
 
 
-class LbBackendServer(TeaModel):
-    def __init__(
-        self,
-        container_name: str = None,
-        weight: int = None,
-        relation_type: str = None,
-        env_id: str = None,
-    ):
-        # 应用容器名称
-        self.container_name = container_name
-        # lb backendServer权值
-        self.weight = weight
-        # lb和backendServer关系
-        self.relation_type = relation_type
-        # 环境id
-        self.env_id = env_id
-
-    def validate(self):
-        self.validate_required(self.container_name, 'container_name')
-        self.validate_required(self.weight, 'weight')
-        self.validate_required(self.relation_type, 'relation_type')
-        self.validate_required(self.env_id, 'env_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.container_name is not None:
-            result['container_name'] = self.container_name
-        if self.weight is not None:
-            result['weight'] = self.weight
-        if self.relation_type is not None:
-            result['relation_type'] = self.relation_type
-        if self.env_id is not None:
-            result['env_id'] = self.env_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('container_name') is not None:
-            self.container_name = m.get('container_name')
-        if m.get('weight') is not None:
-            self.weight = m.get('weight')
-        if m.get('relation_type') is not None:
-            self.relation_type = m.get('relation_type')
-        if m.get('env_id') is not None:
-            self.env_id = m.get('env_id')
-        return self
-
-
 class LbListener(TeaModel):
     def __init__(
         self,
         protocol: str = None,
         listener_port: int = None,
         backend_server_port: int = None,
         backend_server_forward_port: int = None,
@@ -4110,101 +5497,160 @@
         if m.get('deployment_unit_identity') is not None:
             self.deployment_unit_identity = m.get('deployment_unit_identity')
         if m.get('deployment_unit_instance_identity') is not None:
             self.deployment_unit_instance_identity = m.get('deployment_unit_instance_identity')
         return self
 
 
-class AppInstance(TeaModel):
+class ApplicationInstance(TeaModel):
     def __init__(
         self,
-        env_id: str = None,
-        prod_code: str = None,
-        app_name: str = None,
+        name: str = None,
         app_version: str = None,
+        namespace: str = None,
+        storage_class: str = None,
+        topology_constraints: TopologyConstraints = None,
+        lifecycle: Lifecycle = None,
+        app_envs: List[AppEnv] = None,
+        application_dependencies: List[str] = None,
+        resource_spec: ResourceSpec = None,
+        persistent_volume_configs: List[PersistentVolumeConfig] = None,
+        ops_spec: OpsSpec = None,
+        pod_management_policy: str = None,
         image: str = None,
-        status: str = None,
-        deployment_unit_identity: str = None,
-        deployment_unit_instance_identity: str = None,
-        expect_replica: str = None,
     ):
-        # 环境id
-        self.env_id = env_id
-        # 产品码
-        self.prod_code = prod_code
-        # 应用名称
-        self.app_name = app_name
+        # 应用实例的名字，一般为应用code的小写字母
+        self.name = name
         # 应用版本
         self.app_version = app_version
-        # 应用镜像名
+        # 应用实例的命名空间，一般：站点code-prodCode小写
+        self.namespace = namespace
+        # 一般为空，系统自动填充默认值
+        self.storage_class = storage_class
+        # 应用部署的拓扑约束，一般为：亲和性、反亲和性、sidecar等
+        self.topology_constraints = topology_constraints
+        # 健康检查、hook配置
+        self.lifecycle = lifecycle
+        # 应用的环境变量
+        self.app_envs = app_envs
+        # 依赖的应用名列表
+        self.application_dependencies = application_dependencies
+        # 应用的规格
+        self.resource_spec = resource_spec
+        # 持久化存储，可为空数组
+        self.persistent_volume_configs = persistent_volume_configs
+        # 运维策略
+        self.ops_spec = ops_spec
+        # OrderedReady:顺序更新，Parallel：并行更新
+        self.pod_management_policy = pod_management_policy
+        # 镜像
         self.image = image
-        # 应用基线状态：ACTIVE、FAILED、UPGRADING
-        self.status = status
-        # 部署单元标识id
-        self.deployment_unit_identity = deployment_unit_identity
-        # 部署单元实例id
-        self.deployment_unit_instance_identity = deployment_unit_instance_identity
-        # 应用期望实例数
-        self.expect_replica = expect_replica
 
     def validate(self):
-        self.validate_required(self.env_id, 'env_id')
-        self.validate_required(self.prod_code, 'prod_code')
-        self.validate_required(self.app_name, 'app_name')
+        self.validate_required(self.name, 'name')
         self.validate_required(self.app_version, 'app_version')
+        self.validate_required(self.namespace, 'namespace')
+        if self.topology_constraints:
+            self.topology_constraints.validate()
+        if self.lifecycle:
+            self.lifecycle.validate()
+        if self.app_envs:
+            for k in self.app_envs:
+                if k:
+                    k.validate()
+        self.validate_required(self.resource_spec, 'resource_spec')
+        if self.resource_spec:
+            self.resource_spec.validate()
+        self.validate_required(self.persistent_volume_configs, 'persistent_volume_configs')
+        if self.persistent_volume_configs:
+            for k in self.persistent_volume_configs:
+                if k:
+                    k.validate()
+        self.validate_required(self.ops_spec, 'ops_spec')
+        if self.ops_spec:
+            self.ops_spec.validate()
+        self.validate_required(self.pod_management_policy, 'pod_management_policy')
         self.validate_required(self.image, 'image')
-        self.validate_required(self.status, 'status')
-        self.validate_required(self.expect_replica, 'expect_replica')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.env_id is not None:
-            result['env_id'] = self.env_id
-        if self.prod_code is not None:
-            result['prod_code'] = self.prod_code
-        if self.app_name is not None:
-            result['app_name'] = self.app_name
+        if self.name is not None:
+            result['name'] = self.name
         if self.app_version is not None:
             result['app_version'] = self.app_version
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.storage_class is not None:
+            result['storage_class'] = self.storage_class
+        if self.topology_constraints is not None:
+            result['topology_constraints'] = self.topology_constraints.to_map()
+        if self.lifecycle is not None:
+            result['lifecycle'] = self.lifecycle.to_map()
+        result['app_envs'] = []
+        if self.app_envs is not None:
+            for k in self.app_envs:
+                result['app_envs'].append(k.to_map() if k else None)
+        if self.application_dependencies is not None:
+            result['application_dependencies'] = self.application_dependencies
+        if self.resource_spec is not None:
+            result['resource_spec'] = self.resource_spec.to_map()
+        result['persistent_volume_configs'] = []
+        if self.persistent_volume_configs is not None:
+            for k in self.persistent_volume_configs:
+                result['persistent_volume_configs'].append(k.to_map() if k else None)
+        if self.ops_spec is not None:
+            result['ops_spec'] = self.ops_spec.to_map()
+        if self.pod_management_policy is not None:
+            result['pod_management_policy'] = self.pod_management_policy
         if self.image is not None:
             result['image'] = self.image
-        if self.status is not None:
-            result['status'] = self.status
-        if self.deployment_unit_identity is not None:
-            result['deployment_unit_identity'] = self.deployment_unit_identity
-        if self.deployment_unit_instance_identity is not None:
-            result['deployment_unit_instance_identity'] = self.deployment_unit_instance_identity
-        if self.expect_replica is not None:
-            result['expect_replica'] = self.expect_replica
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('env_id') is not None:
-            self.env_id = m.get('env_id')
-        if m.get('prod_code') is not None:
-            self.prod_code = m.get('prod_code')
-        if m.get('app_name') is not None:
-            self.app_name = m.get('app_name')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         if m.get('app_version') is not None:
             self.app_version = m.get('app_version')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('storage_class') is not None:
+            self.storage_class = m.get('storage_class')
+        if m.get('topology_constraints') is not None:
+            temp_model = TopologyConstraints()
+            self.topology_constraints = temp_model.from_map(m['topology_constraints'])
+        if m.get('lifecycle') is not None:
+            temp_model = Lifecycle()
+            self.lifecycle = temp_model.from_map(m['lifecycle'])
+        self.app_envs = []
+        if m.get('app_envs') is not None:
+            for k in m.get('app_envs'):
+                temp_model = AppEnv()
+                self.app_envs.append(temp_model.from_map(k))
+        if m.get('application_dependencies') is not None:
+            self.application_dependencies = m.get('application_dependencies')
+        if m.get('resource_spec') is not None:
+            temp_model = ResourceSpec()
+            self.resource_spec = temp_model.from_map(m['resource_spec'])
+        self.persistent_volume_configs = []
+        if m.get('persistent_volume_configs') is not None:
+            for k in m.get('persistent_volume_configs'):
+                temp_model = PersistentVolumeConfig()
+                self.persistent_volume_configs.append(temp_model.from_map(k))
+        if m.get('ops_spec') is not None:
+            temp_model = OpsSpec()
+            self.ops_spec = temp_model.from_map(m['ops_spec'])
+        if m.get('pod_management_policy') is not None:
+            self.pod_management_policy = m.get('pod_management_policy')
         if m.get('image') is not None:
             self.image = m.get('image')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('deployment_unit_identity') is not None:
-            self.deployment_unit_identity = m.get('deployment_unit_identity')
-        if m.get('deployment_unit_instance_identity') is not None:
-            self.deployment_unit_instance_identity = m.get('deployment_unit_instance_identity')
-        if m.get('expect_replica') is not None:
-            self.expect_replica = m.get('expect_replica')
         return self
 
 
 class ContainerInstance(TeaModel):
     def __init__(
         self,
         resource_id: str = None,
@@ -4328,14 +5774,448 @@
         if m.get('deployment_unit_instance_identity') is not None:
             self.deployment_unit_instance_identity = m.get('deployment_unit_instance_identity')
         if m.get('deployment_unit_identity') is not None:
             self.deployment_unit_identity = m.get('deployment_unit_identity')
         return self
 
 
+class ApplicationMeta(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        code: str = None,
+        version: str = None,
+        product_code: str = None,
+        dependencies: List[str] = None,
+        kind: str = None,
+    ):
+        # 产品名称
+        self.name = name
+        # 应用code
+        self.code = code
+        # 应用版本
+        self.version = version
+        # 所属产品code
+        self.product_code = product_code
+        # 应用之间的依赖
+        self.dependencies = dependencies
+        # 应用类型    STANDARD("standard"),
+        # JOB("job"),
+        # SIDECAR("sidecar"),
+        # DAEMON("daemon");
+        self.kind = kind
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.code, 'code')
+        self.validate_required(self.version, 'version')
+        self.validate_required(self.product_code, 'product_code')
+        self.validate_required(self.kind, 'kind')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.code is not None:
+            result['code'] = self.code
+        if self.version is not None:
+            result['version'] = self.version
+        if self.product_code is not None:
+            result['product_code'] = self.product_code
+        if self.dependencies is not None:
+            result['dependencies'] = self.dependencies
+        if self.kind is not None:
+            result['kind'] = self.kind
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('product_code') is not None:
+            self.product_code = m.get('product_code')
+        if m.get('dependencies') is not None:
+            self.dependencies = m.get('dependencies')
+        if m.get('kind') is not None:
+            self.kind = m.get('kind')
+        return self
+
+
+class AppInstance(TeaModel):
+    def __init__(
+        self,
+        env_id: str = None,
+        prod_code: str = None,
+        app_name: str = None,
+        app_version: str = None,
+        image: str = None,
+        status: str = None,
+        deployment_unit_identity: str = None,
+        deployment_unit_instance_identity: str = None,
+        expect_replica: str = None,
+    ):
+        # 环境id
+        self.env_id = env_id
+        # 产品码
+        self.prod_code = prod_code
+        # 应用名称
+        self.app_name = app_name
+        # 应用版本
+        self.app_version = app_version
+        # 应用镜像名
+        self.image = image
+        # 应用基线状态：ACTIVE、FAILED、UPGRADING
+        self.status = status
+        # 部署单元标识id
+        self.deployment_unit_identity = deployment_unit_identity
+        # 部署单元实例id
+        self.deployment_unit_instance_identity = deployment_unit_instance_identity
+        # 应用期望实例数
+        self.expect_replica = expect_replica
+
+    def validate(self):
+        self.validate_required(self.env_id, 'env_id')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.app_name, 'app_name')
+        self.validate_required(self.app_version, 'app_version')
+        self.validate_required(self.image, 'image')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.expect_replica, 'expect_replica')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.env_id is not None:
+            result['env_id'] = self.env_id
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.app_name is not None:
+            result['app_name'] = self.app_name
+        if self.app_version is not None:
+            result['app_version'] = self.app_version
+        if self.image is not None:
+            result['image'] = self.image
+        if self.status is not None:
+            result['status'] = self.status
+        if self.deployment_unit_identity is not None:
+            result['deployment_unit_identity'] = self.deployment_unit_identity
+        if self.deployment_unit_instance_identity is not None:
+            result['deployment_unit_instance_identity'] = self.deployment_unit_instance_identity
+        if self.expect_replica is not None:
+            result['expect_replica'] = self.expect_replica
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('env_id') is not None:
+            self.env_id = m.get('env_id')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('app_name') is not None:
+            self.app_name = m.get('app_name')
+        if m.get('app_version') is not None:
+            self.app_version = m.get('app_version')
+        if m.get('image') is not None:
+            self.image = m.get('image')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('deployment_unit_identity') is not None:
+            self.deployment_unit_identity = m.get('deployment_unit_identity')
+        if m.get('deployment_unit_instance_identity') is not None:
+            self.deployment_unit_instance_identity = m.get('deployment_unit_instance_identity')
+        if m.get('expect_replica') is not None:
+            self.expect_replica = m.get('expect_replica')
+        return self
+
+
+class SiteInfo(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        code: str = None,
+    ):
+        # 站点名称
+        self.name = name
+        # 站点code
+        self.code = code
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.code, 'code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.code is not None:
+            result['code'] = self.code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        return self
+
+
+class LbBackendServer(TeaModel):
+    def __init__(
+        self,
+        container_name: str = None,
+        weight: int = None,
+        relation_type: str = None,
+        env_id: str = None,
+    ):
+        # 应用容器名称
+        self.container_name = container_name
+        # lb backendServer权值
+        self.weight = weight
+        # lb和backendServer关系
+        self.relation_type = relation_type
+        # 环境id
+        self.env_id = env_id
+
+    def validate(self):
+        self.validate_required(self.container_name, 'container_name')
+        self.validate_required(self.weight, 'weight')
+        self.validate_required(self.relation_type, 'relation_type')
+        self.validate_required(self.env_id, 'env_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.container_name is not None:
+            result['container_name'] = self.container_name
+        if self.weight is not None:
+            result['weight'] = self.weight
+        if self.relation_type is not None:
+            result['relation_type'] = self.relation_type
+        if self.env_id is not None:
+            result['env_id'] = self.env_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('container_name') is not None:
+            self.container_name = m.get('container_name')
+        if m.get('weight') is not None:
+            self.weight = m.get('weight')
+        if m.get('relation_type') is not None:
+            self.relation_type = m.get('relation_type')
+        if m.get('env_id') is not None:
+            self.env_id = m.get('env_id')
+        return self
+
+
+class ProductDeployInitOption(TeaModel):
+    def __init__(
+        self,
+        namespace: str = None,
+        name: str = None,
+        prod_code: str = None,
+        site_code: str = None,
+        release_order: int = None,
+        apps: List[AppDeployInitOption] = None,
+    ):
+        # 命名空间
+        self.namespace = namespace
+        # 产品实例名称
+        self.name = name
+        # 产品code
+        self.prod_code = prod_code
+        # 站点code
+        self.site_code = site_code
+        # 多个产品实例时，本产品的发布顺序
+        self.release_order = release_order
+        # 产品内应用分部署配置
+        self.apps = apps
+
+    def validate(self):
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.release_order, 'release_order')
+        self.validate_required(self.apps, 'apps')
+        if self.apps:
+            for k in self.apps:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.name is not None:
+            result['name'] = self.name
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.release_order is not None:
+            result['release_order'] = self.release_order
+        result['apps'] = []
+        if self.apps is not None:
+            for k in self.apps:
+                result['apps'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('release_order') is not None:
+            self.release_order = m.get('release_order')
+        self.apps = []
+        if m.get('apps') is not None:
+            for k in m.get('apps'):
+                temp_model = AppDeployInitOption()
+                self.apps.append(temp_model.from_map(k))
+        return self
+
+
+class ProductDeployInitOptionRequest(TeaModel):
+    def __init__(
+        self,
+        site_code: str = None,
+        product_instances: List[ProductInstanceMeta] = None,
+    ):
+        # 站点code
+        self.site_code = site_code
+        # 需要部署的产品实例元数据
+        self.product_instances = product_instances
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.product_instances, 'product_instances')
+        if self.product_instances:
+            for k in self.product_instances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        result['product_instances'] = []
+        if self.product_instances is not None:
+            for k in self.product_instances:
+                result['product_instances'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        self.product_instances = []
+        if m.get('product_instances') is not None:
+            for k in m.get('product_instances'):
+                temp_model = ProductInstanceMeta()
+                self.product_instances.append(temp_model.from_map(k))
+        return self
+
+
+class Product(TeaModel):
+    def __init__(
+        self,
+        database: List[DatabaseSchema] = None,
+        meta: ProductMeta = None,
+        parameters: List[Parameter] = None,
+    ):
+        # 数据库变更
+        self.database = database
+        # 产品元信息
+        self.meta = meta
+        # 产品共享参数
+        self.parameters = parameters
+
+    def validate(self):
+        self.validate_required(self.database, 'database')
+        if self.database:
+            for k in self.database:
+                if k:
+                    k.validate()
+        self.validate_required(self.meta, 'meta')
+        if self.meta:
+            self.meta.validate()
+        if self.parameters:
+            for k in self.parameters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['database'] = []
+        if self.database is not None:
+            for k in self.database:
+                result['database'].append(k.to_map() if k else None)
+        if self.meta is not None:
+            result['meta'] = self.meta.to_map()
+        result['parameters'] = []
+        if self.parameters is not None:
+            for k in self.parameters:
+                result['parameters'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.database = []
+        if m.get('database') is not None:
+            for k in m.get('database'):
+                temp_model = DatabaseSchema()
+                self.database.append(temp_model.from_map(k))
+        if m.get('meta') is not None:
+            temp_model = ProductMeta()
+            self.meta = temp_model.from_map(m['meta'])
+        self.parameters = []
+        if m.get('parameters') is not None:
+            for k in m.get('parameters'):
+                temp_model = Parameter()
+                self.parameters.append(temp_model.from_map(k))
+        return self
+
+
 class ProdMetaInfo(TeaModel):
     def __init__(
         self,
         env_id: str = None,
         prod_code: str = None,
         prod_version: str = None,
         deploy_topology_identity: str = None,
@@ -7372,14 +9252,15 @@
         prod_code: str = None,
         solution_id: str = None,
         force: bool = None,
         need_beta: bool = None,
         group_strategy: str = None,
         submitter_id: str = None,
         submitter_name: str = None,
+        auto_confirm_plan: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 应用码
         self.apps = apps
         # 将要发布的单元id
@@ -7395,14 +9276,17 @@
         # TWO_GROUP分两组ALL_ONE共分一组无灰生产禁用EACH_ONE每台一组SYSTEM_RECOMMENDATION系统推荐
         self.group_strategy = group_strategy
         # 操作人ID
         self.submitter_id = submitter_id
         # 
         # 操作人名称（花名或者真名）
         self.submitter_name = submitter_name
+        # 是否由云游自动确认资源规划，默认false；
+        # 云游自动确认规划可能不符合预期，请谨慎使用
+        self.auto_confirm_plan = auto_confirm_plan
 
     def validate(self):
         self.validate_required(self.apps, 'apps')
         self.validate_required(self.cell_ids, 'cell_ids')
         self.validate_required(self.prod_code, 'prod_code')
         self.validate_required(self.solution_id, 'solution_id')
         self.validate_required(self.force, 'force')
@@ -7431,14 +9315,16 @@
             result['need_beta'] = self.need_beta
         if self.group_strategy is not None:
             result['group_strategy'] = self.group_strategy
         if self.submitter_id is not None:
             result['submitter_id'] = self.submitter_id
         if self.submitter_name is not None:
             result['submitter_name'] = self.submitter_name
+        if self.auto_confirm_plan is not None:
+            result['auto_confirm_plan'] = self.auto_confirm_plan
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -7457,14 +9343,16 @@
             self.need_beta = m.get('need_beta')
         if m.get('group_strategy') is not None:
             self.group_strategy = m.get('group_strategy')
         if m.get('submitter_id') is not None:
             self.submitter_id = m.get('submitter_id')
         if m.get('submitter_name') is not None:
             self.submitter_name = m.get('submitter_name')
+        if m.get('auto_confirm_plan') is not None:
+            self.auto_confirm_plan = m.get('auto_confirm_plan')
         return self
 
 
 class CreateAppdeployResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -7653,33 +9541,33 @@
 class ImportSolutioninstanceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         box_data: str = None,
         env_id: str = None,
-        work_no: str = None,
-        name: str = None,
+        submitter_id: str = None,
+        submitter_name: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # com.alipay.cloud.apyunqing.boxing.model.box序列化后的结果
+        # 解决方案序列化后的结果
         self.box_data = box_data
         # 环境id
         self.env_id = env_id
-        # 工号
-        self.work_no = work_no
-        # 花名
-        self.name = name
+        # 操作人ID
+        self.submitter_id = submitter_id
+        # 操作人名称
+        self.submitter_name = submitter_name
 
     def validate(self):
         self.validate_required(self.box_data, 'box_data')
         self.validate_required(self.env_id, 'env_id')
-        self.validate_required(self.work_no, 'work_no')
+        self.validate_required(self.submitter_id, 'submitter_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -7687,50 +9575,53 @@
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.box_data is not None:
             result['box_data'] = self.box_data
         if self.env_id is not None:
             result['env_id'] = self.env_id
-        if self.work_no is not None:
-            result['work_no'] = self.work_no
-        if self.name is not None:
-            result['name'] = self.name
+        if self.submitter_id is not None:
+            result['submitter_id'] = self.submitter_id
+        if self.submitter_name is not None:
+            result['submitter_name'] = self.submitter_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('box_data') is not None:
             self.box_data = m.get('box_data')
         if m.get('env_id') is not None:
             self.env_id = m.get('env_id')
-        if m.get('work_no') is not None:
-            self.work_no = m.get('work_no')
-        if m.get('name') is not None:
-            self.name = m.get('name')
+        if m.get('submitter_id') is not None:
+            self.submitter_id = m.get('submitter_id')
+        if m.get('submitter_name') is not None:
+            self.submitter_name = m.get('submitter_name')
         return self
 
 
 class ImportSolutioninstanceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        ops_plan_id: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 发布单id
+        self.ops_plan_id = ops_plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7739,24 +9630,28 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.ops_plan_id is not None:
+            result['ops_plan_id'] = self.ops_plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('ops_plan_id') is not None:
+            self.ops_plan_id = m.get('ops_plan_id')
         return self
 
 
 class CheckSolutioninstanceImportRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -7765,15 +9660,15 @@
         box_data: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 环境id
         self.env_id = env_id
-        # com.alipay.cloud.apyunqing.boxing.model.box序列化后的结果
+        # 解决方案文件序列化后的结果
         self.box_data = box_data
 
     def validate(self):
         self.validate_required(self.env_id, 'env_id')
         self.validate_required(self.box_data, 'box_data')
 
     def to_map(self):
@@ -10737,14 +12632,2100 @@
         if m.get('deployment_unit_snapshots') is not None:
             for k in m.get('deployment_unit_snapshots'):
                 temp_model = DeploymentUnitSnapshotOP()
                 self.deployment_unit_snapshots.append(temp_model.from_map(k))
         return self
 
 
+class EnableProdAutotestRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        env_id: str = None,
+        prod_codes: List[str] = None,
+        prod_status: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 环境id
+        self.env_id = env_id
+        # 产品码
+        self.prod_codes = prod_codes
+        # READY("READY", "准备执行"), DEPLOYING("DEPLOYING", "部署中, 首次部署时的状态"),  UPGRADING("UPGRADING", "升级中, 首次部署时的状态"),      ROLL_BACKING("ROLL_BACKING", "回滚中, 包括产品回滚和应用回滚"),      ACTIVE("ACTIVE", "可用"),      FAILED("FAILED", "失败"),ROLLBACKED("ROLLBACKED", "已回滚"),APP_ROLLBACKED("APP_ROLLBACKED", "应用回滚")
+        self.prod_status = prod_status
+
+    def validate(self):
+        self.validate_required(self.env_id, 'env_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.env_id is not None:
+            result['env_id'] = self.env_id
+        if self.prod_codes is not None:
+            result['prod_codes'] = self.prod_codes
+        if self.prod_status is not None:
+            result['prod_status'] = self.prod_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('env_id') is not None:
+            self.env_id = m.get('env_id')
+        if m.get('prod_codes') is not None:
+            self.prod_codes = m.get('prod_codes')
+        if m.get('prod_status') is not None:
+            self.prod_status = m.get('prod_status')
+        return self
+
+
+class EnableProdAutotestResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        options: List[AutoTestAvailableProdOption] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否可执行测试用例结果
+        self.options = options
+
+    def validate(self):
+        if self.options:
+            for k in self.options:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['options'] = []
+        if self.options is not None:
+            for k in self.options:
+                result['options'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.options = []
+        if m.get('options') is not None:
+            for k in m.get('options'):
+                temp_model = AutoTestAvailableProdOption()
+                self.options.append(temp_model.from_map(k))
+        return self
+
+
+class QuerySystemParameterRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        env_ids: str = None,
+        types: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 环境ids
+        self.env_ids = env_ids
+        # 参数名s
+        self.types = types
+
+    def validate(self):
+        self.validate_required(self.env_ids, 'env_ids')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.env_ids is not None:
+            result['env_ids'] = self.env_ids
+        if self.types is not None:
+            result['types'] = self.types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('env_ids') is not None:
+            self.env_ids = m.get('env_ids')
+        if m.get('types') is not None:
+            self.types = m.get('types')
+        return self
+
+
+class QuerySystemParameterResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        system_parameters: List[SystemParameterInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 系统参数值
+        self.system_parameters = system_parameters
+
+    def validate(self):
+        if self.system_parameters:
+            for k in self.system_parameters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['system_parameters'] = []
+        if self.system_parameters is not None:
+            for k in self.system_parameters:
+                result['system_parameters'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.system_parameters = []
+        if m.get('system_parameters') is not None:
+            for k in m.get('system_parameters'):
+                temp_model = SystemParameterInfo()
+                self.system_parameters.append(temp_model.from_map(k))
+        return self
+
+
+class QueryOpsplanNodetreeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        ops_plan_id: str = None,
+        sub_tree_node_root_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 发布单id
+        self.ops_plan_id = ops_plan_id
+        # 发布单节点树根节点id
+        self.sub_tree_node_root_id = sub_tree_node_root_id
+
+    def validate(self):
+        self.validate_required(self.ops_plan_id, 'ops_plan_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.ops_plan_id is not None:
+            result['ops_plan_id'] = self.ops_plan_id
+        if self.sub_tree_node_root_id is not None:
+            result['sub_tree_node_root_id'] = self.sub_tree_node_root_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('ops_plan_id') is not None:
+            self.ops_plan_id = m.get('ops_plan_id')
+        if m.get('sub_tree_node_root_id') is not None:
+            self.sub_tree_node_root_id = m.get('sub_tree_node_root_id')
+        return self
+
+
+class QueryOpsplanNodetreeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        node_tree: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发布单节点树，为json string
+        self.node_tree = node_tree
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.node_tree is not None:
+            result['node_tree'] = self.node_tree
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('node_tree') is not None:
+            self.node_tree = m.get('node_tree')
+        return self
+
+
+class ListAapSitesRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class ListAapSitesResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        sites: List[SiteInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # site list
+        self.sites = sites
+
+    def validate(self):
+        if self.sites:
+            for k in self.sites:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['sites'] = []
+        if self.sites is not None:
+            for k in self.sites:
+                result['sites'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.sites = []
+        if m.get('sites') is not None:
+            for k in m.get('sites'):
+                temp_model = SiteInfo()
+                self.sites.append(temp_model.from_map(k))
+        return self
+
+
+class ImportAapMetaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        meta_context: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # yaml的string格式
+        self.meta_context = meta_context
+
+    def validate(self):
+        self.validate_required(self.meta_context, 'meta_context')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.meta_context is not None:
+            result['meta_context'] = self.meta_context
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('meta_context') is not None:
+            self.meta_context = m.get('meta_context')
+        return self
+
+
+class ImportAapMetaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否上传成功
+        self.success = success
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class InitAapProductinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        namespace: str = None,
+        name: str = None,
+        prod_code: str = None,
+        prod_version: str = None,
+        topology_code: str = None,
+        site_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 命名空间，命名格式：siteCode-prodCode （小写）
+        self.namespace = namespace
+        # 产品实例名称，推荐产品code的小写字母
+        self.name = name
+        # 产品code
+        self.prod_code = prod_code
+        # 产品版本
+        self.prod_version = prod_version
+        # 产品部署的拓扑名称，部署时会根据该信息进行部署
+        self.topology_code = topology_code
+        # 站点code
+        self.site_code = site_code
+
+    def validate(self):
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.prod_version, 'prod_version')
+        self.validate_required(self.topology_code, 'topology_code')
+        self.validate_required(self.site_code, 'site_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.name is not None:
+            result['name'] = self.name
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.prod_version is not None:
+            result['prod_version'] = self.prod_version
+        if self.topology_code is not None:
+            result['topology_code'] = self.topology_code
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('prod_version') is not None:
+            self.prod_version = m.get('prod_version')
+        if m.get('topology_code') is not None:
+            self.topology_code = m.get('topology_code')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        return self
+
+
+class InitAapProductinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class InitAapReleaseRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        product_deploy_init_option_request: ProductDeployInitOptionRequest = None,
+        site_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 需要升级的产品实例
+        self.product_deploy_init_option_request = product_deploy_init_option_request
+        # 站点code
+        self.site_code = site_code
+
+    def validate(self):
+        self.validate_required(self.product_deploy_init_option_request, 'product_deploy_init_option_request')
+        if self.product_deploy_init_option_request:
+            self.product_deploy_init_option_request.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.product_deploy_init_option_request is not None:
+            result['product_deploy_init_option_request'] = self.product_deploy_init_option_request.to_map()
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('product_deploy_init_option_request') is not None:
+            temp_model = ProductDeployInitOptionRequest()
+            self.product_deploy_init_option_request = temp_model.from_map(m['product_deploy_init_option_request'])
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        return self
+
+
+class InitAapReleaseResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        deploy_init_options: List[ProductDeployInitOption] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 初始化的结果，可用此调用发布接口
+        self.deploy_init_options = deploy_init_options
+
+    def validate(self):
+        if self.deploy_init_options:
+            for k in self.deploy_init_options:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['deploy_init_options'] = []
+        if self.deploy_init_options is not None:
+            for k in self.deploy_init_options:
+                result['deploy_init_options'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.deploy_init_options = []
+        if m.get('deploy_init_options') is not None:
+            for k in m.get('deploy_init_options'):
+                temp_model = ProductDeployInitOption()
+                self.deploy_init_options.append(temp_model.from_map(k))
+        return self
+
+
+class DeployAapProductinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        product_deploy_init_options: List[ProductDeployInitOption] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 站点code
+        self.site_code = site_code
+        # 产品部署参数
+        self.product_deploy_init_options = product_deploy_init_options
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.product_deploy_init_options, 'product_deploy_init_options')
+        if self.product_deploy_init_options:
+            for k in self.product_deploy_init_options:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        result['product_deploy_init_options'] = []
+        if self.product_deploy_init_options is not None:
+            for k in self.product_deploy_init_options:
+                result['product_deploy_init_options'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        self.product_deploy_init_options = []
+        if m.get('product_deploy_init_options') is not None:
+            for k in m.get('product_deploy_init_options'):
+                temp_model = ProductDeployInitOption()
+                self.product_deploy_init_options.append(temp_model.from_map(k))
+        return self
+
+
+class DeployAapProductinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        release_plan_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发布单id
+        self.release_plan_id = release_plan_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.release_plan_id is not None:
+            result['release_plan_id'] = self.release_plan_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('release_plan_id') is not None:
+            self.release_plan_id = m.get('release_plan_id')
+        return self
+
+
+class GetAapReleaseRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        release_plan_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 发布单id
+        self.release_plan_id = release_plan_id
+
+    def validate(self):
+        self.validate_required(self.release_plan_id, 'release_plan_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.release_plan_id is not None:
+            result['release_plan_id'] = self.release_plan_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('release_plan_id') is not None:
+            self.release_plan_id = m.get('release_plan_id')
+        return self
+
+
+class GetAapReleaseResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        status: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发布单状态:
+        # TOBE_DEPLOY("TOBE_DEPLOY","待执行","待执行"),
+        # EXECUTING("EXECUTING","执行中","执行中"),
+        # SUCCESS("SUCCESS","完成","完成"),
+        # CANCELED("CANCELED","已取消","已取消"),
+        # FAILED("FAILED","失败","失败"),
+        # WAITING_CONFIRM("WAITING_CONFIRM","待确认","待确认");
+        self.status = status
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class UpdateAapApplicationinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        application_instance: ApplicationInstance = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 站点code
+        self.site_code = site_code
+        # 应用实例
+        self.application_instance = application_instance
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.application_instance, 'application_instance')
+        if self.application_instance:
+            self.application_instance.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.application_instance is not None:
+            result['application_instance'] = self.application_instance.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('application_instance') is not None:
+            temp_model = ApplicationInstance()
+            self.application_instance = temp_model.from_map(m['application_instance'])
+        return self
+
+
+class UpdateAapApplicationinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class QueryAapApplicationinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        namespace: str = None,
+        prod_code: str = None,
+        product_instance_name: str = None,
+        app_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # sitecode
+        # 
+        self.site_code = site_code
+        # namespace
+        self.namespace = namespace
+        # 产品code
+        self.prod_code = prod_code
+        # 产品实例name
+        self.product_instance_name = product_instance_name
+        # app name
+        self.app_name = app_name
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+        self.validate_required(self.app_name, 'app_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        if self.app_name is not None:
+            result['app_name'] = self.app_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        if m.get('app_name') is not None:
+            self.app_name = m.get('app_name')
+        return self
+
+
+class QueryAapApplicationinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        site_code: str = None,
+        application_instance: ApplicationInstance = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # siteCode
+        self.site_code = site_code
+        # 应用实例
+        self.application_instance = application_instance
+
+    def validate(self):
+        if self.application_instance:
+            self.application_instance.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.application_instance is not None:
+            result['application_instance'] = self.application_instance.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('application_instance') is not None:
+            temp_model = ApplicationInstance()
+            self.application_instance = temp_model.from_map(m['application_instance'])
+        return self
+
+
+class SetAapApplicationinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        resource_spec: ResourceSpec = None,
+        namespace: str = None,
+        product_instance_name: str = None,
+        prod_code: str = None,
+        app_code: str = None,
+        site_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 规格修改
+        self.resource_spec = resource_spec
+        # 命名空间
+        self.namespace = namespace
+        # 产品实例名称
+        self.product_instance_name = product_instance_name
+        # 产品code
+        self.prod_code = prod_code
+        # 应用名称
+        self.app_code = app_code
+        # 站点code
+        self.site_code = site_code
+
+    def validate(self):
+        self.validate_required(self.resource_spec, 'resource_spec')
+        if self.resource_spec:
+            self.resource_spec.validate()
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.app_code, 'app_code')
+        self.validate_required(self.site_code, 'site_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.resource_spec is not None:
+            result['resource_spec'] = self.resource_spec.to_map()
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.app_code is not None:
+            result['app_code'] = self.app_code
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('resource_spec') is not None:
+            temp_model = ResourceSpec()
+            self.resource_spec = temp_model.from_map(m['resource_spec'])
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('app_code') is not None:
+            self.app_code = m.get('app_code')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        return self
+
+
+class SetAapApplicationinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否修改成功
+        self.success = success
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class SetAapImagesRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        images: ApplicationImage = None,
+        namespace: str = None,
+        site_code: str = None,
+        prod_code: str = None,
+        product_instance_name: str = None,
+        app_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 应用镜像，默认使用amd64
+        self.images = images
+        # namespace
+        self.namespace = namespace
+        # siteCode
+        self.site_code = site_code
+        # 产品code
+        self.prod_code = prod_code
+        # 产品实例名称
+        self.product_instance_name = product_instance_name
+        # 应用code
+        self.app_code = app_code
+
+    def validate(self):
+        self.validate_required(self.images, 'images')
+        if self.images:
+            self.images.validate()
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+        self.validate_required(self.app_code, 'app_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.images is not None:
+            result['images'] = self.images.to_map()
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        if self.app_code is not None:
+            result['app_code'] = self.app_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('images') is not None:
+            temp_model = ApplicationImage()
+            self.images = temp_model.from_map(m['images'])
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        if m.get('app_code') is not None:
+            self.app_code = m.get('app_code')
+        return self
+
+
+class SetAapImagesResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否修改成功
+        self.success = success
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class QueryAapProductinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        namespace: str = None,
+        prod_code: str = None,
+        product_instance_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # site_code
+        self.site_code = site_code
+        # name space
+        self.namespace = namespace
+        # 产品code
+        self.prod_code = prod_code
+        # 产品实例name
+        self.product_instance_name = product_instance_name
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        return self
+
+
+class QueryAapProductinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        namespace: str = None,
+        prod_code: str = None,
+        name: str = None,
+        prod_version: str = None,
+        topology_code: str = None,
+        topology_name: str = None,
+        status: str = None,
+        app_instances: List[ApplicationMeta] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # namespace
+        self.namespace = namespace
+        # prod code
+        self.prod_code = prod_code
+        # 产品实例名称
+        self.name = name
+        # 产品版本
+        self.prod_version = prod_version
+        # 拓扑code
+        self.topology_code = topology_code
+        # 拓扑名称
+        self.topology_name = topology_name
+        # 产品实例状态
+        self.status = status
+        # 应用实例列表
+        self.app_instances = app_instances
+
+    def validate(self):
+        if self.app_instances:
+            for k in self.app_instances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.name is not None:
+            result['name'] = self.name
+        if self.prod_version is not None:
+            result['prod_version'] = self.prod_version
+        if self.topology_code is not None:
+            result['topology_code'] = self.topology_code
+        if self.topology_name is not None:
+            result['topology_name'] = self.topology_name
+        if self.status is not None:
+            result['status'] = self.status
+        result['app_instances'] = []
+        if self.app_instances is not None:
+            for k in self.app_instances:
+                result['app_instances'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('prod_version') is not None:
+            self.prod_version = m.get('prod_version')
+        if m.get('topology_code') is not None:
+            self.topology_code = m.get('topology_code')
+        if m.get('topology_name') is not None:
+            self.topology_name = m.get('topology_name')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        self.app_instances = []
+        if m.get('app_instances') is not None:
+            for k in m.get('app_instances'):
+                temp_model = ApplicationMeta()
+                self.app_instances.append(temp_model.from_map(k))
+        return self
+
+
+class DetailAapApplicationinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        namespace: str = None,
+        prod_code: str = None,
+        product_instance_name: str = None,
+        app_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # site code
+        self.site_code = site_code
+        # namespace
+        self.namespace = namespace
+        # prod code
+        self.prod_code = prod_code
+        # 产品实例名称
+        self.product_instance_name = product_instance_name
+        # 应用code
+        self.app_code = app_code
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+        self.validate_required(self.app_code, 'app_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        if self.app_code is not None:
+            result['app_code'] = self.app_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        if m.get('app_code') is not None:
+            self.app_code = m.get('app_code')
+        return self
+
+
+class DetailAapApplicationinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        name: str = None,
+        image: str = None,
+        replicas: int = None,
+        pod_instances: List[ContainerInstance] = None,
+        version: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 应用名称
+        self.name = name
+        # 镜像
+        self.image = image
+        # 副本数
+        self.replicas = replicas
+        # 容器详情
+        self.pod_instances = pod_instances
+        # 应用版本
+        self.version = version
+
+    def validate(self):
+        if self.pod_instances:
+            for k in self.pod_instances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.name is not None:
+            result['name'] = self.name
+        if self.image is not None:
+            result['image'] = self.image
+        if self.replicas is not None:
+            result['replicas'] = self.replicas
+        result['pod_instances'] = []
+        if self.pod_instances is not None:
+            for k in self.pod_instances:
+                result['pod_instances'].append(k.to_map() if k else None)
+        if self.version is not None:
+            result['version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('image') is not None:
+            self.image = m.get('image')
+        if m.get('replicas') is not None:
+            self.replicas = m.get('replicas')
+        self.pod_instances = []
+        if m.get('pod_instances') is not None:
+            for k in m.get('pod_instances'):
+                temp_model = ContainerInstance()
+                self.pod_instances.append(temp_model.from_map(k))
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        return self
+
+
+class SetAapParametersRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        namespace: str = None,
+        prod_code: str = None,
+        product_instance_name: str = None,
+        app_code: str = None,
+        app_envs: List[AppEnv] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # site code
+        self.site_code = site_code
+        # namespace
+        self.namespace = namespace
+        # prod code
+        self.prod_code = prod_code
+        # product_instance_name
+        self.product_instance_name = product_instance_name
+        # 应用code
+        self.app_code = app_code
+        # 更新的应用参数
+        self.app_envs = app_envs
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+        self.validate_required(self.app_code, 'app_code')
+        self.validate_required(self.app_envs, 'app_envs')
+        if self.app_envs:
+            for k in self.app_envs:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        if self.app_code is not None:
+            result['app_code'] = self.app_code
+        result['app_envs'] = []
+        if self.app_envs is not None:
+            for k in self.app_envs:
+                result['app_envs'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        if m.get('app_code') is not None:
+            self.app_code = m.get('app_code')
+        self.app_envs = []
+        if m.get('app_envs') is not None:
+            for k in m.get('app_envs'):
+                temp_model = AppEnv()
+                self.app_envs.append(temp_model.from_map(k))
+        return self
+
+
+class SetAapParametersResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 更新是否成功
+        self.success = success
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class DeleteAapProductinstanceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        site_code: str = None,
+        namespace: str = None,
+        prod_code: str = None,
+        product_instance_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 站点code
+        self.site_code = site_code
+        # 产品实例所属命名空间
+        self.namespace = namespace
+        # 产品实例code
+        self.prod_code = prod_code
+        # 产品实例名称
+        self.product_instance_name = product_instance_name
+
+    def validate(self):
+        self.validate_required(self.site_code, 'site_code')
+        self.validate_required(self.namespace, 'namespace')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.product_instance_name, 'product_instance_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.site_code is not None:
+            result['site_code'] = self.site_code
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.product_instance_name is not None:
+            result['product_instance_name'] = self.product_instance_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('site_code') is not None:
+            self.site_code = m.get('site_code')
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('product_instance_name') is not None:
+            self.product_instance_name = m.get('product_instance_name')
+        return self
+
+
+class DeleteAapProductinstanceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class CreateEnvRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        env_config_info: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 环境初始化参数配置
+        self.env_config_info = env_config_info
+
+    def validate(self):
+        self.validate_required(self.env_config_info, 'env_config_info')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.env_config_info is not None:
+            result['env_config_info'] = self.env_config_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('env_config_info') is not None:
+            self.env_config_info = m.get('env_config_info')
+        return self
+
+
+class CreateEnvResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        env_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 环境ID
+        self.env_id = env_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.env_id is not None:
+            result['env_id'] = self.env_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('env_id') is not None:
+            self.env_id = m.get('env_id')
+        return self
+
+
 class AllEnvsRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
     ):
         # OAuth模式下的授权token
```

### Comparing `antchain_yunqing-3.14.18/antchain_yunqing.egg-info/PKG-INFO` & `antchain_yunqing-4.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-yunqing
-Version: 3.14.18
+Name: antchain_yunqing
+Version: 4.0.5
 Summary: Ant Chain YUNQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_yunqing-3.14.18/setup.py` & `antchain_yunqing-4.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_yunqing.
 
-Created on 23/08/2022
+Created on 04/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_yunqing"
 NAME = "antchain_yunqing" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain YUNQING SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

