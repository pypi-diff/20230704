# Comparing `tmp/tencentcloud-sdk-python-wav-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-wav-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.925.tar", last modified: Fri Jun 30 02:29:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.926.tar", last modified: Mon Jul  3 00:38:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wav-3.0.925.tar` & `tencentcloud-sdk-python-wav-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/__init__.py
--rw-r--r--   0 root         (0) root         (0)   125778 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/models.py
--rw-r--r--   0 root         (0) root         (0)    24112 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/wav_client.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud_sdk_python_wav.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/tencentcloud_sdk_python_wav.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:29:35.000000 tencentcloud-sdk-python-wav-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud_sdk_python_wav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud_sdk_python_wav.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:38:46.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/
+-rw-r--r--   0 root         (0) root         (0)   139897 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/models.py
+-rw-r--r--   0 root         (0) root         (0)    25908 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/wav_client.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:38:45.000000 tencentcloud-sdk-python-wav-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-wav-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wav-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/models.py` & `tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,71 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ArrivalInfo(AbstractModel):
+    """发生过到店的潜客到店信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClueId: 线索id
+        :type ClueId: int
+        :param CustomerId: 客户id
+        :type CustomerId: int
+        :param UserName: 客户姓名
+        :type UserName: str
+        :param Phone: 客户的手机号
+        :type Phone: str
+        :param FirstArrival: 是否首次到店，0否，1是
+        :type FirstArrival: int
+        :param ArrivalTime: 到店时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ArrivalTime: int
+        :param EventType: 发生事件
+        :type EventType: int
+        :param EventTypeName: 发生事件名称
+        :type EventTypeName: str
+        :param FollowRecord: 跟进记录
+        :type FollowRecord: str
+        """
+        self.ClueId = None
+        self.CustomerId = None
+        self.UserName = None
+        self.Phone = None
+        self.FirstArrival = None
+        self.ArrivalTime = None
+        self.EventType = None
+        self.EventTypeName = None
+        self.FollowRecord = None
+
+
+    def _deserialize(self, params):
+        self.ClueId = params.get("ClueId")
+        self.CustomerId = params.get("CustomerId")
+        self.UserName = params.get("UserName")
+        self.Phone = params.get("Phone")
+        self.FirstArrival = params.get("FirstArrival")
+        self.ArrivalTime = params.get("ArrivalTime")
+        self.EventType = params.get("EventType")
+        self.EventTypeName = params.get("EventTypeName")
+        self.FollowRecord = params.get("FollowRecord")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ChannelCodeInnerDetail(AbstractModel):
     """渠道活码详情
 
     """
 
     def __init__(self):
         r"""
@@ -412,15 +469,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param ClueId: 线索id，线索唯一识别编码
         :type ClueId: str
-        :param DealerId: 接待客户经销商顾问所属组织id,多个组织使用逗号分割
+        :param DealerId: 接待客户经销商顾问所属经销商code
         :type DealerId: str
         :param EnquireTime: 线索获取时间，用户添加企业微信时间，单位是秒
         :type EnquireTime: int
         :param UnionId: 客户在微信生态中唯一识别码
         :type UnionId: str
         :param Name: 微信昵称
         :type Name: str
@@ -468,14 +525,68 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type ImportAtTime: int
         :param DistributeTime: 完成线索分配的时间戳，单位：秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type DistributeTime: int
         :param CreateAtTime: 获取线索的时间戳，单位：秒
         :type CreateAtTime: int
+        :param WxId: 客户微信id
+        :type WxId: str
+        :param BrandCode: 意向车型对应品牌code
+        :type BrandCode: str
+        :param BuildTime: 建档时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BuildTime: int
+        :param OrderTime: 下订时间，单位：秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OrderTime: int
+        :param ArrivalTime: 到店时间，单位：秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ArrivalTime: int
+        :param DeliveryTime: 交车时间，单位：秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeliveryTime: int
+        :param FollowTime: 上次跟进时间，单位：秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FollowTime: int
+        :param NextFollowTime: 下次跟进时间，单位：秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NextFollowTime: int
+        :param OrgId: 线索所属组织id
+        :type OrgId: int
+        :param OrgName: 线索所属组织名称
+        :type OrgName: str
+        :param Introducer: 介绍人姓名
+        :type Introducer: str
+        :param IntroducerPhone: 介绍人电话
+        :type IntroducerPhone: str
+        :param IsBindWx: 是否关联微信 1 是 0 否
+        :type IsBindWx: int
+        :param IsMerge: 是否经过合并 1 是 0 否
+        :type IsMerge: int
+        :param IsInvalid: 是否无效  1 是 0 否
+        :type IsInvalid: int
+        :param InvalidType: 无效类型
+        :type InvalidType: str
+        :param InvalidTypeName: 无效类型枚举：
+无意向购买、空错号、未接听、其他
+        :type InvalidTypeName: str
+        :param InvalidRemark: 由顾问手动输入的无效原因文字
+        :type InvalidRemark: str
+        :param InvalidTime: 无效时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InvalidTime: int
+        :param DealerName: 经销商名称
+        :type DealerName: str
+        :param ShopId: 经销商下级门店ID
+        :type ShopId: int
+        :param ShopName: 经销商下级门店名称
+        :type ShopName: str
+        :param Position: 职位
+        :type Position: str
         """
         self.ClueId = None
         self.DealerId = None
         self.EnquireTime = None
         self.UnionId = None
         self.Name = None
         self.Phone = None
@@ -496,14 +607,37 @@
         self.Gender = None
         self.CreateTime = None
         self.LeadStatus = None
         self.LevelCode = None
         self.ImportAtTime = None
         self.DistributeTime = None
         self.CreateAtTime = None
+        self.WxId = None
+        self.BrandCode = None
+        self.BuildTime = None
+        self.OrderTime = None
+        self.ArrivalTime = None
+        self.DeliveryTime = None
+        self.FollowTime = None
+        self.NextFollowTime = None
+        self.OrgId = None
+        self.OrgName = None
+        self.Introducer = None
+        self.IntroducerPhone = None
+        self.IsBindWx = None
+        self.IsMerge = None
+        self.IsInvalid = None
+        self.InvalidType = None
+        self.InvalidTypeName = None
+        self.InvalidRemark = None
+        self.InvalidTime = None
+        self.DealerName = None
+        self.ShopId = None
+        self.ShopName = None
+        self.Position = None
 
 
     def _deserialize(self, params):
         self.ClueId = params.get("ClueId")
         self.DealerId = params.get("DealerId")
         self.EnquireTime = params.get("EnquireTime")
         self.UnionId = params.get("UnionId")
@@ -526,14 +660,37 @@
         self.Gender = params.get("Gender")
         self.CreateTime = params.get("CreateTime")
         self.LeadStatus = params.get("LeadStatus")
         self.LevelCode = params.get("LevelCode")
         self.ImportAtTime = params.get("ImportAtTime")
         self.DistributeTime = params.get("DistributeTime")
         self.CreateAtTime = params.get("CreateAtTime")
+        self.WxId = params.get("WxId")
+        self.BrandCode = params.get("BrandCode")
+        self.BuildTime = params.get("BuildTime")
+        self.OrderTime = params.get("OrderTime")
+        self.ArrivalTime = params.get("ArrivalTime")
+        self.DeliveryTime = params.get("DeliveryTime")
+        self.FollowTime = params.get("FollowTime")
+        self.NextFollowTime = params.get("NextFollowTime")
+        self.OrgId = params.get("OrgId")
+        self.OrgName = params.get("OrgName")
+        self.Introducer = params.get("Introducer")
+        self.IntroducerPhone = params.get("IntroducerPhone")
+        self.IsBindWx = params.get("IsBindWx")
+        self.IsMerge = params.get("IsMerge")
+        self.IsInvalid = params.get("IsInvalid")
+        self.InvalidType = params.get("InvalidType")
+        self.InvalidTypeName = params.get("InvalidTypeName")
+        self.InvalidRemark = params.get("InvalidRemark")
+        self.InvalidTime = params.get("InvalidTime")
+        self.DealerName = params.get("DealerName")
+        self.ShopId = params.get("ShopId")
+        self.ShopName = params.get("ShopName")
+        self.Position = params.get("Position")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -570,38 +727,43 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type MainDepartment: str
         :param IsLeaderInDept: 是否为部门负责人，第三方应用可为空。与orgIds值一一对应，多个部门使用逗号隔开，0-否， 1-是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsLeaderInDept: str
         :param Status: 激活状态: 0=已激活，1=已禁用，-1=退出企业"
         :type Status: int
+        :param JobNumber: 工号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobNumber: str
         """
         self.UserId = None
         self.UserName = None
         self.UserOpenId = None
         self.DealerId = None
         self.ShopId = None
         self.Phone = None
         self.OrgIds = None
         self.MainDepartment = None
         self.IsLeaderInDept = None
         self.Status = None
+        self.JobNumber = None
 
 
     def _deserialize(self, params):
         self.UserId = params.get("UserId")
         self.UserName = params.get("UserName")
         self.UserOpenId = params.get("UserOpenId")
         self.DealerId = params.get("DealerId")
         self.ShopId = params.get("ShopId")
         self.Phone = params.get("Phone")
         self.OrgIds = params.get("OrgIds")
         self.MainDepartment = params.get("MainDepartment")
         self.IsLeaderInDept = params.get("IsLeaderInDept")
         self.Status = params.get("Status")
+        self.JobNumber = params.get("JobNumber")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1471,14 +1633,89 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FollowInfo(AbstractModel):
+    """发生过跟进的潜客信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClueId: 线索id
+        :type ClueId: int
+        :param CustomerId: 客户档案id
+        :type CustomerId: int
+        :param UserName: 客户姓名
+        :type UserName: str
+        :param Phone: 客户的手机号
+        :type Phone: str
+        :param IsOverdue: 是否逾期
+        :type IsOverdue: int
+        :param OverdueTime: 逾期时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OverdueTime: int
+        :param EventType: 发生事件
+        :type EventType: int
+        :param EventTypeName: 发生事件名称
+        :type EventTypeName: str
+        :param FollowWayType: 跟进方式
+        :type FollowWayType: str
+        :param FollowWayName: 跟进方式名称
+        :type FollowWayName: str
+        :param FollowTime: 本次跟进时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FollowTime: int
+        :param NextFollowTime: 下次跟进时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NextFollowTime: int
+        :param FollowRecord: 跟进记录
+        :type FollowRecord: str
+        """
+        self.ClueId = None
+        self.CustomerId = None
+        self.UserName = None
+        self.Phone = None
+        self.IsOverdue = None
+        self.OverdueTime = None
+        self.EventType = None
+        self.EventTypeName = None
+        self.FollowWayType = None
+        self.FollowWayName = None
+        self.FollowTime = None
+        self.NextFollowTime = None
+        self.FollowRecord = None
+
+
+    def _deserialize(self, params):
+        self.ClueId = params.get("ClueId")
+        self.CustomerId = params.get("CustomerId")
+        self.UserName = params.get("UserName")
+        self.Phone = params.get("Phone")
+        self.IsOverdue = params.get("IsOverdue")
+        self.OverdueTime = params.get("OverdueTime")
+        self.EventType = params.get("EventType")
+        self.EventTypeName = params.get("EventTypeName")
+        self.FollowWayType = params.get("FollowWayType")
+        self.FollowWayName = params.get("FollowWayName")
+        self.FollowTime = params.get("FollowTime")
+        self.NextFollowTime = params.get("NextFollowTime")
+        self.FollowRecord = params.get("FollowRecord")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FollowUser(AbstractModel):
     """添加了此外部联系人的企业成员信息
 
     """
 
     def __init__(self):
         r"""
@@ -2003,14 +2240,87 @@
             for item in params.get("PageData"):
                 obj = LiveCodeDetail()
                 obj._deserialize(item)
                 self.PageData.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class QueryArrivalListRequest(AbstractModel):
+    """QueryArrivalList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Limit: 分页，预期请求的数据量，取值范围 1 ~ 1000
+        :type Limit: int
+        :param BeginTime: 查询开始时间， 单位秒
+        :type BeginTime: int
+        :param EndTime: 查询结束时间， 单位秒
+        :type EndTime: int
+        :param Cursor: 用于分页查询的游标，字符串类型，由上一次调用返回，首次调用可不填
+        :type Cursor: str
+        """
+        self.Limit = None
+        self.BeginTime = None
+        self.EndTime = None
+        self.Cursor = None
+
+
+    def _deserialize(self, params):
+        self.Limit = params.get("Limit")
+        self.BeginTime = params.get("BeginTime")
+        self.EndTime = params.get("EndTime")
+        self.Cursor = params.get("Cursor")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryArrivalListResponse(AbstractModel):
+    """QueryArrivalList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NextCursor: 分页游标，下次调用带上该值，则从当前的位置继续往后拉，以实现增量拉取。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NextCursor: str
+        :param PageData: 潜客客户存档信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PageData: list of ArrivalInfo
+        :param HasMore: 是否还有更多数据。0-否；1-是。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HasMore: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.NextCursor = None
+        self.PageData = None
+        self.HasMore = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.NextCursor = params.get("NextCursor")
+        if params.get("PageData") is not None:
+            self.PageData = []
+            for item in params.get("PageData"):
+                obj = ArrivalInfo()
+                obj._deserialize(item)
+                self.PageData.append(obj)
+        self.HasMore = params.get("HasMore")
+        self.RequestId = params.get("RequestId")
+
+
 class QueryChannelCodeListRequest(AbstractModel):
     """QueryChannelCodeList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2790,14 +3100,87 @@
             for item in params.get("ExternalUserIdMapping"):
                 obj = ExternalUserMappingInfo()
                 obj._deserialize(item)
                 self.ExternalUserIdMapping.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class QueryFollowListRequest(AbstractModel):
+    """QueryFollowList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Limit: 分页，预期请求的数据量，取值范围 1 ~ 1000
+        :type Limit: int
+        :param BeginTime: 查询开始时间， 单位秒
+        :type BeginTime: int
+        :param EndTime: 查询结束时间， 单位秒
+        :type EndTime: int
+        :param Cursor: 用于分页查询的游标，字符串类型，由上一次调用返回，首次调用可不填
+        :type Cursor: str
+        """
+        self.Limit = None
+        self.BeginTime = None
+        self.EndTime = None
+        self.Cursor = None
+
+
+    def _deserialize(self, params):
+        self.Limit = params.get("Limit")
+        self.BeginTime = params.get("BeginTime")
+        self.EndTime = params.get("EndTime")
+        self.Cursor = params.get("Cursor")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class QueryFollowListResponse(AbstractModel):
+    """QueryFollowList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NextCursor: 分页游标，下次调用带上该值，则从当前的位置继续往后拉，以实现增量拉取。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NextCursor: str
+        :param PageData: 潜客客户存档信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PageData: list of FollowInfo
+        :param HasMore: 是否还有更多数据。0-否；1-是。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HasMore: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.NextCursor = None
+        self.PageData = None
+        self.HasMore = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.NextCursor = params.get("NextCursor")
+        if params.get("PageData") is not None:
+            self.PageData = []
+            for item in params.get("PageData"):
+                obj = FollowInfo()
+                obj._deserialize(item)
+                self.PageData.append(obj)
+        self.HasMore = params.get("HasMore")
+        self.RequestId = params.get("RequestId")
+
+
 class QueryLicenseInfoRequest(AbstractModel):
     """QueryLicenseInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/wav_client.py` & `tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/wav_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def QueryArrivalList(self, request):
+        """查询指定时间范围内发生过到店的潜客到店信息
+
+        :param request: Request instance for QueryArrivalList.
+        :type request: :class:`tencentcloud.wav.v20210129.models.QueryArrivalListRequest`
+        :rtype: :class:`tencentcloud.wav.v20210129.models.QueryArrivalListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryArrivalList", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryArrivalListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def QueryChannelCodeList(self, request):
         """根据游标拉取渠道活码列表信息
 
         :param request: Request instance for QueryChannelCodeList.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryChannelCodeListRequest`
         :rtype: :class:`tencentcloud.wav.v20210129.models.QueryChannelCodeListResponse`
 
@@ -434,14 +457,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def QueryFollowList(self, request):
+        """查询指定时间范围内发生过跟进的潜客信息
+
+        :param request: Request instance for QueryFollowList.
+        :type request: :class:`tencentcloud.wav.v20210129.models.QueryFollowListRequest`
+        :rtype: :class:`tencentcloud.wav.v20210129.models.QueryFollowListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("QueryFollowList", params, headers=headers)
+            response = json.loads(body)
+            model = models.QueryFollowListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def QueryLicenseInfo(self, request):
         """该接口获取license对应的详细信息
 
         :param request: Request instance for QueryLicenseInfo.
         :type request: :class:`tencentcloud.wav.v20210129.models.QueryLicenseInfoRequest`
```

### Comparing `tencentcloud-sdk-python-wav-3.0.925/tencentcloud/wav/v20210129/errorcodes.py` & `tencentcloud-sdk-python-wav-3.0.926/tencentcloud/wav/v20210129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.925/README.rst` & `tencentcloud-sdk-python-wav-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.925/tencentcloud_sdk_python_wav.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.926/tencentcloud_sdk_python_wav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.925/setup.py` & `tencentcloud-sdk-python-wav-3.0.926/setup.py`

 * *Files identical despite different names*

