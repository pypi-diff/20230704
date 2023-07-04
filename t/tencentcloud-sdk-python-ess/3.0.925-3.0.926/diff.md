# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.925.tar", last modified: Fri Jun 30 02:13:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.926.tar", last modified: Mon Jul  3 00:26:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.925.tar` & `tencentcloud-sdk-python-ess-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260887 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)    59451 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24834 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)   262079 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    59451 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:21.000000 tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/__init__.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2330,19 +2330,22 @@
         :type NeedRelievedFlowId: str
         :param ReliveInfo: 解除协议内容
         :type ReliveInfo: :class:`tencentcloud.ess.v20201111.models.RelieveInfo`
         :param ReleasedApprovers: 非必须，解除协议的本企业签署人列表，
 默认使用原流程的签署人列表,当解除协议的签署人与原流程的签署人不能相同时（例如原流程签署人离职了），需要指定本企业其他已实名员工来替换原流程中的原签署人，注意需要指明原签署人的编号(ReceiptId,通过DescribeFlowInfo接口获取)来代表需要替换哪一个签署人
 解除协议的签署人数量不能多于原流程的签署人数量
         :type ReleasedApprovers: list of ReleasedApprover
+        :param Deadline: 签署流程的签署截止时间。 值为unix时间戳,精确到秒,不传默认为当前时间七天后
+        :type Deadline: int
         """
         self.Operator = None
         self.NeedRelievedFlowId = None
         self.ReliveInfo = None
         self.ReleasedApprovers = None
+        self.Deadline = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.NeedRelievedFlowId = params.get("NeedRelievedFlowId")
@@ -2351,14 +2354,15 @@
             self.ReliveInfo._deserialize(params.get("ReliveInfo"))
         if params.get("ReleasedApprovers") is not None:
             self.ReleasedApprovers = []
             for item in params.get("ReleasedApprovers"):
                 obj = ReleasedApprover()
                 obj._deserialize(item)
                 self.ReleasedApprovers.append(obj)
+        self.Deadline = params.get("Deadline")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5969,14 +5973,16 @@
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ReleasedApprover(AbstractModel):
     """解除协议的签署人，如不指定，默认使用待解除流程（即原流程）中的签署人。
     注意：不支持更换C端（个人身份类型）签署人，如果原流程中含有C端签署人，默认使用原流程中的该C端签署人。
+    注意：目前不支持替换C端（个人身份类型）签署人，但是可以指定C端签署人的签署方自定义控件别名，具体见参数ApproverSignRole描述。
+    注意：当指定C端签署人的签署方自定义控件别名不空时，除RelievedApproverReceiptId参数外，可以只参数ApproverSignRole。
 
     """
 
     def __init__(self):
         r"""
         :param Name: 签署人姓名，最大长度50个字符
 
@@ -5985,26 +5991,36 @@
         :type Mobile: str
         :param RelievedApproverReceiptId: 要替换的参与人在原合同参与人列表中的签署人编号,通过DescribeFlowInfo 接口获取（即FlowDetailInfos. FlowApproverInfos 结构中的ReceiptId ）
         :type RelievedApproverReceiptId: str
         :param ApproverType: 指定签署人类型，目前仅支持
 ORGANIZATION-企业
 ENTERPRISESERVER-企业静默签
         :type ApproverType: str
+        :param ApproverSignComponentType: 签署控件类型，支持自定义企业签署方的签署控件为“印章”或“签名”
+- SIGN_SEAL-默认为印章控件类型
+- SIGN_SIGNATURE-手写签名控件类型
+        :type ApproverSignComponentType: str
+        :param ApproverSignRole: 签署方自定义控件别名，最大长度20个字符
+        :type ApproverSignRole: str
         """
         self.Name = None
         self.Mobile = None
         self.RelievedApproverReceiptId = None
         self.ApproverType = None
+        self.ApproverSignComponentType = None
+        self.ApproverSignRole = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Mobile = params.get("Mobile")
         self.RelievedApproverReceiptId = params.get("RelievedApproverReceiptId")
         self.ApproverType = params.get("ApproverType")
+        self.ApproverSignComponentType = params.get("ApproverSignComponentType")
+        self.ApproverSignRole = params.get("ApproverSignRole")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.926/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.925/README.rst` & `tencentcloud-sdk-python-ess-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.926/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.925/setup.py` & `tencentcloud-sdk-python-ess-3.0.926/setup.py`

 * *Files identical despite different names*

