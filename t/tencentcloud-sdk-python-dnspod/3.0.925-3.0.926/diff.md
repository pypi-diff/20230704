# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.925.tar", last modified: Fri Jun 30 02:06:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.926.tar", last modified: Mon Jul  3 00:24:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.925.tar` & `tencentcloud-sdk-python-dnspod-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   209870 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    59836 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)    23664 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-30 02:06:01.000000 tencentcloud-sdk-python-dnspod-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)   212878 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    23664 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60713 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:24:51.000000 tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/__init__.py
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.925'
+__version__ = '3.0.926'
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1339,14 +1339,113 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteRecordBatchDetail(AbstractModel):
+    """批量删除记录详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DomainId: 域名 ID
+        :type DomainId: int
+        :param Domain: 域名
+        :type Domain: str
+        :param Error: 错误信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Error: str
+        :param Status: 删除状态
+        :type Status: str
+        :param Operation: 操作
+        :type Operation: str
+        :param RecordList: 解析记录列表，json 序列化之后的字符串形式
+        :type RecordList: str
+        """
+        self.DomainId = None
+        self.Domain = None
+        self.Error = None
+        self.Status = None
+        self.Operation = None
+        self.RecordList = None
+
+
+    def _deserialize(self, params):
+        self.DomainId = params.get("DomainId")
+        self.Domain = params.get("Domain")
+        self.Error = params.get("Error")
+        self.Status = params.get("Status")
+        self.Operation = params.get("Operation")
+        self.RecordList = params.get("RecordList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteRecordBatchRequest(AbstractModel):
+    """DeleteRecordBatch请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RecordIdList: 解析记录 ID 数组
+        :type RecordIdList: list of int non-negative
+        """
+        self.RecordIdList = None
+
+
+    def _deserialize(self, params):
+        self.RecordIdList = params.get("RecordIdList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteRecordBatchResponse(AbstractModel):
+    """DeleteRecordBatch返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param JobId: 批量任务 ID
+        :type JobId: int
+        :param DetailList: 任务详情
+        :type DetailList: list of DeleteRecordBatchDetail
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.JobId = None
+        self.DetailList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.JobId = params.get("JobId")
+        if params.get("DetailList") is not None:
+            self.DetailList = []
+            for item in params.get("DetailList"):
+                obj = DeleteRecordBatchDetail()
+                obj._deserialize(item)
+                self.DetailList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteRecordGroupRequest(AbstractModel):
     """DeleteRecordGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,14 +367,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteRecordBatch(self, request):
+        """批量删除解析记录
+
+        :param request: Request instance for DeleteRecordBatch.
+        :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordBatchRequest`
+        :rtype: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordBatchResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteRecordBatch", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteRecordBatchResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteRecordGroup(self, request):
         """删除记录分组
 
         :param request: Request instance for DeleteRecordGroup.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordGroupRequest`
         :rtype: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordGroupResponse`
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.926/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.925/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.926/setup.py`

 * *Files identical despite different names*

