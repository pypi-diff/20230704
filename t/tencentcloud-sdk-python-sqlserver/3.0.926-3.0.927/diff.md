# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.926.tar", last modified: Mon Jul  3 00:33:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.927.tar", last modified: Tue Jul  4 00:28:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.926.tar` & `tencentcloud-sdk-python-sqlserver-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   355642 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)   108601 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)     9636 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:33:29.000000 tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)     9722 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   355642 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108601 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:28:49.000000 tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.927/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 # 获取VPC网络信息失败。
 FAILEDOPERATION_GETVPCFAILED = 'FailedOperation.GetVpcFailed'
 
 # 备份导入任务锁定失败。
 FAILEDOPERATION_MIGRATIONLOCKERROR = 'FailedOperation.MigrationLockError'
 
+# 不支持此类操作。
+FAILEDOPERATION_NOTSUPPORT = 'FailedOperation.NotSupport'
+
 # 查询订单失败。
 FAILEDOPERATION_QUERYORDERFAILED = 'FailedOperation.QueryOrderFailed'
 
 # 计费相关错误，查询价格失败。
 FAILEDOPERATION_QUERYPRICEFAILED = 'FailedOperation.QueryPriceFailed'
 
 # 安全组操作失败。
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.927/tencentcloud/__init__.py`

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

