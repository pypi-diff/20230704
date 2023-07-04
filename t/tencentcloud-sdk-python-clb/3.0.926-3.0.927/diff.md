# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.926.tar", last modified: Mon Jul  3 00:22:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.927.tar", last modified: Tue Jul  4 00:18:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.926.tar` & `tencentcloud-sdk-python-clb-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)   331813 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)    89673 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:22:28.000000 tencentcloud-sdk-python-clb-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   331850 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)    89673 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:18:07.000000 tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/__init__.py
```

### Comparing `tencentcloud-sdk-python-clb-3.0.926/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.927/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.926/setup.py` & `tencentcloud-sdk-python-clb-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.926/README.rst` & `tencentcloud-sdk-python-clb-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.927/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4670,15 +4670,15 @@
         :param HttpCode: 健康检查状态码（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式）。可选值：1~31，默认 31。
 1 表示探测后返回值 1xx 代表健康，2 表示返回 2xx 代表健康，4 表示返回 3xx 代表健康，8 表示返回 4xx 代表健康，16 表示返回 5xx 代表健康。若希望多种返回码都可代表健康，则将相应的值相加。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCode: int
         :param HttpCheckPath: 健康检查路径（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCheckPath: str
-        :param HttpCheckDomain: 健康检查域名（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式，当监听器是TCP类型时，该参数为必填项）。
+        :param HttpCheckDomain: 健康检查域名（仅适用于HTTP/HTTPS监听器和TCP监听器的HTTP健康检查方式。针对TCP监听器，当使用HTTP健康检查方式时，建议该参数配置为必填项）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCheckDomain: str
         :param HttpCheckMethod: 健康检查方法（仅适用于HTTP/HTTPS转发规则、TCP监听器的HTTP健康检查方式），默认值：HEAD，可选值HEAD或GET。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpCheckMethod: str
         :param CheckPort: 自定义探测相关参数。健康检查端口，默认为后端服务的端口，除非您希望指定特定端口，否则建议留空。（仅适用于TCP/UDP监听器）。
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.926/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.927/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.927/tencentcloud/__init__.py`

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

