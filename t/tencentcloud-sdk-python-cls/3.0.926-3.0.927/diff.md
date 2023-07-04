# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.926.tar", last modified: Mon Jul  3 00:22:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.927.tar", last modified: Tue Jul  4 00:18:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.926.tar` & `tencentcloud-sdk-python-cls-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)   256323 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)     8715 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67916 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:49.000000 tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    73424 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)   283954 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:18:27.000000 tencentcloud-sdk-python-cls-3.0.927/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-cls-3.0.926/setup.py` & `tencentcloud-sdk-python-cls-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.926/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.927/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.926/README.rst` & `tencentcloud-sdk-python-cls-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.927/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.927/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.926'
+__version__ = '3.0.927'
```

### Comparing `tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -596,14 +596,78 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CheckRechargeKafkaServerRequest(AbstractModel):
+    """CheckRechargeKafkaServer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param KafkaType: 导入Kafka类型，0: 腾讯云CKafka，1: 用户自建Kafka
+        :type KafkaType: int
+        :param KafkaInstance: 腾讯云CKafka实例ID，KafkaType为0时必填
+        :type KafkaInstance: str
+        :param ServerAddr: 服务地址
+        :type ServerAddr: str
+        :param IsEncryptionAddr: ServerAddr是否为加密连接
+        :type IsEncryptionAddr: bool
+        :param Protocol: 加密访问协议，IsEncryptionAddr参数为true时必填
+        :type Protocol: :class:`tencentcloud.cls.v20201016.models.KafkaProtocolInfo`
+        """
+        self.KafkaType = None
+        self.KafkaInstance = None
+        self.ServerAddr = None
+        self.IsEncryptionAddr = None
+        self.Protocol = None
+
+
+    def _deserialize(self, params):
+        self.KafkaType = params.get("KafkaType")
+        self.KafkaInstance = params.get("KafkaInstance")
+        self.ServerAddr = params.get("ServerAddr")
+        self.IsEncryptionAddr = params.get("IsEncryptionAddr")
+        if params.get("Protocol") is not None:
+            self.Protocol = KafkaProtocolInfo()
+            self.Protocol._deserialize(params.get("Protocol"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CheckRechargeKafkaServerResponse(AbstractModel):
+    """CheckRechargeKafkaServer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: Kafka集群可访问状态，0：可正常访问 ...
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Status = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.RequestId = params.get("RequestId")
+
+
 class Ckafka(AbstractModel):
     """CKafka的描述-需要投递到的kafka信息
 
     """
 
     def __init__(self):
         r"""
@@ -1917,14 +1981,103 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CreateKafkaRechargeRequest(AbstractModel):
+    """CreateKafkaRecharge请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TopicId: 导入CLS目标topic ID
+        :type TopicId: str
+        :param Name: Kafka导入配置名称
+        :type Name: str
+        :param KafkaType: 导入Kafka类型，0: 腾讯云CKafka，1: 用户自建Kafka
+        :type KafkaType: int
+        :param UserKafkaTopics: 用户需要导入的Kafka相关topic列表，多个topic之间使用半角逗号隔开
+        :type UserKafkaTopics: str
+        :param Offset: 导入数据位置，-2:最早（默认），-1：最晚
+        :type Offset: int
+        :param KafkaInstance: 腾讯云CKafka实例ID，KafkaType为0时必填
+        :type KafkaInstance: str
+        :param ServerAddr: 服务地址，KafkaType为1时必填
+        :type ServerAddr: str
+        :param IsEncryptionAddr: ServerAddr是否为加密连接，KafkaType为1时必填
+        :type IsEncryptionAddr: bool
+        :param Protocol: 加密访问协议，IsEncryptionAddr参数为true时必填
+        :type Protocol: :class:`tencentcloud.cls.v20201016.models.KafkaProtocolInfo`
+        :param ConsumerGroupName: 用户Kafka消费组名称
+        :type ConsumerGroupName: str
+        :param LogRechargeRule: 日志导入规则
+        :type LogRechargeRule: :class:`tencentcloud.cls.v20201016.models.LogRechargeRuleInfo`
+        """
+        self.TopicId = None
+        self.Name = None
+        self.KafkaType = None
+        self.UserKafkaTopics = None
+        self.Offset = None
+        self.KafkaInstance = None
+        self.ServerAddr = None
+        self.IsEncryptionAddr = None
+        self.Protocol = None
+        self.ConsumerGroupName = None
+        self.LogRechargeRule = None
+
+
+    def _deserialize(self, params):
+        self.TopicId = params.get("TopicId")
+        self.Name = params.get("Name")
+        self.KafkaType = params.get("KafkaType")
+        self.UserKafkaTopics = params.get("UserKafkaTopics")
+        self.Offset = params.get("Offset")
+        self.KafkaInstance = params.get("KafkaInstance")
+        self.ServerAddr = params.get("ServerAddr")
+        self.IsEncryptionAddr = params.get("IsEncryptionAddr")
+        if params.get("Protocol") is not None:
+            self.Protocol = KafkaProtocolInfo()
+            self.Protocol._deserialize(params.get("Protocol"))
+        self.ConsumerGroupName = params.get("ConsumerGroupName")
+        if params.get("LogRechargeRule") is not None:
+            self.LogRechargeRule = LogRechargeRuleInfo()
+            self.LogRechargeRule._deserialize(params.get("LogRechargeRule"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateKafkaRechargeResponse(AbstractModel):
+    """CreateKafkaRecharge返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: Kafka导入配置ID
+        :type Id: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Id = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateLogsetRequest(AbstractModel):
     """CreateLogset请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2622,14 +2775,59 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteKafkaRechargeRequest(AbstractModel):
+    """DeleteKafkaRecharge请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: Kafka导入配置ID
+        :type Id: str
+        :param TopicId: 导入CLS目标topic ID
+        :type TopicId: str
+        """
+        self.Id = None
+        self.TopicId = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.TopicId = params.get("TopicId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteKafkaRechargeResponse(AbstractModel):
+    """DeleteKafkaRecharge返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteLogsetRequest(AbstractModel):
     """DeleteLogset请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3552,14 +3750,76 @@
             self.Rule._deserialize(params.get("Rule"))
         self.ModifyTime = params.get("ModifyTime")
         self.IncludeInternalFields = params.get("IncludeInternalFields")
         self.MetadataFlag = params.get("MetadataFlag")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeKafkaRechargesRequest(AbstractModel):
+    """DescribeKafkaRecharges请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TopicId: 日志主题 ID
+        :type TopicId: str
+        :param Id: 导入配置ID
+        :type Id: str
+        :param Status: 状态   status 1: 运行中, 2: 暂停...
+        :type Status: int
+        """
+        self.TopicId = None
+        self.Id = None
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.TopicId = params.get("TopicId")
+        self.Id = params.get("Id")
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeKafkaRechargesResponse(AbstractModel):
+    """DescribeKafkaRecharges返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Infos: KafkaRechargeInfo 信息列表
+        :type Infos: list of KafkaRechargeInfo
+        :param TotalCount: Kafka导入信息总条数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Infos = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Infos") is not None:
+            self.Infos = []
+            for item in params.get("Infos"):
+                obj = KafkaRechargeInfo()
+                obj._deserialize(item)
+                self.Infos.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLogContextRequest(AbstractModel):
     """DescribeLogContext请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4401,15 +4661,15 @@
         :type Delimiter: str
         :param LogRegex: 整条日志匹配规则，只有log_type为fullregex_log时有效
 注意：此字段可能返回 null，表示取不到有效值。
         :type LogRegex: str
         :param BeginRegex: 行首匹配规则，只有log_type为multiline_log或fullregex_log时有效
 注意：此字段可能返回 null，表示取不到有效值。
         :type BeginRegex: str
-        :param Keys: 取的每个字段的key名字，为空的key代表丢弃这个字段，只有log_type为delimiter_log时有效，json_log的日志使用json本身的key
+        :param Keys: 取的每个字段的key名字，为空的key代表丢弃这个字段，只有log_type为delimiter_log时有效，json_log的日志使用json本身的key。限制100个。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Keys: list of str
         :param FilterKeyRegex: 需要过滤日志的key，及其对应的regex
 注意：此字段可能返回 null，表示取不到有效值。
         :type FilterKeyRegex: list of KeyRegexInfo
         :param UnMatchUpLoadSwitch: 解析失败日志是否上传，true表示上传，false表示不上传
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4837,14 +5097,200 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class KafkaConsumerContent(AbstractModel):
+    """kafka协议消费内容
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Format: 消费格式 0:全文；1:json
+        :type Format: int
+        :param EnableTag: 是否投递 TAG 信息
+Format为0时，此字段不需要赋值
+        :type EnableTag: bool
+        :param MetaFields: 元数据信息列表, 可选值为：\_\_SOURCE\_\_、\_\_FILENAME\_\_
+、\_\_TIMESTAMP\_\_、\_\_HOSTNAME\_\_、\_\_PKGID\_\_
+Format为0时，此字段不需要赋值
+        :type MetaFields: list of str
+        :param TagTransaction: tag数据处理方式：
+1:不平铺（默认值）
+2:平铺
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TagTransaction: int
+        :param JsonType: 消费数据Json格式：
+1：不转义（默认格式）
+2：转义
+        :type JsonType: int
+        """
+        self.Format = None
+        self.EnableTag = None
+        self.MetaFields = None
+        self.TagTransaction = None
+        self.JsonType = None
+
+
+    def _deserialize(self, params):
+        self.Format = params.get("Format")
+        self.EnableTag = params.get("EnableTag")
+        self.MetaFields = params.get("MetaFields")
+        self.TagTransaction = params.get("TagTransaction")
+        self.JsonType = params.get("JsonType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class KafkaProtocolInfo(AbstractModel):
+    """Kafka访问协议
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Protocol: 协议类型，支持的协议类型包括 plaintext、sasl_plaintext 或 sasl_ssl。建议使用 sasl_ssl，此协议会进行连接加密同时需要用户认证
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Protocol: str
+        :param Mechanism: 加密类型，支持 PLAIN、SCRAM-SHA-256 或 SCRAM-SHA-512
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Mechanism: str
+        :param UserName: 用户名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserName: str
+        :param Password: 用户密码
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Password: str
+        """
+        self.Protocol = None
+        self.Mechanism = None
+        self.UserName = None
+        self.Password = None
+
+
+    def _deserialize(self, params):
+        self.Protocol = params.get("Protocol")
+        self.Mechanism = params.get("Mechanism")
+        self.UserName = params.get("UserName")
+        self.Password = params.get("Password")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class KafkaRechargeInfo(AbstractModel):
+    """Kafka导入配置信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 主键ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param TopicId: 日志主题ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TopicId: str
+        :param Name: Kafka导入任务名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param KafkaType: 导入Kafka类型，0: 腾讯云CKafka，1: 用户自建Kafka
+注意：此字段可能返回 null，表示取不到有效值。
+        :type KafkaType: int
+        :param KafkaInstance: 腾讯云CKafka实例ID，KafkaType为0时必填
+注意：此字段可能返回 null，表示取不到有效值。
+        :type KafkaInstance: str
+        :param ServerAddr: 服务地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServerAddr: str
+        :param IsEncryptionAddr: ServerAddr是否为加密连接	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsEncryptionAddr: bool
+        :param Protocol: 加密访问协议，IsEncryptionAddr参数为true时必填
+        :type Protocol: :class:`tencentcloud.cls.v20201016.models.KafkaProtocolInfo`
+        :param UserKafkaTopics: 用户需要导入的Kafka相关topic列表，多个topic之间使用半角逗号隔开
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserKafkaTopics: str
+        :param ConsumerGroupName: 用户Kafka消费组名称	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConsumerGroupName: str
+        :param Status: 状态   status 1: 运行中, 2: 暂停 ...
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param Offset: 导入数据位置，-1:最早（默认），-2：最晚，大于等于0: 指定offset
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Offset: int
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param LogRechargeRule: 日志导入规则
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogRechargeRule: :class:`tencentcloud.cls.v20201016.models.LogRechargeRuleInfo`
+        """
+        self.Id = None
+        self.TopicId = None
+        self.Name = None
+        self.KafkaType = None
+        self.KafkaInstance = None
+        self.ServerAddr = None
+        self.IsEncryptionAddr = None
+        self.Protocol = None
+        self.UserKafkaTopics = None
+        self.ConsumerGroupName = None
+        self.Status = None
+        self.Offset = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.LogRechargeRule = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.TopicId = params.get("TopicId")
+        self.Name = params.get("Name")
+        self.KafkaType = params.get("KafkaType")
+        self.KafkaInstance = params.get("KafkaInstance")
+        self.ServerAddr = params.get("ServerAddr")
+        self.IsEncryptionAddr = params.get("IsEncryptionAddr")
+        if params.get("Protocol") is not None:
+            self.Protocol = KafkaProtocolInfo()
+            self.Protocol._deserialize(params.get("Protocol"))
+        self.UserKafkaTopics = params.get("UserKafkaTopics")
+        self.ConsumerGroupName = params.get("ConsumerGroupName")
+        self.Status = params.get("Status")
+        self.Offset = params.get("Offset")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        if params.get("LogRechargeRule") is not None:
+            self.LogRechargeRule = LogRechargeRuleInfo()
+            self.LogRechargeRule._deserialize(params.get("LogRechargeRule"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class KeyRegexInfo(AbstractModel):
     """需要过滤日志的key，及其对应的regex
 
     """
 
     def __init__(self):
         r"""
@@ -5085,14 +5531,100 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class LogRechargeRuleInfo(AbstractModel):
+    """日志导入规则
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RechargeType: 导入类型，支持json_log：json格式日志，minimalist_log: 单行全文，fullregex_log: 单行完全正则
+        :type RechargeType: str
+        :param EncodingFormat: 解析编码格式，0: UTF-8（默认值），1: GBK
+        :type EncodingFormat: int
+        :param DefaultTimeSwitch: 使用默认时间，true：开启（默认值）， flase：关闭
+        :type DefaultTimeSwitch: bool
+        :param LogRegex: 整条日志匹配规则，只有RechargeType为fullregex_log时有效
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogRegex: str
+        :param UnMatchLogSwitch: 解析失败日志是否上传，true表示上传，false表示不上传
+        :type UnMatchLogSwitch: bool
+        :param UnMatchLogKey: 解析失败日志的键名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UnMatchLogKey: str
+        :param UnMatchLogTimeSrc: 解析失败日志时间来源，0: 系统当前时间，1: Kafka消息时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UnMatchLogTimeSrc: int
+        :param DefaultTimeSrc: 默认时间来源，0: 系统当前时间，1: Kafka消息时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefaultTimeSrc: int
+        :param TimeKey: 时间字段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TimeKey: str
+        :param TimeRegex: 时间提取正则表达式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TimeRegex: str
+        :param TimeFormat: 时间字段格式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TimeFormat: str
+        :param TimeZone: 时间字段时区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TimeZone: str
+        :param Metadata: 元数据信息，Kafka导入支持kafka_topic,kafka_partition,kafka_offset,kafka_timestamp
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Metadata: list of str
+        :param Keys: 日志Key列表，RechargeType为full_regex_log时必填
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Keys: list of str
+        """
+        self.RechargeType = None
+        self.EncodingFormat = None
+        self.DefaultTimeSwitch = None
+        self.LogRegex = None
+        self.UnMatchLogSwitch = None
+        self.UnMatchLogKey = None
+        self.UnMatchLogTimeSrc = None
+        self.DefaultTimeSrc = None
+        self.TimeKey = None
+        self.TimeRegex = None
+        self.TimeFormat = None
+        self.TimeZone = None
+        self.Metadata = None
+        self.Keys = None
+
+
+    def _deserialize(self, params):
+        self.RechargeType = params.get("RechargeType")
+        self.EncodingFormat = params.get("EncodingFormat")
+        self.DefaultTimeSwitch = params.get("DefaultTimeSwitch")
+        self.LogRegex = params.get("LogRegex")
+        self.UnMatchLogSwitch = params.get("UnMatchLogSwitch")
+        self.UnMatchLogKey = params.get("UnMatchLogKey")
+        self.UnMatchLogTimeSrc = params.get("UnMatchLogTimeSrc")
+        self.DefaultTimeSrc = params.get("DefaultTimeSrc")
+        self.TimeKey = params.get("TimeKey")
+        self.TimeRegex = params.get("TimeRegex")
+        self.TimeFormat = params.get("TimeFormat")
+        self.TimeZone = params.get("TimeZone")
+        self.Metadata = params.get("Metadata")
+        self.Keys = params.get("Keys")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class LogsetInfo(AbstractModel):
     """日志集相关信息
 
     """
 
     def __init__(self):
         r"""
@@ -5924,14 +6456,103 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyKafkaRechargeRequest(AbstractModel):
+    """ModifyKafkaRecharge请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: Kafka导入配置ID
+        :type Id: str
+        :param TopicId: 导入CLS目标topic ID
+        :type TopicId: str
+        :param Name: Kafka导入配置名称
+        :type Name: str
+        :param KafkaType: 导入Kafka类型，0: 腾讯云CKafka，1: 用户自建Kafka
+        :type KafkaType: int
+        :param KafkaInstance: 腾讯云CKafka实例ID，KafkaType为0时必填
+        :type KafkaInstance: str
+        :param ServerAddr: 服务地址
+        :type ServerAddr: str
+        :param IsEncryptionAddr: ServerAddr是否为加密连接
+        :type IsEncryptionAddr: bool
+        :param Protocol: 加密访问协议，IsEncryptionAddr参数为true时必填
+        :type Protocol: :class:`tencentcloud.cls.v20201016.models.KafkaProtocolInfo`
+        :param UserKafkaTopics: 用户需要导入的Kafka相关topic列表，多个topic之间使用半角逗号隔开
+        :type UserKafkaTopics: str
+        :param ConsumerGroupName: 用户Kafka消费组名称
+        :type ConsumerGroupName: str
+        :param LogRechargeRule: 日志导入规则
+        :type LogRechargeRule: :class:`tencentcloud.cls.v20201016.models.LogRechargeRuleInfo`
+        :param StatusControl: 导入控制，1：暂停，2：继续
+        :type StatusControl: int
+        """
+        self.Id = None
+        self.TopicId = None
+        self.Name = None
+        self.KafkaType = None
+        self.KafkaInstance = None
+        self.ServerAddr = None
+        self.IsEncryptionAddr = None
+        self.Protocol = None
+        self.UserKafkaTopics = None
+        self.ConsumerGroupName = None
+        self.LogRechargeRule = None
+        self.StatusControl = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.TopicId = params.get("TopicId")
+        self.Name = params.get("Name")
+        self.KafkaType = params.get("KafkaType")
+        self.KafkaInstance = params.get("KafkaInstance")
+        self.ServerAddr = params.get("ServerAddr")
+        self.IsEncryptionAddr = params.get("IsEncryptionAddr")
+        if params.get("Protocol") is not None:
+            self.Protocol = KafkaProtocolInfo()
+            self.Protocol._deserialize(params.get("Protocol"))
+        self.UserKafkaTopics = params.get("UserKafkaTopics")
+        self.ConsumerGroupName = params.get("ConsumerGroupName")
+        if params.get("LogRechargeRule") is not None:
+            self.LogRechargeRule = LogRechargeRuleInfo()
+            self.LogRechargeRule._deserialize(params.get("LogRechargeRule"))
+        self.StatusControl = params.get("StatusControl")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyKafkaRechargeResponse(AbstractModel):
+    """ModifyKafkaRecharge返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyLogsetRequest(AbstractModel):
     """ModifyLogset请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6360,22 +6981,28 @@
 
     def __init__(self):
         r"""
         :param FromTopicId: CLS控制台创建的TopicId
         :type FromTopicId: str
         :param Compression: 压缩方式[0:NONE；2:SNAPPY；3:LZ4]
         :type Compression: int
+        :param ConsumerContent: kafka协议消费数据格式
+        :type ConsumerContent: :class:`tencentcloud.cls.v20201016.models.KafkaConsumerContent`
         """
         self.FromTopicId = None
         self.Compression = None
+        self.ConsumerContent = None
 
 
     def _deserialize(self, params):
         self.FromTopicId = params.get("FromTopicId")
         self.Compression = params.get("Compression")
+        if params.get("ConsumerContent") is not None:
+            self.ConsumerContent = KafkaConsumerContent()
+            self.ConsumerContent._deserialize(params.get("ConsumerContent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6505,14 +7132,104 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PreviewKafkaRechargeRequest(AbstractModel):
+    """PreviewKafkaRecharge请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PreviewType: 预览类型，1:源数据预览，2:导出结果预览
+        :type PreviewType: int
+        :param KafkaType: 导入Kafka类型，0: 腾讯云CKafka，1: 用户自建Kafka
+        :type KafkaType: int
+        :param UserKafkaTopics: 用户需要导入的Kafka相关topic列表，多个topic之间使用半角逗号隔开
+        :type UserKafkaTopics: str
+        :param Offset: 导入数据位置，-2:最早（默认），-1：最晚
+        :type Offset: int
+        :param KafkaInstance: 腾讯云CKafka实例ID，KafkaType为0时必填
+        :type KafkaInstance: str
+        :param ServerAddr: 服务地址
+        :type ServerAddr: str
+        :param IsEncryptionAddr: ServerAddr是否为加密连接
+        :type IsEncryptionAddr: bool
+        :param Protocol: 加密访问协议，IsEncryptionAddr参数为true时必填
+        :type Protocol: :class:`tencentcloud.cls.v20201016.models.KafkaProtocolInfo`
+        :param ConsumerGroupName: 用户Kafka消费组
+        :type ConsumerGroupName: str
+        :param LogRechargeRule: 日志导入规则
+        :type LogRechargeRule: :class:`tencentcloud.cls.v20201016.models.LogRechargeRuleInfo`
+        """
+        self.PreviewType = None
+        self.KafkaType = None
+        self.UserKafkaTopics = None
+        self.Offset = None
+        self.KafkaInstance = None
+        self.ServerAddr = None
+        self.IsEncryptionAddr = None
+        self.Protocol = None
+        self.ConsumerGroupName = None
+        self.LogRechargeRule = None
+
+
+    def _deserialize(self, params):
+        self.PreviewType = params.get("PreviewType")
+        self.KafkaType = params.get("KafkaType")
+        self.UserKafkaTopics = params.get("UserKafkaTopics")
+        self.Offset = params.get("Offset")
+        self.KafkaInstance = params.get("KafkaInstance")
+        self.ServerAddr = params.get("ServerAddr")
+        self.IsEncryptionAddr = params.get("IsEncryptionAddr")
+        if params.get("Protocol") is not None:
+            self.Protocol = KafkaProtocolInfo()
+            self.Protocol._deserialize(params.get("Protocol"))
+        self.ConsumerGroupName = params.get("ConsumerGroupName")
+        if params.get("LogRechargeRule") is not None:
+            self.LogRechargeRule = LogRechargeRuleInfo()
+            self.LogRechargeRule._deserialize(params.get("LogRechargeRule"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PreviewKafkaRechargeResponse(AbstractModel):
+    """PreviewKafkaRecharge返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LogSample: 日志样例，PreviewType为2时返回
+        :type LogSample: str
+        :param LogData: 日志预览结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogData: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.LogSample = None
+        self.LogData = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.LogSample = params.get("LogSample")
+        self.LogData = params.get("LogData")
+        self.RequestId = params.get("RequestId")
+
+
 class RetryShipperTaskRequest(AbstractModel):
     """RetryShipperTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.926/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.927/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CheckRechargeKafkaServer(self, request):
+        """本接口用于校验Kafka服务集群是否可以正常访问
+
+        :param request: Request instance for CheckRechargeKafkaServer.
+        :type request: :class:`tencentcloud.cls.v20201016.models.CheckRechargeKafkaServerRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.CheckRechargeKafkaServerResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CheckRechargeKafkaServer", params, headers=headers)
+            response = json.loads(body)
+            model = models.CheckRechargeKafkaServerResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CloseKafkaConsumer(self, request):
         """关闭Kafka协议消费
 
         :param request: Request instance for CloseKafkaConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.CloseKafkaConsumerRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.CloseKafkaConsumerResponse`
 
@@ -275,14 +298,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateKafkaRecharge(self, request):
+        """本接口用于创建Kafka数据订阅任务
+
+        :param request: Request instance for CreateKafkaRecharge.
+        :type request: :class:`tencentcloud.cls.v20201016.models.CreateKafkaRechargeRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.CreateKafkaRechargeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateKafkaRecharge", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateKafkaRechargeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateLogset(self, request):
         """本接口用于创建日志集，返回新创建的日志集的 ID。
 
         :param request: Request instance for CreateLogset.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateLogsetRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.CreateLogsetResponse`
 
@@ -551,14 +597,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteKafkaRecharge(self, request):
+        """本接口用于删除Kafka数据订阅任务
+
+        :param request: Request instance for DeleteKafkaRecharge.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DeleteKafkaRechargeRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DeleteKafkaRechargeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteKafkaRecharge", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteKafkaRechargeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteLogset(self, request):
         """本接口用于删除日志集。
 
         :param request: Request instance for DeleteLogset.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteLogsetRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DeleteLogsetResponse`
 
@@ -896,14 +965,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeKafkaRecharges(self, request):
+        """本接口用于获取Kafka数据订阅任务
+
+        :param request: Request instance for DescribeKafkaRecharges.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaRechargesRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaRechargesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeKafkaRecharges", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeKafkaRechargesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeLogContext(self, request):
         """本接口用于搜索日志上下文附近的内容
 
         :param request: Request instance for DescribeLogContext.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeLogContextRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeLogContextResponse`
 
@@ -1333,14 +1425,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyKafkaRecharge(self, request):
+        """本接口用于修改Kafka数据订阅任务
+
+        :param request: Request instance for ModifyKafkaRecharge.
+        :type request: :class:`tencentcloud.cls.v20201016.models.ModifyKafkaRechargeRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.ModifyKafkaRechargeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyKafkaRecharge", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyKafkaRechargeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyLogset(self, request):
         """本接口用于修改日志集信息
 
         :param request: Request instance for ModifyLogset.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyLogsetRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.ModifyLogsetResponse`
 
@@ -1446,14 +1561,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def PreviewKafkaRecharge(self, request):
+        """本接口用于预览Kafka数据订阅任务客户日志信息
+
+        :param request: Request instance for PreviewKafkaRecharge.
+        :type request: :class:`tencentcloud.cls.v20201016.models.PreviewKafkaRechargeRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.PreviewKafkaRechargeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("PreviewKafkaRecharge", params, headers=headers)
+            response = json.loads(body)
+            model = models.PreviewKafkaRechargeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def RetryShipperTask(self, request):
         """重试失败的投递任务
 
         :param request: Request instance for RetryShipperTask.
         :type request: :class:`tencentcloud.cls.v20201016.models.RetryShipperTaskRequest`
```

