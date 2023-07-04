# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.925.tar", last modified: Fri Jun 30 02:05:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.926.tar", last modified: Mon Jul  3 00:24:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.925.tar` & `tencentcloud-sdk-python-dlc-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   351937 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    82325 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:05:54.000000 tencentcloud-sdk-python-dlc-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)   351970 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)    82325 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:24:46.000000 tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1235,15 +1235,15 @@
         :type Mode: int
         :param AutoResume: 是否自动启动集群
         :type AutoResume: bool
         :param MinClusters: 最小资源
         :type MinClusters: int
         :param MaxClusters: 最大资源
         :type MaxClusters: int
-        :param DefaultDataEngine: 是否为默虚拟集群
+        :param DefaultDataEngine: 是否为默认虚拟集群
         :type DefaultDataEngine: bool
         :param CidrBlock: VPC网段
         :type CidrBlock: str
         :param Message: 描述信息
         :type Message: str
         :param Size: 集群规模
         :type Size: int
@@ -1273,15 +1273,15 @@
         :type AutoSuspendTime: int
         :param ResourceType: 资源类型。Standard_CU：标准型；Memory_CU：内存型
         :type ResourceType: str
         :param DataEngineConfigPairs: 集群高级配置
         :type DataEngineConfigPairs: list of DataEngineConfigPair
         :param ImageVersionName: 集群镜像版本名字。如SuperSQL-P 1.1;SuperSQL-S 3.2等,不传，默认创建最新镜像版本的集群
         :type ImageVersionName: str
-        :param MainClusterName: 主集群名称
+        :param MainClusterName: 主集群名称，创建容灾集群时指定
         :type MainClusterName: str
         :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
         :type ElasticSwitch: bool
         :param ElasticLimit: spark jar 包年包月集群弹性上限
         :type ElasticLimit: int
         :param SessionResourceTemplate: spark作业集群session资源配置模板
         :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.926/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/README.rst` & `tencentcloud-sdk-python-dlc-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.926/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.926/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.925/setup.py` & `tencentcloud-sdk-python-dlc-3.0.926/setup.py`

 * *Files identical despite different names*

