# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.925.tar", last modified: Fri Jun 30 02:13:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.926.tar", last modified: Mon Jul  3 00:26:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.925.tar` & `tencentcloud-sdk-python-essbasic-3.0.926.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240706 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)    52742 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:13:57.000000 tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/essbasic_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)   241947 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52742 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:26:28.000000 tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1381,22 +1381,25 @@
         :type ReleasedApprovers: list of ReleasedApprover
         :param CallbackUrl: 签署完回调url，最大长度1000个字符
         :type CallbackUrl: str
         :param Organization: 暂未开放
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
         :param Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
+        :param Deadline: 签署流程的签署截止时间。 值为unix时间戳,精确到秒,不传默认为当前时间七天后
+        :type Deadline: int
         """
         self.Agent = None
         self.NeedRelievedFlowId = None
         self.ReliveInfo = None
         self.ReleasedApprovers = None
         self.CallbackUrl = None
         self.Organization = None
         self.Operator = None
+        self.Deadline = None
 
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.NeedRelievedFlowId = params.get("NeedRelievedFlowId")
@@ -1412,14 +1415,15 @@
         self.CallbackUrl = params.get("CallbackUrl")
         if params.get("Organization") is not None:
             self.Organization = OrganizationInfo()
             self.Organization._deserialize(params.get("Organization"))
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
+        self.Deadline = params.get("Deadline")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5136,14 +5140,16 @@
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ReleasedApprover(AbstractModel):
     """解除协议的签署人，如不指定，默认使用待解除流程（即原流程）中的签署人。
     注意：不支持更换C端（个人身份类型）签署人，如果原流程中含有C端签署人，默认使用原流程中的该签署人。
+    注意：目前不支持替换C端（个人身份类型）签署人，但是可以指定C端签署人的签署方自定义控件别名，具体见参数ApproverSignRole描述。
+    注意：当指定C端签署人的签署方自定义控件别名不空时，除参数ApproverNumber外，可以只参数ApproverSignRole。
 
     如果需要指定B端（机构身份类型）签署人，其中ReleasedApprover需要传递的参数如下：
     ApproverNumber, OrganizationName, ApproverType必传。
     对于其他身份标识
     - 子客企业指定经办人：OpenId必传，OrganizationOpenId必传；
     - 非子客企业：Name、Mobile必传。
 
@@ -5171,36 +5177,46 @@
         :param Mobile: 签署人手机号，脱敏显示。大陆手机号为11位，暂不支持海外手机号
         :type Mobile: str
         :param OrganizationOpenId: 企业签署方在同一第三方应用下的其他合作企业OpenId，签署方为非发起方企业场景下必传，最大长度64个字符
         :type OrganizationOpenId: str
         :param OpenId: 用户侧第三方id，最大长度64个字符
 当签署方为同一第三方应用下的员工时，该字必传
         :type OpenId: str
+        :param ApproverSignComponentType: 签署控件类型，支持自定义企业签署方的签署控件为“印章”或“签名”
+- SIGN_SEAL-默认为印章控件类型
+- SIGN_SIGNATURE-手写签名控件类型
+        :type ApproverSignComponentType: str
+        :param ApproverSignRole: 签署方自定义控件别名，最大长度20个字符
+        :type ApproverSignRole: str
         """
         self.OrganizationName = None
         self.ApproverNumber = None
         self.ApproverType = None
         self.Name = None
         self.IdCardType = None
         self.IdCardNumber = None
         self.Mobile = None
         self.OrganizationOpenId = None
         self.OpenId = None
+        self.ApproverSignComponentType = None
+        self.ApproverSignRole = None
 
 
     def _deserialize(self, params):
         self.OrganizationName = params.get("OrganizationName")
         self.ApproverNumber = params.get("ApproverNumber")
         self.ApproverType = params.get("ApproverType")
         self.Name = params.get("Name")
         self.IdCardType = params.get("IdCardType")
         self.IdCardNumber = params.get("IdCardNumber")
         self.Mobile = params.get("Mobile")
         self.OrganizationOpenId = params.get("OrganizationOpenId")
         self.OpenId = params.get("OpenId")
+        self.ApproverSignComponentType = params.get("ApproverSignComponentType")
+        self.ApproverSignRole = params.get("ApproverSignRole")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5914,15 +5930,15 @@
 class UploadFilesRequest(AbstractModel):
     """UploadFiles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Agent: 应用相关信息，若是第三方应用集成调用 appid 和proxyappid 必填
+        :param Agent: 应用相关信息，若是第三方应用集成调用 若是第三方应用集成调用,Agent.AppId 和 Agent.ProxyOrganizationOpenId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param BusinessType: 文件对应业务类型
 1. TEMPLATE - 模板； 文件类型：.pdf/.doc/.docx/.html
 2. DOCUMENT - 签署过程及签署后的合同文档/图片控件 文件类型：.pdf/.doc/.docx/.jpg/.png/.xls.xlsx/.html
         :type BusinessType: str
         :param FileInfos: 上传文件内容数组，最多支持20个文件
         :type FileInfos: list of UploadFile
@@ -5961,32 +5977,32 @@
 class UploadFilesResponse(AbstractModel):
     """UploadFiles返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FileIds: 文件id数组，有效期一个小时；有效期内此文件id可以反复使用
-        :type FileIds: list of str
         :param TotalCount: 上传成功文件数量
         :type TotalCount: int
+        :param FileIds: 文件id数组，有效期一个小时；有效期内此文件id可以反复使用
+        :type FileIds: list of str
         :param FileUrls: 文件Url
         :type FileUrls: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.FileIds = None
         self.TotalCount = None
+        self.FileIds = None
         self.FileUrls = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
-        self.FileIds = params.get("FileIds")
         self.TotalCount = params.get("TotalCount")
+        self.FileIds = params.get("FileIds")
         self.FileUrls = params.get("FileUrls")
         self.RequestId = params.get("RequestId")
 
 
 class UsageDetail(AbstractModel):
     """用量明细
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.926/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.926/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.925/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.926/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

