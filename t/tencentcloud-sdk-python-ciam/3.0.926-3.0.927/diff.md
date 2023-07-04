# Comparing `tmp/tencentcloud-sdk-python-ciam-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-ciam-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ciam-3.0.926.tar", last modified: Mon Jul  3 00:22:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ciam-3.0.927.tar", last modified: Tue Jul  4 00:17:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ciam-3.0.926.tar` & `tencentcloud-sdk-python-ciam-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/setup.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud_sdk_python_ciam.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud_sdk_python_ciam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud_sdk_python_ciam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud_sdk_python_ciam.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/
--rw-r--r--   0 root         (0) root         (0)    66357 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/models.py
--rw-r--r--   0 root         (0) root         (0)    13795 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/ciam_client.py
--rw-r--r--   0 root         (0) root         (0)     5610 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:22:02.000000 tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/
+-rw-r--r--   0 root         (0) root         (0)     8558 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    85555 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20629 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/ciam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:17:39.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud_sdk_python_ciam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud_sdk_python_ciam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud_sdk_python_ciam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:17:40.000000 tencentcloud-sdk-python-ciam-3.0.927/tencentcloud_sdk_python_ciam.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/setup.py` & `tencentcloud-sdk-python-ciam-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/README.rst` & `tencentcloud-sdk-python-ciam-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-ciam-3.0.927/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ciam
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Ciam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ciam-3.0.927/tencentcloud_sdk_python_ciam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ciam
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Ciam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/models.py` & `tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,49 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AppAssociatedUserGroupIds(AbstractModel):
+    """用户组删除时关联的应用信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserGroupId: 用户组id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserGroupId: str
+        :param ApplicationId: 应用id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ApplicationId: str
+        :param ApplicationName: 应用名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ApplicationName: str
+        """
+        self.UserGroupId = None
+        self.ApplicationId = None
+        self.ApplicationName = None
+
+
+    def _deserialize(self, params):
+        self.UserGroupId = params.get("UserGroupId")
+        self.ApplicationId = params.get("ApplicationId")
+        self.ApplicationName = params.get("ApplicationName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateApiImportUserJobRequest(AbstractModel):
     """CreateApiImportUserJob请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -145,14 +180,63 @@
     def _deserialize(self, params):
         if params.get("Job") is not None:
             self.Job = Job()
             self.Job._deserialize(params.get("Job"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateUserGroupRequest(AbstractModel):
+    """CreateUserGroup请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DisplayName: 用户组名称
+        :type DisplayName: str
+        :param UserStoreId: 用户目录ID
+        :type UserStoreId: str
+        :param Description: 用户组描述
+        :type Description: str
+        """
+        self.DisplayName = None
+        self.UserStoreId = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.DisplayName = params.get("DisplayName")
+        self.UserStoreId = params.get("UserStoreId")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateUserGroupResponse(AbstractModel):
+    """CreateUserGroup返回参数结构体
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
 class CreateUserRequest(AbstractModel):
     """CreateUser请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -254,14 +338,156 @@
     def _deserialize(self, params):
         if params.get("User") is not None:
             self.User = User()
             self.User._deserialize(params.get("User"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateUserStoreRequest(AbstractModel):
+    """CreateUserStore请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserPoolName: 用户池名字
+        :type UserPoolName: str
+        :param UserPoolDesc: 用户池描述
+        :type UserPoolDesc: str
+        :param UserPoolLogo: 用户池logo
+        :type UserPoolLogo: str
+        """
+        self.UserPoolName = None
+        self.UserPoolDesc = None
+        self.UserPoolLogo = None
+
+
+    def _deserialize(self, params):
+        self.UserPoolName = params.get("UserPoolName")
+        self.UserPoolDesc = params.get("UserPoolDesc")
+        self.UserPoolLogo = params.get("UserPoolLogo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateUserStoreResponse(AbstractModel):
+    """CreateUserStore返回参数结构体
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
+class DeleteUserGroupsRequest(AbstractModel):
+    """DeleteUserGroups请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserGroupIds: 用户组ID数组
+        :type UserGroupIds: list of str
+        :param UserStoreId: 用户目录ID
+        :type UserStoreId: str
+        """
+        self.UserGroupIds = None
+        self.UserStoreId = None
+
+
+    def _deserialize(self, params):
+        self.UserGroupIds = params.get("UserGroupIds")
+        self.UserStoreId = params.get("UserStoreId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteUserGroupsResponse(AbstractModel):
+    """DeleteUserGroups返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserGroupDeletedInfo: 删除的用户组关联的应用信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserGroupDeletedInfo: :class:`tencentcloud.ciam.v20220331.models.UserGroupDeleteResp`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.UserGroupDeletedInfo = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("UserGroupDeletedInfo") is not None:
+            self.UserGroupDeletedInfo = UserGroupDeleteResp()
+            self.UserGroupDeletedInfo._deserialize(params.get("UserGroupDeletedInfo"))
+        self.RequestId = params.get("RequestId")
+
+
+class DeleteUserStoreRequest(AbstractModel):
+    """DeleteUserStore请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserPoolId: 用户池ID
+        :type UserPoolId: str
+        """
+        self.UserPoolId = None
+
+
+    def _deserialize(self, params):
+        self.UserPoolId = params.get("UserPoolId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteUserStoreResponse(AbstractModel):
+    """DeleteUserStore返回参数结构体
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
 class DeleteUsersRequest(AbstractModel):
     """DeleteUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1058,14 +1284,94 @@
             for item in params.get("Users"):
                 obj = User()
                 obj._deserialize(item)
                 self.Users.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class ListUserGroupsRequest(AbstractModel):
+    """ListUserGroups请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserStoreId: 用户目录ID
+        :type UserStoreId: str
+        :param Pageable: 分页数据
+        :type Pageable: :class:`tencentcloud.ciam.v20220331.models.Pageable`
+        :param Filters: Key可选值为condition
+
+<li> **condition** </li>	Values = 查询条件，用户组ID或用户组名称
+        :type Filters: list of Filter
+        """
+        self.UserStoreId = None
+        self.Pageable = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.UserStoreId = params.get("UserStoreId")
+        if params.get("Pageable") is not None:
+            self.Pageable = Pageable()
+            self.Pageable._deserialize(params.get("Pageable"))
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ListUserGroupsResponse(AbstractModel):
+    """ListUserGroups返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Content: 用户组列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Content: list of UserGroup
+        :param Total: 总条数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param Pageable: 分页
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Pageable: :class:`tencentcloud.ciam.v20220331.models.Pageable`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Content = None
+        self.Total = None
+        self.Pageable = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Content") is not None:
+            self.Content = []
+            for item in params.get("Content"):
+                obj = UserGroup()
+                obj._deserialize(item)
+                self.Content.append(obj)
+        self.Total = params.get("Total")
+        if params.get("Pageable") is not None:
+            self.Pageable = Pageable()
+            self.Pageable._deserialize(params.get("Pageable"))
+        self.RequestId = params.get("RequestId")
+
+
 class ListUserRequest(AbstractModel):
     """ListUser请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1143,14 +1449,47 @@
             for item in params.get("Content"):
                 obj = User()
                 obj._deserialize(item)
                 self.Content.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class ListUserStoreRequest(AbstractModel):
+    """ListUserStore请求参数结构体
+
+    """
+
+
+class ListUserStoreResponse(AbstractModel):
+    """ListUserStore返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserStoreSet: 用户目录列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserStoreSet: list of UserStore
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.UserStoreSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("UserStoreSet") is not None:
+            self.UserStoreSet = []
+            for item in params.get("UserStoreSet"):
+                obj = UserStore()
+                obj._deserialize(item)
+                self.UserStoreSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class LogMessage(AbstractModel):
     """日志详情
 
     """
 
     def __init__(self):
         r"""
@@ -1557,14 +1896,67 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class UpdateUserGroupRequest(AbstractModel):
+    """UpdateUserGroup请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserGroupId: 用户组ID
+        :type UserGroupId: str
+        :param DisplayName: 用户组名称
+        :type DisplayName: str
+        :param UserStoreId: 用户目录ID
+        :type UserStoreId: str
+        :param Description: 用户组描述
+        :type Description: str
+        """
+        self.UserGroupId = None
+        self.DisplayName = None
+        self.UserStoreId = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.UserGroupId = params.get("UserGroupId")
+        self.DisplayName = params.get("DisplayName")
+        self.UserStoreId = params.get("UserStoreId")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateUserGroupResponse(AbstractModel):
+    """UpdateUserGroup返回参数结构体
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
 class UpdateUserRequest(AbstractModel):
     """UpdateUser请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1719,14 +2111,67 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UpdateUserStoreRequest(AbstractModel):
+    """UpdateUserStore请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserPoolId: 用户池ID
+        :type UserPoolId: str
+        :param UserPoolName: 用户池名字
+        :type UserPoolName: str
+        :param UserPoolDesc: 用户池描述
+        :type UserPoolDesc: str
+        :param UserPoolLogo: 用户池logo
+        :type UserPoolLogo: str
+        """
+        self.UserPoolId = None
+        self.UserPoolName = None
+        self.UserPoolDesc = None
+        self.UserPoolLogo = None
+
+
+    def _deserialize(self, params):
+        self.UserPoolId = params.get("UserPoolId")
+        self.UserPoolName = params.get("UserPoolName")
+        self.UserPoolDesc = params.get("UserPoolDesc")
+        self.UserPoolLogo = params.get("UserPoolLogo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateUserStoreResponse(AbstractModel):
+    """UpdateUserStore返回参数结构体
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
 class User(AbstractModel):
     """用户信息
 
     """
 
     def __init__(self):
         r"""
@@ -1942,8 +2387,167 @@
         self.IndexedAttribute5 = params.get("IndexedAttribute5")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UserGroup(AbstractModel):
+    """用户组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserGroupId: 用户组ID
+        :type UserGroupId: str
+        :param DisplayName: 用户组名称
+        :type DisplayName: str
+        :param Description: 用户组描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param UserStoreId: 用户目录ID
+        :type UserStoreId: str
+        :param TenantId: 租户ID
+        :type TenantId: str
+        :param CreatedDate: 创建时间
+        :type CreatedDate: int
+        :param LastModifyDate: 最近更新时间
+        :type LastModifyDate: int
+        """
+        self.UserGroupId = None
+        self.DisplayName = None
+        self.Description = None
+        self.UserStoreId = None
+        self.TenantId = None
+        self.CreatedDate = None
+        self.LastModifyDate = None
+
+
+    def _deserialize(self, params):
+        self.UserGroupId = params.get("UserGroupId")
+        self.DisplayName = params.get("DisplayName")
+        self.Description = params.get("Description")
+        self.UserStoreId = params.get("UserStoreId")
+        self.TenantId = params.get("TenantId")
+        self.CreatedDate = params.get("CreatedDate")
+        self.LastModifyDate = params.get("LastModifyDate")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UserGroupDeleteResp(AbstractModel):
+    """删除用户组信息时返回的详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ErrorMessage: 错误详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorMessage: str
+        :param AppAssociatedUserGroupIds: 用户组关联的应用信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppAssociatedUserGroupIds: list of AppAssociatedUserGroupIds
+        """
+        self.ErrorMessage = None
+        self.AppAssociatedUserGroupIds = None
+
+
+    def _deserialize(self, params):
+        self.ErrorMessage = params.get("ErrorMessage")
+        if params.get("AppAssociatedUserGroupIds") is not None:
+            self.AppAssociatedUserGroupIds = []
+            for item in params.get("AppAssociatedUserGroupIds"):
+                obj = AppAssociatedUserGroupIds()
+                obj._deserialize(item)
+                self.AppAssociatedUserGroupIds.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UserStore(AbstractModel):
+    """用户池
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TenantId: 租户ID
+        :type TenantId: str
+        :param UserStoreLogo: 用户池logo
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserStoreLogo: str
+        :param UserStoreDesc: 用户池描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserStoreDesc: str
+        :param UserStoreName: 用户池名称
+        :type UserStoreName: str
+        :param UserNum: 用户数量
+        :type UserNum: int
+        :param UserStoreId: 用户池ID
+        :type UserStoreId: str
+        :param AppNum: 应用数量
+        :type AppNum: int
+        :param LastStatus: 上次切换的用户池
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastStatus: bool
+        :param DefaultStatus: 默认用户池
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefaultStatus: bool
+        :param CreateDate: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateDate: int
+        :param LastStatusTime: 上次切换时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastStatusTime: int
+        :param UserStoreProtocolHost: 用户目录域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserStoreProtocolHost: str
+        """
+        self.TenantId = None
+        self.UserStoreLogo = None
+        self.UserStoreDesc = None
+        self.UserStoreName = None
+        self.UserNum = None
+        self.UserStoreId = None
+        self.AppNum = None
+        self.LastStatus = None
+        self.DefaultStatus = None
+        self.CreateDate = None
+        self.LastStatusTime = None
+        self.UserStoreProtocolHost = None
+
+
+    def _deserialize(self, params):
+        self.TenantId = params.get("TenantId")
+        self.UserStoreLogo = params.get("UserStoreLogo")
+        self.UserStoreDesc = params.get("UserStoreDesc")
+        self.UserStoreName = params.get("UserStoreName")
+        self.UserNum = params.get("UserNum")
+        self.UserStoreId = params.get("UserStoreId")
+        self.AppNum = params.get("AppNum")
+        self.LastStatus = params.get("LastStatus")
+        self.DefaultStatus = params.get("DefaultStatus")
+        self.CreateDate = params.get("CreateDate")
+        self.LastStatusTime = params.get("LastStatusTime")
+        self.UserStoreProtocolHost = params.get("UserStoreProtocolHost")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/ciam_client.py` & `tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/ciam_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -91,14 +91,106 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateUserGroup(self, request):
+        """创建用户组
+
+        :param request: Request instance for CreateUserGroup.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.CreateUserGroupRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.CreateUserGroupResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateUserGroup", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateUserGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateUserStore(self, request):
+        """创建用户目录
+
+        :param request: Request instance for CreateUserStore.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.CreateUserStoreRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.CreateUserStoreResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateUserStore", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateUserStoreResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteUserGroups(self, request):
+        """批量删除用户组
+
+        :param request: Request instance for DeleteUserGroups.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.DeleteUserGroupsRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.DeleteUserGroupsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteUserGroups", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteUserGroupsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteUserStore(self, request):
+        """删除用户目录
+
+        :param request: Request instance for DeleteUserStore.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.DeleteUserStoreRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.DeleteUserStoreResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteUserStore", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteUserStoreResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteUsers(self, request):
         """批量删除用户
 
         :param request: Request instance for DeleteUsers.
         :type request: :class:`tencentcloud.ciam.v20220331.models.DeleteUsersRequest`
         :rtype: :class:`tencentcloud.ciam.v20220331.models.DeleteUsersResponse`
 
@@ -275,14 +367,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ListUserGroups(self, request):
+        """查询用户组列表
+
+        :param request: Request instance for ListUserGroups.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.ListUserGroupsRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.ListUserGroupsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ListUserGroups", params, headers=headers)
+            response = json.loads(body)
+            model = models.ListUserGroupsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ListUserStore(self, request):
+        """查询用户目录列表
+
+        :param request: Request instance for ListUserStore.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.ListUserStoreRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.ListUserStoreResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ListUserStore", params, headers=headers)
+            response = json.loads(body)
+            model = models.ListUserStoreResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ResetPassword(self, request):
         """重置用户密码
 
         :param request: Request instance for ResetPassword.
         :type request: :class:`tencentcloud.ciam.v20220331.models.ResetPasswordRequest`
         :rtype: :class:`tencentcloud.ciam.v20220331.models.ResetPasswordResponse`
 
@@ -344,14 +482,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def UpdateUserGroup(self, request):
+        """更新用户组
+
+        :param request: Request instance for UpdateUserGroup.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserGroupRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.UpdateUserGroupResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateUserGroup", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateUserGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def UpdateUserStatus(self, request):
         """更新用户状态
 
         :param request: Request instance for UpdateUserStatus.
         :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserStatusRequest`
         :rtype: :class:`tencentcloud.ciam.v20220331.models.UpdateUserStatusResponse`
 
@@ -364,8 +525,31 @@
             model = models.UpdateUserStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateUserStore(self, request):
+        """更新用户目录
+
+        :param request: Request instance for UpdateUserStore.
+        :type request: :class:`tencentcloud.ciam.v20220331.models.UpdateUserStoreRequest`
+        :rtype: :class:`tencentcloud.ciam.v20220331.models.UpdateUserStoreResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateUserStore", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateUserStoreResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/ciam/v20220331/errorcodes.py` & `tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/ciam/v20220331/errorcodes.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 
 # 从账号已经被融合过，不允许再次融合。
 FAILEDOPERATION_ACCOUNTALREADYBELINKED = 'FailedOperation.AccountAlreadyBeLinked'
 
 # 用户属性格式异常。
 FAILEDOPERATION_ATTRIBUTEFORMATERROR = 'FailedOperation.AttributeFormatError'
 
+# 认证源名称已存在。
+FAILEDOPERATION_AUTHSOURCENAMEALREADYEXISTS = 'FailedOperation.AuthSourceNameAlreadyExists'
+
+# 认证源不存在。
+FAILEDOPERATION_AUTHSOURCENOTFOUND = 'FailedOperation.AuthSourceNotFound'
+
 # 已存在2个有效的任务，请等待其中一部分完成后重试。
 FAILEDOPERATION_DATAFLOWTOOMANYREQUESTS = 'FailedOperation.DataFlowTooManyRequests'
 
 # 该邮箱已被用户绑定。
 FAILEDOPERATION_EMAILALREADYEXISTS = 'FailedOperation.EmailAlreadyExists'
 
 # 邮箱地址不能为空。
@@ -76,14 +82,17 @@
 
 # 配额超限，如有需求请联系客服人员。
 FAILEDOPERATION_QUOTALIMITEXCEEDED = 'FailedOperation.QuotaLimitExceeded'
 
 # 从用户不存在。
 FAILEDOPERATION_SECONDARYUSERNOTFOUND = 'FailedOperation.SecondaryUserNotFound'
 
+# 用户组名称已存在。
+FAILEDOPERATION_USERGROUPNAMEALREADYEXISTS = 'FailedOperation.UserGroupNameAlreadyExists'
+
 # 用户组不存在。
 FAILEDOPERATION_USERGROUPNOTFOUND = 'FailedOperation.UserGroupNotFound'
 
 # 用户已被冻结。
 FAILEDOPERATION_USERISFREEZE = 'FailedOperation.UserIsFreeze'
 
 # 用户名称已存在。
@@ -91,23 +100,47 @@
 
 # 用户名不能为空。
 FAILEDOPERATION_USERNAMEISNULL = 'FailedOperation.UserNameIsNull'
 
 # 用户不存在。
 FAILEDOPERATION_USERNOTFOUND = 'FailedOperation.UserNotFound'
 
+# 属性标识已存在。
+FAILEDOPERATION_USERPROPERTYCODEALREADYEXISTS = 'FailedOperation.UserPropertyCodeAlreadyExists'
+
+# 用户属性不存在。
+FAILEDOPERATION_USERPROPERTYNOTFOUND = 'FailedOperation.UserPropertyNotFound'
+
 # 更新状态必传。
 FAILEDOPERATION_USERSTATUSREQUIRED = 'FailedOperation.UserStatusRequired'
 
+# 已存在相同用户目录名。
+FAILEDOPERATION_USERSTOREALREADYEXISTS = 'FailedOperation.UserStoreAlreadyExists'
+
+# 已存在相同域名。
+FAILEDOPERATION_USERSTOREDOMAINALREADYEXISTS = 'FailedOperation.UserStoreDomainAlreadyExists'
+
+# 用户目录不存在。
+FAILEDOPERATION_USERSTORENOTEXIST = 'FailedOperation.UserStoreNotExist'
+
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
+# 判断存在用户内部请求错误，请稍后重试。
+INTERNALERROR_JUDGEUSEREXISTEXCEPTION = 'InternalError.JudgeUserExistException'
+
 # 未知错误。
 INTERNALERROR_UNKNOWNERROR = 'InternalError.UnknownError'
 
+# 创建用户目录时创建秘钥失败。
+INTERNALERROR_USERSTORECREATESECRETFAIL = 'InternalError.UserStoreCreateSecretFail'
+
+# 删除用户目录时删除用户失败。
+INTERNALERROR_USERSTOREDELETEUSERFAIL = 'InternalError.UserStoreDeleteUserFail'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 请求参数不合法。
 INVALIDPARAMETER_PARAMETERILLEGAL = 'InvalidParameter.ParameterIllegal'
 
 # 参数取值错误。
@@ -153,7 +186,37 @@
 UNAUTHORIZEDOPERATION_TENANTNOTACTIVATED = 'UnauthorizedOperation.TenantNotActivated'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# 认证源已启用，不允许删除。
+UNSUPPORTEDOPERATION_ENABLEDAUTHSOURCECANNOTBEDELETED = 'UnsupportedOperation.EnabledAuthSourceCanNotBeDeleted'
+
+# 认证源已启用，不允许更新。
+UNSUPPORTEDOPERATION_ENABLEDAUTHSOURCECANNOTBEUPDATED = 'UnsupportedOperation.EnabledAuthSourceCanNotBeUpdated'
+
+# 内置属性不支持该操作。
+UNSUPPORTEDOPERATION_INTERNALUSERPROPERTY = 'UnsupportedOperation.InternalUserProperty'
+
+# 属性被应用关联，不允许删除。
+UNSUPPORTEDOPERATION_LINKEDAPPUSERPROPERTYCANNOTBEDELETED = 'UnsupportedOperation.LinkedAppUserPropertyCanNotBeDeleted'
+
+# 认证源被应用关联，不允许关闭。
+UNSUPPORTEDOPERATION_LINKEDAUTHSOURCECANNOTBECLOSED = 'UnsupportedOperation.LinkedAuthSourceCanNotBeClosed'
+
+# 认证源被应用关联，不允许删除。
+UNSUPPORTEDOPERATION_LINKEDAUTHSOURCECANNOTBEDELETED = 'UnsupportedOperation.LinkedAuthSourceCanNotBeDeleted'
+
+# 属性被认证源关联，不允许删除。
+UNSUPPORTEDOPERATION_LINKEDAUTHSOURCEUSERPROPERTYCANNOTBEDELETED = 'UnsupportedOperation.LinkedAuthSourceUserPropertyCanNotBeDeleted'
+
+# 属性被其它模块关联，不允许删除。
+UNSUPPORTEDOPERATION_LINKEDUSERPROPERTYCANNOTBEDELETED = 'UnsupportedOperation.LinkedUserPropertyCanNotBeDeleted'
+
+# 不允许使用平台域名后缀作为自有域名后缀。
+UNSUPPORTEDOPERATION_PLATFORMDOMAINSUFFIXCANNOTBEUSED = 'UnsupportedOperation.PlatformDomainSuffixCanNotBeUsed'
+
+# 用户池下已存在用户，用户属性不允许被删除。
+UNSUPPORTEDOPERATION_WHENUSEREXISTUSERPROPERTYCANNOTBEDELETED = 'UnsupportedOperation.WhenUserExistUserPropertyCanNotBeDeleted'
```

### Comparing `tencentcloud-sdk-python-ciam-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ciam-3.0.927/tencentcloud/__init__.py`

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

