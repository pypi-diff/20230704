# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.925.tar", last modified: Fri Jun 30 02:20:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.926.tar", last modified: Mon Jul  3 00:32:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.925.tar` & `tencentcloud-sdk-python-scf-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   192210 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    31630 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    42711 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)   192214 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)    31630 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:32:50.000000 tencentcloud-sdk-python-scf-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.926/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,15 @@
         :type Description: str
         :param MemorySize: 函数运行时内存大小，默认为 128M，可选范围 64、128MB-3072MB，并且以 128MB 为阶梯
         :type MemorySize: int
         :param Timeout: 函数最长执行时间，单位为秒，可选值范围 1-900 秒，默认为 3 秒
         :type Timeout: int
         :param Environment: 函数的环境变量
         :type Environment: :class:`tencentcloud.scf.v20180416.models.Environment`
-        :param Runtime: 函数运行环境，目前仅支持 Python2.7，Python3.6，Nodejs6.10，Nodejs8.9，Nodejs10.15，Nodejs12.16， Php5， Php7，Go1，Java8 和 CustomRuntime，默认Python2.7
+        :param Runtime: 函数运行环境，目前仅支持 Python2.7，Python3.6，Nodejs6.10，Nodejs8.9，Nodejs10.15，Nodejs12.16， Php5.2， Php7.4，Go1，Java8 和 CustomRuntime，默认Python2.7
         :type Runtime: str
         :param VpcConfig: 函数的私有网络配置
         :type VpcConfig: :class:`tencentcloud.scf.v20180416.models.VpcConfig`
         :param Namespace: 函数所属命名空间
         :type Namespace: str
         :param Role: 函数绑定的角色
         :type Role: str
```

### Comparing `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.926/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.925/README.rst` & `tencentcloud-sdk-python-scf-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.926/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.925/setup.py` & `tencentcloud-sdk-python-scf-3.0.926/setup.py`

 * *Files identical despite different names*

