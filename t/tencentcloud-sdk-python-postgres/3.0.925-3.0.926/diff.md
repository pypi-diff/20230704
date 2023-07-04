# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.925.tar", last modified: Fri Jun 30 02:19:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.926.tar", last modified: Mon Jul  3 00:32:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.925.tar` & `tencentcloud-sdk-python-postgres-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85773 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)   277957 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    20749 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-30 02:19:27.000000 tencentcloud-sdk-python-postgres-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-30 02:19:26.000000 tencentcloud-sdk-python-postgres-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   277960 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    20749 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85773 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:32:03.000000 tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5209,15 +5209,15 @@
         r"""
         :param DBInstanceId: 实例ID
         :type DBInstanceId: str
         :param MinBackupStartTime: 实例最早开始备份时间
         :type MinBackupStartTime: str
         :param MaxBackupStartTime: 实例最晚开始备份时间
         :type MaxBackupStartTime: str
-        :param BaseBackupRetentionPeriod: 实例备份保留时长，取值范围为3-7，单位是天
+        :param BaseBackupRetentionPeriod: 实例备份保留时长，取值范围为7-1830，单位是天
         :type BaseBackupRetentionPeriod: int
         :param BackupPeriod: 实例备份周期，按照星期维度，格式为小写星期英文单词
         :type BackupPeriod: list of str
         """
         self.DBInstanceId = None
         self.MinBackupStartTime = None
         self.MaxBackupStartTime = None
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.926/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.926/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/README.rst` & `tencentcloud-sdk-python-postgres-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.926/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.925/setup.py` & `tencentcloud-sdk-python-postgres-3.0.926/setup.py`

 * *Files identical despite different names*

