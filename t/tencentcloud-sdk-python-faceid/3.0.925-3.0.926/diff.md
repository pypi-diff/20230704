# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.925.tar", last modified: Fri Jun 30 02:14:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.926.tar", last modified: Mon Jul  3 00:26:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.925.tar` & `tencentcloud-sdk-python-faceid-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   141706 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)    34030 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-30 02:14:08.000000 tencentcloud-sdk-python-faceid-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)   141598 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)    34030 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:26:44.000000 tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         :param IdCard: 开户证件号，与CertType参数的证件类型一致，如：身份证，则传入身份证号。
         :type IdCard: str
         :param Name: 姓名
         :type Name: str
         :param BankCard: 银行卡
         :type BankCard: str
         :param CertType: 证件类型，请确认该证件为开户时使用的证件类型，未用于开户的证件信息不支持验证。
-目前默认：0 身份证，其他证件类型需求可以添加[腾讯云人脸核身小助手](https://cloud.tencent.com/document/product/1007/56130)进行确认。
+目前默认：0 身份证，其他证件类型暂不支持。
         :type CertType: int
         :param Encryption: 敏感数据加密信息。对传入信息（姓名、身份证号、银行卡号）有加密需求的用户可使用此参数，详情请点击左侧链接。
         :type Encryption: :class:`tencentcloud.faceid.v20180301.models.Encryption`
         """
         self.IdCard = None
         self.Name = None
         self.BankCard = None
@@ -1755,15 +1755,15 @@
         if params.get("IntentionQuestionResult") is not None:
             self.IntentionQuestionResult = IntentionQuestionResult()
             self.IntentionQuestionResult._deserialize(params.get("IntentionQuestionResult"))
         self.RequestId = params.get("RequestId")
 
 
 class GetEidTokenConfig(AbstractModel):
-    """获取token时的的配置
+    """获取token时的配置
 
     """
 
     def __init__(self):
         r"""
         :param InputType: 姓名身份证输入方式。
 1：传身份证正反面OCR
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.926/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/README.rst` & `tencentcloud-sdk-python-faceid-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.926/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.926/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.925/setup.py` & `tencentcloud-sdk-python-faceid-3.0.926/setup.py`

 * *Files identical despite different names*

