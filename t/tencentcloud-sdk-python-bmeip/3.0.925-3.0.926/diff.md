# Comparing `tmp/tencentcloud-sdk-python-bmeip-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-bmeip-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bmeip-3.0.925.tar", last modified: Fri Jun 30 02:01:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bmeip-3.0.926.tar", last modified: Mon Jul  3 00:19:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bmeip-3.0.925.tar` & `tencentcloud-sdk-python-bmeip-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud_sdk_python_bmeip.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud_sdk_python_bmeip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud_sdk_python_bmeip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud_sdk_python_bmeip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud_sdk_python_bmeip.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44190 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)    17952 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/bmeip_client.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-30 02:01:01.000000 tencentcloud-sdk-python-bmeip-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud_sdk_python_bmeip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud_sdk_python_bmeip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud_sdk_python_bmeip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud_sdk_python_bmeip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud_sdk_python_bmeip.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/
+-rw-r--r--   0 root         (0) root         (0)    44190 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17952 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/bmeip_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:19:42.000000 tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud_sdk_python_bmeip.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bmeip-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmeip
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Bmeip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/models.py` & `tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/bmeip_client.py` & `tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/bmeip_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/tencentcloud/bmeip/v20180625/errorcodes.py` & `tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud/bmeip/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/README.rst` & `tencentcloud-sdk-python-bmeip-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-bmeip-3.0.926/tencentcloud_sdk_python_bmeip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmeip
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Bmeip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmeip-3.0.925/setup.py` & `tencentcloud-sdk-python-bmeip-3.0.926/setup.py`

 * *Files identical despite different names*

