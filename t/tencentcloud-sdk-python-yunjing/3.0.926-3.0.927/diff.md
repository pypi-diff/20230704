# Comparing `tmp/tencentcloud-sdk-python-yunjing-3.0.926.tar.gz` & `tmp/tencentcloud-sdk-python-yunjing-3.0.927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yunjing-3.0.926.tar", last modified: Mon Jul  3 00:39:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yunjing-3.0.927.tar", last modified: Tue Jul  4 00:34:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yunjing-3.0.926.tar` & `tencentcloud-sdk-python-yunjing-3.0.927.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud_sdk_python_yunjing.egg-info/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud_sdk_python_yunjing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud_sdk_python_yunjing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud_sdk_python_yunjing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/
--rw-r--r--   0 root         (0) root         (0)   240956 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)    93972 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/yunjing_client.py
--rw-r--r--   0 root         (0) root         (0)     3960 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:39:09.000000 tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud_sdk_python_yunjing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud_sdk_python_yunjing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud_sdk_python_yunjing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud_sdk_python_yunjing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    93972 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/yunjing_client.py
+-rw-r--r--   0 root         (0) root         (0)   240956 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 00:34:31.000000 tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/__init__.py
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/setup.py` & `tencentcloud-sdk-python-yunjing-3.0.927/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunjing
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Yunjing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/README.rst` & `tencentcloud-sdk-python-yunjing-3.0.927/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/PKG-INFO` & `tencentcloud-sdk-python-yunjing-3.0.927/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunjing
-Version: 3.0.926
+Version: 3.0.927
 Summary: Tencent Cloud Yunjing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/models.py` & `tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/yunjing_client.py` & `tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/yunjing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.926/tencentcloud/yunjing/v20180228/errorcodes.py` & `tencentcloud-sdk-python-yunjing-3.0.927/tencentcloud/yunjing/v20180228/errorcodes.py`

 * *Files identical despite different names*

